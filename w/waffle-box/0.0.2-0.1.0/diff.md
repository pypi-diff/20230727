# Comparing `tmp/waffle_box-0.0.2.tar.gz` & `tmp/waffle_box-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_box-0.0.2.tar", max compression
+gzip compressed data, was "waffle_box-0.1.0.tar", max compression
```

## Comparing `waffle_box-0.0.2.tar` & `waffle_box-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      647 2023-07-17 01:24:46.969274 waffle_box-0.0.2/README.md
--rw-r--r--   0        0        0      141 2023-07-21 04:10:43.147871 waffle_box-0.0.2/app_manager/__init__.py
--rw-r--r--   0        0        0     9018 2023-07-21 09:26:55.273182 waffle_box-0.0.2/app_manager/app_manager.py
--rw-r--r--   0        0        0     2898 2023-07-21 06:59:24.736512 waffle_box-0.0.2/app_manager/app_structure.py
--rw-r--r--   0        0        0     2060 2023-07-21 03:54:46.601453 waffle_box-0.0.2/app_manager/nvinfer_config_parser.py
--rw-r--r--   0        0        0       83 2023-07-14 01:41:24.140847 waffle_box-0.0.2/maker_manager/__init__.py
--rw-r--r--   0        0        0     2359 2023-07-21 06:58:47.380531 waffle_box-0.0.2/maker_manager/convert_option.py
--rw-r--r--   0        0        0     9925 2023-07-21 09:06:57.535079 waffle_box-0.0.2/maker_manager/maker_manager.py
--rw-r--r--   0        0        0      599 2023-07-21 09:27:26.724869 waffle_box-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      119 2023-07-21 07:13:17.494080 waffle_box-0.0.2/waffle_box/__init__.py
--rw-r--r--   0        0        0     2579 2023-07-14 06:58:20.777371 waffle_box-0.0.2/waffle_box/bake_service.py
--rw-r--r--   0        0        0     4281 2023-07-21 09:24:44.814491 waffle_box-0.0.2/waffle_box/cli.py
--rw-r--r--   0        0        0     5048 2023-07-21 08:48:35.416144 waffle_box-0.0.2/waffle_box/convert_service.py
--rw-r--r--   0        0        0     2229 2023-07-21 09:08:04.510093 waffle_box-0.0.2/waffle_box/pull_service.py
--rw-r--r--   0        0        0       67 2023-07-17 00:29:45.225470 waffle_box-0.0.2/waffle_box_exception/__init__.py
--rw-r--r--   0        0        0     1512 2023-07-21 03:54:46.601453 waffle_box-0.0.2/waffle_box_exception/waffle_box_exception.py
--rw-r--r--   0        0        0     1193 1970-01-01 00:00:00.000000 waffle_box-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      781 2023-07-27 05:40:09.951813 waffle_box-0.1.0/README.md
+-rw-r--r--   0        0        0      141 2023-07-27 05:40:09.951813 waffle_box-0.1.0/app_manager/__init__.py
+-rw-r--r--   0        0        0     9411 2023-07-27 05:40:09.951813 waffle_box-0.1.0/app_manager/app_manager.py
+-rw-r--r--   0        0        0     2786 2023-07-27 05:40:09.951813 waffle_box-0.1.0/app_manager/app_structure.py
+-rw-r--r--   0        0        0     2304 2023-07-27 05:40:09.951813 waffle_box-0.1.0/app_manager/nvinfer_config_parser.py
+-rw-r--r--   0        0        0       83 2023-07-27 05:40:09.951813 waffle_box-0.1.0/maker_manager/__init__.py
+-rw-r--r--   0        0        0     2476 2023-07-27 05:40:09.955814 waffle_box-0.1.0/maker_manager/convert_option.py
+-rw-r--r--   0        0        0     9703 2023-07-27 05:40:09.955814 waffle_box-0.1.0/maker_manager/maker_manager.py
+-rw-r--r--   0        0        0      645 2023-07-27 05:40:09.955814 waffle_box-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-07-27 05:40:09.955814 waffle_box-0.1.0/waffle_box/__init__.py
+-rw-r--r--   0        0        0     3231 2023-07-27 05:40:09.955814 waffle_box-0.1.0/waffle_box/bake_service.py
+-rw-r--r--   0        0        0     6280 2023-07-27 05:40:09.955814 waffle_box-0.1.0/waffle_box/cli.py
+-rw-r--r--   0        0        0     4486 2023-07-27 05:40:09.955814 waffle_box-0.1.0/waffle_box/convert_service.py
+-rw-r--r--   0        0        0     2262 2023-07-27 05:40:09.955814 waffle_box-0.1.0/waffle_box/pull_service.py
+-rw-r--r--   0        0        0       67 2023-07-27 05:40:09.955814 waffle_box-0.1.0/waffle_box_exception/__init__.py
+-rw-r--r--   0        0        0     1573 2023-07-27 05:40:09.955814 waffle_box-0.1.0/waffle_box_exception/waffle_box_exception.py
+-rw-r--r--   0        0        0     1327 1970-01-01 00:00:00.000000 waffle_box-0.1.0/PKG-INFO
```

### Comparing `waffle_box-0.0.2/app_manager/app_manager.py` & `waffle_box-0.1.0/app_manager/app_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,40 +11,29 @@
 
 
 class AppManager:
     """ Base App을 파싱하고 새로운 App을 생성
 
     Base App을 파싱 후 모델을 교체해 새로운 App을 생성한다.
 
-    # Attributes
-    - workspace: Path
-        - 작업할 경로
-        - 일반적으로 ~/.waffle_box
-    - app_structure: AppStructure
-        - 작업할 App의 구조
+    Attributes:
+        workspace (Path): 작업할 경로로 일반적으로 ~/.waffle_box 사용
+        app_structure (AppStructure): 작업할 App의 구조
 
     """
 
     def __init__(self, workspace: Path, app_path: Path) -> None:
         """
-        # Parameters
-        - workspace: Path
-            - 작업할 경로
-        - app_path: Path
-            - Base 앱 경로
-
-        # Raises
-        - IOError
-            - workspace를 생성할 수 없음
-        - AppParsingError
-            - App parsing error
-
-        # Raises
-        - APP_STRUCTURE_EXCEPTION
-        - APP_CONFIG_ERROR
+        Args: 
+            workspace (Path): 작업할 경로
+            app_path (Path): Base 앱 경로
+
+        Raises:
+            APP_STRUCTURE_EXCEPTION
+            APP_CONFIG_ERROR
 
         """
         self.workspace: Path = workspace
 
         self._app_structure: AppStructure = self._extract_app(app_path)
 
     def _extract_app(self, app_path: Path) -> AppStructure:
