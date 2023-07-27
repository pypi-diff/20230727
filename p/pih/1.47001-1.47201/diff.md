# Comparing `tmp/pih-1.47001.tar.gz` & `tmp/pih-1.47201.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.47001.tar", last modified: Sun Jul 23 22:34:30 2023, max compression
+gzip compressed data, was "pih-1.47201.tar", last modified: Thu Jul 27 12:44:31 2023, max compression
```

## Comparing `pih-1.47001.tar` & `pih-1.47201.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 22:34:31.026589 pih-1.47001/
--rw-rw-rw-   0        0        0      261 2023-07-23 22:34:31.042215 pih-1.47001/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-23 22:34:30.760968 pih-1.47001/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47001/pih/__init__.py
--rw-rw-rw-   0        0        0    20299 2023-07-23 12:16:34.000000 pih-1.47001/pih/collection.py
--rw-rw-rw-   0        0        0    59317 2023-07-23 13:04:31.000000 pih-1.47001/pih/console_api.py
--rw-rw-rw-   0        0        0   108878 2023-07-23 12:45:02.000000 pih-1.47001/pih/const.py
--rw-rw-rw-   0        0        0   307138 2023-07-23 22:34:04.000000 pih-1.47001/pih/pih.py
--rw-rw-rw-   0        0        0    24697 2023-07-17 14:57:37.000000 pih-1.47001/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47001/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47001/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-06-14 04:29:04.000000 pih-1.47001/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6403 2023-07-20 06:09:44.000000 pih-1.47001/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47001/pih/service_example.py
--rw-rw-rw-   0        0        0    37894 2023-07-20 06:21:53.000000 pih-1.47001/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47001/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-23 22:34:30.995344 pih-1.47001/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-07-23 22:34:28.000000 pih-1.47001/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-07-23 22:34:29.000000 pih-1.47001/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 22:34:28.000000 pih-1.47001/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-23 22:34:28.000000 pih-1.47001/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-23 22:34:28.000000 pih-1.47001/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2009 2023-07-14 01:37:00.000000 pih-1.47001/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-23 22:34:31.042215 pih-1.47001/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-27 12:44:30.986915 pih-1.47201/
+-rw-rw-rw-   0        0        0      261 2023-07-27 12:44:32.068396 pih-1.47201/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 12:44:31.771566 pih-1.47201/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47201/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47201/pih/collection.py
+-rw-rw-rw-   0        0        0    61082 2023-07-27 07:03:42.000000 pih-1.47201/pih/console_api.py
+-rw-rw-rw-   0        0        0   110191 2023-07-27 06:39:11.000000 pih-1.47201/pih/const.py
+-rw-rw-rw-   0        0        0   309358 2023-07-27 07:23:27.000000 pih-1.47201/pih/pih.py
+-rw-rw-rw-   0        0        0    24697 2023-07-17 14:57:37.000000 pih-1.47201/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47201/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47201/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-06-14 04:29:04.000000 pih-1.47201/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47201/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47201/pih/service_example.py
+-rw-rw-rw-   0        0        0    38109 2023-07-26 00:20:00.000000 pih-1.47201/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47201/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-27 12:44:32.021521 pih-1.47201/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-07-27 12:44:29.000000 pih-1.47201/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-07-27 12:44:30.000000 pih-1.47201/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 12:44:29.000000 pih-1.47201/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-27 12:44:30.000000 pih-1.47201/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-27 12:44:30.000000 pih-1.47201/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2009 2023-07-14 01:37:00.000000 pih-1.47201/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-27 12:44:32.084019 pih-1.47201/setup.cfg
```

### Comparing `pih-1.47001/pih/collection.py` & `pih-1.47201/pih/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -721,14 +721,19 @@
     auto_init: bool = True
 
 
 @dataclass
 class IntStorageValue(StorageValue):
     default_value: int = 0
 
+
+@dataclass
+class MinIntStorageValue(IntStorageValue):
+    min_value: int = 0
+
 @dataclass
 class IntStorageValueWithMin(IntStorageValue):
     min_value: int = 0
 
 
 @dataclass
 class FloatStorageValue(StorageValue):
@@ -756,14 +761,19 @@
     document_name: str
 
 @dataclass
 class ThresholdedText:
     title: str
     threshold: float
 
+@dataclass
+class CommandMenuItem:
+
+    command: str | None = None
+    name: str | None = None
 
 @dataclass
 class PolibaseDocumentDescription(ThresholdedText):
     title_top: int = 0
     title_height: int = 0
     page_count: int = 1
```

### Comparing `pih-1.47001/pih/console_api.py` & `pih-1.47201/pih/console_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,49 +16,49 @@
 from pih.collection import (Mark, User, FullName, 
                             PersonDivision, UserBase, LoginPasswordPair, 
                             MarkGroup, Result, FieldItemList,
                             WorkstationDescription, ResourceStatus, SiteResourceStatus,
                             CTIndicationsValue, Workstation, RobocopyJobStatus, 
                             ChillerIndicationsValueContainer, PrinterReport, DiskStatistics,
                             IntStorageValue)
-from pih.tools import j
+from pih.tools import j, nl
 from pih import A
 
 class ConsoleAppsApi:
 
     LINE: str = "........................................................"
 
-    def __init__(self, pih: PIH = None):
+    def __init__(self, pih: PIH | None = None):
         self.pih = pih or PIH
-        self.full_name: FullName = None
-        self.tab_number: str = None
-        self.telephone_number: str = None
-        self.division_id: int = None
+        self.full_name: FullName | None = None
+        self.tab_number: str | None = None
+        self.telephone_number: str | None = None
+        self.division_id: int | None = None
         self.user_is_exists: bool = False
-        self.login: str = None
-        self.password: str = None
-        self.internal_email: str = None
-        self.external_email: str = None
-        self.email_password: str = None
-        self.polibase_login: str = None
-        self.polibase_password: str = None
+        self.login: str | None = None
+        self.password: str | None = None
+        self.internal_email: str | None = None
+        self.external_email: str | None = None
+        self.email_password: str | None = None
+        self.polibase_login: str | None = None
+        self.polibase_password: str | None = None
         self.user_container: UserBase
-        self.description: str = None
+        self.description: str | None = None
         self.use_template_user: bool
-        self.need_to_create_mark: bool = None
+        self.need_to_create_mark: bool | None = None
 
     def create_qr_code_for_mobile_helper_command(self, command: str | None = None, title: str | None = None, show_result: bool = True) -> str | None:
         command = command or self.input.input("Введите название команды")
         title = title or self.input.input("Введите заголовок")
         result = A.A_QR.for_mobile_helper_command(command, title, os.path.join(A.PTH.MOBILE_HELPER.QR_CODE_FOLDER, A.PTH.replace_prohibited_symbols_from_path_with_symbol(A.PTH.add_extension(command, FILE.EXTENSION.PNG))), 56)
         qr_code_image_path: str = A.PTH_QR.mobile_helper_command(command)
         if show_result:
             if result:
                 self.output.good(
-                    f"Файл qr кода {self.bold(title)} создан.\nПуть к файлу:\n{self.bold(qr_code_image_path)}\n")
+                    j((nl(f"Файл qr кода {self.bold(title)} создан."), nl("Путь к файлу:"), nl(self.bold(qr_code_image_path)))))
             else:
                 self.output.error("qr код не был создан")
         return qr_code_image_path
 
     def create_qr_code_for_card_registry_folder(self, card_registry_folder_name: str | None = None, show_result: bool = True) -> list[str]:
         if A.D_C.empty(card_registry_folder_name):
             card_registry_folder_name = self.input.input(f"Введите название папки (или несколько значений названий папок разделенной запятой или пробелом)")
@@ -74,31 +74,32 @@
                     self.output.error("qr код не был создан")
             if result:
                 result_path_list.append(qr_code_image_path)
         return result_path_list
     
     def disks_information(self, host: str | None = None) -> None:
         host = host or self.input.input("Введите название хоста (компьютера или сервера)")
-        if A.C_R.accessibility_by_ping(host):
-            disk_statistics_list: list[DiskStatistics] = list(filter(lambda item: item.size > 0, A.PS.get_disk_statistics_list(host)))
-            if A.D_C.empty(disk_statistics_list):
-                self.output.error("Хост не имеет дисков")
+        with self.output.make_indent(2, True):
+            if A.C_R.accessibility_by_ping(host):
+                disk_statistics_list: list[DiskStatistics] = list(filter(lambda item: item.size > 0, A.PS.get_disk_statistics_list(host)))
+                if A.D_C.empty(disk_statistics_list):
+                    self.output.error("Хост не имеет дисков")
+                else:
+                    self.output.write_line(nl("Информация о дисках:"))
+                    for disk_statistics in disk_statistics_list:
+                        self.output.write_line(f"{A.CT_V.BULLET} {self.bold(disk_statistics.name)}: {A.D_F.size(disk_statistics.free_space)} из {A.D_F.size(disk_statistics.size)}")
             else:
