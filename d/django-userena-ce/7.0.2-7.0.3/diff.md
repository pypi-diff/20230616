# Comparing `tmp/django_userena_ce-7.0.2.tar.gz` & `tmp/django_userena_ce-7.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_userena_ce-7.0.2.tar", max compression
+gzip compressed data, was "django_userena_ce-7.0.3.tar", max compression
```

## Comparing `django_userena_ce-7.0.2.tar` & `django_userena_ce-7.0.3.tar`

### file list

```diff
@@ -1,150 +1,149 @@
--rw-r--r--   0        0        0     1520 2022-12-19 11:15:08.407396 django_userena_ce-7.0.2/LICENSE
--rw-r--r--   0        0        0     1967 2022-12-19 11:15:08.407396 django_userena_ce-7.0.2/README.md
--rw-r--r--   0        0        0     3022 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/__init__.py
--rw-r--r--   0        0        0     1040 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/admin.py
--rw-r--r--   0        0        0      118 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/apps.py
--rw-r--r--   0        0        0     2080 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/backends.py
--rw-r--r--   0        0        0      105 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/compat.py
--rw-r--r--   0        0        0        0 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/__init__.py
--rw-r--r--   0        0        0        0 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/__init__.py
--rw-r--r--   0        0        0      921 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/admin.py
--rw-r--r--   0        0        0     2118 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/fields.py
--rw-r--r--   0        0        0      978 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/fixtures/messages.json
--rw-r--r--   0        0        0      951 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/forms.py
--rw-r--r--   0        0        0     4188 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/managers.py
--rw-r--r--   0        0        0     5232 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/migrations/__init__.py
--rw-r--r--   0        0        0     4595 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/models.py
--rw-r--r--   0        0        0       77 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/signals.py
--rw-r--r--   0        0        0      661 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/templates/base.html
--rw-r--r--   0        0        0       26 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/templates/umessages/base_message.html
--rw-r--r--   0        0        0      478 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/templates/umessages/message_detail.html
--rw-r--r--   0        0        0      461 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/templates/umessages/message_form.html
--rw-r--r--   0        0        0     1283 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/templates/umessages/message_list.html
--rw-r--r--   0        0        0        0 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/templatetags/__init__.py
--rw-r--r--   0        0        0     2771 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/templatetags/umessages_tags.py
--rw-r--r--   0        0        0        0 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/tests/__init__.py
--rw-r--r--   0        0        0     2985 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/tests/test_fields.py
--rw-r--r--   0        0        0     1614 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/tests/test_forms.py
--rw-r--r--   0        0        0     1854 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/tests/test_managers.py
--rw-r--r--   0        0        0     1915 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/tests/test_models.py
--rw-r--r--   0        0        0     7276 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/tests/test_views.py
--rw-r--r--   0        0        0     1180 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/urls.py
--rw-r--r--   0        0        0     8124 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/contrib/umessages/views.py
--rw-r--r--   0        0        0     1267 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/decorators.py
--rw-r--r--   0        0        0      470 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/fixtures/profiles.json
--rw-r--r--   0        0        0     2279 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/fixtures/users.json
--rw-r--r--   0        0        0    11758 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/forms.py
--rw-r--r--   0        0        0    19029 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    31747 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    16155 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    22979 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/locale/bg/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    15002 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    23485 2022-12-19 11:15:08.415404 django_userena_ce-7.0.2/userena/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    14919 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/de_du/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    23612 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/de_du/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    17934 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    26040 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/el/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    14184 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    22919 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    14259 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    22220 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    26763 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/gl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    14329 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    23489 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    15465 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    25474 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/nb/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10652 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    21708 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    14182 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    23285 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9390 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    20382 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/pt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    13825 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    23368 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    16377 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    26959 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/ro/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    18106 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    27613 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    14198 2022-12-19 11:15:08.419408 django_userena_ce-7.0.2/userena/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    22614 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/locale/tr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    13346 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    21633 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11391 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/locale/zh_Hant/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18105 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/locale/zh_Hant/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2830 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/mail.py
--rw-r--r--   0        0        0        0 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/management/__init__.py
--rw-r--r--   0        0        0        0 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/management/commands/__init__.py
--rw-r--r--   0        0        0     1959 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/management/commands/check_permissions.py
--rw-r--r--   0        0        0      387 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/management/commands/clean_expired.py
--rw-r--r--   0        0        0    11321 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/managers.py
--rw-r--r--   0        0        0     1411 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/middleware.py
--rw-r--r--   0        0        0     3289 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/migrations/0001_initial.py
--rw-r--r--   0        0        0      760 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/migrations/0002_auto_20171130_0921.py
--rw-r--r--   0        0        0        0 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/migrations/__init__.py
--rw-r--r--   0        0        0    13067 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/models.py
--rw-r--r--   0        0        0        0 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/runtests/__init__.py
--rw-r--r--   0        0        0   245760 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/runtests/private/development.db
--rw-r--r--   0        0        0     4764 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/runtests/settings.py
--rw-r--r--   0        0        0       82 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/runtests/templates/404.html
--rw-r--r--   0        0        0      927 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/runtests/urls.py
--rw-r--r--   0        0        0     3853 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/settings.py
--rw-r--r--   0        0        0      466 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/signals.py
--rw-r--r--   0        0        0      661 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/base.html
--rw-r--r--   0        0        0      488 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/activate_fail.html
--rw-r--r--   0        0        0      588 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/activate_form.html
--rw-r--r--   0        0        0      494 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/activate_pending.html
--rw-r--r--   0        0        0      516 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/activate_retry.html
--rw-r--r--   0        0        0      630 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/activate_retry_success.html
--rw-r--r--   0        0        0       26 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/base_userena.html
--rw-r--r--   0        0        0      400 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/disabled.html
--rw-r--r--   0        0        0      602 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/email_change_complete.html
--rw-r--r--   0        0        0      388 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/email_confirm_complete.html
--rw-r--r--   0        0        0      409 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/email_confirm_fail.html
--rw-r--r--   0        0        0     1099 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/email_form.html
--rw-r--r--   0        0        0      615 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/emails/activation_email_message.html
--rw-r--r--   0        0        0      522 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/emails/activation_email_message.txt
--rw-r--r--   0        0        0      101 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/emails/activation_email_subject.txt
--rw-r--r--   0        0        0      660 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/emails/confirmation_email_message_new.html
--rw-r--r--   0        0        0      555 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/emails/confirmation_email_message_new.txt
--rw-r--r--   0        0        0      666 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/emails/confirmation_email_message_old.html
--rw-r--r--   0        0        0      553 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/emails/confirmation_email_message_old.txt
--rw-r--r--   0        0        0      139 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/emails/confirmation_email_subject_new.html
--rw-r--r--   0        0        0      109 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/emails/confirmation_email_subject_new.txt
--rw-r--r--   0        0        0      136 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/emails/confirmation_email_subject_old.txt
--rw-r--r--   0        0        0      908 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/emails/password_reset_message.html
--rw-r--r--   0        0        0      645 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/emails/password_reset_message.txt
--rw-r--r--   0        0        0      329 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/password_complete.html
--rw-r--r--   0        0        0     1210 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/password_form.html
--rw-r--r--   0        0        0      403 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/password_reset_complete.html
--rw-r--r--   0        0        0      501 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/password_reset_confirm_form.html
--rw-r--r--   0        0        0      353 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/password_reset_done.html
--rw-r--r--   0        0        0      423 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/password_reset_form.html
--rw-r--r--   0        0        0     2985 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/profile_detail.html
--rw-r--r--   0        0        0     1204 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/profile_form.html
--rw-r--r--   0        0        0     1244 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/profile_list.html
--rw-r--r--   0        0        0     1261 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/signin_form.html
--rw-r--r--   0        0        0      310 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/signout.html
--rw-r--r--   0        0        0      757 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/signup_complete.html
--rw-r--r--   0        0        0      952 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/templates/userena/signup_form.html
--rw-r--r--   0        0        0        0 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/tests/profiles/__init__.py
--rw-r--r--   0        0        0     1153 2022-12-19 11:15:08.423412 django_userena_ce-7.0.2/userena/tests/profiles/models.py
--rw-r--r--   0        0        0     2593 2022-12-19 11:15:08.427416 django_userena_ce-7.0.2/userena/tests/test_backends.py
--rw-r--r--   0        0        0     4903 2022-12-19 11:15:08.427416 django_userena_ce-7.0.2/userena/tests/test_commands.py
--rw-r--r--   0        0        0      309 2022-12-19 11:15:08.427416 django_userena_ce-7.0.2/userena/tests/test_migrations.py
--rw-r--r--   0        0        0     2847 2022-12-19 11:15:08.427416 django_userena_ce-7.0.2/userena/tests/test_privacy.py
--rw-r--r--   0        0        0      756 2022-12-19 11:15:08.427416 django_userena_ce-7.0.2/userena/tests/tests_decorators.py
--rw-r--r--   0        0        0     9342 2022-12-19 11:15:08.427416 django_userena_ce-7.0.2/userena/tests/tests_forms.py
--rw-r--r--   0        0        0     6525 2022-12-19 11:15:08.427416 django_userena_ce-7.0.2/userena/tests/tests_managers.py
--rw-r--r--   0        0        0     2899 2022-12-19 11:15:08.427416 django_userena_ce-7.0.2/userena/tests/tests_middleware.py
--rw-r--r--   0        0        0    11649 2022-12-19 11:15:08.427416 django_userena_ce-7.0.2/userena/tests/tests_models.py
--rw-r--r--   0        0        0      815 2022-12-19 11:15:08.427416 django_userena_ce-7.0.2/userena/tests/tests_urls.py
--rw-r--r--   0        0        0     3158 2022-12-19 11:15:08.427416 django_userena_ce-7.0.2/userena/tests/tests_utils.py
--rw-r--r--   0        0        0    23722 2022-12-19 11:15:08.427416 django_userena_ce-7.0.2/userena/tests/tests_views.py
--rw-r--r--   0        0        0     4846 2022-12-19 11:15:08.427416 django_userena_ce-7.0.2/userena/urls.py
--rw-r--r--   0        0        0     5682 2022-12-19 11:15:08.427416 django_userena_ce-7.0.2/userena/utils.py
--rw-r--r--   0        0        0    36270 2022-12-19 11:15:08.427416 django_userena_ce-7.0.2/userena/views.py
--rw-r--r--   0        0        0     4181 1970-01-01 00:00:00.000000 django_userena_ce-7.0.2/setup.py
--rw-r--r--   0        0        0     3238 1970-01-01 00:00:00.000000 django_userena_ce-7.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1520 2023-06-16 07:11:16.726118 django_userena_ce-7.0.3/LICENSE
+-rw-r--r--   0        0        0     1962 2023-06-16 07:11:16.726118 django_userena_ce-7.0.3/README.md
+-rw-r--r--   0        0        0     2865 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/__init__.py
+-rw-r--r--   0        0        0     1040 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/admin.py
+-rw-r--r--   0        0        0      118 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/apps.py
+-rw-r--r--   0        0        0     2080 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/backends.py
+-rw-r--r--   0        0        0      105 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/compat.py
+-rw-r--r--   0        0        0        0 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/contrib/umessages/__init__.py
+-rw-r--r--   0        0        0      921 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/contrib/umessages/admin.py
+-rw-r--r--   0        0        0     2118 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/contrib/umessages/fields.py
+-rw-r--r--   0        0        0      978 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/contrib/umessages/fixtures/messages.json
+-rw-r--r--   0        0        0      951 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/contrib/umessages/forms.py
+-rw-r--r--   0        0        0     4188 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/contrib/umessages/managers.py
+-rw-r--r--   0        0        0     5232 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/contrib/umessages/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/contrib/umessages/migrations/__init__.py
+-rw-r--r--   0        0        0     4595 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/contrib/umessages/models.py
+-rw-r--r--   0        0        0       77 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/contrib/umessages/signals.py
+-rw-r--r--   0        0        0      661 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/contrib/umessages/templates/base.html
+-rw-r--r--   0        0        0       26 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/contrib/umessages/templates/umessages/base_message.html
+-rw-r--r--   0        0        0      478 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/contrib/umessages/templates/umessages/message_detail.html
+-rw-r--r--   0        0        0      461 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/contrib/umessages/templates/umessages/message_form.html
+-rw-r--r--   0        0        0     1283 2023-06-16 07:11:16.730118 django_userena_ce-7.0.3/userena/contrib/umessages/templates/umessages/message_list.html
+-rw-r--r--   0        0        0        0 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/contrib/umessages/templatetags/__init__.py
+-rw-r--r--   0        0        0     2771 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/contrib/umessages/templatetags/umessages_tags.py
+-rw-r--r--   0        0        0        0 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/contrib/umessages/tests/__init__.py
+-rw-r--r--   0        0        0     2985 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/contrib/umessages/tests/test_fields.py
+-rw-r--r--   0        0        0     1614 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/contrib/umessages/tests/test_forms.py
+-rw-r--r--   0        0        0     1854 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/contrib/umessages/tests/test_managers.py
+-rw-r--r--   0        0        0     1915 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/contrib/umessages/tests/test_models.py
+-rw-r--r--   0        0        0     7276 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/contrib/umessages/tests/test_views.py
+-rw-r--r--   0        0        0     1180 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/contrib/umessages/urls.py
+-rw-r--r--   0        0        0     8124 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/contrib/umessages/views.py
+-rw-r--r--   0        0        0     1267 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/decorators.py
+-rw-r--r--   0        0        0      470 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/fixtures/profiles.json
+-rw-r--r--   0        0        0     2279 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/fixtures/users.json
+-rw-r--r--   0        0        0    11758 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/forms.py
+-rw-r--r--   0        0        0    19029 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    31747 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    16155 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    22979 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/locale/bg/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    15002 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    23485 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    14919 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/locale/de_du/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    23612 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/locale/de_du/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    17934 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    26040 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/locale/el/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    14184 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    22919 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    14259 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    22220 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    26763 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/locale/gl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    14329 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    23489 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    15465 2023-06-16 07:11:16.734119 django_userena_ce-7.0.3/userena/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    25474 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10652 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    21708 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    14182 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    23285 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9390 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    20382 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/locale/pt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    13825 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    23368 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    16377 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    26959 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/locale/ro/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    18106 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    27613 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    14198 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    22614 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    13346 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    21633 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11391 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/locale/zh_Hant/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18105 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/locale/zh_Hant/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2830 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/mail.py
+-rw-r--r--   0        0        0        0 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/management/commands/__init__.py
+-rw-r--r--   0        0        0     1959 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/management/commands/check_permissions.py
+-rw-r--r--   0        0        0      387 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/management/commands/clean_expired.py
+-rw-r--r--   0        0        0    11321 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/managers.py
+-rw-r--r--   0        0        0     1410 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/middleware.py
+-rw-r--r--   0        0        0     3289 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/migrations/0001_initial.py
+-rw-r--r--   0        0        0      760 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/migrations/0002_auto_20171130_0921.py
+-rw-r--r--   0        0        0        0 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/migrations/__init__.py
+-rw-r--r--   0        0        0    13067 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/models.py
+-rw-r--r--   0        0        0        0 2023-06-16 07:11:16.738119 django_userena_ce-7.0.3/userena/runtests/__init__.py
+-rw-r--r--   0        0        0   245760 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/runtests/private/development.db
+-rw-r--r--   0        0        0     4764 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/runtests/settings.py
+-rw-r--r--   0        0        0       82 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/runtests/templates/404.html
+-rw-r--r--   0        0        0      927 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/runtests/urls.py
+-rw-r--r--   0        0        0     3853 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/settings.py
+-rw-r--r--   0        0        0      466 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/signals.py
+-rw-r--r--   0        0        0      661 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/base.html
+-rw-r--r--   0        0        0      488 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/activate_fail.html
+-rw-r--r--   0        0        0      588 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/activate_form.html
+-rw-r--r--   0        0        0      494 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/activate_pending.html
+-rw-r--r--   0        0        0      516 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/activate_retry.html
+-rw-r--r--   0        0        0      630 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/activate_retry_success.html
+-rw-r--r--   0        0        0       26 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/base_userena.html
+-rw-r--r--   0        0        0      400 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/disabled.html
+-rw-r--r--   0        0        0      602 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/email_change_complete.html
+-rw-r--r--   0        0        0      388 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/email_confirm_complete.html
+-rw-r--r--   0        0        0      409 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/email_confirm_fail.html
+-rw-r--r--   0        0        0     1099 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/email_form.html
+-rw-r--r--   0        0        0      615 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/emails/activation_email_message.html
+-rw-r--r--   0        0        0      522 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/emails/activation_email_message.txt
+-rw-r--r--   0        0        0      101 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/emails/activation_email_subject.txt
+-rw-r--r--   0        0        0      660 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/emails/confirmation_email_message_new.html
+-rw-r--r--   0        0        0      555 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/emails/confirmation_email_message_new.txt
+-rw-r--r--   0        0        0      666 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/emails/confirmation_email_message_old.html
+-rw-r--r--   0        0        0      553 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/emails/confirmation_email_message_old.txt
+-rw-r--r--   0        0        0      139 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/emails/confirmation_email_subject_new.html
+-rw-r--r--   0        0        0      109 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/emails/confirmation_email_subject_new.txt
+-rw-r--r--   0        0        0      136 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/emails/confirmation_email_subject_old.txt
+-rw-r--r--   0        0        0      908 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/emails/password_reset_message.html
+-rw-r--r--   0        0        0      645 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/emails/password_reset_message.txt
+-rw-r--r--   0        0        0      329 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/password_complete.html
+-rw-r--r--   0        0        0     1210 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/password_form.html
+-rw-r--r--   0        0        0      403 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/password_reset_complete.html
+-rw-r--r--   0        0        0      501 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/password_reset_confirm_form.html
+-rw-r--r--   0        0        0      353 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/password_reset_done.html
+-rw-r--r--   0        0        0      423 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/password_reset_form.html
+-rw-r--r--   0        0        0     2985 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/profile_detail.html
+-rw-r--r--   0        0        0     1204 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/profile_form.html
+-rw-r--r--   0        0        0     1244 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/profile_list.html
+-rw-r--r--   0        0        0     1261 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/signin_form.html
+-rw-r--r--   0        0        0      310 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/signout.html
+-rw-r--r--   0        0        0      757 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/signup_complete.html
+-rw-r--r--   0        0        0      952 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/templates/userena/signup_form.html
+-rw-r--r--   0        0        0        0 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/tests/profiles/__init__.py
+-rw-r--r--   0        0        0     1153 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/tests/profiles/models.py
+-rw-r--r--   0        0        0     2593 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/tests/test_backends.py
+-rw-r--r--   0        0        0     4903 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/tests/test_commands.py
+-rw-r--r--   0        0        0      309 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/tests/test_migrations.py
+-rw-r--r--   0        0        0     2847 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/tests/test_privacy.py
+-rw-r--r--   0        0        0      756 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/tests/tests_decorators.py
+-rw-r--r--   0        0        0     9342 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/tests/tests_forms.py
+-rw-r--r--   0        0        0     6525 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/tests/tests_managers.py
+-rw-r--r--   0        0        0     2899 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/tests/tests_middleware.py
+-rw-r--r--   0        0        0    11649 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/tests/tests_models.py
+-rw-r--r--   0        0        0      815 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/tests/tests_urls.py
+-rw-r--r--   0        0        0     3158 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/tests/tests_utils.py
+-rw-r--r--   0        0        0    23722 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/tests/tests_views.py
+-rw-r--r--   0        0        0     4846 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/urls.py
+-rw-r--r--   0        0        0     5682 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/utils.py
+-rw-r--r--   0        0        0    36270 2023-06-16 07:11:16.742119 django_userena_ce-7.0.3/userena/views.py
+-rw-r--r--   0        0        0     3178 1970-01-01 00:00:00.000000 django_userena_ce-7.0.3/PKG-INFO
```

### Comparing `django_userena_ce-7.0.2/LICENSE` & `django_userena_ce-7.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/README.md` & `django_userena_ce-7.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 the signup, activation, messaging and more. It's BSD licensed, which means you
 can use it commercially for free!
 
 ## Supported Software
 
 Software | Versions
 ---|---