@@ -52,17 +41,20 @@
 
         입력받은 App 파일을 workspace의 temp 폴더에 압축 해제한다.
         만약 temp 파일이 이미 존재한다면 폴더를 삭제하고 압축을 새로 해제한다.
 
         App 파일 내부 모델도 모두 압축 해제 후 
         model info를 담은 AppStructure를 반환한다.
 
-        # Raises
-        - APP_STRUCTURE_EXCEPTION
-        - APP_CONFIG_ERROR
+        Args:
+            app_path (Path): App 경로
+
+        Raises:
+            APP_STRUCTURE_EXCEPTION
+            APP_CONFIG_ERROR
 
         """
         if not app_path.exists():
             raise WaffleBoxException('Wrong input file.', ExceptionCode.APP_NO_SUCH_FILE)
         
         # app 압축을 풀 임시 폴더
         temp_dir = self.workspace.joinpath('temp')
@@ -118,16 +110,19 @@
         """ 모델 압축 풀기
 
         모델 파일은 zip 파일 이름과 동일한 이름의 폴더에 압축을 푼다.
         예) PeopleNet.zip -> PeopleNet 폴더에 압축 풀기
 
         압축을 풀면 zip 파일을 삭제한다.
 
-        # Return
-        - 모델 파일을 압축 푼 위치
+        Args:
+            model_path (Path): 모델 경로
+
+        Return:
+            모델 파일을 압축 푼 위치
 
         """
         model_dir = self._remove_extention(model_path.name)
         model_dir = model_path.parent.joinpath(model_dir)
 
         zip_file = ZipFile(model_path)
         zip_file.extractall(model_dir)
@@ -140,16 +135,22 @@
     def _make_model_info(self, model_path: Path, model_id: UUID,
                          model_name: str, model_precision: str) -> ModelInfo:
         """ 압축 푼 모델 폴더에서 정보를 추출한다.
 
         압축 푼 모델 폴더의 infer_nvinfer_config.txt 파일을 읽고
         필요한 정보들을 추출한다.
 
-        # Raises
-        - APP_CONFIG_ERROR
+        Args:
+            model_path (Path): 모델 경로
+            model_id (UUID): 모델 id
+            model_name (str): 모델 이름
+            model_precision (str): 모델 precision
+
+        Raises:
+            APP_CONFIG_ERROR
 
         """
         nvinfer_parser = NvinferConfigParser(
             model_path.joinpath('infer_nvinfer_config.txt'))
 
         engine_file_name = nvinfer_parser.get('model-engine-file')
         if not engine_file_name:
@@ -172,30 +173,32 @@
             id=model_id, name=model_name, precision=model_precision,
             engine_file_name=engine_file_name, input_dims=input_dims,
             max_batch_size=batch_size, path=model_path,
         )
 
     def _remove_extention(self, file_name: str) -> str:
         """ 파일 이름에서 마지막 확장자 명을 제거한다.
+
+        Args:
+            file_name (str): 확장자 명을 제거할 파일 경로 스트링
         """
         return file_name[:file_name.rfind('.')]
 
     def replace_model(self, model_id: UUID, new_model: Path) -> None:
         """ 모델의 trt 엔진 파일을 교체한다.
 
         입력한 id에 해당하는 모델의 trt 엔진 파일을 새로운 trt 엔진 파일로 교체한다.
 
-        # Parameters
-        - model_id
-        - new_model
-
-        # Raises
-        - APP_NO_SUCH_FILE
-            - 기존 모델의 엔진 파일이 존재하지 않음
-            - 새로운 모델 파일이 존재하지 않음
+        Args:
+            model_id (UUID): 교체할 모델의 id
+            new_model (Path): 새로운 모델 주소
+
+        Raises:
+            APP_NO_SUCH_FILE: 기존 모델의 엔진 파일이 존재하지 않음,
+                새로운 모델 파일이 존재하지 않음
 
         """
         model = self._app_structure.find_model_by_id(model_id)
 
         if not model:
             raise WaffleBoxException(
                 f'No such model: ID - {model_id}', ExceptionCode.APP_NO_SUCH_FILE)
@@ -216,21 +219,19 @@
         shutil.copyfile(new_model, origin_model)
 
     def package(self, output: Path) -> None:
         """ 새로운 App으로 생성한다.
 
         엔진 파일 교체가 끝나면 새로운 App으로 패키징한다.
 