-                self.output.write_line("Информация о дисках:\n")
-                for disk_statistics in disk_statistics_list:
-                    self.output.write_line(f" {A.CT_V.BULLET} {self.bold(disk_statistics.name)}: {A.D_F.size(disk_statistics.free_space)} из {A.D_F.size(disk_statistics.size)}")
-        else:
-            self.output.error("Хост не доступен или не найден")
+                self.output.error("Хост не доступен или не найден")
 
     @property
     def is_mobile(self) -> bool:
         return self.session.name == "mobile"
 
     def resources_and_indications_check(self, checkable_section_list: list[CheckableSections], ask_for_update_before: bool = False, force_update: bool = False, all: bool = False) -> None:
-        with self.output.make_indent(1):
+        with self.output.make_indent(2):
             if CheckableSections.RESOURCES in checkable_section_list or (
                 CheckableSections.WS in checkable_section_list\
                 or CheckableSections.SERVERS in checkable_section_list):
                 def label_function(resource: ResourceStatus, index: int) -> str:
                     result: list[str] = [] 
                     accessable: bool = resource.accessable
                     status: str = A.D_F.yes_no(accessable, True)
@@ -117,47 +118,54 @@
                     self.output.write_line(
                         self.italic(f"{self.get_formatted_given_name()}, ожидайте получение результата..."))
                 for checkable_section in [CheckableSections.RESOURCES, CheckableSections.WS, CheckableSections.SERVERS]:
                     if checkable_section in checkable_section_list:
                         if self.is_mobile:
                             self.output.new_line()
                         if all:
-                            self.output.write_line(" ".join((A.CT_V.BULLET, self.bold(A.D.check(checkable_section == CheckableSections.RESOURCES, "Основные ресурсы", A.D.check(checkable_section == CheckableSections.WS, "Наблюдаемые компьютеры", "Серверы"))))))
+                            self.output.write_line(" ".join((A.CT_V.BULLET, self.bold(A.D.check(checkable_section == CheckableSections.RESOURCES, "Основные ресурсы", A.D.check(checkable_section == CheckableSections.WS, "Наблюдаемые компьютеры", "Сервера"))))))
                         with self.output.make_indent(2, True):
                             self.output.write_result(A.R_R.get_status_list([checkable_section], force_update, all if len(checkable_section_list) == 1 and CheckableSections.WS in checkable_section_list else False), False, label_function=label_function, separated_result_item=self.is_mobile)
             if CheckableSections.INDICATIONS in checkable_section_list:
                 #self.output.separated_line()
                 #self.output.write_line(f"Показания доступны по адрессу:\n{self.bold('http://indications')}, если заходить с рабочего компьютера\nили\n{self.bold('http://192.168.100.138')}, если заходить с мобильного телефона, подключенного к корпоративной wifi сети")
                 if self.is_mobile:
                     self.output.new_line()
                 self.output.write_line(self.bold(f"{A.CT_V.BULLET} Показания в помещении КТ"))
                 with self.output.make_indent(2, True):
                     self.output.write_result(A.R_I.last_ct_value_containers(True))
+                    self.output.write_image(j(("   ", A.CT_V.BULLET, " ", self.output.bold("График показаний"))), A.D_CO.file_to_base64(
+                        A.PTH.STATISTICS.get_file_path(A.D.get(A.CT_STATISTICS.TYPES.CT))))
                 self.output.separated_line()
                 self.output.write_line(self.bold(f"{A.CT_V.BULLET} Показания в техническом помещении МРТ"))
                 chiller_indications_value_container_result: Result[list[ChillerIndicationsValueContainer]] = A.R_I.last_chiller_value_containers(True)
                 chiller_indications_value_container: ChillerIndicationsValueContainer = A.R.get_first_item(chiller_indications_value_container_result)
                 path: str = A.PTH_I.CHILLER_DATA_IMAGE_LAST
                 modification_timstamp: float = os.path.getmtime(path)
                 file_creating_datetime: datetime | None = datetime.fromtimestamp(modification_timstamp if modification_timstamp > 0 else os.path.getctime(path))
                 with self.output.make_indent(2, True):
-                    self.output.write_result(chiller_indications_value_container_result, title="Показания чиллера\n" if A.D_C.INDICATIONS.chiller_value_actual(chiller_indications_value_container) else f"{self.bold('Внимание!')}: Показания чиллера неактуальны\n", separated_result_item=False)
-                    self.output.write_image(f"Изображение дисплея чиллера\nВремя снятия: {A.D_F.datetime(file_creating_datetime)}", A.D_CO.file_to_base64(A.PTH_I.CHILLER_DATA_IMAGE_LAST_RESULT))
+                    if A.C_E.has(A.E_B.chiller_was_turned_off()):
+                        self.output.write_line(j((A.CT_V.WARNING, "Чиллер выключен!", A.CT_V.WARNING)))
+                    else:
+                        self.output.write_result(chiller_indications_value_container_result, title="Показания чиллера\n" if A.D_C.INDICATIONS.chiller_value_actual(chiller_indications_value_container) else f"{self.bold('Внимание!')}: Показания чиллера неактуальны\n", separated_result_item=False)
+                        self.output.write_image(f"    Изображение дисплея чиллера\nВремя снятия: {A.D_F.datetime(file_creating_datetime)}", A.D_CO.file_to_base64(A.PTH_I.CHILLER_DATA_IMAGE_LAST_RESULT))
             if CheckableSections.MATERIALIZED_RESOURCES in checkable_section_list:
                 if self.is_mobile:
                     self.output.new_line()
                 self.output.separated_line()
                 self.output.write_line(
-                    self.bold(f"{A.CT_V.BULLET} Материальные ресурсы:"))
+                    self.bold(f"{A.CT_V.BULLET} Материальные ресурсы"))
                 with self.output.make_indent(2, True):
                     for resource_type in A.CT_MR.TYPES:
                         self.output.write_line(f"{A.CT_V.BULLET} {self.bold(A.D.get(resource_type).description)}")
                         with self.output.make_indent(2, True):
-                            self.output.write_line(j(("\nКоличество: ", str(A.D_MR.get_count(resource_type)))))
+                            self.output.write_line(nl(j((nl(), self.output.bold("Количество"), ": ", str(A.D_MR.get_count(resource_type)), " штук"))))
                             self.output.write_line(A.D_F.statistics(resource_type))
+                            self.output.write_image(f"   {A.CT_V.BULLET} График выработки фильтров чиллера МРТ", A.D_CO.file_to_base64(
+                                A.PTH.STATISTICS.get_file_path(resource_type.name)))
             if CheckableSections.VALENTA in checkable_section_list:
                 scanned_file_path_list: list[str] = A.PTH.get_file_list_by_directory_info(
                     A.PTH.WS_816_SCAN.VALUE)
                 count: int = len(scanned_file_path_list)
                 if self.is_mobile:
                     self.output.new_line()
                 self.output.separated_line()
@@ -176,18 +184,25 @@
                     admin_description_list: list[str] = ("" or printer_report.adminDescription).split(",")
                     name: str = printer_report.ip.split('.')[0]
                     report_list.append(f"{self.bold('Модель')}: {printer_report.model}\n{self.bold('Название')}: {name}\n{self.bold('Описание')}: {printer_report.description}")
                     if printer_report.name != -401 and "infoless" not in admin_description_list:   
                         for item in (("Тонер", printer_report.get_toner), None if "drumless" in admin_description_list else ("Драм-юнит", printer_report.get_drum)):
                             if A.D.is_not_none(item):
                                 report_list.append(f" {A.CT_V.BULLET} {self.bold(item[0])}")
-                                report_list += [f"   {self.bold(color.upper())}: %d%%" % item[1](color) for color in (["k"] if "bw" in admin_description_list else ["c", "m", "y", "k"])]
+                                def get_value(function: Callable[[str], int], color: str) -> str:
+                                    value: int = function(color)
+                                    result: str = str(value)
+                                    if value < 5:
+                                        result += j((" ", A.CT_V.WARNING))
+                                    return result
+                                report_list += [f"   {self.bold(color.upper())}: {get_value(item[1], color)}" for color in (
+                                    ["k"] if "bw" in admin_description_list else ["c", "m", "y", "k"])]
                     else:
                         report_list.append(f"Принтер {A.D.if_check(printer_report.accessable, '', 'не ')}доступен")
-                    return "\n".join(report_list)
+                    return nl().join(report_list)
                 if self.is_mobile:
                     self.output.new_line()
                 self.output.separated_line()
                 self.output.write_line(
                     self.bold(f"{A.CT_V.BULLET} Отчет по принтерам"))
                 printer_report_list: list[PrinterReport] = A.R_PR.report().data
                 for printer_report_item in printer_report_list:
@@ -208,18 +223,18 @@
                         if job_status.active:
                             date = "выполняется"
                         else:
                             if job_status.last_created is not None:
                                 date = f"{A.D_F.datetime(job_status.last_created)}"
                             status = job_status.last_status
                         variants: list[str] = ["--" if status is None else self.bold(str(status)), "--" if A.D_C.empty(date) else self.bold(date)]
