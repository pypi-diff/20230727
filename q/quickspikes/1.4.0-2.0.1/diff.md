# Comparing `tmp/quickspikes-1.4.0.tar.gz` & `tmp/quickspikes-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickspikes-1.4.0.tar", last modified: Fri Sep 30 02:29:18 2022, max compression
+gzip compressed data, was "quickspikes-2.0.1.tar", last modified: Thu Jul 27 14:48:21 2023, max compression
```

## Comparing `quickspikes-1.4.0.tar` & `quickspikes-2.0.1.tar`

### file list

```diff
@@ -1,25 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 02:29:18.459316 quickspikes-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-09-30 02:29:05.000000 quickspikes-1.4.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-30 02:29:05.000000 quickspikes-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5865 2022-09-30 02:29:18.459316 quickspikes-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5033 2022-09-30 02:29:05.000000 quickspikes-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-09-30 02:29:05.000000 quickspikes-1.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 02:29:18.459316 quickspikes-1.4.0/quickspikes/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-09-30 02:29:05.000000 quickspikes-1.4.0/quickspikes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7728 2022-09-30 02:29:05.000000 quickspikes-1.4.0/quickspikes/intracellular.py
--rw-r--r--   0 runner    (1001) docker     (121)     7319 2022-09-30 02:29:05.000000 quickspikes-1.4.0/quickspikes/spikes.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     5546 2022-09-30 02:29:05.000000 quickspikes-1.4.0/quickspikes/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 02:29:18.459316 quickspikes-1.4.0/quickspikes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5865 2022-09-30 02:29:18.000000 quickspikes-1.4.0/quickspikes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-09-30 02:29:18.000000 quickspikes-1.4.0/quickspikes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-30 02:29:18.000000 quickspikes-1.4.0/quickspikes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-30 02:29:18.000000 quickspikes-1.4.0/quickspikes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-30 02:29:18.000000 quickspikes-1.4.0/quickspikes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-30 02:29:18.000000 quickspikes-1.4.0/quickspikes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-30 02:29:05.000000 quickspikes-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-09-30 02:29:18.459316 quickspikes-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-09-30 02:29:05.000000 quickspikes-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 02:29:18.459316 quickspikes-1.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)   200080 2022-09-30 02:29:05.000000 quickspikes-1.4.0/test/intra_spike.npy
--rw-r--r--   0 runner    (1001) docker     (121)   160128 2022-09-30 02:29:05.000000 quickspikes-1.4.0/test/intra_spike_narrow.npy
--rw-r--r--   0 runner    (1001) docker     (121)     8702 2022-09-30 02:29:05.000000 quickspikes-1.4.0/test/test_quickspikes.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-07-27 14:48:21.134334 quickspikes-2.0.1/
+-rw-r--r--   0 dmeliza    (503) staff       (20)       92 2022-08-25 19:49:13.000000 quickspikes-2.0.1/.gitignore
+-rw-r--r--   0 dmeliza    (503) staff       (20)    35147 2015-07-31 18:46:36.000000 quickspikes-2.0.1/COPYING
+-rw-r--r--   0 dmeliza    (503) staff       (20)       64 2017-09-25 20:42:33.000000 quickspikes-2.0.1/MANIFEST.in
+-rw-r--r--   0 dmeliza    (503) staff       (20)     5865 2023-07-27 14:48:21.134499 quickspikes-2.0.1/PKG-INFO
+-rw-r--r--   0 dmeliza    (503) staff       (20)     5033 2022-09-30 02:27:24.000000 quickspikes-2.0.1/README.md
+-rw-r--r--   0 dmeliza    (503) staff       (20)   489347 2015-07-31 18:45:45.000000 quickspikes-2.0.1/algorithm.png
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-07-27 14:48:21.086470 quickspikes-2.0.1/f2py/
+-rw-r--r--   0 dmeliza    (503) staff       (20)     3136 2015-07-31 19:37:35.000000 quickspikes-2.0.1/f2py/spikes.c
+-rw-r--r--   0 dmeliza    (503) staff       (20)     3639 2015-07-31 19:04:57.000000 quickspikes-2.0.1/f2py/spikes.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1692 2015-07-31 18:38:48.000000 quickspikes-2.0.1/f2py/spikes.pyf
+-rw-r--r--   0 dmeliza    (503) staff       (20)       83 2022-09-30 02:27:24.000000 quickspikes-2.0.1/pyproject.toml
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-07-27 14:48:21.105293 quickspikes-2.0.1/quickspikes/
+-rw-r--r--   0 dmeliza    (503) staff       (20)      284 2023-07-27 14:26:01.000000 quickspikes-2.0.1/quickspikes/__init__.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)      420 2023-05-01 13:18:31.000000 quickspikes-2.0.1/quickspikes/extracellular.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     7786 2023-07-27 14:25:55.000000 quickspikes-2.0.1/quickspikes/intracellular.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)  1315042 2023-04-25 22:18:54.000000 quickspikes-2.0.1/quickspikes/spikes.c
+-rw-r--r--   0 dmeliza    (503) staff       (20)     7328 2023-07-27 14:25:55.000000 quickspikes-2.0.1/quickspikes/spikes.pyx
+-rw-r--r--   0 dmeliza    (503) staff       (20)     6333 2023-07-27 14:26:01.000000 quickspikes-2.0.1/quickspikes/tools.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-07-27 14:48:21.117932 quickspikes-2.0.1/quickspikes.egg-info/
+-rw-r--r--   0 dmeliza    (503) staff       (20)     5865 2023-07-27 14:48:20.000000 quickspikes-2.0.1/quickspikes.egg-info/PKG-INFO
+-rw-r--r--   0 dmeliza    (503) staff       (20)      579 2023-07-27 14:48:21.000000 quickspikes-2.0.1/quickspikes.egg-info/SOURCES.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)        1 2023-07-27 14:48:20.000000 quickspikes-2.0.1/quickspikes.egg-info/dependency_links.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)        1 2023-05-12 14:13:27.000000 quickspikes-2.0.1/quickspikes.egg-info/not-zip-safe
+-rw-r--r--   0 dmeliza    (503) staff       (20)       14 2023-07-27 14:48:20.000000 quickspikes-2.0.1/quickspikes.egg-info/requires.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)       12 2023-07-27 14:48:20.000000 quickspikes-2.0.1/quickspikes.egg-info/top_level.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)       22 2020-12-25 21:34:08.000000 quickspikes-2.0.1/requirements.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1141 2023-07-27 14:48:21.135875 quickspikes-2.0.1/setup.cfg
+-rw-r--r--   0 dmeliza    (503) staff       (20)      259 2022-09-30 02:27:24.000000 quickspikes-2.0.1/setup.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-07-27 14:48:21.133572 quickspikes-2.0.1/test/
+-rw-r--r--   0 dmeliza    (503) staff       (20)   200080 2015-08-06 23:31:30.000000 quickspikes-2.0.1/test/intra_spike.npy
+-rw-r--r--   0 dmeliza    (503) staff       (20)   160128 2022-09-24 13:15:10.000000 quickspikes-2.0.1/test/intra_spike_narrow.npy
+-rw-r--r--   0 dmeliza    (503) staff       (20)     8260 2023-07-27 14:25:55.000000 quickspikes-2.0.1/test/test_quickspikes.py
```

### Comparing `quickspikes-1.4.0/COPYING` & `quickspikes-2.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `quickspikes-1.4.0/PKG-INFO` & `quickspikes-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickspikes
-Version: 1.4.0
+Version: 2.0.1
 Summary: detect and extract spikes in time series data
 Home-page: https://github.com/melizalab/quickspikes
 Author: Dan Meliza
 Author-email: dan@meliza.org
 Maintainer: Dan Meliza
 Maintainer-email: dan@meliza.org
 License: GNU General Public License (GPL)
```

