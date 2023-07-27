# Comparing `tmp/PyAutoscoper-1.1.3.tar.gz` & `tmp/PyAutoscoper-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAutoscoper-1.1.3.tar", last modified: Thu Mar 23 17:27:48 2023, max compression
+gzip compressed data, was "PyAutoscoper-2.0.0.tar", last modified: Thu Jul 27 15:30:25 2023, max compression
```

## Comparing `PyAutoscoper-1.1.3.tar` & `PyAutoscoper-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:27:48.839532 PyAutoscoper-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-03-23 17:27:48.839532 PyAutoscoper-1.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:27:48.835531 PyAutoscoper-1.1.3/PyAutoscoper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 17:27:24.000000 PyAutoscoper-1.1.3/PyAutoscoper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20405 2023-03-23 17:27:24.000000 PyAutoscoper-1.1.3/PyAutoscoper/connect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:27:48.839532 PyAutoscoper-1.1.3/PyAutoscoper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-03-23 17:27:48.000000 PyAutoscoper-1.1.3/PyAutoscoper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-23 17:27:48.000000 PyAutoscoper-1.1.3/PyAutoscoper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 17:27:48.000000 PyAutoscoper-1.1.3/PyAutoscoper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-23 17:27:48.000000 PyAutoscoper-1.1.3/PyAutoscoper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-23 17:27:48.000000 PyAutoscoper-1.1.3/PyAutoscoper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-03-23 17:27:24.000000 PyAutoscoper-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-03-23 17:27:24.000000 PyAutoscoper-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 17:27:48.839532 PyAutoscoper-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:30:25.586954 PyAutoscoper-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-27 15:30:25.586954 PyAutoscoper-2.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:30:25.582954 PyAutoscoper-2.0.0/PyAutoscoper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:30:12.000000 PyAutoscoper-2.0.0/PyAutoscoper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-07-27 15:30:12.000000 PyAutoscoper-2.0.0/PyAutoscoper/connect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:30:25.582954 PyAutoscoper-2.0.0/PyAutoscoper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-27 15:30:24.000000 PyAutoscoper-2.0.0/PyAutoscoper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-27 15:30:25.000000 PyAutoscoper-2.0.0/PyAutoscoper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 15:30:24.000000 PyAutoscoper-2.0.0/PyAutoscoper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 15:30:24.000000 PyAutoscoper-2.0.0/PyAutoscoper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-27 15:30:24.000000 PyAutoscoper-2.0.0/PyAutoscoper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-27 15:30:12.000000 PyAutoscoper-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:30:25.586954 PyAutoscoper-2.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-27 15:30:12.000000 PyAutoscoper-2.0.0/examples/pyautoscoper-examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-27 15:30:12.000000 PyAutoscoper-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 15:30:25.586954 PyAutoscoper-2.0.0/setup.cfg
```

### Comparing `PyAutoscoper-1.1.3/PyAutoscoper/connect.py` & `PyAutoscoper-2.0.0/PyAutoscoper/connect.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,70 @@
 import os
 import socket
 import struct
+from enum import Enum
+
+EXPECTED_SERVER_VERSION = 2
+
+
+class CostFunction(Enum):
+    """Enum for the different cost functions available in PyAutoscoper."""
+
+    NORMALIZED_CROSS_CORRELATION = 0
+    SUM_OF_ABSOLUTE_DIFFERENCES = 1
+
+
+class OptimizationInitializationHeuristic(Enum):
+    """Enum for the different optimization initialization heuristics available in PyAutoscoper."""
+
+    CURRENT_FRAME = 0
+    PREVIOUS_FRAME = 1
+    LINEAR_EXTRAPOLATION = 2
+    SPLINE_INTERPOLATION = 3
+
+
+class OptimizationMethod(Enum):
+    """Enum for the different optimization methods available in PyAutoscoper."""
+
+    PARTICLE_SWARM_OPTIMIZATION = 0
+    DOWNHILL_SIMPLEX = 1
 
 
 class AutoscoperServerError(Exception):
     """Exception raised when the server reports an error."""
 
     def __str__(self):
         return f"Autoscoper Server error: {super().__str__()}"
 
 