-                        return "".join([f" {A.CT_V.BULLET} ", variants[not sort_by_status], ": ", variants[sort_by_status], "".join([ "\n   ", name, ": ", source, A.CT_V.ARROW, destination])])
+                        return j((f" {A.CT_V.BULLET} ", variants[not sort_by_status], ": ", variants[sort_by_status], j((nl(), "   ", name, ": ", source, A.CT_V.ARROW, destination))))
                     variants: list[str] = [self.bold("Статус"), self.bold("Дата выполнения")]
                     self.output.write_result(
-                        robocopy_job_status_list, False, label_function=job_status_item_label_function, separated_result_item=False, title="".join([f" {A.CT_V.BULLET} ", variants[not sort_by_status], ": ", variants[sort_by_status], "\n", "   Название Robocopy-задания", f"\n{ConsoleAppsApi.LINE}"]))
+                        robocopy_job_status_list, False, label_function=job_status_item_label_function, separated_result_item=False, title=j((f" {A.CT_V.BULLET} ", variants[not sort_by_status], ": ", variants[sort_by_status], nl(), "   Название Robocopy-задания", nl(), ConsoleAppsApi.LINE)))
 
     def polibase_restart(self) -> None:
         if self.input.yes_no("Перезапустить сервер Polibase"):
             check_word: str = A.CT_P.NAME
             test: bool = not (check_word == self.input.input(
                 f"Введите контрольное слово: {self.bold(check_word)}"))
             notify: bool = test or self.input.yes_no("Уведомить пользователей", True)
@@ -289,15 +304,15 @@
 
     def send_whatsapp_message(self, telephone_number: str, message: str) -> bool:
         return A.ME_WH_W.send(telephone_number, message, A.CT_ME_WH_W.PROFILE.IT)
 
     def mark_find(self, value: str | None = None) -> None:
         self.output.mark.by_any(value or self.input.mark.any())
 
-    def arg(self, index: int = 0, default_value: Any = None) -> Any:
+    def arg(self, index: int = 0, default_value: Any | None = None) -> Any:
         return self.session.arg(index, default_value)
 
     def register_ct_indications(self) -> None:
         text: str = f"число, которое может содержать дробную часть разделенную {self.bold('точкой')} или {self.bold('запятой')}"
         number_format_notification_text: str = f"- {self.italic(text)}"
         def float_check_function(value: str | None, show_error: bool = True) -> str | None:
             result: float | None = None
@@ -314,43 +329,43 @@
         indications_value: CTIndicationsValue = CTIndicationsValue(temperature, humidity)
         if A.A_I_CT.register(indications_value):
             with self.output.send_to_group(A.CT_ME_WH.GROUP.CT_INDICATIONS):
                 self.output.write_result(
                     Result(A.CT_FC.INDICATIONS.CT_VALUE, indications_value), title=f"{self.get_formatted_given_name()}, отправил следующие показания в помещение КТ:")
             self.output.good("Спасибо, показания отправлены")
 
-    def find_free_mark(self, value: str = None) -> None:
+    def find_free_mark(self, value: str | None = None) -> None:
         self.output.mark.result(A.R_M.by_any(
             value or self.input.mark.any()), "Список свободных карт доступа:")
 
-    def find_user(self, value: str = None) -> None:
+    def find_user(self, value: str | None = None) -> None:
         try:
             result: Result[list[User]] = A.R_U.by_any(
                 value or self.input.user.title_any())
         except NotFound as error:
             self.output.error(error.get_details())
         else:
             self.output.user.result(result, "Пользователи:")
 
     def create_password(self) -> str:
-        password: str = None
+        password: str | None = None
         password_settings: PasswordSettings = PASSWORD.get(self.input.indexed_field_list(
             "Выберите тип пароля", A.CT_FC.POLICY.PASSWORD_TYPE))
         while True:
             password = self.input.user.generate_password(
                 True, password_settings)
             self.output.value("Пароль", password)
             if self.input.yes_no("Использовать", True):
                 break
         if self.input.yes_no("Отправить в ИТ отдел"):
             A.L.it(f"Сгенерированный пароль:")
             A.L.it(password)
         return password
 
-    def make_mark_as_free(self, value: str = None) -> None:
+    def make_mark_as_free(self, value: str | None = None) -> None:
         mark: Mark = self.input.mark.by_any(value)
         mark_type: int = A.D.get(MarkType, mark.type)
         if mark_type == MarkType.FREE:
             self.output.error(
                 "Карта доступа с введенным номером уже свободная")
         else:
             if self.input.yes_no("Сделать карту свободной"):
@@ -367,15 +382,15 @@
                     self.output.good(
                         f"Карта доступа с номером {mark.TabNumber} стала свободной")
                 else:
                     self.output.error("Ошибка")
             else:
                 self.output.error("Отмена")
 
-    def who_lost_the_mark(self, tab_number: str = None):
+    def who_lost_the_mark(self, tab_number: str | None = None):
         try:
             tab_number = tab_number or self.input.tab_number()
             if tab_number is not None:
                 try:
                     mark: Mark = self.pih.RESULT.MARK.by_tab_number(
                         tab_number).data
                     mark_type: MarkType = A.D.get(MarkType, mark.type)
@@ -422,36 +437,36 @@
 
     def bold(self, value: str) -> str:
         return self.output.bold(value)
 
     def italic(self, value: str) -> str:
         return self.output.italic(value)
 
-    def run_command(self, command_list: list[str] = None) -> None:
+    def run_command(self, command_list: list[str] | None = None) -> None:
         default_host: str = A.CT_H.DC2.NAME
-        host: str = None
+        host: str | None = None
         def get_command_list() -> list[str]:
             command_list: tuple[list[str], list[str]] = A.D.dequotes(
                 self.pih.input.input("Введите команду"))
             return list(filter(lambda item: not A.D_C.empty(item), command_list[0] + command_list[1]))
         command_list = command_list or get_command_list()
         use_psexec: bool = A.D_C.empty([value for value in list(map(
             lambda item: item.lower(), command_list)) if value in A.CT.PSTOOLS.COMMAND_LIST])
-        result: CompletedProcess = None
+        result: CompletedProcess | None = None
         if use_psexec:
             if A.D_C.empty(host):
                 if self.input.yes_no(f"Использовать хост {self.bold(default_host)}, для выполнения команды", no_label=f"{self.bold('Или введите название хоста')}"):
                     host = default_host
                 else:
                     host = self.input.answer
             while True:
                 host = host.lower()
                 if A.C_R.accessibility_by_ping(host, count=1):
                     self.output.write_line(
-                        f"Команда будет запущена на хосте {self.bold(host)}\n")
+                        nl(f"Команда будет запущена на хосте {self.bold(host)}"))
                     break
                 else:
                     self.output.error(f"Хост {self.bold(host)} не доступен")
                     host = self.input.input(
                         "Введите имя хоста, на котором будет выполнена команда")
             self.output.write_line(
                 f"{self.get_formatted_given_name()}, ожидайте окончания выполнения команды...")
@@ -467,18 +482,18 @@
             self.output.write_line(result_out)
         if result.returncode != 0:
             error: str = result.stderr
             self.output.write_line(error)
 
     def create_new_mark(self):
 
-        self.full_name = None
-        self.tab_number = None
-        self.telephone_number = None
-        self.division_id = None
+        self.full_name: str | None = None
+        self.tab_number: str | None = None
+        self.telephone_number: str | None = None
+        self.division_id: int | None = None
 
         def get_full_name() -> ActionValue:
             self.output.header("Заполните ФИО персоны")
             self.full_name = self.input.full_name(True)
             user_exists: bool = not self.pih.CHECK.MARK.exists_by_full_name(
                 self.full_name)
             if user_exists:
@@ -536,16 +551,16 @@
     def user(self) -> User:
         return self.session.user
 
     @property
     def user_description(self) -> str:
         return A.D_F.description(self.user.description)
 
-    def send_workstation_message(self, recipient_name: str = None, message: str | None = None, ask_for_use_dialog: bool = True) -> None:
-        recipient: User | WorkstationDescription = None
+    def send_workstation_message(self, recipient_name: str | None = None, message: str | None = None, ask_for_use_dialog: bool = True) -> None:
+        recipient: User | WorkstationDescription | None = None
         while True:
             try:
                 recipient = A.D.get_first_item(
                     self.input.user.by_any(recipient_name, True))
                 if recipient is not None:
                     break
             except NotFound as error:
@@ -593,28 +608,28 @@
     @property
     def user_given_name(self) -> str:
         return self.session.user_given_name
     
     def get_formatted_given_name(self, value: str | None = None) -> str:
         return self.output.user.get_formatted_given_name(value or self.user_given_name)
 
-    def create_temporary_mark(self, owner_mark: Mark = None) -> None:
+    def create_temporary_mark(self, owner_mark: Mark | None = None) -> None:
         owner_mark = owner_mark or self.input.mark.by_any()