### Comparing `quickspikes-1.4.0/README.md` & `quickspikes-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `quickspikes-1.4.0/quickspikes/intracellular.py` & `quickspikes-2.0.1/quickspikes/intracellular.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # -*- mode: python -*-
 """specialized functions for intracellular data"""
-from typing import Tuple, Optional, Iterator, Mapping
+from typing import Tuple, Optional, Iterator
 from collections import namedtuple
 import logging
 import numpy as np
 
 log = logging.getLogger("quickspikes")
 
 Spike = namedtuple(
@@ -26,14 +26,15 @@
     ],
 )
 
 
 def spike_shape(
     spike: np.ndarray,
     dt: float,
+    *,
     deriv_thresh: float = 10.0,
     t_baseline: float = 2.0,
     min_rise: float = 0.25,
 ) -> Optional[Spike]:
     """Computes spike shape features:
 
     takeoff: the voltage/time when the derivative of the waveform exceeds
@@ -68,15 +69,15 @@
     min_rise = int(min_rise / dt)
     peak_ind = spike.argmax()
     if peak_ind in (0, spike.size - 1):
         return None
     peak_v = spike[peak_ind]
     deriv = np.gradient(spike, dt)
     # trough
-    dV0_ind = find_run(deriv[peak_ind:], 0, min_rise) or spike.size
+    dV0_ind = find_run(deriv[peak_ind:], thresh=0, min_run=min_rise) or spike.size
     trough_ind = spike[peak_ind : peak_ind + dV0_ind].argmin()
     # min and max dV/dt
     dVmax_ind = deriv[:peak_ind].argmax()
     dVmin_ind = deriv[peak_ind:].argmin()
 
     # takeoff
     mdV = deriv[:n_baseline].mean()
@@ -88,18 +89,19 @@
         takeoff_ind = pp[-1]
     except IndexError:
         takeoff_t = takeoff_v = half_rise_t = half_decay_t = None
     else:
         takeoff_v = spike[takeoff_ind]
         takeoff_t = (peak_ind - takeoff_ind) * dt
         half_ampl = (peak_v + takeoff_v) / 2
-        half_rise_ind = find_run(spike[:peak_ind], half_ampl, 1) or 0
+        half_rise_ind = find_run(spike[:peak_ind], thresh=half_ampl, min_run=1) or 0
         half_rise_t = (peak_ind - half_rise_ind) * dt
         half_decay_ind = (
-            find_run(-spike[peak_ind:], -half_ampl, 2) or spike.size - peak_ind
+            find_run(-spike[peak_ind:], thresh=-half_ampl, min_run=2)
+            or spike.size - peak_ind
         )
         half_decay_t = half_decay_ind * dt
     return Spike(
         peak_t=peak_ind * dt,
         peak_V=peak_v,
         takeoff_t=takeoff_t,
         takeoff_V=takeoff_v,
@@ -132,28 +134,29 @@
         self.n_rise = n_rise
         self.n_before = n_before
         self.n_after = n_after
 
     def calculate_threshold(
         self,
         V: np.ndarray,
+        *,
         thresh_rel: float = 0.35,
         thresh_min: float = -50,
         deriv_thresh: float = 10.0,
     ) -> Optional[Spike]:
         """Calculate the detection threshold from the amplitude of the first spike in V.
 
         If no spike can be detected in the signal, returns None. Otherwise, the
         instance's threshold is set at `thresh_rel` times the amplitude of the
         first spike, or `thresh_min` (whichever is greater), and the spike shape
         is returned.
 
         """
         self.spike_thresh = self.first_spike_amplitude = None
-        first_peak_idx = V[self.n_before:-self.n_after].argmax() + self.n_before
+        first_peak_idx = V[self.n_before : -self.n_after].argmax() + self.n_before
         first_spike = V[first_peak_idx - self.n_before : first_peak_idx + self.n_after]
         shape = spike_shape(
             first_spike,
             dt=1,
             deriv_thresh=deriv_thresh,
             t_baseline=self.n_before // 2,
             min_rise=self.n_rise // 4,
@@ -165,23 +168,22 @@
         self.spike_thresh = max(
             spike_base + thresh_rel * first_spike_amplitude,
             thresh_min,
         )
         return shape
 
     def detect_spikes(self, V: np.ndarray) -> Iterator[int]:
-        """ Using the calculated threshold, detect spikes that are extractable """
+        """Using the calculated threshold, detect spikes that are extractable"""
         from quickspikes import detector, filter_times
+
         det = detector(self.spike_thresh, self.n_rise)
-        return filter_times(
-            det.send(V), self.n_before, V.size - self.n_after
-        )
+        return filter_times(det.send(V), self.n_before, V.size - self.n_after)
 
     def extract_spikes(
-        self, V: np.ndarray, min_amplitude: float, upsample: int = 2, jitter: int = 4
+        self, V: np.ndarray, *, min_amplitude: float, upsample: int = 2, jitter: int = 4
     ) -> Iterator[Tuple[int, np.ndarray]]:
         """Detect and extract spikes from V.
 
         V: input signal
         min_amplitude: only yield spikes that are at least this much above threshold
         upsample: the upsampling factor to use in realigning spikes
         jitter: the expected jitter in peak position