-        # Parameters
-        - output
-            - App 저장 경로
-
-        # Raises
-        - APP_FILE_ALREADY_EXIST
-            - output 파일이 이미 존재함
+        Args:
+            output (Path): App 저장 경로
+
+        Raises:
+            APP_FILE_ALREADY_EXIST: output 파일이 이미 존재함
 
         """
         if output.exists():
             raise WaffleBoxException(
                 f'File already exists: {output}', ExceptionCode.APP_FILE_ALREADY_EXIST)
 
         for model in self._app_structure.models:
@@ -253,20 +254,26 @@
 
     def find_model_info_by_id(self, id: UUID) -> ModelInfo | None:
         """ App의 모델 정보를 id로 찾는다.
 
         App의 모델 정보를 id로 찾는다. 
         만약 없다면 None을 리턴한다.
 
+        Args:
+            id (UUID): 찾고싶은 모델의 id
+
         """
         return self._app_structure.find_model_by_id(id)
 
     def find_model_info_by_name(self, name: str) -> ModelInfo | None:
         """ App의 모델 정보를 이름으로 찾는다.
 
         App의 모델 정보를 이름으로 찾는다.
         만약 없다면 None을 리턴한다.
+
+        Args:
+            name (str): 찾고싶은 모델의 이름
         """
         return self._app_structure.find_model_by_name(name)
 
 if __name__ == '__main__':
     ap = AppManager(Path('/'), Path('/'))
```

### Comparing `waffle_box-0.0.2/app_manager/app_structure.py` & `waffle_box-0.1.0/app_manager/app_structure.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,36 +6,28 @@
 from pathlib import Path
 
 
 @dataclass(frozen=True)
 class ModelInfo:
     """ 모델 정보
 
-    모델의 기본 정보를 저장한다. (변경 불가)
+    모델의 기본 정보를 저장한다. (불변값)
 
-    # Attributes
-    - id: UUID
-        - model.json에 기술되어 있는 모델의 uuid
-    - name: str
-        - model.json에 기술되어 있는 모델의 이름
-    - precision: str
-        - 모델의 precision
-        - fp32, fp16, int8 중 하나
-    - engine_file_name
-        - engine 파일 이름
-        - 보통 model.engine
-    - input_dims
-        - 모델의 input shape, x로 구분
-        - 예) 3x640x640
-    - batch_size
-        - 모델의 batch size
-        - Autocare-D는 기본적으로 dynamic batch를 가정하므로
-        모델에 적혀있는 batch-size는 max batch size로 간주한다.
-    - path: Path
-        - 모델 폴더 경로
+    Attributes:
+        id (UUID): model.json에 기술되어 있는 모델의 uuid
+        name (str): model.json에 기술되어 있는 모델의 이름
+        precision (str): 모델의 precision, 
+            fp32, fp16, int8 중 하나
+        engine_file_name (str): engine 파일 이름, 보통 model.engine
+        input_dims (str): 모델의 input shape, x로 구분
+            예) 3x640x640
+        max_batch_size (int): 모델의 batch size
+            Autocare-D는 기본적으로 dynamic batch를 가정하므로
+            모델에 적혀있는 batch-size는 max batch size로 간주한다.
+        path (Path): 모델 폴더 경로
 
     """
 
     id: UUID
     name: str
     precision: str
     engine_file_name: str
@@ -59,59 +51,50 @@
 
 @dataclass(frozen=True)
 class AppStructure:
     """ App 구조 정보
 
     App의 구조 정보를 저장한다. (변경 불가)
 
-    # Attributes
-    - id: UUID
-        - app.json에 기술되어 있는 App의 UUID
-    - models: List[ModelInfo]
-        - App이 모델 정보 리스트
-    - path: Path
-        - App을 압축 푼 경로
+    Attributes: 
+        id (UUID): app.json에 기술되어 있는 App의 UUID
+        models (List[ModelInfo]): App이 모델 정보 리스트
+        path (Path): App을 압축 푼 경로
 
     """
     id: UUID
     models: List[ModelInfo]
     path: Path
 
     def find_model_by_id(self, id: UUID) -> ModelInfo | None:
         """ id 값으로 모델을 찾는다.
 
-        # Parameters
-        - id
-            - 찾는 모델의 uuid
-
-        # Returns
-        - ModelInfo
-            - 입력한 id와 일치하는 모델
-        - None
-            - 입력한 id와 일치하는 모델을 찾지 못했을 때
+        Args:
+            id (UUID): 찾는 모델의 uuid
+
+        Returns:
+            ModelInfo: 입력한 id와 일치하는 모델
+            None: 입력한 id와 일치하는 모델을 찾지 못했을 때
 
         """
         for m in self.models:
             if m.id == id:
                 return m
 
         return None
 
     def find_model_by_name(self, name: str) -> ModelInfo | None:
         """ 이름으로 모델을 찾는다.
 
-        # Parameters
-        - name
-            - 찾는 모델의 이름
-
-        # Returns
-        - ModelInfo
-            - 입력한 이름과 일치하는 모델
-        - None
-            - 입력한 이름과 일치하는 모델을 찾지 못했을 때
+        Args:
+            name (str): 찾는 모델의 이름
+
+        Returns:
+            ModelInfo: 입력한 이름과 일치하는 모델
+            None: 입력한 이름과 일치하는 모델을 찾지 못했을 때
 
         """
         for m in self.models:
             if m.name == name:
                 return m
 
         return None
```

### Comparing `waffle_box-0.0.2/app_manager/nvinfer_config_parser.py` & `waffle_box-0.1.0/app_manager/nvinfer_config_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,40 +7,41 @@
 
     정확한 trt 엔진 변환을하기 위해 nvinfer config 파일을 읽고
     변환 설정 값을 만들기 위해 사용된다.
 
     설정값 접근은 get함수로 config 파일의 key 값을 입력해 찾는다.
     key값이 없을 경우 Exception을 발생한다.
 
-    # Attributes:
-    - _configs
-        - config값을 저장하는 dictionary
+    Attributes:
+        _configs (dict[str, str]): config값을 저장하는 dictionary
 
     """
 
     def __init__(self, file: Path) -> None:
         """
-        # Parameters
-        - file
-            - config 파일 위치 
-            - 예) /home/yoon/.waffle_box/temp/car_make_net_v0.1.0a/infer_nvinfer_config.txt
+        Args:
+            file (Path): config 파일 위치 
+                예) /home/yoon/.waffle_box/temp/car_make_net_v0.1.0a/infer_nvinfer_config.txt
 
         """
         self._configs: dict[str, str] = {}
 
         self._read_config_file(file)
 
     def _read_config_file(self, file: Path) -> None:
         """ config 파일 파싱
 
         config 파일을 읽고 설정 값만 _configs에 저장한다.
 
-        # Raises
-        - APP_NO_SUCH_FILE
-        - APP_CONFIG_ERROR
+        Args:
+            file (Path): nvinfer config 파일 경로
+
+        Raises:
+            APP_NO_SUCH_FILE: 파일 없음
+            APP_CONFIG_ERROR
 
         """
         try:
             with open(file) as f:
                 lines = f.readlines()
 
                 for l in lines:
@@ -61,9 +62,16 @@
 
     def get(self, key: str) -> str | None:
         """ config 값 읽어오기
 
         key를 통해 config 값을 읽어온다.
         key값이 존재하지 않을경우 None을 리턴한다.
 
+        Args:
+            key (str): 읽어올 설정값의 키
+        
+        Returns:
+            str: 읽어온 key의 값
+            None: key 없음
+
         """
         return self._configs.get(key)
```

### Comparing `waffle_box-0.0.2/maker_manager/convert_option.py` & `waffle_box-0.1.0/maker_manager/convert_option.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,48 +2,48 @@
 from waffle_box_exception import WaffleBoxException, ExceptionCode
 
 
 @dataclass(frozen=True)
 class ONNXConvConfigs:
     """ trt 엔진 변환을 위해 필요한 설정 값 정보
 
-    # Attributes
-    - precision
-        - 모델의 precision
-        - fp32, fp16, int8 중 하나
-    - input_shape
-        - 모델의 input shape
-        - dynamic batch를 사용하기 위해 trtexec에 
-        min, opt, max input shape을 입력할 때 사용
-    - max_batch
-        - 모델의 최대 batch 크기
-        - min, opt, max input shape의 batch 크기를 결정할 때 사용
+    Attributes:
+        precision (str): 모델의 precision,
+            fp32, fp16, int8 중 하나
+        input_shape (str): 모델의 input shape
+            dynamic batch를 사용하기 위해 trtexec에 
+            min, opt, max input shape을 입력할 때 사용
+        max_batch (int): 모델의 최대 batch 크기
+            min, opt, max input shape의 batch 크기를 결정할 때 사용
 
     """
 
     precision: str
     input_shapes: str
     max_batch: int
 
     def to_trtexec_args(self) -> list[str]:
         """ trtexec 변환에 필요한 argument 리스트로 변환
 
         ONNXConvConfigs의 값을 trtexec 변환에 필요한 argument 리스트로 변환한다.
 
-        # precision
-        trtexec의 precision 기본값은 fp32이므로 fp32일때는 아무런 옵션을 생성하지 않는다.
-        fp16일 경우 --fp16, int8일 경우 --int8을 리턴한다.
-
-        # input_shape & max_batch
-        dynamic batch를 사용하기 위해 min, opt, max shape을 설정해야 한다.  
-        모델의 input_shape은 그대로 사용하며 batch size는 min=1, opt=max_batch/2, max=max_batch로 설정한다.
-
-        # output_name
-        App의 원본 엔진파일 이름을 맞추기 위해 설정한다.
-        --saveEngine=<output_name>
+        precision:
+            trtexec의 precision 기본값은 fp32이므로 fp32일때는 아무런 옵션을 생성하지 않는다.
+            fp16일 경우 --fp16, int8일 경우 --int8을 리턴한다.
+
+        input_shape & max_batch:
+            dynamic batch를 사용하기 위해 min, opt, max shape을 설정해야 한다.  
+            모델의 input_shape은 그대로 사용하며 batch size는 min=1, opt=max_batch/2, max=max_batch로 설정한다.
+
+        output_name:
+            App의 원본 엔진파일 이름을 맞추기 위해 설정한다.
+            --saveEngine=<output_name>
+        
+        Returns:
+            list[str]: trtexec에 필요한 argument 리스트
 
         """
 
         args: list[str] = []
 
         # precision
         if self.precision == 'fp16':
```

### Comparing `waffle_box-0.0.2/maker_manager/maker_manager.py` & `waffle_box-0.1.0/maker_manager/maker_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,35 +13,34 @@
 
 class MakerManager:
     """Waffle Maker Manager
 
     ONNX 파일을 TensorRT 엔진 파일로 변환하는 Waffle Maker를 관리하는 클래스.
     이미지 다운로드, 모델 파일 변환 등의 기능을 제공한다.
 
-    # Attributes
-    - img_tag: str
-        - 실행할 이미지 태그
-    - gpu_num: int
-        - 컨테이너를 동작할 gpu 번호
+    Attributes:
+        img_tag (str): 실행할 이미지 태그
+        gpu_num (int): 컨테이너를 동작할 gpu 번호
+        container_id (int | None): 실행한 컨테이너 ID로 
+            컨테이너를 정상적으로 종료시키지 못했을 때 회수하기 위해 저장한다.
+            None일경우 회수할 컨테이너 없음
+        workspace (Path): 압축푸는 작업 등 파일 관리를 위한 workspace
+        client (DockerClient): 도커 클라이언트
+    
     """
 
     def __init__(self, img_tag: str, gpu_num: int, workspace: Path) -> None:
         """
-        # Parameters
-        - img_tag: str
-            - 실행할 이미지 태그
-        - gpu_num: str
-            - 컨테이너를 동작할 gpu 번호
-        - workspace: Path
-            - 작업할 경로
-            - 일반적으로 ~/.waffle_box
+        Args: 
+            img_tag (str): 실행할 이미지 태그
+            gpu_num (str): 컨테이너를 동작할 gpu 번호
+            workspace (Path): 작업할 경로, 일반적으로 ~/.waffle_box
             
-        # Raises
-        - DockerDaemonError
-            - Docker daemon에 접속 불가
+        Raises:
+            DockerDaemonError: Docker daemon에 접속 불가
 
         """
         self.img_tag = img_tag
         self.gpu_num = gpu_num
         self.container_id = None
         self.workspace = workspace
 