-        mark_group: MarkGroup = None
+        mark_group: MarkGroup | None = None
         if self.input.yes_no("Выдать временную карту доступа из той же группы доступа"):
             mark_group = owner_mark
         temporary_mark: Mark = self.input.mark.free(mark_group)
         self.output.temporary_candidate_for_mark(temporary_mark)
         full_name: str = owner_mark.FullName
         tab_number: str = temporary_mark.TabNumber
         if self.input.yes_no(f"Создать временную карту для {full_name} с табельным номеров {tab_number}", True):
             if A.A_M.make_as_temporary(temporary_mark, owner_mark):
                 self.output.good("Временная карта создана")
                 telephone_number: str = owner_mark.telephoneNumber
-                A.Eit_notify_about_create_temporary_mark(
+                A.E.it_notify_about_create_temporary_mark(
                     full_name, tab_number)
                 if not A.C.telephone_number(telephone_number):
                     user: User = A.R.get_first_item(A.R_U.by_any(
                         owner_mark))
                     if user is not None:
                         telephone_number = user.telephoneNumber
                 if A.C.telephone_number(telephone_number):
@@ -664,17 +679,17 @@
                         self.output.good(
                             f"{user.name}: телефон присутствует")
                         self.telephone_number_fix_action(user)
             else:
                 self.output.notify(
                     f"{user.name}, похоже не пользователь, у которого должен быть номер телефона")
 
-    def start_user_property_setter(self, property_name: str, search_value: str = None, choose_user: bool = False) -> None:
+    def start_user_property_setter(self, property_name: str, search_value: str | None = None, choose_user: bool = False) -> None:
         try:
-            user_list: list[User] = None
+            user_list: list[User] | None = None
             fields: FieldItemList = A.CT_FC.AD.USER
             active: bool | None = True if (
                 property_name == A.CT_UP.PASSWORD or property_name == A.CT_UP.TELEPHONE_NUMBER) else None
             if choose_user:
                 user_list = self.input.user.by_any(search_value, active)
             else:
                 result: Result[list[User]] = A.R_U.by_any(
@@ -723,15 +738,15 @@
                                 else:
                                     self.output.error("Ошибка")
                             else:
                                 self.output.error("Отмена")
                         elif property_name == A.CT_UP.PASSWORD:
                             self.output.user.result(
                                 Result(fields, [user]), "Пользователи:")
-                            password: str = None
+                            password: str | None = None
                             while True:
                                 password = self.input.user.generate_password(True, PASSWORD.get(
                                     self.input.indexed_field_list("Выберите тип пароля", A.CT_FC.POLICY.PASSWORD_TYPE)))
                                 self.output.value("Пароль", password)
                                 if self.input.yes_no("Использовать", True):
                                     break
                             if self.input.yes_no("Установить", True):
@@ -751,30 +766,30 @@
 
     @property
     def session(self) -> Session:
         return self.pih.session
 
     def create_new_user(self) -> None:
 
-        self.full_name = None
-        self.tab_number = None
-        self.telephone_number = None
-        self.division_id = None
-        self.user_is_exists = False
-        self.login = None
-        self.password = None
-        self.internal_email = None
-        self.external_email = None
-        self.email_password = None
-        self.polibase_login = None
-        self.polibase_password = None
-        self.user_container = None
-        self.description = None
-        self.use_template_user = None
-        self.need_to_create_mark = None
+        self.full_name: FullName | None = None
+        self.tab_number: str | None = None
+        self.telephone_number: str | None = None
+        self.division_id: int | None = None
+        self.user_is_exists: bool = False
+        self.login: str | None = None
+        self.password: str | None = None
+        self.internal_email: str | None = None
+        self.external_email: str | None = None
+        self.email_password: str | None = None
+        self.polibase_login: str | None = None
+        self.polibase_password: str | None = None
+        self.user_container: User | None = None
+        self.description: str | None = None
+        self.use_template_user: bool | None = None
+        self.need_to_create_mark: bool | None = None
 
         def get_full_name() -> ActionValue:
             self.output.header("Заполнение ФИО пользователя")
             self.full_name = self.input.full_name(True)
             self.user_is_exists = self.pih.CHECK.USER.exists_by_full_name(
                 self.full_name)
             if self.user_is_exists:
```

### Comparing `pih-1.47001/pih/const.py` & `pih-1.47201/pih/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 from pih.collection import (FieldItem, FieldItemList, EventDescription, 
                             ParamItem, PasswordSettings, StorageValue, 
                             ResourceDescription, SiteResourceDescription, PolibaseDocumentDescription, 
                             MedicalDirectionDescription, ActionDescription, IntStorageValue, 
                             BoolStorageValue, TimeStorageValue, DateListStorageValue, 
-                            FloatStorageValue)
+                            FloatStorageValue, MinIntStorageValue)
 from pih.rpc_collection import ServiceDescription, ServiceInformationBase
 from pih.rpc_const import ServiceCommands
 
 class DATA:
 
     #deprecated
     class EXTRACTOR:
@@ -309,23 +309,23 @@
 
     GROUP_PREFIX: str = "group:"
 
     SITE_PROTOCOL: str = "https://"
     UNTRUST_SITE_PROTOCOL: str = "http://" 
     
     SITE_NAME: str = "pacifichosp"
-    SITE_URL: str = f"{SITE_NAME}.com"
-    EMAIL_SERVER_URL: str = f"mail.{SITE_URL}"
+    SITE_ADDRESS: str = f"{SITE_NAME}.com"
+    EMAIL_SERVER_ADDRESS: str = f"mail.{SITE_ADDRESS}"
     RECEPTION_EMAIL_LOGIN: str = f"reception.{SITE_NAME}"
 
     WIKI_SITE_NAME: str = f"wiki"
-    WIKI_SITE_ADDRESS: str = f"{UNTRUST_SITE_PROTOCOL}{WIKI_SITE_NAME}"
+    WIKI_SITE_ADDRESS: str = WIKI_SITE_NAME
     OMS_SITE_NAME: str = "oms"
-    OMS_SITE_ADDRESS: str = f"{UNTRUST_SITE_PROTOCOL}{OMS_SITE_NAME}"
-    API_SITE_URL: str = f"api.{SITE_URL}"
+    OMS_SITE_ADDRESS: str = OMS_SITE_NAME
+    API_SITE_ADDRESS: str = f"api.{SITE_ADDRESS}"
     BITRIX_SITE_URL: str = "bitrix.cmrt.ru"
 
     INTERNATIONAL_TELEPHONE_NUMBER_PREFIX: str = "7"
     TELEPHONE_NUMBER_PREFIX: str = f"+{INTERNATIONAL_TELEPHONE_NUMBER_PREFIX}"
     INTERNAL_TELEPHONE_NUMBER_PREFIX: str = "тел."
 
     DATETIME_SPLITTER: str = "T"
@@ -654,14 +654,15 @@
             def sorted() -> list:
                 return sorted(CONST.POLIBASE.DOCUMENT_DESCRIPTIONS, key=lambda item: item.value.title_height, reverse=True)
     
     class VISUAL:
 
         YES: str = "✅"
         NO: str = "❌"
+        WARNING: str =  "⚠️"
 
         NUMBER_SYMBOLS: list[str] = [
            "0️⃣",
            "1️⃣",
            "2️⃣",
            "3️⃣", 
            "4️⃣",
@@ -682,15 +683,16 @@
 class MATERIALIZED_RESOURCES:
 
     NAME: str = "MATERIALIZED_RESOURCES"
     ALIAS: str = "MR"
 
     class TYPES(Enum):
     
-        CHILLER_FILTER_COUNT: IntStorageValue = IntStorageValue("CHF", description="Фильтры для чиллера")
+        CHILLER_FILTER: MinIntStorageValue = MinIntStorageValue(
+            "CHF", description="Фильтры для чиллера", min_value=2)
 
 
 class RESOURCES:
 
     class DESCRIPTIONS:
     
         INTERNET: ResourceDescription = ResourceDescription(
@@ -702,24 +704,24 @@
         PACS_SPB: ResourceDescription = ResourceDescription(
             "10.76.12.124:4242", "Соединение PACS SPB", (2, 100, 5))
 
         POLIBASE: ResourceDescription = ResourceDescription("polibase", "Polibase", inaccessibility_check_values=(2, 10000, 15))
 
         SITE_LIST: list[SiteResourceDescription] = [
             SiteResourceDescription(
-                        CONST.SITE_URL, f"Сайт компании: {CONST.SITE_URL}", check_certificate_status=True, check_free_space_status=False),
-            SiteResourceDescription(CONST.EMAIL_SERVER_URL,
-                        f"Сайт корпоративной почты: {CONST.EMAIL_SERVER_URL}", check_certificate_status=True, check_free_space_status=True, driver_name="/dev/mapper/centos_tenant26--02-var"),
-            SiteResourceDescription(CONST.API_SITE_URL,
-                                    f"Api сайта {CONST.SITE_URL}: {CONST.API_SITE_URL}", check_certificate_status=True, check_free_space_status=False),
-            SiteResourceDescription(CONST.BITRIX_SITE_URL, f"Сайт Битрикс ЦМРТ24: {CONST.BITRIX_SITE_URL}"),
+                        CONST.SITE_ADDRESS, f"Сайт компании: {CONST.SITE_ADDRESS}", check_certificate_status=True, check_free_space_status=False),
+            SiteResourceDescription(CONST.EMAIL_SERVER_ADDRESS,
+                        f"Сайт корпоративной почты: {CONST.EMAIL_SERVER_ADDRESS}", check_certificate_status=True, check_free_space_status=True, driver_name="/dev/mapper/centos_tenant26--02-var"),
+            SiteResourceDescription(CONST.API_SITE_ADDRESS,
+                                    f"Api сайта {CONST.SITE_ADDRESS}: {CONST.API_SITE_ADDRESS}", check_certificate_status=True, check_free_space_status=False),
+            SiteResourceDescription(CONST.BITRIX_SITE_URL, f"Сайт ЦМРТ24: {CONST.BITRIX_SITE_URL}"),
             SiteResourceDescription(
-                CONST.OMS_SITE_ADDRESS, f"Сайт омс: {CONST.OMS_SITE_ADDRESS}", internal = True),
+                CONST.OMS_SITE_ADDRESS, f"Внутренний сайт омс: {CONST.OMS_SITE_ADDRESS}", internal = True),
             SiteResourceDescription(
-                CONST.WIKI_SITE_ADDRESS, f"Сайт wiki: {CONST.WIKI_SITE_ADDRESS}",  internal=True)
+                CONST.WIKI_SITE_ADDRESS, f"Внутренний сайт Вики: {CONST.WIKI_SITE_ADDRESS}", internal=True)
         ]
     
     class INACCESSABLE_REASONS(Enum):
 
         CERTIFICATE_ERROR: str = "Ошибка проверки сертификата"
         SERVICE_UNAVAILABLE: str = "Ошибка 503: Сервис недоступен"
 
