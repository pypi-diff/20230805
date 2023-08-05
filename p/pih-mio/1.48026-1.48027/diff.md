# Comparing `tmp/pih-mio-1.48026.tar.gz` & `tmp/pih-mio-1.48027.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-1.48026.tar", last modified: Fri Aug  4 02:07:45 2023, max compression
+gzip compressed data, was "pih-mio-1.48027.tar", last modified: Sat Aug  5 01:23:08 2023, max compression
```

## Comparing `pih-mio-1.48026.tar` & `pih-mio-1.48027.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 02:07:45.622200 pih-mio-1.48026/
-drwxrwxrwx   0        0        0        0 2023-08-04 02:07:45.904269 pih-mio-1.48026/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48026/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48026/MobileHelperCore/__main__.py
--rw-rw-rw-   0        0        0   165341 2023-08-04 02:06:57.000000 pih-mio-1.48026/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48026/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9540 2023-08-04 02:06:12.000000 pih-mio-1.48026/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48026/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-08-04 02:07:46.107386 pih-mio-1.48026/PKG-INFO
--rw-rw-rw-   0        0        0     1651 2023-08-03 07:25:38.000000 pih-mio-1.48026/pih-mio_setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:07:46.076139 pih-mio-1.48026/pih_mio.egg-info/
--rw-rw-rw-   0        0        0      279 2023-08-04 02:07:44.000000 pih-mio-1.48026/pih_mio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-08-04 02:07:45.000000 pih-mio-1.48026/pih_mio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 02:07:44.000000 pih-mio-1.48026/pih_mio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-08-04 02:07:44.000000 pih-mio-1.48026/pih_mio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-08-04 02:07:45.000000 pih-mio-1.48026/pih_mio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-04 02:07:45.000000 pih-mio-1.48026/pih_mio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 02:07:46.107386 pih-mio-1.48026/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 01:23:08.316552 pih-mio-1.48027/
+drwxrwxrwx   0        0        0        0 2023-08-05 01:23:08.550935 pih-mio-1.48027/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48027/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48027/MobileHelperCore/__main__.py
+-rw-rw-rw-   0        0        0   168458 2023-08-05 01:21:48.000000 pih-mio-1.48027/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48027/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9589 2023-08-05 00:19:42.000000 pih-mio-1.48027/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48027/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-08-05 01:23:08.790007 pih-mio-1.48027/PKG-INFO
+-rw-rw-rw-   0        0        0     1651 2023-08-03 07:25:38.000000 pih-mio-1.48027/pih-mio_setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 01:23:08.754044 pih-mio-1.48027/pih_mio.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-08-05 01:23:07.000000 pih-mio-1.48027/pih_mio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-08-05 01:23:08.000000 pih-mio-1.48027/pih_mio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 01:23:07.000000 pih-mio-1.48027/pih_mio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-08-05 01:23:07.000000 pih-mio-1.48027/pih_mio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-08-05 01:23:07.000000 pih-mio-1.48027/pih_mio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-05 01:23:07.000000 pih-mio-1.48027/pih_mio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 01:23:08.800922 pih-mio-1.48027/setup.cfg
```

### Comparing `pih-mio-1.48026/MobileHelperCore/api.py` & `pih-mio-1.48027/MobileHelperCore/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,30 +16,30 @@
     sys.path.append("//pih/facade")
 from pih import (PIH, A, NotFound, 
                 Stdin, Session, Output,
                 Input, while_not_do, MarkInput,
                 UserInput, UserOutput, MarkOutput, 
                 SessionBase, BarcodeNotFound)
 from pih.const import CheckableSections, Actions
-from pih.tools import BitMask as BM, ResultUnpack, i, b, nl, j
+from pih.tools import BitMask as BM, ResultUnpack, i, b, nl, j, if_else
 from pih.console_api import ConsoleAppsApi
 from pih.collection import (User, Result, Workstation, 
                             RobocopyJobStatus, Mark, MarkGroup, 
                             FieldItem, FieldItemList, PolibasePerson, 
                             Note, ActionDescription, StorageValue, 
                             IntStorageValue, TimeStorageValue, BoolStorageValue,
-                            CommandMenuItem)
+                            CommandMenuItem, EventDS, CardRegistryFolderPosition)
 from MobileHelperContent.content import MEDIA_CONTENT
 import requests
 from io import BytesIO
 
 class MIO:
 
     NAME: str = "mio"       