@@ -57,17 +56,17 @@
             )
 
     def check_image_exist_at_local(self) -> bool:
         """로컬에 이미지가 설치되어 있는지 확인한다.
 
         MakerManager를 생성할 때 입력한 이미지 태그가 로컬에 존재하는지 확인한다.
 
-        # Returns
-        -True: 이미지가 설치되어 있음
-        -False: 이미지가 설치되어 있지 않음
+        Returns:
+            True: 이미지가 설치되어 있음
+            False: 이미지가 설치되어 있지 않음
         """
         try:
             self.client.images.get(self.img_tag)
 
         except Exception as e:
             return False
 
@@ -77,29 +76,22 @@
         self, print_output: bool, id: str = "", pw: str = ""
     ) -> None:
         """로컬에 이미지를 다운받는다.
 
         MakerManager를 생성할 때 입력한 이미지 태그를 로컬에 다운받는다.
         만약 id와 pw를 입력했다면 docker hub에 로그인을 한 후 다운받는다.
 
-        # Parameters
-        - id: str
-            - docker hub id
-            - 빈값이라면 로그인을 하지 않는다.
-        - pw: str
-            - docker hub password
-            - 빈값이라면 로그인을 하지 않는다.
-
-        # Raises
-        - LoginError
-            - id 혹은 pw가 잘못됨
-        - AlreadExistError
-            - 이미 이미지가 설치되어 있음
-        - PermissionError
-            - 이미지를 설치할 권한이 없음
+        Args:
+            id (str): docker hub id, 빈값이라면 로그인을 하지 않는다.
+            pw (str): docker hub password, 빈값이라면 로그인을 하지 않는다.
+
+        Raises:
+            LoginError: id 혹은 pw가 잘못됨
+            AlreadExistError: 이미 이미지가 설치되어 있음
+            PermissionError: 이미지를 설치할 권한이 없음
 
         """
         if id and pw:
             try:
                 self.client.login(id, pw)
 
             except docker.errors.APIError as e:
@@ -161,30 +153,23 @@
         print_output: bool,
     ) -> None:
         """입력한 모델 파일을 trt 엔진으로 변환
 
         입력한 모델을 컨테이너 내부에서 TensorRT 엔진으로 변환한다.
         변환한 모델은 output path에 저장한다.
 
-        # Parameters
-        - input: Path
-            - 변환할 모델 경로
-        - output: Path
-            - 변환한 모델 저장 경로
-        - convert_config: ONNXConvConfigs
-            - trtexec를 실행할 os.remove('temp.tar') 때 필요한 설정값들
-        - print_output: bool
-            - container 출력 결과 표시 여부
-
-        # Raises
-        - IOError
-            - input 파일이 존재하지 않음
-            - output 파일이 이미 존재함
-        - ConvertError
-            - 변환 실패
+        Args:
+            input (Path): 변환할 모델 경로
+            output (Path): 변환한 모델 저장 경로
+            convert_config (ONNXConvConfigs): trtexec를 실행할 os.remove('temp.tar') 때 필요한 설정값들
+            print_output (bool): container 출력 결과 표시 여부
+
+        Raises:
+            IOError: input 파일이 존재하지 않음, output 파일이 이미 존재함
+            ConvertError: 변환 실패
 
         """
 
         def create_tar_file(input_path: Path):
             def set_permissions(tarinfo):
                 tarinfo.mode = 0o777
                 return tarinfo
@@ -286,18 +271,7 @@
     def exit_container_handler(self):
         try:
             container = self.client.containers.get(self.container_id)
             container.kill()
         
         except Exception as e:
             pass