@@ -826,14 +828,26 @@
 
     NAME: str = "data"
     FOLDER: str = os.path.join(PATH_APP.FOLDER, NAME)
 
     OCR_RESULT_NAME: str = "ocr result"
     OCR_RESULT_FOLDER: str =  os.path.join(FOLDER, OCR_RESULT_NAME)
 
+
+class PATH_STATISTICS:
+
+    NAME: str = "statistics"
+    CHART_FILE_NAME_PREFIX: str = "chart_"
+    FOLDER: str = os.path.join(PATH_APP_DATA.FOLDER, NAME)
+
+    @staticmethod
+    def get_file_path(name: str) -> str:
+        return os.path.join(PATH_STATISTICS.FOLDER, f"{name}.{FILE.EXTENSION.PNG}")
+
+
 class PATH_INDICATIONS:
 
     NAME: str = "indications"
     FOLDER: str =  os.path.join(PATH_APP_DATA.FOLDER, NAME)
 
     CHILLER_DATA_NAME: str = "chiller"
     CHILLER_DATA_FOLDER: str = os.path.join(FOLDER, CHILLER_DATA_NAME)
@@ -946,14 +960,15 @@
     WS: PATH_WS = PATH_WS()
     BACKUP: PATH_BACKUP = PATH_BACKUP()
     DOCS: PATH_DOCS = PATH_DOCS()
     FONTS: PATH_FONTS = PATH_FONTS()
     MOBILE_HELPER: PATH_MOBILE_HELPER = PATH_MOBILE_HELPER()
     APP_DATA: PATH_APP_DATA = PATH_APP_DATA()
     INDICATIONS: PATH_INDICATIONS = PATH_INDICATIONS()
+    STATISTICS: PATH_STATISTICS = PATH_STATISTICS()
 
 class MarkType(Enum):
 
     NORMAL: int = auto()
     FREE: int = auto()
     GUEST: int = auto()
     TEMPORARY: int = auto()
@@ -1576,17 +1591,22 @@
                                                                 ServiceCommands.create_barcode_for_polibase_person,
                                                                 ServiceCommands.create_qr_code,
                                                                 ServiceCommands.check_inventory_report,
                                                                 ServiceCommands.save_inventory_report_item,
                                                                 ServiceCommands.close_inventory_report,
                                                                 ServiceCommands.create_note,
                                                                 ServiceCommands.get_note,
+                                                                ServiceCommands.create_statistics_chart
                                                             ],
-                                                            modules=["xlsxwriter", "xlrd", "xlutils", "openpyxl",
-                                                                    "python-barcode", "Pillow", "qrcode", "docx-mailmerge", "gkeepapi"]
+                                                            modules=["xlsxwriter", "xlrd", "xlutils", 
+                                                                     "openpyxl", "python-barcode", "Pillow", 
+                                                                     "qrcode", "docx-mailmerge", "gkeepapi", 
+                                                                     "numpy", "panda", "ipywidgets", 
+                                                                     "kaleido", "plotly"
+                                                                     ]
                                                         )
 
     MARK: ServiceDescription = ServiceDescription(
                                                 name="Orion",
                                                 description="Orion service",
                                                 host=CONST.HOST.DC2.NAME,
                                                 commands=
@@ -1729,15 +1749,16 @@
             ServiceCommands.recognize_document
         ]
     )
 
     FILE_OGANIZER: ServiceDescription = ServiceDescription(
         name="FileOrganizer",
         description="File organizer service",
-        host=CONST.HOST.WS255.NAME
+        host=CONST.HOST.WS255.NAME,
+        modules=["pdf2image", "PyPDF2"]
     )
 
     RECOGNIZE_TEST: ServiceDescription = ServiceDescription(
         name="RecognizeTest",
         description="Recognize test service",
         host=CONST.HOST.WS255.NAME,
         auto_start=False,
@@ -1990,15 +2011,15 @@
     EMAIL_VALIDATION_IS_ON: BoolStorageValue = BoolStorageValue("EMAIL_VALIDATION_IS_ON", True)
     EMAIL_VALIDATION_TEST: BoolStorageValue = BoolStorageValue("EMAIL_VALIDATION_TEST", False)
 
     CHILLER_ALERT_TEMPEARTURE: FloatStorageValue = FloatStorageValue(
         "CHILLER_ALERT_TEMPEARTURE", 17.0)
     
     CHILLER_MAX_TEMPEARTURE: IntStorageValue = IntStorageValue(
-        "CHILLER_MAX_TEMPEARTURE", 16)
+        "CHILLER_MAX_TEMPEARTURE", 17)
     
     CHILLER_MIN_TEMPEARTURE: IntStorageValue = IntStorageValue(
         "CHILLER_MIN_TEMPEARTURE", 10)
     
 class PARAM_ITEMS:
 
     NAME: ParamItem = ParamItem(FIELD_NAME_COLLECTION.NAME, "")
@@ -2125,15 +2146,18 @@
     MRI_CHILLER_FILTER_WAS_CHANGED: EventDescription = EventDescription(
         "Фильтр водяного охлаждения МРТ был заменён. Количество оставшихся фильтров: {}", LogMessageChannels.RESOURCES, (LogMessageFlags.NOTIFICATION, LogMessageFlags.SAVE), [PARAM_ITEMS.COUNT])
     
     MRI_CHILLER_TEMPERATURE_ALERT_WAS_FIRED: EventDescription = EventDescription(
         "Превышена температура чиллера", LogMessageChannels.RESOURCES, (LogMessageFlags.ERROR, LogMessageFlags.SAVE))
     
     MRI_CHILLER_WAS_TURNED_OFF: EventDescription = EventDescription(
-        "чиллера", LogMessageChannels.RESOURCES, (LogMessageFlags.ERROR, LogMessageFlags.SAVE), (ParamItem(FIELD_NAME_COLLECTION.DATE, ""), ))
+        "Чиллер был выключен", LogMessageChannels.RESOURCES, (LogMessageFlags.NOTIFICATION, LogMessageFlags.SAVE_ONCE))
+    
+    MRI_CHILLER_WAS_TURNED_ON: EventDescription = EventDescription(
+        "Чиллер был включен", LogMessageChannels.RESOURCES, (LogMessageFlags.NOTIFICATION, LogMessageFlags.SAVE_ONCE))
 
     #POLIBASE
 
     POLIBASE_PERSON_DUPLICATION_WAS_DETECTED: EventDescription("Регистратор {registrator_person_name} создал персону {person_name} ({person_pin}), которая дублирует {duplicated_person_name} ({duplicated_person_pin})", LogMessageChannels.POLIBASE_ERROR, LogMessageFlags.SAVE, (ParamItem(
         "person_name", ""), ParamItem("person_pin", ""), ParamItem("duplicated_person_name", ""), ParamItem("duplicated_person_pin", ""),  ParamItem("registrator_person_name", "")))
 
     POLIBASE_PERSON_VISIT_WAS_REGISTERED: EventDescription = EventDescription("Зарегистрировано новое посещение: {name} ({type_string})", LogMessageChannels.POLIBASE, LogMessageFlags.NOTIFICATION, (PARAM_ITEMS.NAME, ParamItem("type_string", ""), ParamItem("visit", "")))