+class AutoscoperServerVersionMismatch(Exception):
+    """Exception raised when the client attempt to connect to an unsupported server."""
+
+    def __init__(self, server_version):
+        self.server_version = server_version
+        msg = f"server_version {self.server_version}, expected_version {EXPECTED_SERVER_VERSION}"
+        super().__init__(msg)
+
+    def __str__(self):
+        return f"Autoscoper Server Version mismatch: {super().__str__()}"
+
+
 class AutoscoperConnectionError(Exception):
     """Exception raised when the connection to the server is lost."""
 
     def __str__(self):
         return f"Error communicating with Autoscoper server: {super().__str__()}"
 
 
 class AutoscoperConnection:
     def __init__(self, address="127.0.0.1", verbose=False) -> None:
         self.address = address
         self.verbose = verbose
         self.socket = self._openConnection()
+        self._checkVersion()
 
     def __str__(self):
         return f"Autoscoper connection to {self.address}"
 
     def __repr__(self):
         return f"AutoscoperConnection('{self.address}', verbose={self.verbose})"
 
@@ -99,14 +138,35 @@
 
         Called automatically upon init.
         """
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         s.connect((self.address, 30007))
         return s
 
+    def _checkVersion(self):
+        """
+        Internal function, should not be called by a user.
+
+        Checks that the server version is compatible with the client version.
+
+        Called automatically upon init.
+
+        :raises AutoscoperServerVersionMismatch: If the server version does not match the client version
+        """
+        response = self._send_command(0x10)  # 16
+        server_version = struct.unpack("i", response[1:])[0]  # version string formatted as "NUMBER"
+
+        if server_version != EXPECTED_SERVER_VERSION:
+            raise AutoscoperServerVersionMismatch(server_version)
+
+        if self.verbose:
+            print(f"Server version: {server_version}")
+
+        return
+
     @property
     def is_connected(self):
         """
         Returns the status of the connection to the PyAutoscoper server.
 
         :rtype: Boolean
         """
@@ -118,15 +178,15 @@
 
     def loadTrial(self, trial_file):
         """
         Load a trial file into the PyAutoscoper server.
 
         :param trial_file: The path to the trial file to load
         :type trial_file: str