@@ -190,23 +192,22 @@
         """
         from quickspikes import peaks
         from quickspikes.tools import trim_waveforms, realign_spikes
 
         spike_times = self.detect_spikes(V)
         if len(spike_times) == 0:
             return
-        spikes = peaks(V, spike_times, self.n_before, self.n_after)
+        spikes = peaks(V, spike_times, n_before=self.n_before, n_after=self.n_after)
         spike_times, spikes = realign_spikes(
             spike_times,
             spikes,
-            upsample,
-            reflect_fft=True,
+            upsample=upsample,
             expected_peak=self.n_before,
         )
         # original version of this located the peak after resampling, but I
         # don't think this is generally necessary
         for time, spike in trim_waveforms(
-            spikes, spike_times, self.n_before, self.n_rise * 2
+            spikes, spike_times, peak_t=self.n_before, n_rise=self.n_rise * 2
         ):
             if not np.any(spike - self.spike_thresh > min_amplitude):
                 continue
             yield (time // upsample, spike)
```

### Comparing `quickspikes-1.4.0/quickspikes/spikes.pyx` & `quickspikes-2.0.1/quickspikes/spikes.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
     def reset(self):
         """Reset the detector's internal state"""
         self.state = BELOW_THRESHOLD
 
 
 @boundscheck(False)