@@ -2191,11 +2215,18 @@
 
     TIME_TRACKING_REPORT: ActionDescription = ActionDescription(
         "TIME_TRACKING_REPORT", ("tt", "урв"), "Отчеты по учёту рабочего времени", "Создать", False, True)
 
 
 class EMAIL:
 
-    NAS: str = "@".join(("nas", CONST.SITE_URL))
-    IT: str = "@".join(("it", CONST.SITE_URL))
+    NAS: str = "@".join(("nas", CONST.SITE_ADDRESS))
+    IT: str = "@".join(("it", CONST.SITE_ADDRESS))
     EXTERNAL_MAIL_SERVICE: str = "mail.pacifichosp@mail.ru"
     MAILER_DAEMON: str = "mailer-daemon@corp.mail.ru"
+
+class STATISTICS:
+
+    class TYPES(Enum):
+
+        CT: str = "CT"
+        CHILLER_FILTER: str = MATERIALIZED_RESOURCES.TYPES.CHILLER_FILTER.name
```

### Comparing `pih-1.47001/pih/pih.py` & `pih-1.47201/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,15 +432,15 @@
 
     def by_any(self, value: str | None = None, active: bool | None = None, title: str | None = None, use_all: bool = False) -> list[User]:
         raise NotImplemented()
 
     def telephone_number(self, value: str | None = None, active: bool | None = None, title: str | None = None) -> User:
         raise NotImplemented()
 
-    def template(self) -> dict:
+    def template(self) -> User:
         raise NotImplemented()
 
     def search_attribute(self) -> str:
         raise NotImplemented()
 
     def search_value(self, search_attribute: str) -> str:
         raise NotImplemented()
@@ -1380,15 +1380,15 @@
     def telephone_number(self, value: str | None = None, active: bool | None = None, title: str | None = None) -> User:
         try:
             return self.by_any(value, active, title)
         except NotFound:
             return None
 
 
-    def template(self) -> dict:
+    def template(self) -> User:
         result: Result[list[User]] = PIH.RESULT.USER.template_list()
         self.parent.output.template_users_for_result(result, True)
         return self.parent.item_by_index("Выберите шаблон пользователя, введя индекс", result.data)
 
     def search_attribute(self) -> str:
         return self.parent.indexed_field_list("Выберите по какому критерию искать, введя индекс",
                                              FIELD_COLLECTION.AD.SEARCH_ATTRIBUTE)
@@ -1599,22 +1599,23 @@
             self.session: Session = session
         
     class MIO:
     
         ANSWER: dict[str, list[str]] = defaultdict(list)
 
         @staticmethod
-        def create_output(recipient: str | Enum, use_login: bool = True) -> Output:
+        def create_output(recipient: str | Enum, say_hello: bool = True) -> Output:
             from MobileHelperCore.api import MobileOutput, MobileSession, Flags, format_given_name
             recipient = recipient if isinstance(recipient, str) else EnumTool.get(recipient)
             session: MobileSession = MobileSession(recipient, EnumTool.get(Flags.SILENCE))
             recipient_as_whatsapp_group: bool = recipient.endswith(A.CT_ME_WH.GROUP_SUFFIX)
-            if use_login and not recipient_as_whatsapp_group:
-                session.say_hello()
             output: MobileOutput = MobileOutput(session)
+            session.output = output
+            if say_hello and not recipient_as_whatsapp_group:
+                session.say_hello()
             if not recipient_as_whatsapp_group:
                 output.user.get_formatted_given_name = lambda: format_given_name(session, output)
             return output
 
         @staticmethod
         def waiting_for_input_from(recipient: str, handler: Callable[[str, Callable[[None], None]], None] | None = None) -> str | None:
             def internal_handler(message: str, close_handler: Callable[[None], None]) -> None:
@@ -1627,15 +1628,15 @@
                 recipient, internal_handler)
             return PIH.MIO.ANSWER[recipient][-1] 
 
     class VERSION:
 
         @staticmethod
         def local() -> str:
-            return "1.47001"
+            return "1.47201"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
@@ -1669,14 +1670,21 @@
 
         notify_about_error: bool = True
 
         @staticmethod
         def create_error_header(details: str) -> str:
             return f"\nВерсия: {PIH.VERSION.local()}\nПользователь: {PIH.OS.get_login()}\nКомпьютер: {PIH.OS.host()}\n{details}"
 
+        @contextmanager
+        def detect() -> bool:
+            try:
+                yield True
+            except Exception as error:
+                PIH.ERROR.global_except_hook(type(error), error, error.__traceback__)
+        
         @staticmethod
         def rpc_error_handler(details: str, code: tuple, description: ServiceRoles, command: ServiceCommands) -> None:
             if isinstance(command, ServiceCommands):
                 if code == StatusCode.UNAVAILABLE:
                     if PIH.ERROR.notify_about_error:
                         PIH.output.error(f"Error: {details}")
                     return
@@ -1690,15 +1698,15 @@
 
         @staticmethod
         def global_except_hook(exctype, value, __traceback__):
             details_list: list[str] = []
             for item in value.args:
                 if isinstance(item, str):
                     details_list.append(item)
-            details: str = "\n".join(traceback.format_exception(value))
+            details: str = j(traceback.format_exception(value), nl())
             if PIH.ERROR.notify_about_error:
                 PIH.LOG.debug(
                     PIH.ERROR.create_error_header(details), LogMessageFlags.ERROR)
             sys.__excepthook__(exctype, value, traceback)
 
         sys.excepthook = global_except_hook
 
@@ -1710,15 +1718,15 @@
 
         
         class USER:
 
             @staticmethod
             def get_not_found_error(title: str, active: bool, value: str) -> str:
                 start: str | None = None
-                if active is None:
+                if DataTool.is_none(active):
                     start = "Пользователь"
                 elif active:
                     start = "Активный пользователь"
                 else:
                     start = "Неактивный пользователь"
                 return NotFound(f"{start} с {title} '{value}' не найден", value)
 
@@ -2060,15 +2068,15 @@
                 except Error as error:
                     PIH.output.error("Log send error")
             PIH.LOG.executor.submit(internal_send_command,
                                     value.name, PIH.EVENT.BUILDER.create_parameters_map(value, parameters))   
 
         @staticmethod
         def mri_filter_was_changed() -> None:
-            PIH.EVENT.send(Events.MRI_CHILLER_FILTER_WAS_CHANGED, (PIH.DATA.MATERIALIZED_RESOURCES.get_count(MATERIALIZED_RESOURCES.TYPES.CHILLER_FILTER_COUNT),))
+            PIH.EVENT.send(Events.MRI_CHILLER_FILTER_WAS_CHANGED, (PIH.DATA.MATERIALIZED_RESOURCES.get_count(MATERIALIZED_RESOURCES.TYPES.CHILLER_FILTER),))
 
         @staticmethod
         def computer_was_started(name: str) -> None:
             PIH.EVENT.send(
                 Events.COMPUTER_WAS_STARTED, (name,))
 
         @staticmethod
@@ -2165,14 +2173,18 @@
             def card_registry_folder_complete_card_sorting(name: str | None = None) -> Events | tuple[Events, tuple[Any]]:
                 return PIH.EVENT.BUILDER.create_event(
                         Events.CARD_REGISTRY_FOLDER_COMPLETE_CARD_SORTING, name, lambda: (PIH.DATA.FORMAT.polibase_person_card_registry_folder(name), ))
 
             staticmethod
             def chiller_was_turned_off() -> Events:
                 return PIH.EVENT.BUILDER.create_event(Events.MRI_CHILLER_WAS_TURNED_OFF)
+            
+            @staticmethod
+            def chiller_was_turned_on() -> Events:
+                return PIH.EVENT.BUILDER.create_event(Events.MRI_CHILLER_WAS_TURNED_ON)
 
             @staticmethod
             def service_was_stopped(information: ServiceInformationBase | None = None) -> Events | tuple[Events, tuple[Any]]:
                 return PIH.EVENT.BUILDER.create_event(Events.SERVICE_WAS_STOPPED, information, lambda: (information.name, information) )
             
             @staticmethod
             def polibase_persons_barcodes_old_format_were_detected(person_pin_list: list[int] | None = None) -> Events | tuple[Events, tuple[Any]]:
@@ -2652,14 +2664,16 @@
                             if DataTool.is_in(sig.parameters, "subscribtion_result"):
                                 return call_handler(EnumTool.get(ServiceCommands, command_name), parameter_list, PIH.DATA.EXTRACT.subscribtion_result(parameter_list))    
                         return call_handler(EnumTool.get(ServiceCommands, command_name), parameter_list) 
                     return None   
                 service.serve(service_description, internal_call_handler,
                               internal_start_handler, max_workers, depends_on_list, show_output)
 
+
+
             @staticmethod
             def stop(role_or_information: ServiceRoles | ServiceInformationBase, check_on_started: bool = True, direct_call: bool = False) -> bool:
                 description: ServiceDescription = ServiceRoles.description(role_or_information)
                 if not check_on_started or PIH.SERVICE.check_accessibility(description):
                     if PIH.SERVICE.is_service_as_listener(description) or direct_call:
                         A.SRV.call(description, ServiceCommands.stop_service)
                         return True