-Python | 3.7, 3.8, 3.9, 3.10, 3.11
-Django | 3.2, 4.0, 4.1
+Python | 3.8, 3.9, 3.10, 3.11
+Django | 3.2, 4.1, 4.2
 Django Guardian | \>2.0
 
 ## [Documentation](https://django-userena-ce.github.io/django-userena-ce/index.html)
 
 Complete documentation about the
 [installation](https://django-userena-ce.github.io/django-userena-ce/installation.html),
 [settings](https://django-userena-ce.github.io/django-userena-ce/settings.html) and
```

### Comparing `django_userena_ce-7.0.2/pyproject.toml` & `django_userena_ce-7.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "django-userena-ce"
-version = "7.0.2"
+version = "7.0.3"
 description = "Complete user management application for Django"
 authors = ["James Meakin <django-userena-ce@jmsmkn.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/django-userena-ce/django-userena-ce"
 packages = [
     { include = "userena" },
 ]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment',
     'Framework :: Django',
     'Framework :: Django :: 3.2',
-    'Framework :: Django :: 4.0',
     'Framework :: Django :: 4.1',
+    'Framework :: Django :: 4.2',
     'Intended Audience :: Developers',
     'Operating System :: OS Independent',
     'Topic :: Utilities',
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 easy-thumbnails = "*"
 django-guardian = ">=2.0"
 html2text = "*"
-Django = ">=3.2,<4.2"
+Django = ">=3.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-django = "*"
 pytest-cov = "*"
 coveralls = "*"
 sphinx = "*"
@@ -42,15 +42,15 @@
 [tool.isort]
 profile = "black"
 known_first_party = ["userena"]
 line_length = 79
 
 [tool.black]
 line-length = 79
-target-version = ["py37"]
+target-version = ["py38"]
 
 [tool.pytest.ini_options]
 DJANGO_SETTINGS_MODULE = "userena.runtests.settings"
 minversion = "6.0"
 testpaths = [
     "userena/tests",
     "userena/contrib/umessages/tests",
@@ -61,44 +61,41 @@
 filterwarnings = []
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = True
 envlist =
-    ; py37 support was officially introduced in django2.1 and dropped in 4.0
-    py37-django{32}
-    ; py38 support was officially introduced in django3.0
-    py38-django{32,40,41}
-    ; py39 support was officially introduced in django 2.2.17, 3.0.11 and 3.1.3
-    py39-django{32,40,41}
-    ; py310 was officially introduced in django 3.2.9 and 4.0
-    py310-django{32,40,41}
-    ; py311 was officially introduced in django 4.1.3
-    py311-django{41}
+    ; py38 support was introduced in django3.0
+    py38-django{32,41,42}
+    ; py39 support was introduced in django 2.2.17, 3.0.11 and 3.1.3
+    py39-django{32,41,42}
+    ; py310 was introduced in django 3.2.9 and 4.0
+    py310-django{32,41,42}
+    ; py311 was introduced in django 4.1.3
+    py311-django{41,42}
     coverage
 
 [gh-actions]
 python =
-    3.7: py37
     3.8: py38
     3.9: py39
     3.10: py310
     3.11: py311, coverage
 
 [testenv]
 allowlist_externals =
     poetry
     bash
 setenv =
     PYTHONPATH = {toxinidir}
 deps =
     django32: django>=3.2,<3.3
-    django40: django>=4.0,<4.1
     django41: django>=4.1,<4.2
+    django42: django>=4.2,<4.3
     coverage: django>=4.0,<4.1
 commands =
     poetry lock
     # See https://github.com/python-poetry/poetry/issues/1745#issuecomment-648365339
     bash -c 'poetry export --dev --without-hashes -f requirements.txt | grep -v "^[dD]jango==" | poetry run pip install --no-deps -r /dev/stdin'
     poetry run pytest --basetemp={envtmpdir} {posargs}
```

### Comparing `django_userena_ce-7.0.2/userena/admin.py` & `django_userena_ce-7.0.3/userena/admin.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/backends.py` & `django_userena_ce-7.0.3/userena/backends.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/contrib/umessages/admin.py` & `django_userena_ce-7.0.3/userena/contrib/umessages/admin.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/contrib/umessages/fields.py` & `django_userena_ce-7.0.3/userena/contrib/umessages/fields.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/contrib/umessages/fixtures/messages.json` & `django_userena_ce-7.0.3/userena/contrib/umessages/fixtures/messages.json`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/contrib/umessages/forms.py` & `django_userena_ce-7.0.3/userena/contrib/umessages/forms.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/contrib/umessages/managers.py` & `django_userena_ce-7.0.3/userena/contrib/umessages/managers.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/contrib/umessages/migrations/0001_initial.py` & `django_userena_ce-7.0.3/userena/contrib/umessages/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/contrib/umessages/models.py` & `django_userena_ce-7.0.3/userena/contrib/umessages/models.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/contrib/umessages/templates/base.html` & `django_userena_ce-7.0.3/userena/contrib/umessages/templates/base.html`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/contrib/umessages/templates/umessages/message_list.html` & `django_userena_ce-7.0.3/userena/contrib/umessages/templates/umessages/message_list.html`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/contrib/umessages/templatetags/umessages_tags.py` & `django_userena_ce-7.0.3/userena/contrib/umessages/templatetags/umessages_tags.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/contrib/umessages/tests/test_fields.py` & `django_userena_ce-7.0.3/userena/contrib/umessages/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/contrib/umessages/tests/test_forms.py` & `django_userena_ce-7.0.3/userena/contrib/umessages/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/contrib/umessages/tests/test_managers.py` & `django_userena_ce-7.0.3/userena/contrib/umessages/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/contrib/umessages/tests/test_models.py` & `django_userena_ce-7.0.3/userena/contrib/umessages/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/contrib/umessages/tests/test_views.py` & `django_userena_ce-7.0.3/userena/contrib/umessages/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/contrib/umessages/urls.py` & `django_userena_ce-7.0.3/userena/contrib/umessages/urls.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/contrib/umessages/views.py` & `django_userena_ce-7.0.3/userena/contrib/umessages/views.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/decorators.py` & `django_userena_ce-7.0.3/userena/decorators.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/fixtures/users.json` & `django_userena_ce-7.0.3/userena/fixtures/users.json`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/forms.py` & `django_userena_ce-7.0.3/userena/forms.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/ar/LC_MESSAGES/django.mo` & `django_userena_ce-7.0.3/userena/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/ar/LC_MESSAGES/django.po` & `django_userena_ce-7.0.3/userena/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/bg/LC_MESSAGES/django.mo` & `django_userena_ce-7.0.3/userena/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/bg/LC_MESSAGES/django.po` & `django_userena_ce-7.0.3/userena/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/de/LC_MESSAGES/django.mo` & `django_userena_ce-7.0.3/userena/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/de/LC_MESSAGES/django.po` & `django_userena_ce-7.0.3/userena/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/de_du/LC_MESSAGES/django.mo` & `django_userena_ce-7.0.3/userena/locale/de_du/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/de_du/LC_MESSAGES/django.po` & `django_userena_ce-7.0.3/userena/locale/de_du/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/el/LC_MESSAGES/django.mo` & `django_userena_ce-7.0.3/userena/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/el/LC_MESSAGES/django.po` & `django_userena_ce-7.0.3/userena/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/es/LC_MESSAGES/django.mo` & `django_userena_ce-7.0.3/userena/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/es/LC_MESSAGES/django.po` & `django_userena_ce-7.0.3/userena/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/fr/LC_MESSAGES/django.mo` & `django_userena_ce-7.0.3/userena/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/fr/LC_MESSAGES/django.po` & `django_userena_ce-7.0.3/userena/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/gl/LC_MESSAGES/django.po` & `django_userena_ce-7.0.3/userena/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/it/LC_MESSAGES/django.mo` & `django_userena_ce-7.0.3/userena/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/it/LC_MESSAGES/django.po` & `django_userena_ce-7.0.3/userena/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/nb/LC_MESSAGES/django.mo` & `django_userena_ce-7.0.3/userena/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/nb/LC_MESSAGES/django.po` & `django_userena_ce-7.0.3/userena/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/nl/LC_MESSAGES/django.mo` & `django_userena_ce-7.0.3/userena/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/nl/LC_MESSAGES/django.po` & `django_userena_ce-7.0.3/userena/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/pl/LC_MESSAGES/django.mo` & `django_userena_ce-7.0.3/userena/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/pl/LC_MESSAGES/django.po` & `django_userena_ce-7.0.3/userena/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/pt/LC_MESSAGES/django.mo` & `django_userena_ce-7.0.3/userena/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/pt/LC_MESSAGES/django.po` & `django_userena_ce-7.0.3/userena/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/pt_BR/LC_MESSAGES/django.mo` & `django_userena_ce-7.0.3/userena/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/pt_BR/LC_MESSAGES/django.po` & `django_userena_ce-7.0.3/userena/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/ro/LC_MESSAGES/django.mo` & `django_userena_ce-7.0.3/userena/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/ro/LC_MESSAGES/django.po` & `django_userena_ce-7.0.3/userena/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/ru/LC_MESSAGES/django.mo` & `django_userena_ce-7.0.3/userena/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/ru/LC_MESSAGES/django.po` & `django_userena_ce-7.0.3/userena/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/tr/LC_MESSAGES/django.mo` & `django_userena_ce-7.0.3/userena/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/tr/LC_MESSAGES/django.po` & `django_userena_ce-7.0.3/userena/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/zh_Hans/LC_MESSAGES/django.mo` & `django_userena_ce-7.0.3/userena/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/zh_Hans/LC_MESSAGES/django.po` & `django_userena_ce-7.0.3/userena/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/zh_Hant/LC_MESSAGES/django.mo` & `django_userena_ce-7.0.3/userena/locale/zh_Hant/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/locale/zh_Hant/LC_MESSAGES/django.po` & `django_userena_ce-7.0.3/userena/locale/zh_Hant/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/mail.py` & `django_userena_ce-7.0.3/userena/mail.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/management/commands/check_permissions.py` & `django_userena_ce-7.0.3/userena/management/commands/check_permissions.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/managers.py` & `django_userena_ce-7.0.3/userena/managers.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/middleware.py` & `django_userena_ce-7.0.3/userena/middleware.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     switch languages depending if the cookie is set.
 
     """
 
     def process_request(self, request):
         lang_cookie = request.session.get(settings.LANGUAGE_COOKIE_NAME)
         if not lang_cookie:
-
             authenticated = request.user.is_authenticated
 
             if authenticated:
                 try:
                     profile = get_user_profile(user=request.user)
                 except (ObjectDoesNotExist, SiteProfileNotAvailable):
                     profile = False
```

### Comparing `django_userena_ce-7.0.2/userena/migrations/0001_initial.py` & `django_userena_ce-7.0.3/userena/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/migrations/0002_auto_20171130_0921.py` & `django_userena_ce-7.0.3/userena/migrations/0002_auto_20171130_0921.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/models.py` & `django_userena_ce-7.0.3/userena/models.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/runtests/private/development.db` & `django_userena_ce-7.0.3/userena/runtests/private/development.db`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/runtests/settings.py` & `django_userena_ce-7.0.3/userena/runtests/settings.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/runtests/urls.py` & `django_userena_ce-7.0.3/userena/runtests/urls.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/settings.py` & `django_userena_ce-7.0.3/userena/settings.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/base.html` & `django_userena_ce-7.0.3/userena/templates/base.html`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/activate_form.html` & `django_userena_ce-7.0.3/userena/templates/userena/activate_form.html`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/activate_retry.html` & `django_userena_ce-7.0.3/userena/templates/userena/activate_retry.html`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/activate_retry_success.html` & `django_userena_ce-7.0.3/userena/templates/userena/activate_retry_success.html`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/email_change_complete.html` & `django_userena_ce-7.0.3/userena/templates/userena/email_change_complete.html`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/email_form.html` & `django_userena_ce-7.0.3/userena/templates/userena/email_form.html`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/emails/activation_email_message.html` & `django_userena_ce-7.0.3/userena/templates/userena/emails/activation_email_message.html`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/emails/activation_email_message.txt` & `django_userena_ce-7.0.3/userena/templates/userena/emails/activation_email_message.txt`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/emails/confirmation_email_message_new.html` & `django_userena_ce-7.0.3/userena/templates/userena/emails/confirmation_email_message_new.html`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/emails/confirmation_email_message_new.txt` & `django_userena_ce-7.0.3/userena/templates/userena/emails/confirmation_email_message_new.txt`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/emails/confirmation_email_message_old.html` & `django_userena_ce-7.0.3/userena/templates/userena/emails/confirmation_email_message_old.html`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/emails/confirmation_email_message_old.txt` & `django_userena_ce-7.0.3/userena/templates/userena/emails/confirmation_email_message_old.txt`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/emails/password_reset_message.html` & `django_userena_ce-7.0.3/userena/templates/userena/emails/password_reset_message.html`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/emails/password_reset_message.txt` & `django_userena_ce-7.0.3/userena/templates/userena/emails/password_reset_message.txt`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/password_form.html` & `django_userena_ce-7.0.3/userena/templates/userena/password_form.html`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/profile_detail.html` & `django_userena_ce-7.0.3/userena/templates/userena/profile_detail.html`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/profile_form.html` & `django_userena_ce-7.0.3/userena/templates/userena/profile_form.html`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/profile_list.html` & `django_userena_ce-7.0.3/userena/templates/userena/profile_list.html`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/signin_form.html` & `django_userena_ce-7.0.3/userena/templates/userena/signin_form.html`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/signup_complete.html` & `django_userena_ce-7.0.3/userena/templates/userena/signup_complete.html`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/templates/userena/signup_form.html` & `django_userena_ce-7.0.3/userena/templates/userena/signup_form.html`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/tests/profiles/models.py` & `django_userena_ce-7.0.3/userena/tests/profiles/models.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/tests/test_backends.py` & `django_userena_ce-7.0.3/userena/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/tests/test_commands.py` & `django_userena_ce-7.0.3/userena/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/tests/test_privacy.py` & `django_userena_ce-7.0.3/userena/tests/test_privacy.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/tests/tests_decorators.py` & `django_userena_ce-7.0.3/userena/tests/tests_decorators.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/tests/tests_forms.py` & `django_userena_ce-7.0.3/userena/tests/tests_forms.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/tests/tests_managers.py` & `django_userena_ce-7.0.3/userena/tests/tests_managers.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/tests/tests_middleware.py` & `django_userena_ce-7.0.3/userena/tests/tests_middleware.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/tests/tests_models.py` & `django_userena_ce-7.0.3/userena/tests/tests_models.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/tests/tests_urls.py` & `django_userena_ce-7.0.3/userena/tests/tests_urls.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/tests/tests_utils.py` & `django_userena_ce-7.0.3/userena/tests/tests_utils.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/tests/tests_views.py` & `django_userena_ce-7.0.3/userena/tests/tests_views.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/urls.py` & `django_userena_ce-7.0.3/userena/urls.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/utils.py` & `django_userena_ce-7.0.3/userena/utils.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/userena/views.py` & `django_userena_ce-7.0.3/userena/views.py`

 * *Files identical despite different names*

### Comparing `django_userena_ce-7.0.2/PKG-INFO` & `django_userena_ce-7.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: django-userena-ce
-Version: 7.0.2
+Version: 7.0.3
 Summary: Complete user management application for Django
 Home-page: https://github.com/django-userena-ce/django-userena-ce
 License: BSD-3-Clause
 Author: James Meakin
 Author-email: django-userena-ce@jmsmkn.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Dist: Django (>=3.2,<4.2)
+Requires-Dist: Django (>=3.2)
 Requires-Dist: django-guardian (>=2.0)
 Requires-Dist: easy-thumbnails
 Requires-Dist: html2text
 Project-URL: Repository, https://github.com/django-userena-ce/django-userena-ce
 Description-Content-Type: text/markdown
 
 # Django Userena (Community Edition)
@@ -47,16 +46,16 @@
 the signup, activation, messaging and more. It's BSD licensed, which means you
 can use it commercially for free!
 
 ## Supported Software
 
 Software | Versions
 ---|---
-Python | 3.7, 3.8, 3.9, 3.10, 3.11
-Django | 3.2, 4.0, 4.1
+Python | 3.8, 3.9, 3.10, 3.11
+Django | 3.2, 4.1, 4.2
 Django Guardian | \>2.0
 
 ## [Documentation](https://django-userena-ce.github.io/django-userena-ce/index.html)
 
 Complete documentation about the
 [installation](https://django-userena-ce.github.io/django-userena-ce/installation.html),
 [settings](https://django-userena-ce.github.io/django-userena-ce/settings.html) and
```