-def peaks(sample_t[:] samples, times, size_t n_before=75, size_t n_after=400):
+def peaks(sample_t[:] samples, times, *, size_t n_before=75, size_t n_after=400):
     """Extracts samples around times
 
     Returns a 2D array with len(times) rows and (n_before + n_after) columns
     containing the values surrounding the sample indices in times.
 
     Note: all values of times must be greater than n_before and less than
     samples.size - n_after. See `tools.filter_spikes`
@@ -150,15 +150,15 @@
             raise ValueError("spike %d waveform ends after input data" % i)
         else:
             arr[i,:] = samples[event-n_before:event+n_after]
 
     return out
 
 
-def find_run(sample_t[:] values, sample_t thresh, long min_run):
+def find_run(sample_t[:] values, *, sample_t thresh, long min_run):
     """ Return the index of the first element in values that starts a run of at
     least min_run in length, or None if no such run exists. """
     cdef long i
     cdef long run_start = 0
     cdef bint in_run = False
     for i in range(values.size):
         if values[i] > thresh:
@@ -168,15 +168,15 @@
             if i - run_start >= min_run:
                 return run_start
         else:
             in_run = False
     return None
 
 
-def subthreshold(double[:] samples, times,
+def subthreshold(double[:] samples, times, *,
                  double v_thresh=-50, double dv_thresh=0, size_t min_size=10):
     """Removes spikes from time series
 
     Spikes are removed from the voltage trace by beginning at each peak and
     moving in either direction until V drops below thresh_v OR dv drops below
     thresh_dv. This algorithm does not work with negative peaks, so invert your
     signal if you need to.