@@ -2848,21 +2862,21 @@
             def set(name: str, value: Any) -> None:
                 PIH.ACTION.DATA_STORAGE.value(value, name, section=PIH.DATA.VARIABLE.NAME)
 
         class ACTIONS:
 
             @staticmethod
             def get(action_or_name: str | Actions) -> Actions | None:
-                _action: Actions | None = None if isinstance(action_or_name, str) else action_or_name
-                if DataTool.is_none(_action):
+                action: Actions | None = None if isinstance(action_or_name, str) else action_or_name
+                if DataTool.is_none(action):
                     for item in Actions:
                         if item.name == action_or_name or item.value.name == action_or_name or action_or_name in item.value.alias:
-                            _action = item
+                            action = item
                             break
-                return _action
+                return action
 
 
         class MATERIALIZED_RESOURCES:
 
             @staticmethod
             def find(value: str | None) -> list[MATERIALIZED_RESOURCES.TYPES]:
                 result: list[SETTINGS] = []
@@ -2925,14 +2939,31 @@
             @staticmethod
             def users_by_dn(data: list[User], dn: str) -> list:
                 return list(filter(lambda x: x.distinguishedName.find(dn) != -1, data))
 
         class EXTRACT:
 
             @staticmethod
+            def command_menu(value: str) -> tuple[str, list[CommandMenuItem]]:
+                result: list[CommandMenuItem] = []
+                fields: list[str] = [name for _, name, _, _ in Formatter().parse(value) if name]
+                for field_item in fields:
+                    index_start: int = field_item.find("\"menu\"")
+                    if index_start != -1:
+                        index_start = value.find("\"menu\":")
+                        index_end: int = value.find("]}") + 2
+                        index_start -= 1
+                        manu_text: str = value[index_start: index_end]
+                        value = value[0: index_start] + value[index_end: len(value) - 1]
+                        menu_json = json.loads(manu_text)
+                        for menu_json_item in menu_json["menu"]:
+                            result.append(CommandMenuItem(menu_json_item["command"], menu_json_item["label"]))
+                return value, result
+
+            @staticmethod
             def new_mail_message(value: dict) -> NewMailMessage:
                 return A.D.fill_data_from_source(NewMailMessage(), value)
 
             @staticmethod
             def mailbox_info(value: dict | None) -> MailboxInfo | None:
                 if DataTool.is_none(value):
                     return None
@@ -3186,19 +3217,21 @@
 
             @staticmethod 
             def bytes_to_string(value: bytes) -> str:
                 return value.decode("utf-8")
             
         class STATISTICS:
 
+            NAME: str = "statistics"
+
             @staticmethod
             def by_name(value: str) -> TimeSeriesStatistics | None:
                 def is_equal(value: MATERIALIZED_RESOURCES.TYPES, name: str) -> bool:
                     return EnumTool.get(value).key_name == name or value.name == name
-                if is_equal(MATERIALIZED_RESOURCES.TYPES.CHILLER_FILTER_COUNT, value):
+                if is_equal(MATERIALIZED_RESOURCES.TYPES.CHILLER_FILTER, value):
                     return PIH.DATA.STATISTICS.for_chiller_filter()
                 return None
 
             @staticmethod
             def for_chiller_filter() -> TimeSeriesStatistics | None:
                 events_result: Result[list[EventDS]] = PIH.RESULT.EVENTS.get(*PIH.EVENT.BUILDER.action_was_done(A.CT_ACT.CHILLER_FILTER_CHANGING))
                 if ResultTool.is_empty(events_result):
@@ -3258,18 +3291,18 @@
             @staticmethod
             def statistics(type: MATERIALIZED_RESOURCES.TYPES) -> str | None:
                 statistics: TimeSeriesStatistics | None = PIH.DATA.STATISTICS.by_name(type.name)
                 if DataTool.is_none(statistics):
                     return None
                 count: int = PIH.DATA.MATERIALIZED_RESOURCES.get_count(type)
                 def to_days(value: int) -> int:
-                    return int(value / 60 / 60 / 24)
+                    return int(DateTimeTool.seconds_to_days(value))
                 return j(
                     (
-                        "Осталось по времени (дней):",
+                        "Остаток по времени (дней):",
                         f" {CONST.VISUAL.BULLET} Максимально: {count * to_days(statistics.max)}",
                         f" {CONST.VISUAL.BULLET} Минимально: {count * to_days(statistics.min)}",
                         f" {CONST.VISUAL.BULLET} В среднем: {count * to_days(statistics.avg)}",
                     ),
                     "\n"
                 )
 
@@ -3279,14 +3312,15 @@
                 c: Callable[[bool, Callable[[None], Any | None] | Any, Callable[[None], Any | None] | Any], Any] = DataTool.check
                 return c(value, c(symbolic, CONST.VISUAL.YES, "Да"), c(symbolic, CONST.VISUAL.NO, "Нет"))
 
             @staticmethod
             def size(value: int) -> str:
                 return str(int(value / 1024 / 1024 / 1024 )) + " Гб"
 
+
             @staticmethod
             def format(value: str) -> str:
                 fields: list[str] = [name for _, name, _, _ in Formatter().parse(value) if name]
                 #my_fields: list[str] = DataTool.to_list(DATA.FORMATTER)
                 formatter: dict[str, str] = {}
                 for field_item in fields:
                     #if field_item in my_fields:
@@ -3334,23 +3368,32 @@
                 if isinstance(datetime, str):
                     datetime = PIH.DATA.datetime_from_string(datetime, CONST.ISO_DATETIME_FORMAT)
                 return PIH.PATH.replace_prohibited_symbols_from_path_with_symbol(PIH.DATA.datetime_to_string(datetime, A.CT.DATETIME_FORMAT))
 
             @staticmethod
             def by_formatter_name(value: Enum | str, data: Any | None) -> str | None:
                 if isinstance(value, str):
-                    value = A.D.get_by_value(DATA.FORMATTER, value) or value
+                    value = EnumTool.get_by_value(DATA.FORMATTER, value) or value
+                if isinstance(value, str):
+                    name: str = j((PIH.DATA.STATISTICS.NAME, "_"))
+                    index: int = value.lower().find(name)
+                    if index != -1:
+                        index += len(name)
+                        type: MATERIALIZED_RESOURCES.TYPES | None = EnumTool.get_by_value_or_key(MATERIALIZED_RESOURCES.TYPES, value[index: ].upper())
+                        if DataTool.is_none(type):
+                            return None
+                        return PIH.DATA.FORMAT.statistics(type)
                 if isinstance(value, str):
                     return PIH.SETTINGS.get(value) or PIH.DATA.VARIABLE.get(value)
                 if value == DATA.FORMATTER.MY_DATETIME:
                     return PIH.DATA.FORMAT.datetime(data)
                 if value == DATA.FORMATTER.MY_DATE:
                     return PIH.DATA.FORMAT.date(data)
                 if value == DATA.FORMATTER.CHILLER_FILTER_COUNT:
-                    return str(PIH.DATA.MATERIALIZED_RESOURCES.get_count(MATERIALIZED_RESOURCES.TYPES.CHILLER_FILTER_COUNT))
+                    return str(PIH.DATA.MATERIALIZED_RESOURCES.get_count(MATERIALIZED_RESOURCES.TYPES.CHILLER_FILTER))
                 if value == DATA.FORMATTER.CHILLER_INDICATIONS_VALUE_INDICATORS:
                     result_list: list[str] = [] 
                     for index in range(len(INDICATIONS.CHILLER.INDICATOR_NAME)):
                         if BM.has_index(data, index):
                             result_list.append(f"{A.CT_V.BULLET} {INDICATIONS.CHILLER.INDICATOR_NAME[index]}")
                     return "\n".join(("\n", "\n".join(result_list), ""))
                 return None
@@ -3403,15 +3446,15 @@
             @staticmethod
             def telephone_number_international(value: str) -> str:
                 return PIH.DATA.FORMAT.telephone_number(value, CONST.INTERNATIONAL_TELEPHONE_NUMBER_PREFIX)
 
             @staticmethod
             def email(value: str, add_default_domain: bool = False, remove_restricted_symbols: bool = False) -> str:
                 if add_default_domain and value.find("@") == -1:
-                    return PIH.DATA.FORMAT.email("@".join((value, CONST.SITE_URL)))
+                    return PIH.DATA.FORMAT.email("@".join((value, CONST.SITE_ADDRESS)))
                 if remove_restricted_symbols:
                     for char in "\"(),:;<>[\\] ":
                         value = value.replace(char, "")
                 return value#.lower()
 
             @staticmethod
             def name(value: str, remove_non_alpha: bool = False, name_part_minimal_length: int | None = None) -> str:
@@ -4317,23 +4360,23 @@
                 return Result(FIELD_COLLECTION.AD.USER, DataTool.check(value, lambda: DataTool.get_first_item(PIH.RESULT.USER.by_full_name(FullNameTool.fullname_from_string(value.FullName)).data)))
 
     class CHECK:
 
         class EVENTS:
 
             @staticmethod