-    VERSION: str = "1.48026"  
+    VERSION: str = "1.48027"  
 
 class InternalInterrupt(Exception):
 
     @property
     def type(self) -> int:
         return self.args[0]
 
@@ -847,15 +847,15 @@
             robocopy_node,
             polibase_backup_node
         ]
         run_command_node: CommandNode = CommandNode(
             "run|Выполнение команд|!", None, self.run_commnad_handler, MobileHelper.ADM)
         #######################
         polibase_person_find_node: CommandNode = CommandNode("fclient", "Поиск пациента|Поиск",
-                                                             self.polibase_person_find_handler, MobileHelper.ADM)
+                                                             self.polibase_person_find_handler)
         polibase_person_find_card_registry_folder_node: CommandNode = CommandNode(None, "Поиск карты пациента|Поиск карты",
                                                                                   self.polibase_person_card_registry_folder_find_handler, filter_function=lambda: A.D_C.empty(get_polibase_person_card_registry_folder_name()))
         
         check_email_node: CommandNode = CommandNode(
             "email|почт^ы|mail", "Проверка адресса электронной почты|Адресс электронной почты", lambda: self.check_email_address_handler())  
         
         check_valenta_node: CommandNode = CommandNode(
@@ -927,14 +927,15 @@
             polibase_restart_node,
             polibase_close_node
         ]
 
         def get_polibase_person_card_registry_folder_name() -> str:
             result: str = self.first_arg("")
             return "" if not A.C_P.person_card_registry_folder(result) or A.D_C.empty(result) else f" \"{result}\""
+        
         #######################
         infinity_study_course_node: CommandNode = CommandNode(
             "infinity", "Обучающий курс \"Регистартор и Оператор колл-центра: инфинити\"", lambda: self.study_course_handler(
                 None, INFINITY_STUDY_COURSE_COLLECTION, INFINITY_STUDY_COURCE_CONTENT_LIST, lambda:  MEDIA_CONTENT.IMAGE.INFINITY_WIKI_LOCATION))
         card_registry_study_course_node: CommandNode = CommandNode(
             "card", "Обучающий курс \"Реестр карт пациентов\"", lambda: self.study_course_handler(
                 None, CARD_REGISTRY_STUDY_COURSE_COLLECTION, CARD_REGISTRY_STUDY_COURCE_CONTENT_LIST, lambda: MEDIA_CONTENT.IMAGE.CARD_REGISTRY_WIKI_LOCATION), filter_function=lambda: A.D_C.empty(get_polibase_person_card_registry_folder_name()))
@@ -954,23 +955,26 @@
         def polibase_person_sort_card_registry_folder_title_and_label() -> str:
             value: str = get_polibase_person_card_registry_folder_name()
             if not A.D_C.empty(value):
                 value = f" {value}"
             return f"Сортировка карт папки{value}|Сортировать карты в папке{value}"
         polibase_person_card_add_to_card_registry_folder_node: CommandNode = CommandNode(
             "add|добавить|+", polibase_person_add_to_card_registry_folder_title_and_label, self.add_polibase_person_to_card_registry_folder_handler, MobileHelper.ADM + [A.CT_AD.Groups.CardRegistry], text="Добавляет карту пациента в папку реестра", help = lambda: f"{b('название_папки')} [ {b('поисковый запрос для поиска пациента')} ]. Например pih add п1к {A.CT.TEST.PIN}")