```

### Comparing `quickspikes-1.4.0/quickspikes/tools.py` & `quickspikes-2.0.1/quickspikes/tools.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,97 @@
 # -*- coding: utf-8 -*-
 # -*- mode: python -*-
 """spike detection and extraction
 
 Copyright (C) 2013 Dan Meliza <dmeliza@gmail.com>
 Created Fri Jul 12 14:05:16 2013
 """
-from typing import Iterable, Union, Tuple, Optional, Iterator, Mapping
+from typing import Iterable, Union, Tuple, Optional, Iterator, Callable
 import numpy as np
 
 numeric = Union[int, float, np.number]
 
 
 def filter_times(
     times: Iterable[numeric], min: numeric, max: numeric
 ) -> Tuple[numeric]:
     return tuple(t for t in times if (t > min) and (t < max))
 
 
+def peak_idx(spikes: np.ndarray):
+    """Return index of maximum negative value"""
+    return spikes.argmax(-1)
+
+
+def trough_idx(spikes: np.ndarray):
+    """Return index of maximum positive value"""
+    return spikes.argmin(-1)
+
+
+def upswing_idx(spikes: np.ndarray):
+    """Return index of the point midway between the trough and the following peak"""
+    trough = trough_idx(spikes)
+    # need to find the local maximum after the trough, not the global max
+    raise NotImplementedError
+
+
 def realign_spikes(
     times: Iterable[numeric],
     spikes: np.ndarray,
-    upsample: int,
+    *,
+    upsample: int = 1,
+    align_by: Callable[[np.ndarray], Union[np.ndarray, int]] = peak_idx,
     jitter: int = 3,
-    reflect_fft: bool = False,
     expected_peak: Optional[int] = None,
 ) -> Tuple[np.ndarray, np.ndarray]:
-    """Realign spikes to their peaks using bandwidth-limited resampling
+    """Realign spikes to their peaks (or some other feature) using bandwidth-limited resampling
 
     times    : one-dimensional array of spike times, in units of samples
     spikes   : array of spike waveforms, with dimensions (nspikes, npoints)
     upsample : integer, the factor by which to upsample the data for realignment (must be greater than 1)
-    jitter   : samples (in original data) to search for true peak
-    expected_peak : if supplied, searches around this index for the peak. If not supplied,
-                    uses the argmax of the mean spike
+    align_by : function that returns the alignment point in each spike (see below)
+    jitter   : samples (in original data) to search for the alignment point
+    expected_peak : if supplied, searches around this index (in original data) for the peak. If not supplied,
+                    uses align_by on the mean spike
+
+    The align_by function takes a 1D or 2D array and returns the index
+    corresponding to the alignment point in the spike. If the array is 1D, the
+    function should return a single number. If the array is 2D, the function
+    must return an array. For example, peak_idx is lambda x: x.argmax(-1)
 