-            def has(value: Events | None, parameters: tuple[Any] | None) -> bool:
+            def has(value: Events | None, parameters: tuple[Any] | None = None) -> bool:
                 return not ResultTool.is_empty(PIH.RESULT.EVENTS.get(value, parameters))
 
             @staticmethod
-            def timeouted(event: Events, parameters: dict | None, timeout: int) -> bool:
+            def timeouted(event: Events, parameters: dict | None, timeout_in_seconds: int) -> bool:
                 event_ds: EventDS | None = A.R.get_first_item(
                     A.R.sort(A.R_E.get(event, parameters), lambda item: item.timestamp, reserve=True))
                 return DataTool.is_none(event_ds) or (
-                    DateTimeTool.now() - event_ds.timestamp).seconds > timeout
+                    DateTimeTool.now() - event_ds.timestamp).total_seconds() > timeout_in_seconds
 
         class SETTINGS:
     
             @staticmethod
             def by_time(current: datetime, settings: SETTINGS) -> bool:
                 return DateTimeTool.is_equal_by_time(current, PIH.SETTINGS.to_datetime(settings))
 
@@ -5222,15 +5265,15 @@
                 return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.register_event, (EventDS(value.name, parameters, DateTimeTool.now()), )))
 
             @staticmethod
             def update(value: Events, parameter_for_search: tuple[Any], parameters_for_set: tuple[Any]) -> bool:
                 return PIH.ACTION.EVENTS.remove(value, parameter_for_search) and PIH.ACTION.EVENTS.register(value, PIH.EVENT.BUILDER.create_parameters_map(value, parameters_for_set))
 
             @staticmethod
-            def remove(value: Events, parameters: tuple[Any] | dict[str, Any]) -> bool:
+            def remove(value: Events, parameters: tuple[Any] | dict[str, Any] | None = None) -> bool:
                 return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.remove_event, EventDS(value.name, DataTool.check(isinstance(parameters, dict), parameters, lambda: PIH.EVENT.BUILDER.create_parameters_map(value, parameters, check_for_parameters_count=False)))))
 
         class NOTES:
         
             @staticmethod
             def create(name: str, note: Note) -> bool:
                 id: str | None = DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.create_note, (note, )))
@@ -5535,15 +5578,15 @@
                 return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.save_base64_as_image, (path, content)))
 
             @staticmethod
             def create_for_user(path: str, full_name: FullName, tab_number: str, pc: LoginPasswordPair, polibase: LoginPasswordPair, email: LoginPasswordPair) -> bool:
                 locale.setlocale(locale.LC_ALL, 'ru_RU')
                 date_now = datetime.now().date()
                 date_now_string = f"{date_now.day} {calendar.month_name[date_now.month]} {date_now.year}"
-                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.create_user_document, (path, date_now_string, CONST.SITE_URL, CONST.SITE_PROTOCOL + CONST.SITE_URL, CONST.EMAIL_SERVER_URL, full_name, tab_number, pc, polibase, email)))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.create_user_document, (path, date_now_string, CONST.SITE_ADDRESS, CONST.SITE_PROTOCOL + CONST.SITE_ADDRESS, CONST.EMAIL_SERVER_ADDRESS, full_name, tab_number, pc, polibase, email)))
 
         class WORKSTATION:
     
             @staticmethod
             def reboot(host: str | None = None, force: bool = False) -> bool:
                 return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.reboot, (host, force)))
 
@@ -5578,15 +5621,15 @@
                 windows_service_information = name, workstation_name
                 if not A.C_WS.windows_service_running(*windows_service_information):
                     return A.A_WS.start_windows_service(*windows_service_information)
                 return None
 
 class ActionStack(list):
 
-    def __init__(self, caption: str = "", *argv, input: InputBase = None, output: OutputBase = None):
+    def __init__(self, caption: str = "", *argv: Callable[[], ActionValue], input: InputBase = None, output: OutputBase = None):
         self.input = input or PIH.input
         self.output = output or PIH.output
         self.acion_value_list: list[ActionValue] = []
         self.caption = caption
         for arg in argv:
             self.append(arg)
         self.start()
@@ -5653,14 +5696,15 @@
     D_FL = D.FILTER
     D_Ex = D.EXTRACT
     D_Ex_E = D_Ex.EVENT
     D_M = D.MARK
     D_C = D.CHECK
     D_STAT = D.STATISTICS
     A = root.ACTION
+    
     A_D = A.DOCUMENTS
     A_QR = A.QR_CODE
     A_I = A.INDICATION
     A_I_CT = A_I.CT
     A_I_CH = A_I.CHILLER
     ME = root.MESSAGE
     ME_P = ME.POLIBASE
@@ -5785,14 +5829,15 @@
     CT_SR = ServiceRoles
     CT_SC = ServiceCommands
     CT_SubT = SubscribtionTypes
     CT_F = FILE
     CT_R = RESOURCES
     CT_R_D = CT_R.DESCRIPTIONS
     CT_R_IR = CT_R.INACCESSABLE_REASONS
+    CT_STATISTICS = STATISTICS
     CT_F_E = CT_F.EXTENSION
     CT_P = CT.POLIBASE
     CT_P_DD = CT_P.DOCUMENT_DESCRIPTIONS
     CT_FC = FIELD_COLLECTION
     CT_S = SETTINGS
     CT_ME = CT.MESSAGE
     CT_ME_WH = CT_ME.WHATSAPP
```

### Comparing `pih-1.47001/pih/rpc.py` & `pih-1.47201/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47001/pih/rpcCommandCall_pb2.py` & `pih-1.47201/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.47001/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.47201/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47001/pih/rpc_collection.py` & `pih-1.47201/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47001/pih/rpc_const.py` & `pih-1.47201/pih/rpc_const.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,8 +167,10 @@
     get_barcode_list_information: int = auto()
     document_type_exists: int = auto()
     #
     listen_for_new_files: int = auto()
     #
     recognize_document: int = auto()
     #
-    get_polibase_person_by_email: int = auto()
+    get_polibase_person_by_email: int = auto()
+    #
+    create_statistics_chart: int = auto()
```

### Comparing `pih-1.47001/pih/service_example.py` & `pih-1.47201/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.47001/pih/tools.py` & `pih-1.47201/pih/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,18 @@
     return value or ""
 
 def b(value: str) -> str:
     if not DataTool.is_empty(value) and value.find("*") == -1:
         return f"*{value}*"
     return value or ""
 
-def nl(value: str, count: int = 1) -> str:
-    return value + "\n"*count
+def nl(value: str = "", count: int = 1) -> str:
+    return j((value, "\n"*count))
 
-def j(value: tuple | list[str], splitter: str = "") -> str:
+def j(value: tuple[str] | list[str], splitter: str = "") -> str:
     return splitter.join(value)
 
 class EnumTool:
 
     @staticmethod
     def get(cls: Enum | Any, key: str | None = None, default_value: Any | None = None, return_value: bool = True) -> Any | None:
         if return_value and DataTool.is_empty(key):
@@ -392,14 +392,18 @@
 
     def set(self, index: int, value: Any) -> None:
         self.list[index] = value
 
 class DateTimeTool:
 
     @staticmethod
+    def seconds_to_days(value: int) -> float:
+        return value/60/60/24
+
+    @staticmethod
     def yesterday() -> datetime:
         return DateTimeTool.today(-1, as_datetime=True)
 
     @staticmethod
     def start_date(value: datetime | date) -> datetime | date:
         return value.replace(hour=0, minute=0, second=0, microsecond=0) if isinstance(value, datetime) else value
     
@@ -653,14 +657,19 @@
 
     @staticmethod
     def unpack_data(result: dict) -> Any:
         return result["data"]
 
    
 class PathTool:
+     
+    @staticmethod
+    def exists(path: str) -> bool:
+        return os.path.exists(path)
+
 
     @staticmethod
     def get_file_list(path: str, created_after: float | None = None) -> list[str]:
         file_list = [(file_path, os.path.getctime(file_path))
                      for file_path in [os.path.join(path, file_path) for file_path in [
                          file_path for file_path in next(walk(path), (None, None, []))[2]]]]
         if created_after is not None:
@@ -689,15 +698,15 @@
         if dot_index != -1:
             source_extension: str = file_path.split(".")[-1]
             if source_extension == extension:
                 file_path = file_path[0: dot_index]
         return f"{file_path}.{extension}"
 
     @staticmethod
-    def get_file_name(path: str, with_extension:bool = False):
+    def get_file_name(path: str, with_extension: bool = False):
         head, tail = ntpath.split(path)
         value = tail or ntpath.basename(head)
         if not with_extension:
             value = value[0: value.rfind(".")]
         return value
 
     @staticmethod
```

### Comparing `pih-1.47001/pih/widgets.py` & `pih-1.47201/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.47001/pih_setup.py` & `pih-1.47201/pih_setup.py`

 * *Files identical despite different names*

