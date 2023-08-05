# Comparing `tmp/pih-1.48035.tar.gz` & `tmp/pih-1.48036.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.48035.tar", last modified: Fri Aug  4 02:07:09 2023, max compression
+gzip compressed data, was "pih-1.48036.tar", last modified: Sat Aug  5 01:22:36 2023, max compression
```

## Comparing `pih-1.48035.tar` & `pih-1.48036.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 02:07:10.152557 pih-1.48035/
--rw-rw-rw-   0        0        0      261 2023-08-04 02:07:10.168187 pih-1.48035/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-04 02:07:09.869509 pih-1.48035/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48035/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48035/pih/collection.py
--rw-rw-rw-   0        0        0    60753 2023-08-04 00:59:36.000000 pih-1.48035/pih/console_api.py
--rw-rw-rw-   0        0        0   109574 2023-08-04 01:03:56.000000 pih-1.48035/pih/const.py
--rw-rw-rw-   0        0        0   320958 2023-08-04 02:06:50.000000 pih-1.48035/pih/pih.py
--rw-rw-rw-   0        0        0    25372 2023-08-04 02:02:54.000000 pih-1.48035/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48035/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48035/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2528 2023-08-03 23:30:35.000000 pih-1.48035/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6492 2023-08-03 06:51:54.000000 pih-1.48035/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48035/pih/service_example.py
--rw-rw-rw-   0        0        0    38338 2023-08-04 01:31:31.000000 pih-1.48035/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48035/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:07:10.121832 pih-1.48035/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-08-04 02:07:07.000000 pih-1.48035/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-08-04 02:07:08.000000 pih-1.48035/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 02:07:07.000000 pih-1.48035/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-08-04 02:07:08.000000 pih-1.48035/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-04 02:07:08.000000 pih-1.48035/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2007 2023-08-03 07:28:58.000000 pih-1.48035/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-08-04 02:07:10.168187 pih-1.48035/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 01:22:37.116229 pih-1.48036/
+-rw-rw-rw-   0        0        0      261 2023-08-05 01:22:37.116229 pih-1.48036/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-05 01:22:36.756857 pih-1.48036/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48036/pih/__init__.py
+-rw-rw-rw-   0        0        0    20623 2023-08-04 07:31:27.000000 pih-1.48036/pih/collection.py
+-rw-rw-rw-   0        0        0    60497 2023-08-04 05:28:08.000000 pih-1.48036/pih/console_api.py
+-rw-rw-rw-   0        0        0   109844 2023-08-05 00:41:16.000000 pih-1.48036/pih/const.py
+-rw-rw-rw-   0        0        0   321386 2023-08-05 01:22:20.000000 pih-1.48036/pih/pih.py
+-rw-rw-rw-   0        0        0    25361 2023-08-04 02:35:41.000000 pih-1.48036/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48036/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48036/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2528 2023-08-03 23:30:35.000000 pih-1.48036/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6492 2023-08-03 06:51:54.000000 pih-1.48036/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48036/pih/service_example.py
+-rw-rw-rw-   0        0        0    38478 2023-08-04 06:53:51.000000 pih-1.48036/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48036/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-05 01:22:37.084979 pih-1.48036/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-08-05 01:22:34.000000 pih-1.48036/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-08-05 01:22:35.000000 pih-1.48036/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 01:22:34.000000 pih-1.48036/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-05 01:22:35.000000 pih-1.48036/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-05 01:22:35.000000 pih-1.48036/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2007 2023-08-03 07:28:58.000000 pih-1.48036/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-08-05 01:22:37.131854 pih-1.48036/setup.cfg
```

### Comparing `pih-1.48035/pih/collection.py` & `pih-1.48036/pih/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,22 @@
 class InaccesableEmailInformation:
     email: str | None = None
     person_pin: int = 0
     person_name: str | None = None
     workstation_name: str | None = None
     registrator_person_name: str | None = None
 
+
+@dataclass
+class CardRegistryFolderPosition:
+    ChartFolder: str | None = None
+    p_a: int = 0
+    p_b: int = 0
+    p_c: int = 0
+
 @dataclass
 class FullName:
     last_name: str = ""
     first_name: str = ""
     middle_name: str = ""
 
 @dataclass
```

### Comparing `pih-1.48035/pih/console_api.py` & `pih-1.48036/pih/console_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,36 +385,36 @@
                 self.output.error("Отмена")
 
     def who_lost_the_mark(self, tab_number: str | None = None):
         try:
             tab_number = tab_number or self.input.tab_number()
             if tab_number is not None:
                 try:
-                    mark: Mark = self.pih.RESULT.MARK.by_tab_number(
+                    mark: Mark = A.R_M.by_tab_number(
                         tab_number).data
                     mark_type: MarkType = A.D.get(MarkType, mark.type)
                     if mark_type == MarkType.FREE:
                         self.output.good("Это свободная карта доступа")
                     elif mark_type == MarkType.GUEST:
                         self.output.good("Это гостевая карта доступа")
                     else:
                         if mark_type == MarkType.TEMPORARY:
-                            mark = self.pih.RESULT.MARK.temporary_mark_owner(
+                            mark = A.R_M.temporary_mark_owner(
                                 mark).data
                             tab_number = mark.TabNumber
                             self.output.good("Это временная карта доступа")
                         if mark is not None:
                             telephone_number: str = mark.telephoneNumber
                             self.output.value("Персона", mark.FullName)
-                            if not self.pih.CHECK.telephone_number(telephone_number):
+                            if not A.C.telephone_number(telephone_number):
                                 user: User = A.R_U.by_tab_number(
                                     tab_number).data
                                 if user is not None:
                                     telephone_number = user.telephoneNumber
-                            if not self.pih.CHECK.telephone_number(telephone_number):
+                            if not A.C.telephone_number(telephone_number):
                                 self.output.error(f"Телефон не указан")
                             else:
                                 self.output.value(
                                     "Телефон", telephone_number)
                                 if self.input.yes_no("Отправить сообщение", True):
                                     details: str = self.input.input(
                                         f"{self.get_formatted_given_name()}, уточните, где забрать найденную карту")
@@ -488,15 +488,15 @@
         self.tab_number: str | None = None
         self.telephone_number: str | None = None
         self.division_id: int | None = None
 
         def get_full_name() -> ActionValue:
             self.output.header("Заполните ФИО персоны")
             self.full_name = self.input.full_name(True)
-            user_exists: bool = not self.pih.CHECK.MARK.exists_by_full_name(
+            user_exists: bool = not A.C.MARK.exists_by_full_name(
                 self.full_name)
             if user_exists:
                 self.output.error(
                     "Персона с данной фамилией, именем и отчеством уже есть!")
                 if not self.input.yes_no("Продолжить"):
                     self.session.exit()
             return self.output.get_action_value("ФИО персоны", A.D.fullname_to_string(self.full_name))
@@ -525,17 +525,17 @@
                     get_division,
                     get_telephone_number,
                     get_tab_number,
                     input=self.input,
                     output=self.output
                     )
         if self.input.yes_no("Создать карту доступа для персоны", True):
-            if self.pih.ACTION.MARK.create(self.full_name, self.division_id, self.tab_number, self.telephone_number):
+            if A.A_M.create(self.full_name, self.division_id, self.tab_number, self.telephone_number):
                 self.output.good("Карты доступа создана!")
-                self.pih.EVENT.it_notify_about_create_new_mark(
+                A.E.it_notify_about_create_new_mark(
                     self.full_name)
                 if self.input.yes_no("Уведомить персону", True):
                     self.send_whatsapp_message(
                         self.telephone_number, f"Сообщение от ИТ отдела Pacific International Hospital: День добрый, {A.D.to_given_name(self.full_name)}, Вам выдана карта доступа с номером {self.tab_number}")
             else:
                 self.output.error("Карта доступа не создана!")
 
@@ -691,29 +691,29 @@
                 user_list = self.input.user.by_any(search_value, active)
             else:
                 result: Result[list[User]] = A.R_U.by_any(
                     self.input.user.title_any(), active)
                 user_list = result.data
             if property_name == A.CT_UP.USER_STATUS:
                 for status in [A.CT_AD.ACTIVE_USERS_CONTAINER_DN, A.CT_AD.INACTIVE_USERS_CONTAINER_DN]:
-                    work_user_list: list[User] = self.pih.DATA.FILTER.users_by_dn(
+                    work_user_list: list[User] = A.D_F.users_by_dn(
                         user_list, A.CT_AD.INACTIVE_USERS_CONTAINER_DN if status == A.CT_AD.ACTIVE_USERS_CONTAINER_DN else A.CT_AD.ACTIVE_USERS_CONTAINER_DN)
                     for index, user in enumerate(work_user_list):
                         try:
                             self.output.user.result(Result(fields, [user]))
                             if self.input.yes_no(f"{'Активировать' if status == A.CT_AD.ACTIVE_USERS_CONTAINER_DN else 'Деактивировать' } пользователя"):
                                 if status == A.CT_AD.ACTIVE_USERS_CONTAINER_DN:
                                     if self.input.yes_no("Использовать шаблон для пользователя", True):
                                         user_container = self.input.user.template()
                                     else:
                                         user_container = self.input.user.container()
                                 else:
                                     user_container = UserBase(
                                         distinguishedName=A.CT_AD.INACTIVE_USERS_CONTAINER_DN)
-                                if self.pih.ACTION.USER.set_status(user, status, user_container):
+                                if A.A_U.set_status(user, status, user_container):
                                     self.output.good("Успешно")
                                 else:
                                     self.output.error("Ошибка")
                             else:
                                 self.output.new_line()
                                 self.output.error("Отмена")
                         except KeyboardInterrupt:
@@ -726,16 +726,16 @@
             else:
                 for index, user in enumerate(user_list):
                     try:
                         if property_name == A.CT_UP.TELEPHONE_NUMBER:
                             self.output.user.result(
                                 Result(fields, [user]), None)
                             telephone = self.input.telephone_number()
-                            if self.pih.CHECK.telephone_number(telephone) and self.input.yes_no("Установить", True):
-                                if self.pih.ACTION.USER.set_telephone_number(user, telephone):
+                            if A.C.telephone_number(telephone) and self.input.yes_no("Установить", True):
+                                if A.A_U.set_telephone_number(user, telephone):
                                     self.output.good("Успешно")
                                 else:
                                     self.output.error("Ошибка")
                             else:
                                 self.output.error("Отмена")
                         elif property_name == A.CT_UP.PASSWORD:
                             self.output.user.result(
@@ -744,15 +744,15 @@
                             while True:
                                 password = self.input.user.generate_password(True, PASSWORD.get(
                                     self.input.indexed_field_list("Выберите тип пароля", A.CT_FC.POLICY.PASSWORD_TYPE)))
                                 self.output.value("Пароль", password)
                                 if self.input.yes_no("Использовать", True):
                                     break
                             if self.input.yes_no("Установить", True):
-                                if self.pih.ACTION.USER.set_password(user, password):
+                                if A.A_U.set_password(user, password):
                                     self.output.good("Успешно")
                                 else:
                                     self.output.error("Ошибка")
                             else:
                                 self.output.error("Отмена")
                     except KeyboardInterrupt:
                         self.output.new_line()
@@ -784,15 +784,15 @@
         self.description: str | None = None
         self.use_template_user: bool | None = None
         self.need_to_create_mark: bool | None = None
 
         def get_full_name() -> ActionValue:
             self.output.header("Заполнение ФИО пользователя")
             self.full_name = self.input.full_name(True)
-            self.user_is_exists = self.pih.CHECK.USER.exists_by_full_name(
+            self.user_is_exists = A.C.USER.exists_by_full_name(
                 self.full_name)
             if self.user_is_exists:
                 self.output.error(
                     "Пользователем с данной фамилией, именем и отчеством уже есть!")
                 if not self.input.yes_no("Продолжить"):
                     self.session.exit()
             return self.output.get_action_value("ФИО пользователя", A.D.fullname_to_string(self.full_name))
@@ -851,20 +851,21 @@
             self.output.header("Добавление внешней почты")
             if self.input.yes_no("Добавить"):
                 self.external_email = self.input.email()
             return self.output.get_action_value("Адресс внешней электронной почты пользователя", self.external_email if self.external_email else "Нет", False)
 
         def get_division() -> ActionValue:
             full_name_string: str = A.D.fullname_to_string(self.full_name)
-            mark: Mark = self.pih.RESULT.MARK.by_name(
+            mark: Mark = A.R_M.by_name(
                 full_name_string, True).data
             if mark is not None:
                 if self.input.yes_no(
                         f"Найдена карта доступа для персоны {full_name_string} с номером {mark.TabNumber}. Использовать", True):
                     self.need_to_create_mark = False
+                    self.tab_number = mark.TabNumber
                     return None
             self.need_to_create_mark = self.input.yes_no(
                 f"Создать карту доступа для персоны '{full_name_string}'", True)
             if self.need_to_create_mark:
                 self.output.header("Выбор подразделения")
                 person_division: PersonDivision = self.input.mark.person_division()
                 self.division_id = person_division.id
@@ -897,33 +898,33 @@
             input=self.input,
             output=self.output
         )
         polibase_login: str = self.login
         polibase_password: str = self.password
         if self.input.yes_no("Создать аккаунт для пользователя", True):
             if self.use_template_user:
-                self.pih.ACTION.USER.create_from_template(
+                A.A_U.create_from_template(
                     self.user_container.distinguishedName, self.full_name, self.login, self.password, self.description, self.telephone_number, self.internal_email or self.external_email)
             else:
-                self.pih.ACTION.USER.create_in_container(
+                A.A_U.create_in_container(
                     self.user_container.distinguishedName, self.full_name, self.login, self.password, self.description, self.telephone_number, self.internal_email or self.external_email)
             if self.need_to_create_mark:
-                self.tab_number = self.tab_number or self.pih.RESULT.MARK.by_name(
+                self.tab_number = self.tab_number or A.R_M.by_name(
                     A.D.fullname_to_string(self.full_name), True).data.TabNumber
-                self.pih.ACTION.MARK.create(
+                A.A_M.create(
                     self.full_name, self.division_id, self.tab_number, self.telephone_number)
-            user_account_document_path: str = self.pih.PATH.USER.get_document_name(
+            user_account_document_path: str = A.PTH_U.get_document_name(
                 A.D.fullname_to_string(self.full_name), self.login if self.user_is_exists else None)
-            if self.pih.ACTION.DOCUMENTS.create_for_user(user_account_document_path, self.full_name, self.tab_number, LoginPasswordPair(self.login, self.password), LoginPasswordPair(
+            if A.A_D.create_for_user(user_account_document_path, self.full_name, self.tab_number, LoginPasswordPair(self.login, self.password), LoginPasswordPair(
                     polibase_login, polibase_password), LoginPasswordPair(self.internal_email, self.email_password)):
-                self.pih.EVENT.hr_notify_about_new_employee(self.login)
-                self.pih.EVENT.it_notify_about_user_creation(
+                A.E.hr_notify_about_new_employee(self.login)
+                A.E.it_notify_about_user_creation(
                     self.login, self.password)
                 if self.need_to_create_mark:
-                    self.pih.EVENT.it_notify_about_create_new_mark(
+                    A.E.it_notify_about_create_new_mark(
                         self.full_name)
                 if self.input.yes_no("Сообщить пользователю о создании документов", True):
                     self.send_whatsapp_message(
                         self.telephone_number, f"Сообщение от ИТ отдела Pacific International Hospital: День добрый, {A.D.to_given_name(self.full_name)}, Вас ожидает документы и карта доступа с номером {self.tab_number} в отделе")
                 if self.input.yes_no("Отправить пользователю данные об аккаунте", True):
                     self.send_whatsapp_message(
                         self.telephone_number, f"Сообщение от ИТ отдела Pacific International Hospital: День добрый, {A.D.to_given_name(self.full_name)}, данные Вашего аккаунта:\nЛогин: {self.login}\nПароль: {self.password}\nЭлектронная почта: {self.internal_email}")
```

### Comparing `pih-1.48035/pih/const.py` & `pih-1.48036/pih/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,26 +484,14 @@
         ACCEPTEULA: str = "-accepteula"
 
     class MSG:
 
         NAME: str = "msg"
         EXECUTOR: str = NAME
 
-    class DOCS:
-
-        EXCEL_TITLE_MAX_LENGTH: int = 31
-
-        class INVENTORY:
-
-            NAME_COLUMN_NAME: str = "наименование, назначение и краткая характеристика объекта"
-            NUMBER_COLUMN_NAME: str = "инвентарный"
-            QUANTITY_COLUMN_NAME: str = "фактическое наличие"
-            NAME_MAX_LENTH: int = 120
-            QUANTITY_NOT_SET: str = "-"
-
     class BARCODE_READER:
 
         PREFIX: str = "("
         SUFFIX: str = ")"
 
     class MOBILE_HELPER:
 
@@ -535,14 +523,21 @@
 
         TIMEOUT: int | None = None
         TIMEOUT_FOR_PING: int = 20
         LONG_OPERATION_DURATION: int | None = None
 
     HOST = HOSTS()
 
+    class CARD_REGISTRY:
+
+        PLACE_NAME: dict[str, str] = {
+            "Т": "Приёмное отдление",
+            "П": "Поликлиника"
+        }
+
     class POLIBASE:
 
         NAME: str = "Polibase"
 
         PROCESS_NAME: str = "Polibase ODAC"
 
         PRERECORDING_PIN: int = 10
@@ -1099,15 +1094,15 @@
               "Индикаторы", data_formatter=DATA.FORMATTER.CHILLER_INDICATIONS_VALUE_INDICATORS.value)
     INDICATION_TIMESTAMP: FieldItem = FieldItem(FIELD_NAME_COLLECTION.TIMESTAMP, "Время снятия показаний", data_formatter=DATA.FORMATTER.MY_DATETIME.value)
     
 
 class FIELD_COLLECTION:
 
     INDEX: FieldItem = FieldItem("__Index__", "Индекс", True)
-    POSITION: FieldItem = FieldItem("position", "Позиция", True, default_value="Нет")
+    POSITION: FieldItem = FieldItem("position", "Расположение", True, default_value="Нет в реестре карт")
 
     VALUE: FieldItem = FieldItem("", "Значение", True)
     VALUE_LIST: FieldItem = FieldItem("", "Список значений", True)
 
     class ORION:
 
         MARK_ACTION: FieldItemList = FieldItemList(
@@ -1251,15 +1246,15 @@
             FieldItem(FIELD_NAME_COLLECTION.TEMPLATE_USER_CONTAINER,
                       "Шаблонный пользователь"),
             FieldItem(FIELD_NAME_COLLECTION.CONTAINER, "Контейнер"))
 
 
     class POLIBASE:
 
-        CARD_REGISTRY_FOLDER: FieldItem = FieldItem(FIELD_NAME_COLLECTION.CARD_REGISTRY_FOLDER, "Папка карты пациента", default_value="Нет папки")
+        CARD_REGISTRY_FOLDER: FieldItem = FieldItem(FIELD_NAME_COLLECTION.CARD_REGISTRY_FOLDER, "Папка карты пациента", default_value="Не зарегистрирована в реестре карт пациентов")
 
         PERSON_BASE: FieldItemList = FieldItemList(FieldItem(FIELD_NAME_COLLECTION.PIN, "Идентификационный номер пациента"),
                                               FieldItem(FIELD_NAME_COLLECTION.FULL_NAME, "ФИО пациента"),
                                               FieldItem(FIELD_NAME_COLLECTION.TELEPHONE_NUMBER, "Телефон"))
 
         PERSON_VISIT: FieldItemList = FieldItemList(PERSON_BASE,
                                               FieldItem(FIELD_NAME_COLLECTION.REGISTRATION_DATE, "Дата регистрации"),
@@ -2188,14 +2183,17 @@
         "Необходимо совершить действие {}: {}", LogMessageChannels.DEBUG, LogMessageFlags.SAVE, [ParamItem(FIELD_NAME_COLLECTION.ACTION_NAME, ""), ParamItem(FIELD_NAME_COLLECTION.ACTION_DESCRIPTION, "")])
     
     NEW_EMAIL_MESSAGE_WAS_RECEIVED: EventDescription = EventDescription(
         "Почтовый ящик: {mailbox}\nНовое письмо было получено от {from}: {title}.", LogMessageChannels.NEW_EMAIL, LogMessageFlags.NOTIFICATION, [ParamItem("mailbox", ""), ParamItem("title", ""), ParamItem("from", ""), ParamItem("value", "")])
     
     CARD_REGISTRY_FOLDER_WAS_SET_FOR_POLIBASE_PERSON: EventDescription = EventDescription(
         "Карта пациента: {} добавлена в папку \"{}\"", LogMessageChannels.CARD_REGISTRY, LogMessageFlags.SAVE, [PARAM_ITEMS.PERSON_PIN, PARAM_ITEMS.CARD_REGISTRY_FOLDER])
+    
+    CARD_REGISTRY_FOLDER_WAS_REGISTERED: EventDescription = EventDescription(
+        "Папка с картами пациентов: {} добавлена в реестр карт пациентов. Положение: шкаф: {}; полка: {}; место на полке: {}", LogMessageChannels.CARD_REGISTRY, LogMessageFlags.SAVE, [PARAM_ITEMS.CARD_REGISTRY_FOLDER, ParamItem("p_a", ""), ParamItem("p_b", ""), ParamItem("p_c", "")])
 
     CARD_REGISTRY_FOLDER_START_CARD_SORTING: EventDescription = EventDescription(
         "Начат процесс сортировки карта пациентов в папке реестра карт \"{}\"", LogMessageChannels.CARD_REGISTRY, LogMessageFlags.SAVE, [PARAM_ITEMS.CARD_REGISTRY_FOLDER])
 
     CARD_REGISTRY_FOLDER_COMPLETE_CARD_SORTING: EventDescription = EventDescription(
         "Закончен процесс сортировки карта пациентов в папке реестра карт \"{}\"", LogMessageChannels.CARD_REGISTRY, LogMessageFlags.SAVE, [PARAM_ITEMS.CARD_REGISTRY_FOLDER])
```

### Comparing `pih-1.48035/pih/pih.py` & `pih-1.48036/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,15 +627,15 @@
 
     def named_arg(self, name: str) -> str | None:
         return self.arg_parser.parse_args().__getattribute__(name)
     
     def add_arg(self, *args, **kwargs) -> None:
         if DataTool.is_none(self.arg_parser):
             self.arg_parser = ArgumentParser(description="Service help")
-        self.arg_parser.add_argument(*args, **kwargs)
+        self.arg_parser.add_argument(j(("--", args[0])), **kwargs)
     
     @property
     def file_path(self) -> str:
         return sys.argv[0]
 
     @property
     def is_standalone(self) -> bool:
@@ -1648,15 +1648,15 @@
                     handler(message, close_handler)  
             PIH.EVENT.waiting_for_mobile_helper_message_input(
                 recipient, internal_handler)
             return PIH.MIO.ANSWER[recipient][-1] 
 
     class VERSION:
 
-        value: str = "1.48035"
+        value: str = "1.48036"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.value < PIH.VERSION.remote()
     
     class INPUT_WAIT:
@@ -1807,15 +1807,15 @@
         def update_localy(version: str | None = None, show_output: bool = False) -> bool:
             return PIH.UPDATER.install_module(PIH.NAME, version, show_output)
 
         @staticmethod
         def install_module(module_name: str, version: str | None = None, show_output: bool = False) -> bool:
             command_list = PIH.UPDATER.get_module_updater_command_list(
                 module_name, version)
-            command_list.pop(0)
+            #command_list.pop(0)
             process_result: CompletedProcess = PIH.EXECUTOR.execute_command(
                 command_list, show_output)
             returncode = process_result.returncode
             return returncode == 0
 
         @staticmethod
         def update_remote(host: str, show_output: bool = False) -> bool:
@@ -2014,21 +2014,21 @@
             result: CompletedProcess = PIH.EXECUTOR.execute_command(PIH.EXECUTOR.create_command_list_for_psexec_command(command_list, host, interactive=True), True, True)
             output: str = result.stdout
             return result.returncode == 0 and output.count("(TTL)") < count
           
         @staticmethod
         def get_executor_path(executor_name: str) -> str:
             return os.path.join(
-                PATHS.WS.PATH, CONST.EXECUTOR.NAME, executor_name)
+                PATHS.WS.PATH, CONST.PSTOOLS.NAME, executor_name)
 
         @staticmethod
         def create_command_list_for_command(executor_name: str, command_list: list[str], login: str | None = None, password: str | None = None) -> list[str]:
             login = "\\".join([AD.DOMAIN_NAME, login or PIH.DATA.get_variable_value(CONST.ADMINISTRATOR_LOGIN_ALIAS)])
             password = password or PIH.DATA.get_variable_value(CONST.ADMINISTRATOR_PASSOWORD_ALIAS)
-            return [PIH.EXECUTOR.get_executor_path(executor_name), CONST.EXECUTOR.NO_BANNER, CONST.EXECUTOR.ACCEPTEULA, "-u", login, "-p", password]  + command_list
+            return [PIH.EXECUTOR.get_executor_path(executor_name), CONST.PSTOOLS.NO_BANNER, CONST.PSTOOLS.ACCEPTEULA, "-u", login, "-p", password]  + command_list
         
         @staticmethod
         def create_command_list_for_psexec_command(command_list: list[str], host: str | None = None, login: str | None = None, password: str | None = None, interactive: bool | None = False, run_from_system_account: bool = False, run_with_elevetion: bool = False) -> list[str]:
             result_command_list: list[str] = DataTool.check_not_none(interactive, lambda: [["-d", "-i"][interactive]], [])
             host_start: str = r"\\"
             if not DataTool.is_empty(host):
                 result_command_list.append(("" if host.startswith(host_start) else host_start) + host)
@@ -2036,15 +2036,15 @@
                 result_command_list.append("-s")
             if run_with_elevetion:
                 result_command_list.append("-h")
             return PIH.EXECUTOR.create_command_list_for_psexec_command_local(result_command_list + command_list, login, password)
         
         @staticmethod
         def create_command_list_for_psexec_command_local(command_list: list[str], login: str | None = None, password: str | None = None) -> list[str]:
-            return PIH.EXECUTOR.create_command_list_for_command(CONST.EXECUTOR.PS_EXECUTOR, command_list, login, password)
+            return PIH.EXECUTOR.create_command_list_for_command(CONST.PSTOOLS.PS_EXECUTOR, command_list, login, password)
 
         @staticmethod
         def create_remote_process_executor_for_service(role_or_information: ServiceRoles | ServiceInformationBase, interactive: bool | None = False) -> list[str]:
             description: ServiceDescription = ServiceRoles.description(role_or_information)
             login: str | None = DataTool.check_not_none(description.login, lambda: PIH.DATA.FORMAT.variable(description.login))
             password: str | None = DataTool.check_not_none(description.password, lambda: PIH.DATA.FORMAT.variable(description.password))
             return PIH.EXECUTOR.create_command_list_for_psexec_command([role_or_information.pyton_executor_path or CONST.PYTHON.EXECUTOR_ALIAS], PIH.SERVICE.get_host(description), login, password, interactive, description.run_from_system_account)
@@ -2068,15 +2068,15 @@
             return PIH.EXECUTOR.execute_command(command, show_output, capture_output, as_text, as_shell)
 
         @staticmethod
         def kill_process(name_or_pid: str | int, host: str, via_taskkill: bool = True, show_output: bool = False) -> bool:
            if via_taskkill:
                 is_string: bool = isinstance(name_or_pid, str)
                 return PIH.EXECUTOR.execute_command(["taskkill", "/s", host, "/t", "/f", "/im" if is_string else "/pid", PIH.PATH.add_extension(name_or_pid, FILE.EXTENSION.EXE) if is_string else str(name_or_pid)], show_output).returncode < 2
-           return PIH.EXECUTOR.execute_command(PIH.EXECUTOR.create_command_list_for_command(CONST.EXECUTOR.PS_KILL_EXECUTOR, [PIH.DATA.FORMAT.host(host), "-t", str(name_or_pid)]), show_output).returncode == 0
+           return PIH.EXECUTOR.execute_command(PIH.EXECUTOR.create_command_list_for_command(CONST.PSTOOLS.PS_KILL_EXECUTOR, [PIH.DATA.FORMAT.host(host), "-t", str(name_or_pid)]), show_output).returncode == 0
 
         @staticmethod
         def process_is_exists(pid: int, host: str | None = None, login: str | None = None, password: str | None = None) -> str:
             command_list: list[str] = ["tasklist", "/fi", f"pid eq {pid}", "/fo", "list"]
             login = "\\".join(
                 [AD.DOMAIN_NAME, login or PIH.DATA.get_variable_value(CONST.ADMINISTRATOR_LOGIN_ALIAS)])
             password = password or PIH.DATA.get_variable_value(CONST.ADMINISTRATOR_PASSOWORD_ALIAS)
@@ -2209,14 +2209,19 @@
 
             @staticmethod
             def polibase_person_set_card_registry_folder(name: str | None = None, person_or_pin: PolibasePerson | int | None = None) -> Events | tuple[Events, tuple[Any]]:
                 return PIH.EVENT.BUILDER.create_event(
                         Events.CARD_REGISTRY_FOLDER_WAS_SET_FOR_POLIBASE_PERSON, (name, person_or_pin), lambda: (DataTool.if_not_empty(person_or_pin, lambda person: PIH.RESULT.POLIBASE._person_pin(person)), name))
             
             @staticmethod
+            def card_registry_folder_was_registered(name: str | None = None, place_a: int | None = None, place_b: int | None = None, place_c: int | None = None) -> Events | tuple[Events, tuple[Any]]:
+                return PIH.EVENT.BUILDER.create_event(
+                        Events.CARD_REGISTRY_FOLDER_WAS_REGISTERED, name, lambda: (name, place_a, place_b, place_c))
+            
+            @staticmethod
             def card_registry_folder_start_card_sorting(name: str | None = None) -> Events | tuple[Events, tuple[Any]]:
                 return PIH.EVENT.BUILDER.create_event(
                         Events.CARD_REGISTRY_FOLDER_START_CARD_SORTING, name, lambda: (name, ))
 
             @staticmethod
             def card_registry_folder_complete_card_sorting(name: str | None = None) -> Events | tuple[Events, tuple[Any]]:
                 return PIH.EVENT.BUILDER.create_event(
@@ -2703,15 +2708,15 @@
                         if stop_before:
                             if PIH.SERVICE.check_accessibility(service_description):
                                 PIH.SERVICE.ADMIN.stop(service_description)
                     def internal_start_handler(service: IService) -> None:
                         if PIH.OS.is_linux():
                             PIH.PATH.make_directory_if_not_exists(PATHS.FACADE.LINUX_MOUNT_POINT_PATH, host)
                             PIH.PATH.mount_facade_storage_on_linux_host(host)
-                        if starts_handler is not None:
+                        if DataTool.is_not_none(starts_handler):
                             if starts_handler.__code__.co_argcount == 1:
                                 starts_handler(service)
                             else:
                                 starts_handler()
                     service: IService = RPC.create_service()
                     from inspect import signature, Signature
                     def internal_call_handler(command_name: str, parameter_list: ParameterList, context) -> Any | None:
@@ -3772,15 +3777,15 @@
 
         @staticmethod
         def make_sudo(command: str, password: str) -> str:
             return f"echo -e '{password}\n' | sudo -S " + command
 
         @staticmethod
         def python_path(host: str | None = None) -> str | None:
-            search_pattern: str = CONST.PYTHON.SEARCH_PATTERNne   
+            search_pattern: str = CONST.PYTHON.SEARCH_PATTERN
             variable_list: list[str] = if_else(DataTool.is_none(host),
                 PIH.OS.get_variable(WINDOWS.ENVIROMENT_VARIABLES.PATH),
                 PIH.EXECUTOR.execute_command(PIH.EXECUTOR.create_command_list_for_psexec_command(
                         [CONST.POWERSHELL.NAME, j((WINDOWS.ENVIROMENT_COMMAND, WINDOWS.ENVIROMENT_VARIABLES.PATH), ":")], host, interactive=True), True, True).stdout).split(";")
             for variable_item in variable_list:
                 index: int = variable_item.find(search_pattern)
                 if index != -1 and len(variable_item) - (index + len(search_pattern)) <= 4:
@@ -4611,15 +4616,15 @@
             def accessibility_by_smb_port(address_or_ip: str, host: str | None = None, count: int | None = None, check_for_all: bool = True) -> bool:
                 return PIH.CHECK.RESOURCE.accessibility_by_ping_with_port(address_or_ip, WINDOWS.PORTS.SMB, host, count, check_for_all)
             
             @staticmethod
             def accessibility_by_ping(address_or_ip: str, host: str | None = None, count: int | None = None, check_for_all: bool = True) -> bool:
                 count = count or 4
                 local_ping_commnad_list: list[str] = [PIH.EXECUTOR.get_executor_path(
-                    CONST.EXECUTOR.PS_PING), CONST.EXECUTOR.ACCEPTEULA, "-4", "-n", str(count), address_or_ip]
+                    CONST.PSTOOLS.PS_PING), CONST.PSTOOLS.ACCEPTEULA, "-4", "-n", str(count), address_or_ip]
                 process_result: CompletedProcess = PIH.EXECUTOR.execute_command(local_ping_commnad_list if host is None else PIH.EXECUTOR.create_command_list_for_psexec_command(local_ping_commnad_list, host, interactive=True), True, True)
                 if process_result.returncode == 0:
                     out: str = process_result.stdout
                     lost_marker: str = "Lost = "
                     index: int = out.find(lost_marker)
                     if index != -1:
                         lost_count: int = int(out[index +
```

### Comparing `pih-1.48035/pih/rpc.py` & `pih-1.48036/pih/rpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
                 A = sys.modules["pih.pih"].A
 
             max_workers = max_workers or RPC.Service.MAX_WORKERS
             service_description: ServiceDescription = role_or_information if isinstance(
                 role_or_information, ServiceInformationBase) else A.CT_SR.description(role_or_information)
             self.description = service_description
             arg_name: str = "isolated"
-            A.SE.add_arg(j(("--", arg_name)),
+            A.SE.add_arg(arg_name,
                             help="Service isolated flag", nargs="?", const=1, type=str, default=None)
             isolate_arg: str | None = None
             try:
                 isolated_arg_value: str | None = A.SE.named_arg(arg_name)
                 if A.D.is_not_none(isolated_arg_value):
                     isolate_arg = str(isolated_arg_value).lower()
             except AttributeError as error:
```

### Comparing `pih-1.48035/pih/rpcCommandCall_pb2.py` & `pih-1.48036/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.48035/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.48036/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48035/pih/rpc_collection.py` & `pih-1.48036/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48035/pih/rpc_const.py` & `pih-1.48036/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.48035/pih/service_example.py` & `pih-1.48036/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.48035/pih/tools.py` & `pih-1.48036/pih/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,26 +25,29 @@
 from pih.const import PASSWORD_GENERATION_ORDER, CONST, FieldCollectionAliases
 from pih.collection import R, T, FieldItem, FieldItemList, FullName, Result, User, PolibasePerson
 
 def if_else(check_value: bool, true_value: Callable[[None], Any | None] | Any, false_value: Callable[[None], Any | None] | Any = None) -> Any | None:
     return (true_value() if callable(true_value) else true_value) if check_value else (false_value() if not DataTool.is_none(false_value) and callable(false_value) else false_value)
 
 
-def i(value: str) -> str:
+def i(value: Any) -> str:
+    value = str(value)
     if not DataTool.is_empty(value) and value.find("_") == -1:
         return f"_{value}_"
     return value or ""
 
-def b(value: str) -> str:
+def b(value: Any) -> str:
+    value = str(value)
     if not DataTool.is_empty(value) and value.find("*") == -1:
         return f"*{value}*"
     return value or ""
 
-def nl(value: str = "", count: int = 1) -> str:
-    return j((value, "\n"*count))
+def nl(value: str = "", count: int = 1, reversed: bool = False) -> str:
+    nl_text: str = "\n"*count
+    return if_else(reversed, j((nl_text, value)), j((value, nl_text)))
 
 def j(value: tuple[str] | list[str], splitter: str = "") -> str:
     return splitter.join(value)
 
 class EnumTool:
 
     @staticmethod
```

### Comparing `pih-1.48035/pih/widgets.py` & `pih-1.48036/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.48035/pih_setup.py` & `pih-1.48036/pih_setup.py`

 * *Files identical despite different names*