-    Returns (times, spikes), with the sampling rate increased by a factor of upsample
+    Returns (times, spikes), with the sampling rate increased by a factor of
+    upsample.
 
     """
-    assert (
-        isinstance(upsample, int) and upsample > 1
-    ), "Upsampling factor must be an integer greater than 1"
+    if not (isinstance(upsample, int) and upsample > 0):
+        raise ValueError("Upsampling factor must be a positive integer")
     nevents, nsamples = spikes.shape
 
-    # first infer the expected peak time
     if expected_peak is None:
-        expected_peak = np.mean(spikes, 0).argmax() * upsample
-    else:
-        expected_peak *= upsample
-    spikes = fftresample(spikes, int(nsamples * upsample), reflect=reflect_fft)
+        # infer expected peak from the mean spike
+        expected_peak = align_by(np.mean(spikes, 0))
+    expected_peak *= upsample
+
+    if upsample > 1:
+        spikes = fftresample(spikes, int(nsamples * upsample), reflect=True)
     # find peaks within upsample samples of mean peak
-    shift = find_peaks(spikes, expected_peak, upsample * jitter)
-    start = shift + upsample * jitter
+    window = upsample * jitter
+    # output array is clipped by jitter on both ends and then upsampled
     nshifted = (nsamples - 2 * jitter) * upsample
     shifted = np.zeros((nevents, nshifted))
+    # offset is the position of the peak (or trough) within the search window
+    search = slice(expected_peak - window, expected_peak + window + 1)
+    start = align_by(spikes[:, search])
     for i, spike in enumerate(spikes):
         shifted[i, :] = spike[start[i] : start[i] + nshifted]
-    return (np.asarray(times) * upsample + shift, shifted)
-
-
-def find_peaks(spikes: np.ndarray, peak: int, window: int) -> np.ndarray:
-    """Locate the peaks in an array of spikes.
-
-    spikes: resampled spike waveforms, dimensions (nspikes, nsamples)
-    peak:   the expected peak location
-    window: the number of samples to either side of the peak to look for the peak
-
-    Returns array of shift values relative to peak
-
-    """
-    r = slice(peak - window, peak + window + 1)
-    return spikes[:, r].argmax(1) - window
+    # spike times are shifted by offset - search window
+    return (np.asarray(times) * upsample + start - window, shifted)
 
 
-def fftresample(S: np.ndarray, npoints: int, reflect: bool = False) -> np.ndarray:
+def fftresample(S: np.ndarray, npoints: int, *, reflect: bool = False) -> np.ndarray:
     """Resample an array of waveforms using discrete fourier transform. The
     signal is transformed in the fourier domain and then padded or truncated to
     the desired size. This should be equivalent to a sinc resampling.
 
     S: a 2D array of waveforms (nspikes, nsamples)
     npoints: the desired duration of the resampled signal
     reflect: if True, pad the sample with reflected copies on either end to suppress edge effects
@@ -94,15 +109,15 @@
         npoints = npoints // 3
         return Srs[:, npoints : npoints * 2]
     else:
         return Srs
 
 
 def trim_waveforms(
-    spikes: Iterable[np.ndarray], times: Iterable[int], peak_t: int, n_rise: int
+    spikes: Iterable[np.ndarray], times: Iterable[int], *, peak_t: int, n_rise: int
 ) -> Iterator[Tuple[int, np.ndarray]]:
     """Trims spike waveforms to remove overlapping peaks.
 
     The peaks() function is used to extract waveforms in a window surrounding
     peak times. The windows for successive peaks may overlap each other if the
     peak times are closer together than the window size, which can result in
     secondary peaks occuring later in the window corresponding to the subsequent
```

### Comparing `quickspikes-1.4.0/quickspikes.egg-info/PKG-INFO` & `quickspikes-2.0.1/quickspikes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickspikes
-Version: 1.4.0
+Version: 2.0.1
 Summary: detect and extract spikes in time series data
 Home-page: https://github.com/melizalab/quickspikes
 Author: Dan Meliza
 Author-email: dan@meliza.org
 Maintainer: Dan Meliza
 Maintainer-email: dan@meliza.org
 License: GNU General Public License (GPL)
```

### Comparing `quickspikes-1.4.0/setup.cfg` & `quickspikes-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `quickspikes-1.4.0/test/intra_spike.npy` & `quickspikes-2.0.1/test/intra_spike.npy`

 * *Files identical despite different names*

### Comparing `quickspikes-1.4.0/test/intra_spike_narrow.npy` & `quickspikes-2.0.1/test/intra_spike_narrow.npy`

 * *Files identical despite different names*