-        :raises AutoScoperServerError: If the server fails to load the trial file
+        :raises AutoscoperServerError: If the server fails to load the trial file
         :raises AutoscoperConnectionError: If the connection to the server is lost
         """
         if self.verbose:
             print(f"Loading trial file: {trial_file}")
         if not os.path.exists(trial_file):
             raise AutoscoperServerError(f"File not found: {trial_file}")
         self._send_command(0x01, trial_file)
@@ -157,15 +217,15 @@
         :type is_with_commas: bool
         :param is_cm: Optional - If true, the tracking data will be loaded in cm. If false, the tracking data will be loaded in mm. Defaults to false.
         :type is_cm: bool
         :param is_rad: Optional - If true, the tracking data will be loaded in radians. If false, the tracking data will be loaded in degrees. Defaults to false.
         :type is_rad: bool
         :param interpolate: Optional - If true, the tracking data will be interpolated using the spline method. If false, the tracking data will be saved as is (with NaN values). Defaults to false.
         :type interpolate: bool
-        :raises AutoScoperServerError: If the server fails to load the tracking data
+        :raises AutoscoperServerError: If the server fails to load the tracking data
         :raises AutoscoperConnectionError: If the connection to the server is lost
         """
         if self.verbose:
             print(f"Loading tracking data: {tracking_data}")
         if not os.path.exists(tracking_data):
             raise AutoscoperServerError(f"Tracking data not found: {tracking_data}")
         self._send_command(
@@ -206,15 +266,15 @@
         :type save_with_commas: bool
         :param convert_to_cm: Optional - If true, the tracking data will be converted to cm. If false, the tracking data will be saved in mm. Defaults to false.
         :type convert_to_cm: bool
         :param convert_to_rad: Optional - If true, the tracking data will be converted to radians. If false, the tracking data will be saved in degrees. Defaults to false.
         :type convert_to_rad: bool
         :param interpolate: Optional - If true, the tracking data will be interpolated using the spline method. If false, the tracking data will be saved as is (with NaN values). Defaults to false.
         :type interpolate: bool
-        :raises AutoScoperServerError: If the server fails to save the tracking data
+        :raises AutoscoperServerError: If the server fails to save the tracking data
         :raises AutoscoperConnectionError: If the connection to the server is lost
         """
         if self.verbose:
             print(f"Saving tracking data: {tracking_file}")
 
         self._send_command(
             0x03,
@@ -232,30 +292,30 @@
         """
         Load filter settings into the PyAutoscoper server.
 
         :param camera: The camera to load the filter settings into
         :type camera: int
         :param settings_file: The path to the filter settings to load
         :type settings_file: str
-        :raises AutoScoperServerError: If the server fails to load the filter settings
+        :raises AutoscoperServerError: If the server fails to load the filter settings
         :raises AutoscoperConnectionError: If the connection to the server is lost
         """
         if self.verbose:
             print(f"Loading filter settings: {settings_file}")
         if not os.path.exists(settings_file):
             raise AutoscoperServerError(f"Filter settings not found: {settings_file}")
         self._send_command(0x04, camera, settings_file)
 
     def setFrame(self, frame):
         """
         Set the frame to be used for the next acquisition.
 
         :param frame: The frame to be used for the next acquisition
         :type frame: int
-        :raises AutoScoperServerError: If the server fails to set the frame
+        :raises AutoscoperServerError: If the server fails to set the frame
         :raises AutoscoperConnectionError: If the connection to the server is lost
         """
         if self.verbose:
             print(f"Setting frame: {frame}")
         self._send_command(0x05, frame)
 
     def getPose(self, volume, frame):
@@ -264,15 +324,15 @@
 
         :param volume: The volume to get the pose of
         :type volume: int
         :param frame: The frame to get the pose at
         :type frame: int
         :return: The pose of the volume at the specified frame
         :rtype: list[float]
-        :raises AutoScoperServerError: If the server fails to get the pose
+        :raises AutoscoperServerError: If the server fails to get the pose
         :raises AutoscoperConnectionError: If the connection to the server is lost
         """
         if self.verbose:
             print(f"Getting pose for volume {volume} on frame {frame}")
         response = self._send_command(0x06, volume, frame)
         return [
             struct.unpack("d", response[1:9])[0],
@@ -289,15 +349,15 @@
 
         :param volume: The volume to set the pose of
         :type volume: int
         :param frame: The frame to set the pose at
         :type frame: int
         :param pose: The pose to set the volume to
         :type pose: list[float]
-        :raises AutoScoperServerError: If the server fails to set the pose
+        :raises AutoscoperServerError: If the server fails to set the pose
         :raises AutoscoperConnectionError: If the connection to the server is lost
         """
         if self.verbose:
             print(f"Setting pose {pose} for volume {volume} on frame {frame}")
         self._send_command(0x07, volume, frame, *pose)
 
     def getNCC(self, volume, pose):
@@ -306,15 +366,15 @@
 
         :param volume: The volume to get the NCC of
         :type volume: int
         :param pose: The pose to get the NCC at
         :type pose: list[float]
         :return: The NCC of the volume at the specified pose
         :rtype: list[float]
-        :raises AutoScoperServerError: If the server fails to get the NCC
+        :raises AutoscoperServerError: If the server fails to get the NCC
         :raises AutoscoperConnectionError: If the connection to the server is lost
         """
         if self.verbose:
             print(f"Getting NCC for volume {volume} on pose {pose}")
         response = self._send_command(0x08, volume, *pose)
         ncc = []
         for i in range(0, 2):
@@ -324,15 +384,15 @@
 
     def setBackground(self, threshold):
         """
         Set the background threshold.
 
         :param threshold: The background threshold
         :type threshold: float
-        :raises AutoScoperServerError: If the server fails to set the background threshold
+        :raises AutoscoperServerError: If the server fails to set the background threshold
         :raises AutoscoperConnectionError: If the connection to the server is lost
         """
         if self.verbose:
             print(f"Setting background threshold: {threshold}")
         self._send_command(0x09, threshold)
 
     def getImageCropped(self, volume, camera, pose):
@@ -343,20 +403,19 @@
         :type volume: int
         :param camera: The camera to get the image from
         :type camera: int
         :param pose: The pose to get the image at
         :type pose: list[float]
         :return: The cropped image of the volume at the specified pose
         :rtype: list[float]
-        :raises Exception: If the server fails to get the image
+        :raises AutoscoperServerError: If the server fails to get the image
+        :raises AutoscoperConnectionError: If the connection to the server is lost
         """
         if self.verbose:
-            print(
-                f"Getting image for volume {volume} on pose {pose} from camera {camera}"
-            )
+            print(f"Getting image for volume {volume} on pose {pose} from camera {camera}")
         response = self._send_command(0x0A, volume, camera, *pose)  # 10
         width = struct.unpack("i", response[1:5])[0]
         height = struct.unpack("i", response[5:9])[0]
         img_data = response[9:]
         return [width, height, img_data]
 
     def optimizeFrame(
@@ -367,14 +426,15 @@
         max_itr,
         min_lim,
         max_lim,
         max_stall_itr,
         dframe,
         opt_method,
         cf_model,
+        opt_init_heuristic,
     ):
         """
         Optimize the pose of the volume at the specified frame.
 
         :param volume: The volume to optimize
         :type volume: int
         :param frame: The frame to optimize
@@ -387,39 +447,53 @@
         :type min_lim: float
         :param max_lim: The maximum limit of the optimization
         :type max_lim: float
         :param max_stall_itr: The maximum number of iterations to stall
         :type max_stall_itr: int
         :param dframe: The amount of frames to skip
         :type dframe: int
-        :param opt_method: The optimization method to use, 0 for Particle Swarm, 1 for Downhill Simplex
-        :type opt_method: int
-        :param cf_model: The cost function model to use, 0 for NCC (Bone Models), 1 for Sum of Absolute Differences (Implant Models)
-        :type cf_model: int
+        :param opt_method: The optimization method to use.
+        :type opt_method: int or :const:`~OptimizationMethod`
+        :param cf_model: The cost function to use. :const:`~CostFunction.NORMALIZED_CROSS_CORRELATION` for Bone Models,  :const:`~CostFunction.SUM_OF_ABSOLUTE_DIFFERENCES` for Implant Models.
+        :type cf_model: int or :const:`~CostFunction`
+        :param opt_init_heuristic: The heuristic to initialize the optimization. See :const:`~OptimizationInitializationHeuristic`.
+        :type opt_init_heuristic: int or :const:`~OptimizationInitializationHeuristic`
+
         :raises AutoscoperServerError: If the server fails to optimize the frame
         :raises AutoscoperConnectionError: If the connection to the server is lost
+        :raises ValueError: If parameters accepting an enum value are incorrectly specified.
+
+        .. versionadded:: 2
+
+          The `opt_init_heuristic` parameter.
         """
-        if opt_method not in [0, 1]:
-            raise Exception("Invalid optimization method")
-        if cf_model not in [0, 1]:
-            raise Exception("Invalid cost function model")
+        if not isinstance(opt_init_heuristic, OptimizationInitializationHeuristic):
+            opt_init_heuristic = OptimizationInitializationHeuristic(opt_init_heuristic)
+
+        if not isinstance(cf_model, CostFunction):
+            cf_model = CostFunction(cf_model)
+
+        if not isinstance(opt_method, OptimizationMethod):
+            opt_method = OptimizationMethod(opt_method)
+
         if self.verbose:
             print(f"Optimizing volume {volume} on frame {frame}")
         self._send_command(
             0x0B,  # 11
             volume,
             frame,
             repeats,
             max_itr,
-            min_lim,
-            max_lim,
+            float(min_lim),
+            float(max_lim),
             max_stall_itr,
             dframe,
-            opt_method,
-            cf_model,
+            opt_method.value,
+            cf_model.value,
+            opt_init_heuristic.value,
         )
 
     def saveFullDRR(self):
         """
         Save the full DRR.
 
         :raises AutoscoperServerError: If the server fails to save the full DRR
@@ -446,24 +520,23 @@
         self,
         volume,
         start_frame,
         end_frame,
         frame_skip=1,
         repeats=1,
         max_itr=1000,
-        min_lim=-3,
-        max_lim=3,
+        min_lim=-3.0,
+        max_lim=3.0,
         max_stall_itr=25,
-        opt_method=0,
-        cf_model=0,
+        opt_method=OptimizationMethod.PARTICLE_SWARM_OPTIMIZATION,
+        cf_model=CostFunction.NORMALIZED_CROSS_CORRELATION,
+        opt_init_heuristic=OptimizationInitializationHeuristic.PREVIOUS_FRAME,
     ):
         """
-        Automatically tracks the volume accross the given frames.
-
-        Currently using previous frame for intial guess.
+        Automatically tracks the volume across the given frames.
 
         :param volume: The id of the volume to be tracked
         :type volume: int
         :param start_frame: The frame to start the tracking on
         :type start_frame: int
         :param end_frame: The frame to end the tracking on
         :type end_frame: int
@@ -475,41 +548,45 @@
         :type max_itr: int
         :param min_lim: The minimum limit of the optimization
         :type min_lim: float
         :param max_lim: The maximum limit of the optimization
         :type max_lim: float
         :param max_stall_itr: The maximum number of iterations to stall
         :type max_stall_itr: int
-        :param opt_method: The optimization method to use, 0 for Particle Swarm, 1 for Downhill Simplex
-        :type opt_method: int
-        :param cf_model: The cost function model to use, 0 for NCC (Bone Models), 1 for Sum of Absolute Differences (Implant Models)
-        :type cf_model: int
+        :param opt_method: The optimization method to use.
+        :type opt_method: int or :const:`~OptimizationMethod`
+        :param cf_model: The cost function to use. :const:`~CostFunction.NORMALIZED_CROSS_CORRELATION` for Bone Models,  :const:`~CostFunction.SUM_OF_ABSOLUTE_DIFFERENCES` for Implant Models.
+        :type cf_model: int or :const:`~CostFunction`
+        :param opt_init_heuristic: The heuristic to initialize the optimization. See :const:`~OptimizationInitializationHeuristic`.
+        :type opt_init_heuristic: int or :const:`~OptimizationInitializationHeuristic`
+
         :raises AutoscoperServerError: If the server fails to track the volume
         :raises AutoscoperConnectionError: If the connection to the server is lost
+        :raises ValueError: If parameters accepting an enum value are incorrectly specified.
+
+        .. versionadded:: 2
+
+          The `opt_init_heuristic` parameter.
         """
         if self.verbose:
-            print(
-                f"Automated tracking of volume {volume} from frame {start_frame} to {end_frame}.\n"
-            )
+            print(f"Automated tracking of volume {volume} from frame {start_frame} to {end_frame}.\n")
         for frame in range(start_frame, end_frame):
             self.setFrame(frame=frame)
-            if frame != 0:
-                pose = self.getPose(volume=volume, frame=(frame - 1))
-                self.setPose(volume=volume, frame=frame, pose=pose)
             self.optimizeFrame(
                 volume=volume,
                 frame=frame,
                 repeats=repeats,
                 max_itr=max_itr,
                 min_lim=min_lim,
                 max_lim=max_lim,
                 max_stall_itr=max_stall_itr,
+                dframe=frame_skip,
                 opt_method=opt_method,
                 cf_model=cf_model,
-                dframe=frame_skip,
+                opt_init_heuristic=opt_init_heuristic,
             )
 
     def getNumVolumes(self):
         """
         Get the number of volumes in the scene.
 
         :return: The number of volumes in the scene
```

### Comparing `PyAutoscoper-1.1.3/pyproject.toml` & `PyAutoscoper-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 [project.optional-dependencies]
 dev = [
     "black>=22.3.0",
 ]
 
 [tool.black]
-line-length = 88
+line-length = 120
 target_version = ['py36']
 include = '\.pyi?$'
 
 [tool.setuptools_scm]
 root = "../.."
 git_describe_command = [
     'git',
```