+        polibase_person_card_registry_folder_register: CommandNode = CommandNode(
+            "register", lambda: f"Зарегистроровать в реестре карту пациента{get_polibase_person_card_registry_folder_name()}", self.register_card_registry_folder_handler, MobileHelper.ADM)
         #sort_card_registry_folder_node: CommandNode = CommandNode(
         #    "sort|сортиров^ать", polibase_person_sort_card_registry_folder_title_and_label, self.sort_card_registry_folder_handler, MobileHelper.ADM + [A.CT_AD.Groups.CardRegistry])
         CARD_REGISTRY_MENU: list[CommandNode] = [
             #card_registry_study_course_node.clone_as(
             #    None, "Обучающий курс \"Реестр карт пациентов\""),
             polibase_persons_by_card_registry_folder_name_node,
             polibase_person_card_add_to_card_registry_folder_node,
             polibase_person_find_card_registry_folder_node,
             polibase_person_card_registry_folder_qr_code_create_node,
+            polibase_person_card_registry_folder_register
             #sort_card_registry_folder_node
         ]
         #######################
         WIKI_BASE_CONTENT_LIST: list[HelpImageContent] = [
             HelpImageContent(lambda: MEDIA_CONTENT.IMAGE.WIKI_ICON,
                              f"Пройти обучение можно на нашем внутреннем сайте: *Wiki*. Ниже покажем Вам, {self.user_given_name}, как зайти на этот сайт.\n\n_*Обратите внимание*, что доступ к данному сайту возможен только с *компьютера* рабочего места пользователя!_", "Найдите на *Рабочем столе* иконку с названием *Wiki* и откройте ее", False),
             HelpImageContent(lambda: MEDIA_CONTENT.IMAGE.WIKI_GET_ACCESS, None,
@@ -1125,14 +1129,15 @@
             }, 
             CommandNode("card|реестр", "Реестр", [A.CT_AD.Groups.CardRegistry], show_in_root_menu=True): CommandNode("registry|карт^ пациентов|cr", "карт пациентов", lambda: self.menu_handler(CARD_REGISTRY_MENU), filter_function=lambda: self.argless),
             CommandNode("card|реестр", "|"): {
                 CommandNode("registry|карт^ пациентов|cr", "|"): {
                     polibase_person_card_add_to_card_registry_folder_node : None,
                     polibase_persons_by_card_registry_folder_name_node: None,
                     polibase_person_card_registry_folder_qr_code_create_node: None,
+                    polibase_person_card_registry_folder_register: None
                     #sort_card_registry_folder_node: None
                 }
             },
             CommandNode("backup", "Бекап", lambda: self.menu_handler(BACKUP_MENU), MobileHelper.ADM, show_in_root_menu=True): None,
             robocopy_node: None,
             polibase_backup_node: None,
             CommandNode("find|поиск|search|найти"):
@@ -1408,27 +1413,27 @@
             self.console_apps_api.start_user_telephone_number_editor()
         else:
             self.console_apps_api.start_user_property_setter(self.input.indexed_field_list(
             "Выберите действие", action_list) if index is None else action_list.get_name_list()[index], self.first_arg(), True)
 
     @property
     def is_all(self) -> bool:
-        return self.has_flag(Flags.ALL)
+        return self.has_flag(Flags.ALL) or BM.has(self.income_flags, Flags.ALL)
     
     @property
     def is_only_result(self) -> bool:
-        return self.has_flag(Flags.ONLY_RESULT)
+        return self.has_flag(Flags.ONLY_RESULT) or BM.has(self.income_flags, Flags.ONLY_RESULT)
 
     @property
     def is_silence(self) -> bool:
         return self.has_flag(Flags.SILENCE) or BM.has(self.income_flags, Flags.SILENCE)
     
     @property
     def is_forced(self) -> bool:
-        return self.has_flag(Flags.FORCED)
+        return self.has_flag(Flags.FORCED) or BM.has(self.income_flags, Flags.FORCED)
 
     def workstation_action_handler(self, action_index: int | None = None) -> None:
         if action_index is None:
             action_index = self.input.index(
                 "Выберите действие", ["Перезагрузить", "Выключить", "Найти"], lambda item, _: item)
         search_value: str | None = None
         is_all: bool = self.is_all
@@ -1851,14 +1856,26 @@
                                     if step_limit > 0 and (step % step_limit) == 0:
                                         self.output.separated_line()
                                         self.input.input("Отправьте любое сообщение для продолжения...")    
                         sort_action(A.D_Ex.decimal(self.input.input("Введите какое количество операций сортировки выводить за раз. Введя 0: появяться все операции для сортировки карт в папке"))) 
                 else:
                     self.show_error(f"Папка реестра карт {card_registry_folder} уже отсортирована")
 
+    def register_card_registry_folder_handler(self) -> None:
+        with self.output.personalized():
+            def check(value: str) -> str | None:
+                return A.D_Ex.decimal(value)
+            polibase_person_card_registry_folder: str = A.D_F.polibase_person_card_registry_folder(self.arg() or self.input.polibase_person_card_registry_folder()) 
+            A.E.send(*A.E_B.card_registry_folder_was_registered(polibase_person_card_registry_folder, 
+                self.input.input("Введите номер шкафа", check_function=check), 
+                self.input.input("Введите номер полки",
+                                 check_function=check),
+                self.input.input("Введите позицию на полке (0 - без позиции)", check_function=check)))
+
+
     def add_polibase_person_to_card_registry_folder_handler(self) -> None: 
         with self.output.personalized():
             interruption: InternalInterrupt | None = None 
             polibase_person_card_registry_folder: str = A.D_F.polibase_person_card_registry_folder(self.arg() or self.input.polibase_person_card_registry_folder()) 
             try:
                 with self.input.input_timeout(None):
                     result_polibase_person_list: Result[list[PolibasePerson]] = A.CR.persons_by_folder(polibase_person_card_registry_folder)
@@ -2047,46 +2064,64 @@
                         person_pin_list: list[int] = A.CR.persons_pin_by_folder(person.ChartFolder)
                         position_map[person.pin] = (person_pin_list.index(person.pin) + 1, len(person_pin_list))
                 A.R.every(person_list_result, prepeare_polibase_person_function)
                 def data_label_function(_, field: FieldItem, person: PolibasePerson, data: Any) -> tuple[bool, str]:
                     result: list[bool, Any] = [True, ""]
                     if field.name in [A.CT_FNC.CARD_REGISTRY_FOLDER, A.CT_FNC.FULL_NAME]:
                         result[1] = f"{b(field.caption)}: {(field.default_value if A.D_C.empty(data) else data)}"
-                        if  field.name == A.CT_FNC.CARD_REGISTRY_FOLDER and not A.D_C.empty(data):
-                            result[1] += (f"\n {A.CT_V.BULLET} {b(A.CT_FC.POSITION.caption)}: " +
-                                        f"{str(position_map[person.pin][0])} из {position_map[person.pin][1]}" if person.pin in position_map else A.CT_FC.POSITION.default_value)
+                        if field.name == A.CT_FNC.CARD_REGISTRY_FOLDER and not A.D_C.empty(data):
+                            result[1] += if_else(person.pin in position_map, lambda: self.get_polibase_person_card_position_label(
+                                person, position_map[person.pin][0], position_map[person.pin][1]), A.CT_FC.POSITION.default_value)
+                            #f" {A.CT_V.BULLET} Карта: {str(position_map[person.pin][0])} из {position_map[person.pin][1]}" if person.pin in position_map else A.CT_FC.POSITION.default_value
                     return tuple(result) 
                 self.output.write_result(
                     person_list_result, False, data_label_function=data_label_function, separated_result_item=False)
                 break
             except NotFound as error:
                 self.show_error(error)
                 value = None
             except BarcodeNotFound as error:
                 self.show_error(error)
 
+    def get_polibase_person_card_position_label(self, person: PolibasePerson, card_position: int | None, card_length: int) -> str:
+        label_list: list[str] = []
+        label_list.append(f"{b(A.CT_FC.POSITION.caption)}:")
+        if not A.D_C.empty(person.ChartFolder):
+            letter: str | None = person.ChartFolder[0]
+            if letter in A.CT.CARD_REGISTRY.PLACE_NAME:
+                label_list.append(f" {A.CT_V.BULLET} Место: {A.CT.CARD_REGISTRY.PLACE_NAME[letter]}")
+            card_registry_folder_was_registered_event: EventDS | None = A.R.get_first_item(A.R_E.get(*A.E_B.card_registry_folder_was_registered(person.ChartFolder)))
+            if not A.D_C.empty(card_registry_folder_was_registered_event):
+                position: CardRegistryFolderPosition = A.D.fill_data_from_source(
+                    CardRegistryFolderPosition(), card_registry_folder_was_registered_event.parameters)
+                label_list.append(j((f" {A.CT_V.BULLET} Папка:\n     шкаф: {b(position.p_a)}\n     полка: {b(position.p_b)}", if_else(
+                    position.p_c > 0, f"\n     позиция на полке: {b(position.p_c)}", ""))))
+            label_list.append(if_else(A.D_C.empty(card_position), A.CT_FC.POSITION.default_value, lambda: f" {A.CT_V.BULLET} Карта в папке: {b(card_position)} из {b(card_length)}"))
+            return nl(j(label_list, nl()), reversed=True)
+        return ""
+
     def polibase_person_find_handler(self) -> None:
         while True:
             try:
-                def action_function(person: PolibasePerson) -> tuple[int, int]:
+                def action_function(person: PolibasePerson) -> tuple[int | None, int]:
                     if not A.D_C.empty(person.ChartFolder):
                         result: Result[list[PolibasePerson]] = A.CR.persons_by_folder(person.ChartFolder)
                         if not A.D_C.empty(result):
                             person_list: list[PolibasePerson] = result.data
                             for index, person_item in enumerate(person_list):
                                 if person_item.pin == person.pin:
                                     return (index + 1, len(person_list))
-                            return (-1, len(person_list))   
-                    return (-1, 0)
+                            return (None, len(person_list))   
+                    return (None, 0)
                 def data_label_function(_, field: FieldItem, person: PolibasePerson, data: Any) -> tuple[bool, str | None]:
                     if field.name == A.CT_FNC.CARD_REGISTRY_FOLDER:
                         if A.D_C.empty(data):
                             return (True, None) 
-                        position_data: tuple[int, int] = action_function(person)
-                        return (True, f"{b(A.CT_FC.POLIBASE.CARD_REGISTRY_FOLDER.caption)}: {data}" + ("" if position_data[0] == 0 else f"\n {A.CT_V.BULLET} {b(A.CT_FC.POSITION.caption)}: {position_data[0]} из {position_data[1]}")) 
+                        position_map: tuple[int | None, int] = action_function(person)
+                        return (True, f"{b(A.CT_FC.POLIBASE.CARD_REGISTRY_FOLDER.caption)}: {data}" + if_else(A.D_C.empty(position_map[0]), "", lambda: self.get_polibase_person_card_position_label(person, position_map[0], position_map[1])))
                     return (False, None)
                 self.output.write_result(
                     A.R_P.persons_by_any(self.first_arg() or self.input.polibase_person_any()), data_label_function=data_label_function)
                 break
             except NotFound as error:
                 self.show_error(error)
             except BarcodeNotFound as error:
```

### Comparing `pih-mio-1.48026/MobileHelperCore/service.py` & `pih-mio-1.48027/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48026/MobileHelperCore/service_api.py` & `pih-mio-1.48027/MobileHelperCore/service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 SR = A.CT_SR
 SC = A.CT_SC
 
 ROLE: SR = SR.MOBILE_HELPER
 
 #version 0.8
 
+AS_DEVELOPER_ALIAS: str = "as_developer"
+
 def as_developer() -> bool:
-    return A.SE.named_arg("as_developer")
+    return A.SE.named_arg(AS_DEVELOPER_ALIAS)
 
 class MobileHelperService():
 
     INIT: bool = False
     INSTANCE: Any | None = None
     NAME: str = "MobileHelper"
    
@@ -45,15 +47,15 @@
         self.checker = checker
         self.service_role: SR = SR.MOBILE_HELPER
         self.allow_send_to_next_service_in_chain: dict[str, bool] = defaultdict(bool)
         MobileHelperService.INSTANCE = self  
            
     def start(self) -> bool:
         if MobileHelperService.INIT:
-            A.SE.add_arg("--as_developer",
+            A.SE.add_arg(AS_DEVELOPER_ALIAS,
                     nargs="?", const=1, type=str, default=None)
             service_role_desctiption: self.ServiceRoleDescription | None = A.SRV_A.create_support_service_or_master_service_description(A.CT_SR.description(self.service_role))
             if not A.D_C.empty(service_role_desctiption):
                 with A.ER.detect_interruption("Выход"):
                     A.SRV_A.serve(service_role_desctiption, self.service_call_handler,
                                 MobileHelperService.service_starts_handler)
                 return True
@@ -166,9 +168,9 @@
             self.receive_message_handler(
                 " ".join((self.root, parameter_list.next())), parameter_list.next(), parameter_list.next())
         return None
 
     @staticmethod
     def service_starts_handler() -> None:
         if as_developer():
-            A.O.blue("For developer")
+            A.O.blue("As developer")
         A.SRV_A.subscribe_on(A.CT_SC.send_event, A.CT_SubT.ON_RESULT_SEQUENTIALLY, MobileHelperService.NAME)
```

### Comparing `pih-mio-1.48026/MobileHelperCore/tools.py` & `pih-mio-1.48027/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48026/pih-mio_setup.py` & `pih-mio-1.48027/pih-mio_setup.py`

 * *Files identical despite different names*

