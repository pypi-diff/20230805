# Comparing `tmp/django-appointment-1.1.0.tar.gz` & `tmp/django-appointment-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-appointment-1.1.0.tar", last modified: Wed Aug  2 20:09:47 2023, max compression
+gzip compressed data, was "django-appointment-1.1.1.tar", last modified: Fri Aug  4 17:33:12 2023, max compression
```

## Comparing `django-appointment-1.1.0.tar` & `django-appointment-1.1.1.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.132937 django-appointment-1.1.0/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)    11347 2023-04-23 10:55:12.000000 django-appointment-1.1.0/LICENSE
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      471 2023-07-26 17:35:01.000000 django-appointment-1.1.0/MANIFEST.in
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     5660 2023-08-02 20:09:47.133040 django-appointment-1.1.0/PKG-INFO
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     4572 2023-04-27 16:04:51.000000 django-appointment-1.1.0/README.md
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.124662 django-appointment-1.1.0/appointment/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.1.0/appointment/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1201 2023-07-26 16:01:23.000000 django-appointment-1.1.0/appointment/admin.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      154 2023-04-20 14:22:00.000000 django-appointment-1.1.0/appointment/apps.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      589 2023-07-25 14:42:24.000000 django-appointment-1.1.0/appointment/email_messages.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.125099 django-appointment-1.1.0/appointment/email_sender/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)       51 2023-04-27 14:38:44.000000 django-appointment-1.1.0/appointment/email_sender/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2109 2023-08-02 20:07:21.000000 django-appointment-1.1.0/appointment/email_sender/email_sender.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      228 2023-07-25 14:42:24.000000 django-appointment-1.1.0/appointment/forms.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      426 2023-08-02 15:56:11.000000 django-appointment-1.1.0/appointment/logger_config.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.125522 django-appointment-1.1.0/appointment/migrations/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     9615 2023-08-02 20:06:18.000000 django-appointment-1.1.0/appointment/migrations/0001_initial.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.1.0/appointment/migrations/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)    13276 2023-08-02 19:34:58.000000 django-appointment-1.1.0/appointment/models.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.126149 django-appointment-1.1.0/appointment/operations/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-07-25 14:20:59.000000 django-appointment-1.1.0/appointment/operations/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     4226 2023-08-02 18:47:28.000000 django-appointment-1.1.0/appointment/operations/database_operations.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2902 2023-07-31 15:59:24.000000 django-appointment-1.1.0/appointment/operations/email_operations.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     3273 2023-07-31 16:46:08.000000 django-appointment-1.1.0/appointment/operations/session_operations.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      985 2023-07-25 19:33:26.000000 django-appointment-1.1.0/appointment/settings.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.119776 django-appointment-1.1.0/appointment/static/
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.126890 django-appointment-1.1.0/appointment/static/css/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     3635 2023-04-16 18:49:57.000000 django-appointment-1.1.0/appointment/static/css/appointments-user-details.css
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     5475 2023-07-28 00:05:15.000000 django-appointment-1.1.0/appointment/static/css/appointments.css
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1272 2023-07-27 15:06:07.000000 django-appointment-1.1.0/appointment/static/css/thank_you.css
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1241 2023-07-27 14:52:09.000000 django-appointment-1.1.0/appointment/static/css/verification_code.css
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.127074 django-appointment-1.1.0/appointment/static/js/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     8832 2023-07-27 22:28:43.000000 django-appointment-1.1.0/appointment/static/js/appointments.js
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.120127 django-appointment-1.1.0/appointment/templates/
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.127982 django-appointment-1.1.0/appointment/templates/appointment/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     8362 2023-07-27 14:32:53.000000 django-appointment-1.1.0/appointment/templates/appointment/appointment_client_information.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     4869 2023-07-27 23:42:29.000000 django-appointment-1.1.0/appointment/templates/appointment/appointments.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1652 2023-07-27 15:10:09.000000 django-appointment-1.1.0/appointment/templates/appointment/default_thank_you.html
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1899 2023-07-27 14:52:44.000000 django-appointment-1.1.0/appointment/templates/appointment/enter_verification_code.html
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.128162 django-appointment-1.1.0/appointment/templates/base_templates/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1938 2023-04-22 14:53:13.000000 django-appointment-1.1.0/appointment/templates/base_templates/base.html
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.128344 django-appointment-1.1.0/appointment/templates/email_sender/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2166 2023-07-27 15:22:04.000000 django-appointment-1.1.0/appointment/templates/email_sender/thank_you_email.html
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.129077 django-appointment-1.1.0/appointment/tests/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 13:38:19.000000 django-appointment-1.1.0/appointment/tests/__init__.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.130814 django-appointment-1.1.0/appointment/tests/models/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 19:12:45.000000 django-appointment-1.1.0/appointment/tests/models/__init__.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     5427 2023-08-02 20:02:13.000000 django-appointment-1.1.0/appointment/tests/models/test_model_appointment.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2802 2023-08-02 20:02:13.000000 django-appointment-1.1.0/appointment/tests/models/test_model_appointment_request.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1881 2023-08-02 19:15:12.000000 django-appointment-1.1.0/appointment/tests/models/test_model_config.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1596 2023-08-02 20:02:13.000000 django-appointment-1.1.0/appointment/tests/models/test_model_email_verification.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2785 2023-08-02 20:02:13.000000 django-appointment-1.1.0/appointment/tests/models/test_model_payment_info.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     4894 2023-08-02 19:59:36.000000 django-appointment-1.1.0/appointment/tests/models/test_model_service.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     8386 2023-08-02 18:47:28.000000 django-appointment-1.1.0/appointment/tests/test_utils.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     6493 2023-08-02 19:57:09.000000 django-appointment-1.1.0/appointment/tests/test_views.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2894 2023-04-22 18:21:14.000000 django-appointment-1.1.0/appointment/tests.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1170 2023-05-08 14:43:55.000000 django-appointment-1.1.0/appointment/urls.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     8306 2023-08-02 18:47:28.000000 django-appointment-1.1.0/appointment/utils.py
--rw-r--r--   0 adamspierredavid   (501) staff       (20)    15141 2023-08-02 19:59:36.000000 django-appointment-1.1.0/appointment/views.py
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.131645 django-appointment-1.1.0/django_appointment.egg-info/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     5660 2023-08-02 20:09:47.000000 django-appointment-1.1.0/django_appointment.egg-info/PKG-INFO
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1932 2023-08-02 20:09:47.000000 django-appointment-1.1.0/django_appointment.egg-info/SOURCES.txt
--rw-r--r--   0 adamspierredavid   (501) staff       (20)        1 2023-08-02 20:09:47.000000 django-appointment-1.1.0/django_appointment.egg-info/dependency_links.txt
--rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-08-02 20:09:47.000000 django-appointment-1.1.0/django_appointment.egg-info/requires.txt
--rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-08-02 20:09:47.000000 django-appointment-1.1.0/django_appointment.egg-info/top_level.txt
-drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 20:09:47.132645 django-appointment-1.1.0/docs/
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2772 2023-04-24 19:37:27.000000 django-appointment-1.1.0/docs/README.md
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     8434 2023-07-31 06:46:57.000000 django-appointment-1.1.0/docs/models.md
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     2595 2023-08-01 14:26:24.000000 django-appointment-1.1.0/docs/operations.md
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     5162 2023-08-01 15:00:53.000000 django-appointment-1.1.0/docs/views.md
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      108 2023-04-22 21:41:01.000000 django-appointment-1.1.0/pyproject.toml
--rw-r--r--   0 adamspierredavid   (501) staff       (20)     1077 2023-08-02 20:09:47.133712 django-appointment-1.1.0/setup.cfg
--rw-r--r--   0 adamspierredavid   (501) staff       (20)      216 2023-04-23 11:41:31.000000 django-appointment-1.1.0/setup.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-04 17:33:12.036919 django-appointment-1.1.1/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)    11347 2023-04-23 10:55:12.000000 django-appointment-1.1.1/LICENSE
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      537 2023-08-04 17:32:30.000000 django-appointment-1.1.1/MANIFEST.in
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     5813 2023-08-04 17:33:12.037090 django-appointment-1.1.1/PKG-INFO
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     4725 2023-08-04 17:19:00.000000 django-appointment-1.1.1/README.md
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-04 17:33:12.025203 django-appointment-1.1.1/appointment/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.1.1/appointment/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1201 2023-07-26 16:01:23.000000 django-appointment-1.1.1/appointment/admin.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      154 2023-04-20 14:22:00.000000 django-appointment-1.1.1/appointment/apps.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      589 2023-07-25 14:42:24.000000 django-appointment-1.1.1/appointment/email_messages.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-04 17:33:12.025840 django-appointment-1.1.1/appointment/email_sender/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)       51 2023-04-27 14:38:44.000000 django-appointment-1.1.1/appointment/email_sender/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2109 2023-08-02 20:07:21.000000 django-appointment-1.1.1/appointment/email_sender/email_sender.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      228 2023-07-25 14:42:24.000000 django-appointment-1.1.1/appointment/forms.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      426 2023-08-02 15:56:11.000000 django-appointment-1.1.1/appointment/logger_config.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-04 17:33:12.026581 django-appointment-1.1.1/appointment/migrations/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     9615 2023-08-02 20:06:18.000000 django-appointment-1.1.1/appointment/migrations/0001_initial.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-04-20 14:22:00.000000 django-appointment-1.1.1/appointment/migrations/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)    13276 2023-08-02 19:34:58.000000 django-appointment-1.1.1/appointment/models.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-04 17:33:12.027796 django-appointment-1.1.1/appointment/operations/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-07-25 14:20:59.000000 django-appointment-1.1.1/appointment/operations/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     4226 2023-08-02 18:47:28.000000 django-appointment-1.1.1/appointment/operations/database_operations.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2902 2023-07-31 15:59:24.000000 django-appointment-1.1.1/appointment/operations/email_operations.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     3273 2023-07-31 16:46:08.000000 django-appointment-1.1.1/appointment/operations/session_operations.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      985 2023-07-25 19:33:26.000000 django-appointment-1.1.1/appointment/settings.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-04 17:33:12.018744 django-appointment-1.1.1/appointment/static/
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-04 17:33:12.028775 django-appointment-1.1.1/appointment/static/css/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     3635 2023-04-16 18:49:57.000000 django-appointment-1.1.1/appointment/static/css/appointments-user-details.css
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     5475 2023-07-28 00:05:15.000000 django-appointment-1.1.1/appointment/static/css/appointments.css
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1272 2023-07-27 15:06:07.000000 django-appointment-1.1.1/appointment/static/css/thank_you.css
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1241 2023-07-27 14:52:09.000000 django-appointment-1.1.1/appointment/static/css/verification_code.css
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-04 17:33:12.028969 django-appointment-1.1.1/appointment/static/js/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     8832 2023-07-27 22:28:43.000000 django-appointment-1.1.1/appointment/static/js/appointments.js
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-04 17:33:12.019088 django-appointment-1.1.1/appointment/templates/
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-04 17:33:12.030137 django-appointment-1.1.1/appointment/templates/appointment/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     8362 2023-07-27 14:32:53.000000 django-appointment-1.1.1/appointment/templates/appointment/appointment_client_information.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     4869 2023-07-27 23:42:29.000000 django-appointment-1.1.1/appointment/templates/appointment/appointments.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1652 2023-07-27 15:10:09.000000 django-appointment-1.1.1/appointment/templates/appointment/default_thank_you.html
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1899 2023-07-27 14:52:44.000000 django-appointment-1.1.1/appointment/templates/appointment/enter_verification_code.html
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-04 17:33:12.030365 django-appointment-1.1.1/appointment/templates/base_templates/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1938 2023-04-22 14:53:13.000000 django-appointment-1.1.1/appointment/templates/base_templates/base.html
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-04 17:33:12.030558 django-appointment-1.1.1/appointment/templates/email_sender/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2166 2023-07-27 15:22:04.000000 django-appointment-1.1.1/appointment/templates/email_sender/thank_you_email.html
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-04 17:33:12.031515 django-appointment-1.1.1/appointment/tests/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 13:38:19.000000 django-appointment-1.1.1/appointment/tests/__init__.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-04 17:33:12.033313 django-appointment-1.1.1/appointment/tests/models/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        0 2023-08-02 19:12:45.000000 django-appointment-1.1.1/appointment/tests/models/__init__.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     5427 2023-08-02 20:02:13.000000 django-appointment-1.1.1/appointment/tests/models/test_model_appointment.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2802 2023-08-02 20:02:13.000000 django-appointment-1.1.1/appointment/tests/models/test_model_appointment_request.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1881 2023-08-02 19:15:12.000000 django-appointment-1.1.1/appointment/tests/models/test_model_config.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1596 2023-08-02 20:02:13.000000 django-appointment-1.1.1/appointment/tests/models/test_model_email_verification.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2785 2023-08-02 20:02:13.000000 django-appointment-1.1.1/appointment/tests/models/test_model_payment_info.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     4894 2023-08-02 19:59:36.000000 django-appointment-1.1.1/appointment/tests/models/test_model_service.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     3256 2023-08-04 17:02:14.000000 django-appointment-1.1.1/appointment/tests/test_availability_slot.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     8386 2023-08-02 18:47:28.000000 django-appointment-1.1.1/appointment/tests/test_utils.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     6493 2023-08-02 19:57:09.000000 django-appointment-1.1.1/appointment/tests/test_views.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2894 2023-04-22 18:21:14.000000 django-appointment-1.1.1/appointment/tests.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1170 2023-05-08 14:43:55.000000 django-appointment-1.1.1/appointment/urls.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     8350 2023-08-04 16:35:08.000000 django-appointment-1.1.1/appointment/utils.py
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)    15141 2023-08-02 19:59:36.000000 django-appointment-1.1.1/appointment/views.py
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-04 17:33:12.034511 django-appointment-1.1.1/django_appointment.egg-info/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     5813 2023-08-04 17:33:11.000000 django-appointment-1.1.1/django_appointment.egg-info/PKG-INFO
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1993 2023-08-04 17:33:11.000000 django-appointment-1.1.1/django_appointment.egg-info/SOURCES.txt
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)        1 2023-08-04 17:33:11.000000 django-appointment-1.1.1/django_appointment.egg-info/dependency_links.txt
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-08-04 17:33:11.000000 django-appointment-1.1.1/django_appointment.egg-info/requires.txt
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)       12 2023-08-04 17:33:11.000000 django-appointment-1.1.1/django_appointment.egg-info/top_level.txt
+drwxr-xr-x   0 adamspierredavid   (501) staff       (20)        0 2023-08-04 17:33:12.036335 django-appointment-1.1.1/docs/
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     3954 2023-08-04 17:21:21.000000 django-appointment-1.1.1/docs/README.md
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     8434 2023-07-31 06:46:57.000000 django-appointment-1.1.1/docs/models.md
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     2595 2023-08-01 14:26:24.000000 django-appointment-1.1.1/docs/operations.md
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     5162 2023-08-01 15:00:53.000000 django-appointment-1.1.1/docs/views.md
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      108 2023-04-22 21:41:01.000000 django-appointment-1.1.1/pyproject.toml
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1930 2023-08-04 17:27:37.000000 django-appointment-1.1.1/release_notes.md
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)     1077 2023-08-04 17:33:12.037624 django-appointment-1.1.1/setup.cfg
+-rw-r--r--   0 adamspierredavid   (501) staff       (20)      216 2023-04-23 11:41:31.000000 django-appointment-1.1.1/setup.py
```

### Comparing `django-appointment-1.1.0/LICENSE` & `django-appointment-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/PKG-INFO` & `django-appointment-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-appointment
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Django app for managing appointment scheduling with ease and flexibility.
 Home-page: https://github.com/adamspd/django-appointment
 Author: Adams Pierre David
 Author-email: adamspd.developer@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -27,22 +27,24 @@
 # Appointment Scheduler
 
 Appointment Scheduler is a Django app designed for managing appointment scheduling with ease and flexibility. It allows
 users to define custom configurations for time slots, lead time, and finish time, or use the default values provided.
 The app also handles conflicts and availability for appointments, ensuring a smooth user experience.
 
 Detailed documentation is in the ["docs"](https://github.com/adamspd/django-appointment/tree/main/docs) directory.
+Please refer to the release notes for changes and migration
+information [here](https://github.com/adamspd/django-appointment/tree/main/release_notes.md).
 
 ## Features
 
 1. Customizable time slots, lead time, and finish time.
 2. Handles appointment conflicts and availability.
 3. Easy integration with Django admin interface for appointment management.
 4. User-friendly interface for viewing available time slots and scheduling appointments.
-5. Sends email notifications to clients when they schedule an appointment.
+5. Send email notifications to clients when they schedule an appointment.
 
 ## Quick start
 
 1. Add "appointment" to your INSTALLED_APPS setting like this:
 
    ```python
    INSTALLED_APPS = [
```

### Comparing `django-appointment-1.1.0/README.md` & `django-appointment-1.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Appointment Scheduler
 
 Appointment Scheduler is a Django app designed for managing appointment scheduling with ease and flexibility. It allows
 users to define custom configurations for time slots, lead time, and finish time, or use the default values provided.
 The app also handles conflicts and availability for appointments, ensuring a smooth user experience.
 
 Detailed documentation is in the ["docs"](https://github.com/adamspd/django-appointment/tree/main/docs) directory.
+Please refer to the release notes for changes and migration
+information [here](https://github.com/adamspd/django-appointment/tree/main/release_notes.md).
 
 ## Features
 
 1. Customizable time slots, lead time, and finish time.
 2. Handles appointment conflicts and availability.
 3. Easy integration with Django admin interface for appointment management.
 4. User-friendly interface for viewing available time slots and scheduling appointments.
-5. Sends email notifications to clients when they schedule an appointment.
+5. Send email notifications to clients when they schedule an appointment.
 
 ## Quick start
 
 1. Add "appointment" to your INSTALLED_APPS setting like this:
 
    ```python
    INSTALLED_APPS = [
```

### Comparing `django-appointment-1.1.0/appointment/admin.py` & `django-appointment-1.1.1/appointment/admin.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/email_messages.py` & `django-appointment-1.1.1/appointment/email_messages.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/email_sender/email_sender.py` & `django-appointment-1.1.1/appointment/email_sender/email_sender.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/migrations/0001_initial.py` & `django-appointment-1.1.1/appointment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/models.py` & `django-appointment-1.1.1/appointment/models.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/operations/database_operations.py` & `django-appointment-1.1.1/appointment/operations/database_operations.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/operations/email_operations.py` & `django-appointment-1.1.1/appointment/operations/email_operations.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/operations/session_operations.py` & `django-appointment-1.1.1/appointment/operations/session_operations.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/settings.py` & `django-appointment-1.1.1/appointment/settings.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/static/css/appointments-user-details.css` & `django-appointment-1.1.1/appointment/static/css/appointments-user-details.css`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/static/css/appointments.css` & `django-appointment-1.1.1/appointment/static/css/appointments.css`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/static/css/thank_you.css` & `django-appointment-1.1.1/appointment/static/css/thank_you.css`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/static/css/verification_code.css` & `django-appointment-1.1.1/appointment/static/css/verification_code.css`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/static/js/appointments.js` & `django-appointment-1.1.1/appointment/static/js/appointments.js`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/templates/appointment/appointment_client_information.html` & `django-appointment-1.1.1/appointment/templates/appointment/appointment_client_information.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/templates/appointment/appointments.html` & `django-appointment-1.1.1/appointment/templates/appointment/appointments.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/templates/appointment/default_thank_you.html` & `django-appointment-1.1.1/appointment/templates/appointment/default_thank_you.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/templates/appointment/enter_verification_code.html` & `django-appointment-1.1.1/appointment/templates/appointment/enter_verification_code.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/templates/base_templates/base.html` & `django-appointment-1.1.1/appointment/templates/base_templates/base.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/templates/email_sender/thank_you_email.html` & `django-appointment-1.1.1/appointment/templates/email_sender/thank_you_email.html`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/tests/models/test_model_appointment.py` & `django-appointment-1.1.1/appointment/tests/models/test_model_appointment.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/tests/models/test_model_appointment_request.py` & `django-appointment-1.1.1/appointment/tests/models/test_model_appointment_request.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/tests/models/test_model_config.py` & `django-appointment-1.1.1/appointment/tests/models/test_model_config.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/tests/models/test_model_email_verification.py` & `django-appointment-1.1.1/appointment/tests/models/test_model_email_verification.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/tests/models/test_model_payment_info.py` & `django-appointment-1.1.1/appointment/tests/models/test_model_payment_info.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/tests/models/test_model_service.py` & `django-appointment-1.1.1/appointment/tests/models/test_model_service.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/tests/test_utils.py` & `django-appointment-1.1.1/appointment/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/tests/test_views.py` & `django-appointment-1.1.1/appointment/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/tests.py` & `django-appointment-1.1.1/appointment/tests.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/urls.py` & `django-appointment-1.1.1/appointment/urls.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/appointment/utils.py` & `django-appointment-1.1.1/appointment/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,16 @@
         while start_time <= end_time:
             if start_time >= buffer_time:
                 slots.append(start_time)
             start_time += slot_duration
         for appointment in appointments:
             appointment_start_time = appointment.get_start_time()
             appointment_end_time = appointment.get_end_time()
-            slots = [slot for slot in slots if not (appointment_start_time <= slot <= appointment_end_time)]
+            slots = [slot for slot in slots if
+                     not (appointment_start_time < slot + slot_duration and slot < appointment_end_time)]
         return [slot.strftime('%I:%M %p') for slot in slots]
 
     @staticmethod
     def get_locale():
         """
         Get the current locale based on the user's language settings.
```

### Comparing `django-appointment-1.1.0/appointment/views.py` & `django-appointment-1.1.1/appointment/views.py`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/django_appointment.egg-info/PKG-INFO` & `django-appointment-1.1.1/django_appointment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-appointment
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Django app for managing appointment scheduling with ease and flexibility.
 Home-page: https://github.com/adamspd/django-appointment
 Author: Adams Pierre David
 Author-email: adamspd.developer@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -27,22 +27,24 @@
 # Appointment Scheduler
 
 Appointment Scheduler is a Django app designed for managing appointment scheduling with ease and flexibility. It allows
 users to define custom configurations for time slots, lead time, and finish time, or use the default values provided.
 The app also handles conflicts and availability for appointments, ensuring a smooth user experience.
 
 Detailed documentation is in the ["docs"](https://github.com/adamspd/django-appointment/tree/main/docs) directory.
+Please refer to the release notes for changes and migration
+information [here](https://github.com/adamspd/django-appointment/tree/main/release_notes.md).
 
 ## Features
 
 1. Customizable time slots, lead time, and finish time.
 2. Handles appointment conflicts and availability.
 3. Easy integration with Django admin interface for appointment management.
 4. User-friendly interface for viewing available time slots and scheduling appointments.
-5. Sends email notifications to clients when they schedule an appointment.
+5. Send email notifications to clients when they schedule an appointment.
 
 ## Quick start
 
 1. Add "appointment" to your INSTALLED_APPS setting like this:
 
    ```python
    INSTALLED_APPS = [
```

### Comparing `django-appointment-1.1.0/django_appointment.egg-info/SOURCES.txt` & `django-appointment-1.1.1/django_appointment.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+release_notes.md
 setup.cfg
 setup.py
 appointment/__init__.py
 appointment/admin.py
 appointment/apps.py
 appointment/email_messages.py
 appointment/forms.py
@@ -32,14 +33,15 @@
 appointment/templates/appointment/appointment_client_information.html
 appointment/templates/appointment/appointments.html
 appointment/templates/appointment/default_thank_you.html
 appointment/templates/appointment/enter_verification_code.html
 appointment/templates/base_templates/base.html
 appointment/templates/email_sender/thank_you_email.html
 appointment/tests/__init__.py
+appointment/tests/test_availability_slot.py
 appointment/tests/test_utils.py
 appointment/tests/test_views.py
 appointment/tests/models/__init__.py
 appointment/tests/models/test_model_appointment.py
 appointment/tests/models/test_model_appointment_request.py
 appointment/tests/models/test_model_config.py
 appointment/tests/models/test_model_email_verification.py
```

### Comparing `django-appointment-1.1.0/docs/models.md` & `django-appointment-1.1.1/docs/models.md`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/docs/operations.md` & `django-appointment-1.1.1/docs/operations.md`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/docs/views.md` & `django-appointment-1.1.1/docs/views.md`

 * *Files identical despite different names*

### Comparing `django-appointment-1.1.0/setup.cfg` & `django-appointment-1.1.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-appointment
-version = 1.1.0
+version = 1.1.1
 description = A Django app for managing appointment scheduling with ease and flexibility.
 url = https://github.com/adamspd/django-appointment
 author = Adams Pierre David
 author_email = adamspd.developer@gmail.com
 author_website = https://adamspierredavid.com/
 readme = README.md
 license = Apache License 2.0
```

