# Comparing `tmp/useq_schema-0.3.0.tar.gz` & `tmp/useq_schema-0.3.1.tar.gz`

## Comparing `useq_schema-0.3.0.tar` & `useq_schema-0.3.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 useq_schema-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 useq_schema-0.3.0/mkdocs.yml
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 useq_schema-0.3.0/setup.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 useq_schema-0.3.0/.github/dependabot.yml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 useq_schema-0.3.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 useq_schema-0.3.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 useq_schema-0.3.0/docs/api.md
--rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 useq_schema-0.3.0/docs/index.md
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 useq_schema-0.3.0/docs/images/favicon.ico
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 useq_schema-0.3.0/docs/schema/axes.md
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 useq_schema-0.3.0/docs/schema/event.md
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 useq_schema-0.3.0/docs/schema/hardware_autofocus.md
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 useq_schema-0.3.0/docs/schema/sequence.md
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 useq_schema-0.3.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/__init__.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_actions.py
--rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_base_model.py
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_channel.py
--rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_grid.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_hardware_autofocus.py
--rw-r--r--   0        0        0     6796 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_mda_event.py
--rw-r--r--   0        0        0    21704 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_mda_sequence.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_position.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_time.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_utils.py
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/_z.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 useq_schema-0.3.0/src/useq/py.typed
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 useq_schema-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0     5291 2020-02-02 00:00:00.000000 useq_schema-0.3.0/tests/test_autofocus.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 useq_schema-0.3.0/tests/test_grid.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 useq_schema-0.3.0/tests/test_misc.py
--rw-r--r--   0        0        0    18536 2020-02-02 00:00:00.000000 useq_schema-0.3.0/tests/test_position_sequence.py
--rw-r--r--   0        0        0    10261 2020-02-02 00:00:00.000000 useq_schema-0.3.0/tests/test_sequence.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 useq_schema-0.3.0/tests/test_serialization.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 useq_schema-0.3.0/tests/fixtures/mda.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 useq_schema-0.3.0/tests/fixtures/mda.yaml
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 useq_schema-0.3.0/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 useq_schema-0.3.0/LICENSE
--rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 useq_schema-0.3.0/README.md
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 useq_schema-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     9578 2020-02-02 00:00:00.000000 useq_schema-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 useq_schema-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 useq_schema-0.3.1/mkdocs.yml
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 useq_schema-0.3.1/setup.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 useq_schema-0.3.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 useq_schema-0.3.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 useq_schema-0.3.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 useq_schema-0.3.1/docs/api.md
+-rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 useq_schema-0.3.1/docs/index.md
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 useq_schema-0.3.1/docs/images/favicon.ico
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 useq_schema-0.3.1/docs/schema/axes.md
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 useq_schema-0.3.1/docs/schema/event.md
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 useq_schema-0.3.1/docs/schema/hardware_autofocus.md
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 useq_schema-0.3.1/docs/schema/sequence.md
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 useq_schema-0.3.1/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/__init__.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_actions.py
+-rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_base_model.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_channel.py
+-rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_grid.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_hardware_autofocus.py
+-rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_mda_event.py
+-rw-r--r--   0        0        0    21704 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_mda_sequence.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_position.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_time.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_utils.py
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/_z.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 useq_schema-0.3.1/src/useq/py.typed
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 useq_schema-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     5291 2020-02-02 00:00:00.000000 useq_schema-0.3.1/tests/test_autofocus.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 useq_schema-0.3.1/tests/test_grid.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 useq_schema-0.3.1/tests/test_misc.py
+-rw-r--r--   0        0        0    18536 2020-02-02 00:00:00.000000 useq_schema-0.3.1/tests/test_position_sequence.py
+-rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 useq_schema-0.3.1/tests/test_sequence.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 useq_schema-0.3.1/tests/test_serialization.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 useq_schema-0.3.1/tests/fixtures/mda.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 useq_schema-0.3.1/tests/fixtures/mda.yaml
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 useq_schema-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 useq_schema-0.3.1/LICENSE
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 useq_schema-0.3.1/README.md
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 useq_schema-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     9578 2020-02-02 00:00:00.000000 useq_schema-0.3.1/PKG-INFO
```

### Comparing `useq_schema-0.3.0/.pre-commit-config.yaml` & `useq_schema-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/mkdocs.yml` & `useq_schema-0.3.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/setup.py` & `useq_schema-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/.github/workflows/test_and_deploy.yml` & `useq_schema-0.3.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/docs/api.md` & `useq_schema-0.3.1/docs/api.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/docs/index.md` & `useq_schema-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/docs/images/favicon.ico` & `useq_schema-0.3.1/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/docs/schema/axes.md` & `useq_schema-0.3.1/docs/schema/axes.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/docs/stylesheets/extra.css` & `useq_schema-0.3.1/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/src/useq/__init__.py` & `useq_schema-0.3.1/src/useq/__init__.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/src/useq/_actions.py` & `useq_schema-0.3.1/src/useq/_actions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Union
+
 from typing_extensions import Literal
 
 from useq._base_model import FrozenModel
 
 
 class Action(FrozenModel):
     """Base class for a [`useq.MDAEvent`][] action.
@@ -50,7 +52,10 @@
         The number of retries if autofocus fails. By default, 3.
     """
 
     type: Literal["hardware_autofocus"] = "hardware_autofocus"
     autofocus_device_name: str
     autofocus_motor_offset: float
     max_retries: int = 3