-
-
-if __name__ == '__main__':
-    manager = MakerManager('snuailab/trt:8.5.2.2', 0)
-    
-    if not manager.check_image_exist_at_local():
-        manager.pull_image_at_local(id='snuailab', pw='init123!!', print_output=True)
-    
-    manager.convert_onnx_to_engine_at_local(Path("model.onnx"), Path("model.engine"), None, print_output=True)
-
-    del manager
```

### Comparing `waffle_box-0.0.2/pyproject.toml` & `waffle_box-0.1.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "waffle-box"
-version = "0.0.2"
+version = "0.1.0"
 description = ""
 authors = ["SangHyeukYoon <shyoon@snuailab.ai>"]
 readme = "README.md"
 packages = [
     { include = "waffle_box" },
     { include = "app_manager" },
     { include = "maker_manager" },
@@ -21,7 +21,11 @@
 
 [tool.poetry.scripts]
 wb = "waffle_box.cli:app"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[virtualenvs]
+create = true
+in-project = true
```

### Comparing `waffle_box-0.0.2/waffle_box/bake_service.py` & `waffle_box-0.1.0/waffle_box/bake_service.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from maker_manager import MakerManager, ONNXConvConfigs
+from waffle_box_exception.waffle_box_exception import ExceptionCode, WaffleBoxException
 
 from pathlib import Path
+import re
 
 
 class BakeService:
     """ ONNX 모델을 trt 엔진으로 변환
 
     사용자가 입력한 ONNX 모델을 타겟 Autocare-D 버전에 맞춰 trt 엔진 파일로 변환한다.
 
-    # 실행 순서
-    1. is_local_maker_installed
-        Waffle Maker 이미지가 로컬에 설치되어 있는지 확인한다.
-    2. convert_model
-        모델을 trt 엔진으로 변환한다.
-
-    # Attributes
-    - workspace
-        - 작업할 경로
-        - 일반적으로 ~/.waffle_box
-    - origin_app_path
-        - 사용자가 입력한 기존 App 경로
-    - final_app_path
-        - 새로운 App을 저장할 경로
-    - img_tag
-        - trt 변환을 위한 컨테이너 태그명
-    - maker_manager
-        - MakerManager
+    실행 순서:
+        1. is_local_maker_installed: Waffle Maker 이미지가 
+            로컬에 설치되어 있는지 확인한다.
+        2. convert_model: 모델을 trt 엔진으로 변환한다.
+
+    Attributes:
+        workspace (Path): 작업할 경로, 일반적으로 ~/.waffle_box
+        origin_app_path (Path): 사용자가 입력한 기존 App 경로
+        final_app_path (Path): 새로운 App을 저장할 경로
+        img_tag (str): trt 변환을 위한 컨테이너 태그명
+        maker_manager (MakerManager): maker manager
 
     """
 
     def __init__(self, workspace: Path, input: Path, output: Path, dx_target_version: str, gpu_num: int) -> None:
         """
-        # Parameters
-        - workspace
-            - 작업할 경로
-        - input
-            - 변환할 모델 경로
-        - output
-            - 변환한 trt 엔진 파일을 저장할 경로
-        - dx_target_version
-            - 변환할 App의 target Autocare-D 버전
-        - gpu_num
-            - 작업할 GPU 번호
+        Args:
+            workspace (Path): 작업할 경로
+            input (Path): 변환할 모델 경로
+            output (Path): 변환한 trt 엔진 파일을 저장할 경로
+            dx_target_version (str): 변환할 App의 target Autocare-D 버전
+            gpu_num (int): 작업할 GPU 번호
 
-        # Raises
-        - MakerManagerError
+        Raises:
+            MakerManagerError
 
         """
         self.workspace: Path = workspace
         self.origin_model_path: Path = input
         self.final_model_path: Path = output
 
         # TODO: make image tag converter
         self.img_tag = 'snuailab/trt:8.5.2.2'
 
-        self.maker_manager = MakerManager(self.img_tag, gpu_num=gpu_num)
+        self.maker_manager = MakerManager(self.img_tag, gpu_num, workspace)
 
     def is_local_maker_installed(self) -> bool:
         """ Waffle maker가 local에 설치되어 있는가?
+
+        Returns:
+            True: 설치되어 있음
+            False: 설치되어 있지 않음
         """
         return self.maker_manager.check_image_exist_at_local()
 
-    def convert_model(self, print_output: bool, precision: str) -> None:
+    def convert_model(self, print_output: bool, precision: str, input_shapes: str, max_batch: int) -> None:
         """ 모델 변환
 
-        # Parameters
-        - print_output
-            - 변환 과정 출력 여부
-        - precision
-            - 모델의 precision
-            - fp32, fp16, int8 중 하나
+        Args:
+            print_output (bool): 변환 과정 출력 여부
+            precision (str): 모델의 precision,
+                fp32, fp16, int8 중 하나
+            input_shapes (str): 모델의 인풋 크기, {channel}x{width}x{height} 포맷
+                예) 3x640x640
 
-        # Raises
-        - MakerManager
+        Raises:
+            INVALID_ARGUMENT: input shapes의 포맷이 잘못됨
 
         """
-        onnx_config = ONNXConvConfigs(precision=precision)
+        # validate input shapes
+        p = re.compile(r'\d+x\d+x\d+')
+        m = p.match(input_shapes)
+
+        if m == None or m.start() != 0 or m.end() != len(input_shapes):
+            raise WaffleBoxException('Invalid input shapes', ExceptionCode.INVALID_ARGUMENT)
+
+        onnx_config = ONNXConvConfigs(precision, input_shapes, max_batch)
         self.maker_manager.convert_onnx_to_engine_at_local(input=self.origin_model_path,
                                                            output=self.final_model_path,
                                                            convert_config=onnx_config,
                                                            print_output=print_output)
```

### Comparing `waffle_box-0.0.2/waffle_box/convert_service.py` & `waffle_box-0.1.0/waffle_box/convert_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,62 +7,44 @@
 
 
 class ConvertService:
     """ 기존 앱을 바탕으로 새로운 앱을 생성
 
     기존 앱에서 모델을 교체해 새로운 앱을 생성한다.
 
-    # 실행 순서
-    1. is_local_maker_installed
-        waffle maker가 local에 설치되어 있는지 확인한다.
-    2. get_model_info
-        입력한 App의 모델 정보를 받아온다.
-    3. add_convert_info
-        모델 정보를 바탕으로 변경할 모델들을 입력한다.
-    4. convert_models
-        입력한 모델을 변환하고 기존 App에서 교체한다.
-    5. package_app
-        새로운 앱으로 패키징한다.
-
-    # Attributes
-    - workspace
-        - 작업할 경로
-        - 일반적으로 ~/.waffle_box
-    - origin_app_path
-        - 사용자가 입력한 기존 App 경로
-    - final_app_path
-        - 새로운 App을 저장할 경로
-    - img_tag
-        - trt 변환을 위한 컨테이너 태그명
-    - convert_list
-        - 변경할 모델 리스트
-    - app_manager
-        - AppManager
-    - maker_manager
-        - MakerManager
+    실행 순서:
+        1. is_local_maker_installed: waffle maker가 local에 설치되어 있는지 확인한다.
+        2. get_model_info: 입력한 App의 모델 정보를 받아온다.
+        3. add_convert_info: 모델 정보를 바탕으로 변경할 모델들을 입력한다.
+        4. convert_models: 입력한 모델을 변환하고 기존 App에서 교체한다.
+        5. package_app: 새로운 앱으로 패키징한다.
+
+    Attributes:
+        workspace (Path): 작업할 경로, 일반적으로 ~/.waffle_box
+        origin_app_path (Path): 사용자가 입력한 기존 App 경로
+        final_app_path (Path): 새로운 App을 저장할 경로
+        img_tag (str): trt 변환을 위한 컨테이너 태그명
+        convert_list (dict[UUID, Path]): 변경할 모델 리스트
+        app_manager (AppManager): app manager
+        maker_manager (MakerManager): maker manager
 
     """
 
     def __init__(self, workspace: Path, input: Path, output: Path, dx_target_version: str, gpu_num: int) -> None:
         """
-        # Parameters
-        - workspace
-            - 작업할 경로
-        - input
-            - 변환할 App 경로
-        - output
-            - 새로운 App을 저장할 경로
-        - dx_target_version
-            - 변환할 App의 target Autocare-D 버전
-        - gpu_num
-            - 작업할 GPU 번호
-
-        # Raises
-        - AppParsingError
-        - DockerError
+        Args:
+            workspace (Path): 작업할 경로
+            input (Path): 변환할 App 경로
+            output (Path): 새로운 App을 저장할 경로
+            dx_target_version (str): 변환할 App의 target Autocare-D 버전
+            gpu_num (int): 작업할 GPU 번호
+
+        Raises:
+            AppParsingError
+            DockerError
 
         """
         self.workspace: Path = workspace
         self.origin_app_path: Path = input
         self.final_app_path: Path = output
 
         # TODO: make image tag converter
@@ -72,52 +54,56 @@
 
         self.app_manager = AppManager(self.workspace, self.origin_app_path)
         self.maker_manager = MakerManager(
             self.img_tag, gpu_num=gpu_num, workspace=self.workspace)
 
     def is_local_maker_installed(self) -> bool:
         """ Waffle maker가 local에 설치되어 있는가?
+
+        Returns:
+            True: 이미지가 설치되어 있음
+            False: 이미지가 설치되어 있지 않음
         """
         return self.maker_manager.check_image_exist_at_local()
 
     def get_model_info(self) -> list[ModelInfo]:
         """ 모델 정보 받아오기
 
         사용자가 입력한 App의 모델 정보들을 리스트로 반환한다.
 
+        Returns:
+            list[ModelInfo]: 모델 정보 리스트
+
         """
         return self.app_manager.app_structure.models
 
     def add_convert_info(self, model_id: UUID, new_model_path: Path) -> None:
         """ 변환할 모델 정보 등록
 
         변환할 모델 정보를 등록한다. App의 모델 id와 새로운 모델 경로를 등록한다.
         등록할 만큼 호출한다.
 
-        # Parameters
-        - model_id
-            - 교체할 모델의 UUID
-        - new_model_path
-            - 새로운 모델 파일 경로
+        Args:
+            model_id (UUID): 교체할 모델의 UUID
+            new_model_path (Path): 새로운 모델 파일 경로
 
         """
         self.convert_list[model_id] = new_model_path
 
     def convert_models(self, print_output: bool) -> None:
         """ 모델 변화
 
         사용자가 등록한 모델들을 변환한다.
 
-        # Parameters
-        - print_output
-            - 변환 과정을 출력 여부
-
-        # Raises
-        - AppManager
-        - MakerManager
+        Args:
+            print_output (bool): 변환 과정을 출력 여부
+
+        Raises:
+            AppManager
+            MakerManager
 
         """
         for id, file_path in self.convert_list.items():
             model_info = self.app_manager.find_model_info_by_id(id)
 
             if not model_info:
                 return
@@ -136,29 +122,7 @@
             # remove converted files
             os.remove(engine_file_path)
 
     def package_app(self) -> None:
         """ 새로운 App 생성
         """
         self.app_manager.package(self.final_app_path)
-
-
-if __name__ == '__main__':
-    workspace = Path('/home/yoon/.waffle_box')
-    input = Path(
-        '/home/yoon/Downloads/app_convert_test/people/4881be2f-b0fa-46e1-a100-7badd8bc50c6_people_net.zip')
-    output = Path('/home/yoon/Downloads/app_convert_test/test.zip')
-    cv = ConvertService(workspace, input, output, '1.6.2', 0)
-
-    if cv.is_local_maker_installed():
-        print('Ok, waffle maker is installed.')
-    else:
-        print('Opps... waffle maker is not installed.')
-
-    models = cv.get_model_info()
-    print(cv.get_model_info())
-
-    cv.add_convert_info(models[0].id, Path(
-        '/home/yoon/Downloads/app_convert_test/people/model.onnx'))
-
-    cv.convert_models(True)
-    cv.package_app()
```

### Comparing `waffle_box-0.0.2/waffle_box/pull_service.py` & `waffle_box-0.1.0/waffle_box/pull_service.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,80 +3,70 @@
 from pathlib import Path
 
 class PullService:
     """ Waffle Maker 이미지 설치
 
     Target Autocare-D 버전에 맞춰 Waffle Maker 이미지를 설치한다.
 
-    # 실행 순서
-    1. is_local_maker_installed
-        Waffle Maker가 local pc에 설치되어 있는지 확인한다.
-    2. (Optional) set_login_info
-        필요하다면 docker hub에 로그인할 정보를 설정한다.
-    3. pull_image_to_local
-        이미지를 로컬 pc에 다운로드 한다.
-
-    # Attributes
-    - dh_id
-        - docker hub id
-        - 빈값일 경우 로그인 시도를 하지 않는다.
-    - dh_pw
-        - docker hub password
-        - 빈값일 경우 로그인 시도를 하지 않는다.
-    - img_tag
-        - 설치할 이미지 태그
-    - maker_manager
-        - MakerManager
+    실행 순서:
+        1. is_local_maker_installed: Waffle Maker가 local pc에 설치되어 있는지 확인한다.
+        2. (Optional) set_login_info: 필요하다면 docker hub에 로그인할 정보를 설정한다.
+        3. pull_image_to_local: 이미지를 로컬 pc에 다운로드 한다.
+
+    Attributes:
+        dh_id (str): docker hub id, 빈값일 경우 로그인 시도를 하지 않는다.
+        dh_pw (str): docker hub password, 빈값일 경우 로그인 시도를 하지 않는다.
+        img_tag (str): 설치할 이미지 태그
+        maker_manager (MakerManager): maker manager
 
     """
 
     def __init__(self, workspace: Path, dx_target_version: str) -> None:
         """
-        # Parameters
-        - workspace
-            - 작업할 경로
-        - dx_target_version
-            - 타겟 Autocare-D 버전
+        Args:
+            workspace (Path): 작업할 경로
+            dx_target_version (str): 타겟 Autocare-D 버전
 
-        # Raises
-            - MakerManagerException
+        Raises:
+            MakerManagerException
 
         """
         # Docker Hub
         self.dh_id: str = ''
         self.dh_pw: str = ''
 
         # TODO: make image tag converter
         self.img_tag = 'snuailab/trt:8.5.2.2'
 
         self.maker_manager = MakerManager(self.img_tag, gpu_num=0, workspace=workspace)
 
     def is_local_maker_installed(self) -> bool:
         """ Waffle Maker 이미지가 로컬 pc에 설치되어 있는지 확인한다.
+
+        Returns:
+            True: 설치되어 있음
+            False: 설치되어 있지 않음
         """
         return self.maker_manager.check_image_exist_at_local()
 
     def set_login_info(self, id: str, pw: str) -> None:
         """ 로그인 정보 입력
 
-        # Parameters
-        - id
-            - docker hub id
-        - pw
-            - docker hub password
+        Args:
+            id (str): docker hub id
+            pw (str): docker hub password
 
         """
         self.dh_id = id
         self.dh_pw = pw
 
     def pull_image_to_local(self, print_output: bool) -> None:
         """ Waffle Maker 이미지를 로컬 pc에 설치
 
-        # Parameters
-        - print_output
-            - 설치 과정 출력 여부
+        Args:
+            print_output (bool): 설치 과정 출력 여부
 
-        # Raises
-        - MakerManagerException
+        Raises:
+            MakerManagerException
 
         """
         self.maker_manager.pull_image_at_local(print_output, self.dh_id, self.dh_pw)
```

### Comparing `waffle_box-0.0.2/waffle_box_exception/waffle_box_exception.py` & `waffle_box-0.1.0/waffle_box_exception/waffle_box_exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,37 +2,40 @@
 
 
 class ExceptionCode(Enum):
     """ Waffle Box에서 생성하는 예외 리스트
 
     Waffle Box에서 생성하는 예외 리스트.
 
-    100 ~ : docker에서 발생한 예외 \n
-    200 ~ : app에서 발생한 예외
-
-    # Attributes
-    - DOCKER_EXCEPTION
-        - docker에서 발생한 예외
-    - APP_STRUCTURE_EXCEPTION
-        - app에서 발생한 예외
+    100번대:
+        Maker Manager에서 발생한 예외
+    200번대: 
+        App Manager에서 발생한 예외
+    300번대:
+        service에서 발생한 예외
 
     """
 
+    ### Maker Manager ###
     DOCKER_EXCEPTION = (100, 'DOCKER_EXCEPTION')
     DOCKER_IMAGE_EXCEPTION = (101, 'DOCKER_IMAGE_EXCEPTION')
     DOCKER_RUN_EXCEPTION = (102, 'DOCKER_RUN_EXCEPTION')
-
     MODEL_IO_EXCEPTION = (103, 'IO_EXCEPTION')
     MODEL_CONVERT_EXCEPTION = (104, 'MODEL_CONVERT_EXCEPTION')
 
+    ### App Manager ###
     APP_STRUCTURE_EXCEPTION = (200, 'APP_STRUCTURE_EXCEPTION')
     APP_NO_SUCH_FILE = (201, 'APP_NO_SUCH_FILE')
     APP_FILE_ALREADY_EXIST = (202, 'APP_FILE_ALREADY_EXIST')
     APP_CONFIG_ERROR = (203, 'APP_CONFIG_ERROR')
 
+    ### Service ###
+    INVALID_ARGUMENT = (300, 'INVALID_ARGUMENT')
+
+
     def __init__(self, code, desc) -> None:
         super().__init__()
 
         self._code: int = code
         self._desc: str = desc
 
     @property
```

### Comparing `waffle_box-0.0.2/PKG-INFO` & `waffle_box-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle-box
-Version: 0.0.2
+Version: 0.1.0
 Summary: 
 Author: SangHyeukYoon
 Author-email: shyoon@snuailab.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -48,7 +48,11 @@
 ```
 
 ## Convert App
 ```bash
 wb --dx-version 1.6.2 convert safety_app_1.0.0.zip -o safety_app_1.0.1.zip
 ```
 
+## Convert Model
+```bash
+wb --dx-version 1.6.2 bake ~/flame.onnx -O ~/model.engine --precision fp32 --batch 16 --shapes 3x640x640
+```
```