+
+
+AnyAction = Union[HardwareAutofocus, AcquireImage]
```

### Comparing `useq_schema-0.3.0/src/useq/_base_model.py` & `useq_schema-0.3.1/src/useq/_base_model.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/src/useq/_channel.py` & `useq_schema-0.3.1/src/useq/_channel.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/src/useq/_grid.py` & `useq_schema-0.3.1/src/useq/_grid.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/src/useq/_hardware_autofocus.py` & `useq_schema-0.3.1/src/useq/_hardware_autofocus.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/src/useq/_mda_event.py` & `useq_schema-0.3.1/src/useq/_mda_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Optional,
     Sequence,
     Tuple,
 )
 
 from pydantic import Field, validator
 
-from useq._actions import AcquireImage, Action
+from useq._actions import AcquireImage, AnyAction
 from useq._base_model import UseqModel
 from useq._utils import ReadOnlyDict
 
 if TYPE_CHECKING:
     from useq._mda_sequence import MDASequence
 
     ReprArgs = Sequence[Tuple[Optional[str], Any]]
@@ -134,15 +134,15 @@
     pos_name: Optional[str] = None
     x_pos: Optional[float] = None
     y_pos: Optional[float] = None
     z_pos: Optional[float] = None
     sequence: Optional[MDASequence] = Field(default=None, repr=False)
     properties: Optional[List[PropertyTuple]] = None
     metadata: Dict[str, Any] = Field(default_factory=dict)
-    action: Action = Field(default_factory=AcquireImage)
+    action: AnyAction = Field(default_factory=AcquireImage)
     keep_shutter_open: bool = False
 
     # action
     # keep shutter open between channels/steps
     @property
     def global_index(self) -> int:
         warnings.warn(
```

### Comparing `useq_schema-0.3.0/src/useq/_mda_sequence.py` & `useq_schema-0.3.1/src/useq/_mda_sequence.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/src/useq/_position.py` & `useq_schema-0.3.1/src/useq/_position.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/src/useq/_time.py` & `useq_schema-0.3.1/src/useq/_time.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/src/useq/_utils.py` & `useq_schema-0.3.1/src/useq/_utils.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/src/useq/_z.py` & `useq_schema-0.3.1/src/useq/_z.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/tests/conftest.py` & `useq_schema-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/tests/test_autofocus.py` & `useq_schema-0.3.1/tests/test_autofocus.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/tests/test_grid.py` & `useq_schema-0.3.1/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/tests/test_position_sequence.py` & `useq_schema-0.3.1/tests/test_position_sequence.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/tests/test_sequence.py` & `useq_schema-0.3.1/tests/test_sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,7 +317,12 @@
     with pytest.warns(UserWarning, match="got unknown keyword arguments"):
         Position(random_key="random_value")
 
 
 def test_skip_channel_do_stack_no_zplan():
     mda = MDASequence(channels=[{"config": "DAPI", "do_stack": False}])
     assert len(list(mda)) == 1
+
+
+def test_event_action_union() -> None:
+    # test that action unions work
+    MDAEvent(action={"autofocus_device_name": "Z", "autofocus_motor_offset": 25})
```

### Comparing `useq_schema-0.3.0/tests/fixtures/mda.json` & `useq_schema-0.3.1/tests/fixtures/mda.json`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/tests/fixtures/mda.yaml` & `useq_schema-0.3.1/tests/fixtures/mda.yaml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/.gitignore` & `useq_schema-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/LICENSE` & `useq_schema-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/README.md` & `useq_schema-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/pyproject.toml` & `useq_schema-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.0/PKG-INFO` & `useq_schema-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useq-schema
-Version: 0.3.0
+Version: 0.3.1
 Summary: Schema for multi-dimensional microscopy experiments
 Project-URL: Source, https://github.com/pymmcore-plus/useq-schema
 Project-URL: Tracker, https://github.com/pymmcore-plus/useq-schema/issues
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Keywords: microscopy,schema
```

