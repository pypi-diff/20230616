# Comparing `tmp/fastapi_all_out-0.3.0.tar.gz` & `tmp/fastapi_all_out-0.4.0.tar.gz`

## Comparing `fastapi_all_out-0.3.0.tar` & `fastapi_all_out-0.4.0.tar`

### file list

```diff
@@ -1,74 +1,78 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/__init__.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/app.py
--rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/code_responses.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/enums.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/lazy.py
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/mailing.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/models.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/responses.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/schemas.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/settings.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/__init__.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/base.py
--rw-r--r--   0        0        0    18042 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/router.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/schemas.py
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/user_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/jwt/__init__.py
--rw-r--r--   0        0        0     8576 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/jwt/backend.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/jwt/schemas.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/jwt/strategy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/roles/__init__.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/roles/router.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/roles/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/__init__.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/conntection.py
--rw-r--r--   0        0        0    34462 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/repository.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/repository_meta.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/user_repository.py
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/user_service.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/fields/__init__.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/filters/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/filters/fk.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/filters/int.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/filters/simple.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/filters/str.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/__init__.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/base.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/base_user.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/content_type.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/permissions.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/temp_code.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/management/__init__.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/management/command.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/pydantic/__init__.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/pydantic/camel_model.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/pydantic/comma_separated.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/__init__.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/field_in_related_model.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/password.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/phonenumber.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/related_list.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/username.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/__init__.py
--rw-r--r--   0        0        0     5133 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/base_repository.py
--rw-r--r--   0        0        0    24940 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/crud_router.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/exceptions.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/utils.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/__init__.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/base.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/bool.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/fk.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/int.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/int_btw.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/str.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/templates/activation.html
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/templates/email_change.html
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/templates/password_reset.html
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/LICENSE.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/README.md
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/__init__.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/app.py
+-rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/code_responses.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/db_connection.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/enums.py
+-rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/lazy_objects.py
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/mailing.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/models.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/responses.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/schemas.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/settings.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/auth/__init__.py
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/auth/base.py
+-rw-r--r--   0        0        0    18081 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/auth/router.py
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/auth/schemas.py
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/auth/user_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/auth/jwt/__init__.py
+-rw-r--r--   0        0        0     8676 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/auth/jwt/backend.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/auth/jwt/config.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/auth/jwt/schemas.py
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/auth/jwt/strategy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/auth/roles/__init__.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/auth/roles/router.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/auth/roles/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/__init__.py
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/config.py
+-rw-r--r--   0        0        0    34495 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/repository.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/repository_meta.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/user_repository.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/user_service.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/fields/__init__.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/filters/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/filters/fk.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/filters/int.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/filters/simple.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/filters/str.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/models/__init__.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/models/base.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/models/base_user.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/models/content_type.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/models/permissions.py
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/models/temp_code.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/management/__init__.py
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/management/command.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/management/createsuperuser.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/pydantic/__init__.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/pydantic/camel_model.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/pydantic/comma_separated.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/pydantic/config_model.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/pydantic/fields/__init__.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/pydantic/fields/field_in_related_model.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/pydantic/fields/password.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/pydantic/fields/phonenumber.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/pydantic/fields/related_list.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/pydantic/fields/username.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/routers/__init__.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/routers/base_repository.py
+-rw-r--r--   0        0        0    25013 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/routers/crud_router.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/routers/exceptions.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/routers/utils.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/routers/filters/__init__.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/routers/filters/base.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/routers/filters/bool.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/routers/filters/fk.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/routers/filters/int.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/routers/filters/int_btw.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/routers/filters/str.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/templates/activation.html
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/templates/email_change.html
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/fastapi_all_out/templates/password_reset.html
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/README.md
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 fastapi_all_out-0.4.0/PKG-INFO
```

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/app.py` & `fastapi_all_out-0.4.0/fastapi_all_out/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,37 @@
 from fastapi import FastAPI, APIRouter, Depends
 
 from fastapi_all_out.responses import \
     default_exception_handlers, \
     change_openapi_validation_error_schema
-from fastapi_all_out.lazy import get_auth_backend
-from fastapi_all_out.settings import MainDB
+from fastapi_all_out.lazy_objects import get_settings, get_global_objects
 
 
 class ExFastAPI(FastAPI):
     router: APIRouter
 
     def __init__(
             self,
             *,
-            db_provider: MainDB = None,
-            db_config: dict = None,
             add_auth_dependency: bool = True,
             **kwargs
     ) -> None:
         kwargs.setdefault('swagger_ui_parameters', {"operationsSorter": "method", "docExpansion": "none"})
         exception_handlers = kwargs.get('exception_handlers', {})
         kwargs['exception_handlers'] = {**default_exception_handlers, **exception_handlers}
         if add_auth_dependency:
             dependencies = kwargs.get('dependencies', [])
-            kwargs['dependencies'] = [Depends(get_auth_backend().authenticate_dependency()), *dependencies]
+            auth_backend = get_global_objects().AUTH_BACKEND
+            kwargs['dependencies'] = [Depends(auth_backend.authenticate_dependency()), *dependencies]
         super().__init__(**kwargs)
 
-        if db_config:
-            match db_provider:
-                case MainDB.tortoise:
-                    from fastapi_all_out.contrib.tortoise import conntection
-                    db_on_start = conntection.on_start(config=db_config)
-                    db_on_shutdown = conntection.on_shutdown
-                case None:
-                    db_on_start = None
-                    db_on_shutdown = None
-                case _:
-                    raise Exception(f'Unknown {db_provider=}')
-            if db_on_start:
-                self.router.on_startup.append(db_on_start)
-            if db_on_shutdown:
-                self.router.on_shutdown.append(db_on_shutdown)
+        # db connections
+        databases = get_settings().get_db_config()
+        self.router.on_startup.append(databases.connect_all)
+        self.router.on_shutdown.append(databases.close_all)
 
         async def default_on_start():
             try:
                 change_openapi_validation_error_schema(self)
             except KeyError:
                 pass
```

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/code_responses.py` & `fastapi_all_out-0.4.0/fastapi_all_out/code_responses.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/mailing.py` & `fastapi_all_out-0.4.0/fastapi_all_out/mailing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,42 @@
+from typing import Any, TYPE_CHECKING
+from pathlib import Path
 from datetime import timedelta
-from enum import Enum
-from typing import Any, TypedDict, TYPE_CHECKING
 
-from fastapi_mail import FastMail, MessageSchema, MessageType
-from pydantic import EmailStr, ValidationError
+from fastapi_mail import ConnectionConfig, FastMail, MessageSchema, MessageType
+from pydantic import EmailStr, DirectoryPath, AnyHttpUrl
 
-from fastapi_all_out.lazy import get_settings_obj, get_mail_settings
-from fastapi_all_out.settings import MailingConfig
 from fastapi_all_out.utils import timedelta_to_string
 
 if TYPE_CHECKING:
     from fastapi_all_out.auth.base import BaseUser, TempCodeProto
 
 
-HOST = get_settings_obj().HOST
-mail_settings: "MailSettingsType" = get_mail_settings()
-endpoints = mail_settings['endpoints']
+class MailingConfig(ConnectionConfig):
+    TEMPLATE_FOLDER: DirectoryPath = Path(__file__).parent / 'templates'
 
-
-class MailSettingsType(TypedDict):
-    sender: str
-    endpoints: dict[str, str]
-    temp_code_duration: dict[Enum | str, timedelta]
+    HOST: AnyHttpUrl = 'http://localhost:8000'
+    endpoints: dict[str, str] = {
+        'activation': 'confirm',
+        'email_change': 'email_change',
+        'password_reset': 'password_reset',
+    }
+    temp_code_duration = {
+        '_default': timedelta(hours=1),
+    }
 
 
 class MailSender:
 
     fast_mail: FastMail
+    conf: MailingConfig
 
-    def __init__(self, conf: MailingConfig):
+    def __init__(self, conf: "MailingConfig"):
         self.fast_mail = FastMail(conf)
+        self.conf = conf
 
     async def send(
             self,
             to: EmailStr | str,
             data: dict[str, Any],
             template: str,
             subject: str
@@ -64,39 +67,33 @@
         }
         await self.send(to=user.email, data=data, template=template, subject=subject)
 
     async def activation_email(self, user: "BaseUser", temp_code: "TempCodeProto") -> None:
         await self.send_tempcode_email(
             user=user,
             temp_code=temp_code,
-            host=HOST,
-            endpoint=endpoints['activation'],
+            host=self.conf.HOST,
+            endpoint=self.conf.endpoints['activation'],
             template='activation.html',
             subject='Account activation',
         )
 
     async def email_change_email(self, user: "BaseUser", temp_code: "TempCodeProto", new_email: str) -> None:
         await self.send_tempcode_email(
             user=user,
             temp_code=temp_code,
-            host=HOST,
-            endpoint=endpoints['email_change'],
+            host=self.conf.HOST,
+            endpoint=self.conf.endpoints['email_change'],
             template='email_change.html',
             subject='Email change',
             new_email=new_email,
         )
 
     async def password_reset_email(self, user: "BaseUser", temp_code: "TempCodeProto") -> None:
         await self.send_tempcode_email(
             user=user,
             temp_code=temp_code,
-            host=HOST,
-            endpoint=endpoints['password_reset'],
+            host=self.conf.HOST,
+            endpoint=self.conf.endpoints['password_reset'],
             template='password_reset.html',
             subject='Password reset',
         )
-
-
-try:
-    mail_sender = MailSender(MailingConfig())
-except ValidationError:
-    mail_sender = None
```

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/models.py` & `fastapi_all_out-0.4.0/fastapi_all_out/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from fastapi_all_out.settings import MainDB
-from fastapi_all_out.lazy import get_main_db
+from typing import Any
 
+from fastapi_all_out.enums import Databases
+from fastapi_all_out.lazy_objects import get_global_objects
 
-match get_main_db():
-    case MainDB.tortoise:
+
+match get_global_objects().auth_db:
+    case Databases.tortoise:
         from fastapi_all_out.contrib.tortoise.models import \
             BaseModel, default_of, max_len_of, \
             Permission, PermissionGroup
     case _:
         BaseModel = None
         default_of = None
         max_len_of = None
```

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/responses.py` & `fastapi_all_out-0.4.0/fastapi_all_out/responses.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/utils.py` & `fastapi_all_out-0.4.0/fastapi_all_out/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/auth/base.py` & `fastapi_all_out-0.4.0/fastapi_all_out/auth/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 from abc import ABC, abstractmethod
 from datetime import datetime, timedelta
-from typing import Callable, Coroutine, Any, Optional, Protocol
+from typing import Callable, Coroutine, Any, Optional, Protocol, Self
 from uuid import UUID
 
 from fastapi import APIRouter
 
 from fastapi_all_out.enums import TempCodeTriggers
-from fastapi_all_out.lazy import get_codes
-
-
-Codes = get_codes()
+from fastapi_all_out.pydantic import ConfigModel
 
 
 class AuthStrategy(ABC):
     authorize_response_model: Any
 
     def authorize(self, user: "BaseUser") -> Any: ...
 
+    @classmethod
+    @abstractmethod
+    def from_config(cls, config: ConfigModel) -> Self: ...
+
 
 class AuthBackend(ABC):
 
     strategy: "AuthStrategy"
 
+    def __init__(self, strategy: "AuthStrategy"):
+        self.strategy = strategy
+
     def authorize(self, user: "BaseUser") -> Any:
         return self.strategy.authorize(user=user)
 
+    @classmethod
+    @abstractmethod
+    def from_config(cls, strategy: AuthStrategy, config: ConfigModel) -> Self: ...
+
     @abstractmethod
     def authenticate_dependency(self) -> Callable[[], Coroutine[Any, Any, None]]: ...
 
     @abstractmethod
     def auth_required_dependency(self) -> Callable[[], Coroutine[Any, Any, None]]: ...
 
     @abstractmethod
@@ -53,14 +61,19 @@
     @abstractmethod
     def add_login_route(self, router: APIRouter) -> None: ...
 
     @abstractmethod
     def add_logout_route(self, router: APIRouter) -> None: ...
 
 
+class AuthConfig(ConfigModel):
+    backend: str
+    strategy: str
+
+
 class BaseUser:
     id: int
     uuid: UUID
     username: Optional[str]
     email: Optional[str]
     password_hash: str
     password_change_dt: datetime
```

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/auth/router.py` & `fastapi_all_out-0.4.0/fastapi_all_out/auth/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 from uuid import uuid4, UUID
 
 from fastapi import Request, BackgroundTasks, Response, Body, Query, Path
 from pydantic import EmailStr, PositiveInt
 
 from fastapi_all_out.auth.base import BaseUser
 from fastapi_all_out.enums import TempCodeTriggers
-from fastapi_all_out.lazy import get_user_repository, get_user_service, get_schema, get_codes, get_auth_backend
+from fastapi_all_out.lazy_objects import get_global_objects, get_schema
 from fastapi_all_out.pydantic import CamelModel
 from fastapi_all_out.routers import CRUDRouter
 from fastapi_all_out.routers.crud_router import LOAD_USER, ACCESS_ALL, LOAD_USER_OPTIONALLY, CHECK_PERMS, REPO
 from fastapi_all_out.routers.exceptions import ObjectErrors, ItemNotFound, OldPasswordIsIncorrect
 from fastapi_all_out.schemas import UserRead, UserMeRead, UserEdit, UserMeEdit, UserCreate, UserRegistration,\
     ChangePassword, PasswordsPair
 
 
-auth_backend = get_auth_backend()
-UserRepository = get_user_repository()
-UserService = get_user_service()
-Codes = get_codes()
+global_objects = get_global_objects()
+
+auth_backend = global_objects.AUTH_BACKEND
+UserRepository = global_objects.USER_REPOSITORY
+UserService = global_objects.USER_SERVICE
+Codes = global_objects.CODES
+
 UserRead = get_schema(UserRead)
 UserMeRead = get_schema(UserMeRead)
 UserEdit = get_schema(UserEdit)
 UserMeEdit = get_schema(UserMeEdit)
 UserCreate = get_schema(UserCreate)
 UserRegistration = get_schema(UserRegistration)
 ChangePassword = get_schema(ChangePassword)
```

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/auth/schemas.py` & `fastapi_all_out-0.4.0/fastapi_all_out/auth/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from datetime import datetime
 from typing import Any, Optional
 
 from pydantic import root_validator, validator, EmailStr, Field
 
 from fastapi_all_out.pydantic import CamelModel, Password, Username, RelatedList, CamelModelORM
 from fastapi_all_out.models import max_len_of
-from fastapi_all_out.lazy import get_user_model, get_schema
+from fastapi_all_out.lazy_objects import get_global_objects, get_schema
 from fastapi_all_out.schemas import PermissionRead
 
 
 __all__ = [
     "PasswordsPair", "ChangePassword", "BaseLoginPasswordSchema", "LoginPasswordSchema",
     "UserRead", "UserMeRead", "UserEdit", "UserMeEdit", "UserCreate", "UserRegistration",
 ]
 
-UserModel = get_user_model()
+UserModel = get_global_objects().USER_MODEL
 Username = get_schema(Username, field=True)
 Password = get_schema(Password, field=True)
 
 
 class PasswordsPair(CamelModel):
     password: Password
     re_password: str
@@ -99,16 +99,16 @@
 
 
 class UserMeEdit(UserWriteBase):
     pass
 
 
 class UserCreate(PasswordsPair, UserWriteBase):
-    permissions: list[int]
-    groups: list[int]
+    permissions: list[int] = []
+    groups: list[int] = []
     is_superuser: Optional[bool]
     is_active: Optional[bool]
 
 
 class UserRegistration(PasswordsPair, UserWriteBase):
     pass
```

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/auth/user_service.py` & `fastapi_all_out-0.4.0/fastapi_all_out/auth/user_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import TypeVar, Any, Generic, Literal, Optional, TYPE_CHECKING, Sequence
 from abc import ABC, abstractmethod
 
 from passlib.context import CryptContext
 from fastapi import Request, BackgroundTasks, Response
 
 from fastapi_all_out.enums import TempCodeTriggers
-from fastapi_all_out.lazy import get_mail_sender
+from fastapi_all_out.lazy_objects import get_global_objects
 from fastapi_all_out.code_responses import BaseCodes
 from .base import BaseUser
 
 if TYPE_CHECKING:
     from fastapi_all_out.auth.base import TempCodeProto
 
 
 USER_MODEL = TypeVar("USER_MODEL", BaseUser, Any)
 UNUSED_PASSWORD_PREFIX = '!'
-mail_sender = get_mail_sender()
+gl = get_global_objects()
 
 
 class BaseUserService(Generic[USER_MODEL], ABC):
 
     user: USER_MODEL
     pwd_context = CryptContext(schemes=["md5_crypt"], deprecated="auto")
 
@@ -53,25 +53,25 @@
         return self.pwd_context.verify(self.get_fake_password(password), self.user.password_hash)
 
     async def post_registration(self, request: Request, background_tasks: BackgroundTasks, response: Response) -> None:
         background_tasks.add_task(self.send_activation_email)
 
     async def send_activation_email(self) -> None:
         temp_code = await self.update_or_create_temp_code(trigger=TempCodeTriggers.EmailActivation)
-        await mail_sender.activation_email(user=self.user, temp_code=temp_code)
+        await gl.MAIL_SENDER.activation_email(user=self.user, temp_code=temp_code)
 
     async def send_email_change_email(self, new_email: str) -> None:
         temp_code = await self.update_or_create_temp_code(
             trigger=TempCodeTriggers.EmailChange, extras={'new_email': new_email}
         )
-        await mail_sender.email_change_email(user=self.user, temp_code=temp_code, new_email=new_email)
+        await gl.MAIL_SENDER.email_change_email(user=self.user, temp_code=temp_code, new_email=new_email)
 
     async def send_password_reset_email(self) -> None:
         temp_code = await self.update_or_create_temp_code(trigger=TempCodeTriggers.PasswordReset)
-        await mail_sender.password_reset_email(user=self.user, temp_code=temp_code)
+        await gl.MAIL_SENDER.password_reset_email(user=self.user, temp_code=temp_code)
 
     @abstractmethod
     async def create_temp_code(
             self, trigger: TempCodeTriggers, extras: dict[str, Any] | list[Any] = None
     ) -> "TempCodeProto": ...
 
     @abstractmethod
```

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/auth/jwt/backend.py` & `fastapi_all_out-0.4.0/fastapi_all_out/auth/jwt/backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 from warnings import warn
-from typing import Callable, Coroutine, Any, cast
+from typing import Callable, Coroutine, Any, cast, Self
 
 from fastapi import APIRouter, Request, BackgroundTasks, Response, Body, Depends
 from fastapi.security import OAuth2PasswordBearer, OAuth2PasswordRequestForm
 
-from fastapi_all_out.lazy import get_schema, get_user_model, get_user_repository, get_user_service, get_codes,\
-    get_settings_obj
+from fastapi_all_out.lazy_objects import get_global_objects, get_schema
 from fastapi_all_out.routers.exceptions import ItemNotFound
 from fastapi_all_out.schemas import LoginPasswordSchema, UserMeRead
 from ..base import AuthBackend, BaseUser, SimpleUser, UnauthenticatedUser
+from .config import JWTAuthConfig
 from .schemas import JWTTokenUser
 from .strategy import JWTAuthStrategy
 
 
+global_objects = get_global_objects()
+
 LoginPasswordSchema = get_schema(LoginPasswordSchema)
 UserMeRead = get_schema(UserMeRead)
 JWTTokenUser = get_schema(JWTTokenUser)
-UserModel = get_user_model()
-UserRepository = get_user_repository()
-UserService = get_user_service()
-Codes = get_codes()
-settings = get_settings_obj()
-oauth2_default = OAuth2PasswordBearer(
-    tokenUrl=settings.API_PREFIX + '/auth/jwt/login',
-    scheme_name='Bearer',
-    auto_error=False,
-)
+UserModel = global_objects.USER_MODEL
+UserRepository = global_objects.USER_REPOSITORY
+UserService = global_objects.USER_SERVICE
+Codes = global_objects.CODES
 
 
-class JWTAuthBackend(AuthBackend):
+class JWTOAuth2PasswordBearerBackend(AuthBackend):
 
-    strategy: "JWTAuthStrategy"
+    strategy: JWTAuthStrategy
     oauth: OAuth2PasswordBearer
     _authenticate: Callable[[Request, str], Coroutine[Any, Any, None]]
     _auth_required: Callable[[Request], Coroutine[Any, Any, None]]
     _load_user: Callable[[Request, BackgroundTasks, Response], Coroutine[Any, Any, None]]
     _load_user_optionally: Callable[[Request, BackgroundTasks, Response], Coroutine[Any, Any, None]]
 
-    def __init__(self, strategy: "JWTAuthStrategy", oauth: OAuth2PasswordBearer = oauth2_default):
+    def __init__(self, strategy: JWTAuthStrategy, oauth: OAuth2PasswordBearer):
         assert isinstance(strategy, JWTAuthStrategy)
-        self.strategy = strategy
+        super().__init__(strategy=strategy)
         self.oauth = oauth
 
+    @classmethod
+    def from_config(cls, strategy: JWTAuthStrategy, config: JWTAuthConfig) -> Self:
+        return cls(
+            strategy=strategy,
+            oauth=config.get_oauth2_password_bearer()
+        )
+
     def authenticate_dependency(self) -> Callable[[Request, str], Coroutine[Any, Any, None]]:
         if not hasattr(self, '_authenticate'):
-            oauth_schema = self.oauth
             authenticate_handler = self.strategy.authenticate
 
-            async def authenticate(request: Request, token: str = Depends(oauth_schema)) -> None:
+            async def authenticate(request: Request, token: str = Depends(self.oauth)) -> None:
                 token_data = await authenticate_handler(token)
                 if token_data is None:
                     request.scope['auth'] = None
                     request.scope['user'] = UnauthenticatedUser()
                 else:
                     user = token_data.user
                     request.scope['auth'] = token_data
@@ -134,15 +136,16 @@
 
     def create_router(self, add_refresh_route: bool = True, **kwargs) -> APIRouter:
         router = super().create_router(**kwargs)
         if add_refresh_route:
             self.add_refresh_route(router)
         return router
 
-    def login_responses(self):
+    @classmethod
+    def login_responses(cls):
         return Codes.responses(Codes.not_authenticated)
 
     def add_login_route(self, router: APIRouter) -> None:
         @router.post(
             '/login', response_model=self.strategy.authorize_response_model,
             responses=self.login_responses()
         )
@@ -168,15 +171,16 @@
                 await user_service.if_cant_login(request=request, background_tasks=background_tasks, response=response)
                 raise Codes.not_authenticated.err()
             return self.authorize(user)
 
     def add_logout_route(self, router: APIRouter) -> None:
         pass
 
-    def refresh_responses(self):
+    @classmethod
+    def refresh_responses(cls):
         return Codes.responses(Codes.not_authenticated)
 
     def add_refresh_route(self, router: APIRouter) -> None:
         @router.post(
             '/refresh', response_model=self.strategy.authorize_response_model,
             responses=self.refresh_responses()
         )
```

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/auth/jwt/schemas.py` & `fastapi_all_out-0.4.0/fastapi_all_out/auth/jwt/schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any
 
 from pydantic import root_validator
 
-from fastapi_all_out.lazy import get_schema
+from fastapi_all_out.lazy_objects import get_schema
 from fastapi_all_out.enums import JWTTokenTypes
 from fastapi_all_out.pydantic import CamelModel, CamelModelORM
 
 
 class JWTTokenUser(CamelModelORM):
     id: int
     username: str
```

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/auth/jwt/strategy.py` & `fastapi_all_out-0.4.0/fastapi_all_out/auth/jwt/strategy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 from abc import abstractmethod
-from datetime import timedelta, datetime
-from typing import Any, Optional
+from datetime import datetime
+from typing import Any, Optional, Self
 
 from jwt import PyJWT, InvalidSignatureError, DecodeError, ExpiredSignatureError
 
 from fastapi_all_out.pydantic import CamelModel
 from fastapi_all_out.responses import DefaultJSONEncoder
-from fastapi_all_out.lazy import get_schema, get_codes
+from fastapi_all_out.lazy_objects import get_schema, get_global_objects
 from fastapi_all_out.enums import JWTTokenTypes
 from fastapi_all_out.schemas import UserMeRead
 from ..base import AuthStrategy, BaseUser
+from .config import JWTAuthConfig
 from .schemas import JWTToken, JWTTokenIssue
 
 
 LIFETIME = dict[JWTTokenTypes, int]
-DEFAULT_LIFETIME: LIFETIME = {
-    JWTTokenTypes.access: int(timedelta(minutes=5).total_seconds()),
-    JWTTokenTypes.refresh: int(timedelta(days=10).total_seconds()),
-}
 
 JWTToken = get_schema(JWTToken)
 JWTTokenIssue = get_schema(JWTTokenIssue)
 UserMeRead = get_schema(UserMeRead)
-Codes = get_codes()
+Codes = get_global_objects().CODES
 
 
 class TokenPair(CamelModel):
     access_token: str
     refresh_token: str
     user: UserMeRead
     token_type: str = 'bearer'
@@ -41,16 +38,18 @@
 
     authorize_response_model = TokenPair
 
     DECODE_SECRET: str
     ENCODE_SECRET: str
     SCHEMA: str
 
-    def __init__(self, *, lifetime: LIFETIME = None, schema: str = "bearer"):
-        self.lifetime = {**DEFAULT_LIFETIME, **(lifetime or {})}
+    def __init__(self, lifetime: LIFETIME, schema: str, encode_secret: str, decode_secret: str):
+        self.lifetime = lifetime
+        self.ENCODE_SECRET = encode_secret
+        self.DECODE_SECRET = decode_secret
         self.SCHEMA = schema.lower()
 
     @property
     @abstractmethod
     def ALGORITHM(self) -> str: ...
 
     def decode(self, token: str) -> dict[str, Any]:
@@ -114,11 +113,18 @@
     def get_refresh_token(self, token: str) -> JWTToken:
         return self.parse_token(token, token_type=JWTTokenTypes.refresh)
 
 
 class RS256JWTAuthStrategy(JWTAuthStrategy):
     ALGORITHM = 'RS256'
 
-    def __init__(self, *args, public_key: str = None, private_key: str = None, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.ENCODE_SECRET = private_key.replace('|||n|||', '\n').strip("'").strip('"') if private_key else None
-        self.DECODE_SECRET = public_key.strip("'").strip('"') if public_key else None
+    @classmethod
+    def from_config(cls, config: JWTAuthConfig) -> Self:
+        return cls(
+            lifetime={
+                JWTTokenTypes.access: config.ACCESS_TOKEN_LIFETIME,
+                JWTTokenTypes.refresh: config.REFRESH_TOKEN_LIFETIME,
+            },
+            schema=config.SCHEMA_NAME,
+            encode_secret=config.RSA_PRIVATE.replace('|||n|||', '\n'),
+            decode_secret=config.RSA_PUBLIC,
+        )
```

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/auth/roles/router.py` & `fastapi_all_out-0.4.0/fastapi_all_out/auth/roles/router.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from fastapi import APIRouter
 
 from fastapi_all_out.routers import CRUDRouter
-from fastapi_all_out.lazy import get_schema, get_repository
+from fastapi_all_out.lazy_objects import get_schema, get_global_objects
 from fastapi_all_out.models import Permission, PermissionGroup
 from fastapi_all_out.schemas import PermissionRead, PermissionGroupRead, PermissionGroupCreate, PermissionGroupEdit
 
 
-Repository = get_repository()
+Repository = get_global_objects().REPOSITORY
 
 
 def get_roles_router(prefix: str = '/roles', **kwargs) -> APIRouter:
     router = APIRouter(prefix=prefix, **kwargs)
 
     router.include_router(CRUDRouter(
         repo=type('PermissionRepository', (Repository, ), {'model': Permission}),  # type: ignore
```

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/auth/roles/schemas.py` & `fastapi_all_out-0.4.0/fastapi_all_out/auth/roles/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/repository.py` & `fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 from typing import Any, Optional, TypeVar, Type, Callable, Coroutine
 
 from tortoise.models import MetaInfo
 from tortoise.fields import ManyToManyRelation, Field, DatetimeField, TimeField
 from tortoise.queryset import QuerySet
 from tortoise.transactions import in_transaction
 
-from fastapi_all_out.lazy import get_auth_backend, get_settings
+from fastapi_all_out.settings import DEBUG
+from fastapi_all_out.lazy_objects import get_global_objects
 from fastapi_all_out.routers.utils import SORT, FILTERS
 from fastapi_all_out.routers.base_repository import BaseRepository, PK, ModelPrefix, Updated
 from fastapi_all_out.routers.exceptions import ItemNotFound, ObjectErrors, FieldError, NotUnique, ListFieldError,\
     NotFoundFK, FieldRequired
 from .repository_meta import TortoiseRepositoryMeta
 from .models import BaseModel
 
 
 DB_MODEL = TypeVar('DB_MODEL', bound=BaseModel)
-DEBUG = get_settings('DEBUG')
+gl = get_global_objects()
 
 
 class TortoiseRepository(BaseRepository[DB_MODEL], metaclass=TortoiseRepositoryMeta):
     opts: MetaInfo
     node_key = 'parent_id'
 
     select_related: tuple[str]
@@ -824,15 +825,15 @@
 
     def with_model_permissions(cls, *names: str) -> Callable[[...], Coroutine[Any, Any, None]]:
         permissions: set[str] = set()
         for name in names:
             if not (name in cls.model.BASE_PERMISSIONS or name in cls.model.EXTRA_PERMISSIONS):
                 raise Exception(f'{cls.model} don`t have {name} permission')
             permissions.add(name)
-        return get_auth_backend().with_permissions_dependency(*((cls.model.__name__, name) for name in permissions))
+        return gl.AUTH_BACKEND.with_permissions_dependency(*((cls.model.__name__, name) for name in permissions))
 
     @classmethod
     def _get_bfk_model(cls, model: Type[BaseModel], field_name: str) -> Type[BaseModel]:
         return model._meta.fields_map[field_name].related_model
 
     @classmethod
     def _get_pk_attr(cls, model: Type[BaseModel]) -> str:
```

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/user_service.py` & `fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/user_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from random import choices
 from string import hexdigits
-from typing import TypeVar, Type, Optional, cast, Any
+from typing import TypeVar, Type, Optional, cast, Any, TYPE_CHECKING
 
 from tortoise import timezone
 
 from fastapi_all_out.auth.user_service import BaseUserService, UNUSED_PASSWORD_PREFIX
-from fastapi_all_out.lazy import get_user_model
+from fastapi_all_out.lazy_objects import get_global_objects
 from fastapi_all_out.enums import TempCodeTriggers
-from .models import TempCode, BaseUser, max_len_of, get_field_param
+from .models import BaseUser, max_len_of, get_field_param
+
+if TYPE_CHECKING:
+    from .models.temp_code import TempCode
 
 
 USER_MODEL = TypeVar("USER_MODEL", bound=BaseUser)
-UserModel = cast(Type[BaseUser], get_user_model())
+UserModel = cast(Type[BaseUser], get_global_objects().USER_MODEL)
 
 
 class TortoiseUserService(BaseUserService[USER_MODEL]):
-    _temp_code_model: Type[TempCode]
+    _temp_code_model: Type["TempCode"]
 
     def set_password(self, password: Optional[str]) -> None:
         user = self.user
         user.password_change_dt = timezone.now()
         user.password_salt = ''.join(choices(hexdigits, k=max_len_of(UserModel)('password_salt')))
         if password:
             user.password_hash = self.get_password_hash(password)
@@ -27,31 +30,31 @@
             user.password_hash = UNUSED_PASSWORD_PREFIX + self.get_password_hash(''.join(choices(hexdigits, k=30)))
 
     async def update_password(self, password: str) -> None:
         self.set_password(password)
         await self.user.save(force_update=True, update_fields=['password_hash', 'password_change_dt', 'password_salt'])
 
     @classmethod
-    def get_temp_code_model(cls) -> Type[TempCode]:
+    def get_temp_code_model(cls) -> Type["TempCode"]:
         if not hasattr(cls, '_temp_code_model'):
             cls._temp_code_model = get_field_param(UserModel, 'temp_code', 'related_model')
         return cls._temp_code_model
 
     async def create_temp_code(
             self, trigger: TempCodeTriggers, extras: dict[str, Any] | list[Any] = None
-    ) -> TempCode:
+    ) -> "TempCode":
         return await self.get_temp_code_model().new(user=self.user, trigger=trigger, extras=extras)
 
     async def get_temp_code(
             self, trigger: TempCodeTriggers
-    ) -> Optional[TempCode]:
+    ) -> Optional["TempCode"]:
         return await self.get_temp_code_model().get_or_none(user=self.user, trigger=trigger)
 
     async def update_temp_code(
-            self, temp_code: TempCode, extras: dict[str, Any] | list[Any] = None
+            self, temp_code: "TempCode", extras: dict[str, Any] | list[Any] = None
     ) -> None:
         await temp_code.update(extras=extras)
 
     async def delete_temp_code(
-            self, temp_code: TempCode
+            self, temp_code: "TempCode"
     ) -> None:
         await temp_code.delete()
```

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py` & `fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/filters/simple.py` & `fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/filters/simple.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/filters/str.py` & `fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/filters/str.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/base.py` & `fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/models/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/base_user.py` & `fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/models/base_user.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,16 +20,14 @@
     password_change_dt: datetime = fields.DatetimeField()
     password_salt: str = fields.CharField(max_length=50)
 
     is_superuser: bool = fields.BooleanField(default=False)
     is_active: bool = fields.BooleanField(default=True)
     created_at: datetime = fields.DatetimeField(auto_now_add=True)
 
-    # temp_code: Union[list["TempCode"], fields.BackwardFKRelation["TempCode"]]
-
     AUTH_FIELDS = ('email', 'username')
     IEXACT_FIELDS = ('email', 'username')
     EMAIL_FIELD = 'email'
     EXTRA_PERMISSIONS = ('change_password',)
 
     class Meta:
         abstract = True
```

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/content_type.py` & `fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/models/content_type.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/permissions.py` & `fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/models/permissions.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/temp_code.py` & `fastapi_all_out-0.4.0/fastapi_all_out/contrib/tortoise/models/temp_code.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 from datetime import timedelta, datetime
 from string import ascii_uppercase, digits
 from random import choices
 
 from tortoise import fields, timezone
 
 from fastapi_all_out.enums import TempCodeTriggers
-from fastapi_all_out.lazy import get_user_model_path, get_mail_settings
+from fastapi_all_out.lazy_objects import get_global_objects, get_settings
 from . import max_len_of
 from . import BaseModel, BaseUser
 
 
+global_objects = get_global_objects()
+
+
 class TempCode(BaseModel):
     id: int = fields.BigIntField(pk=True)
     user: Union["BaseUser", fields.ForeignKeyRelation["BaseUser"]] = fields.ForeignKeyField(
-        get_user_model_path(), related_name='temp_code', on_delete=fields.CASCADE
+        global_objects.user_model_path, related_name='temp_code', on_delete=fields.CASCADE
     )
     code: str = fields.CharField(max_length=6)
     expired_at: datetime = fields.DatetimeField()
     trigger: TempCodeTriggers = fields.CharEnumField(TempCodeTriggers)
     extras: Optional[dict[str, Any] | list[Any]] = fields.JSONField(null=True)
 
     class Meta:
@@ -56,12 +59,12 @@
         await self.save(force_update=True, update_fields=('code', 'expired_at', 'extras'))
 
 
 def get_random_tempcode(code_len: int) -> Callable[[], str]:
     return lambda: ''.join(choices(ascii_uppercase + digits, k=code_len))
 
 
-durations = get_mail_settings()['temp_code_duration']
+durations = get_settings().get_mailing_config().temp_code_duration
 
 
 def get_tempcode_durations(trigger: TempCodeTriggers) -> timedelta:
     return durations.get(trigger) or durations['_default']
```

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/pydantic/camel_model.py` & `fastapi_all_out-0.4.0/fastapi_all_out/pydantic/camel_model.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/pydantic/comma_separated.py` & `fastapi_all_out-0.4.0/fastapi_all_out/pydantic/comma_separated.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/field_in_related_model.py` & `fastapi_all_out-0.4.0/fastapi_all_out/pydantic/fields/field_in_related_model.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/password.py` & `fastapi_all_out-0.4.0/fastapi_all_out/pydantic/fields/password.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/phonenumber.py` & `fastapi_all_out-0.4.0/fastapi_all_out/pydantic/fields/phonenumber.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/related_list.py` & `fastapi_all_out-0.4.0/fastapi_all_out/pydantic/fields/related_list.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/username.py` & `fastapi_all_out-0.4.0/fastapi_all_out/pydantic/fields/username.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/routers/base_repository.py` & `fastapi_all_out-0.4.0/fastapi_all_out/routers/base_repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,7 +161,17 @@
     def get_pass_check_required(self, prefix: ModelPrefix) -> set[str]:
         if self.pass_check_required:
             return self.pass_check_required.get(prefix, set())
         return set()
 
     @abstractmethod
     def _fk_get_default(self, model: Type[DB_MODEL], pk: PK) -> DB_MODEL: ...
+
+
+class BaseUserRepository(BaseRepository[DB_MODEL]):
+
+    @abstractmethod
+    async def create_superuser(self, data: dict[str, Any]) -> None: ...
+
+    @classmethod
+    @abstractmethod
+    def get_create_superuser_fields(cls) -> tuple[str, ...]: ...
```

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/routers/crud_router.py` & `fastapi_all_out-0.4.0/fastapi_all_out/routers/crud_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from fastapi.utils import generate_unique_id
 from pydantic.error_wrappers import ErrorWrapper
 from starlette.responses import JSONResponse
 from starlette.routing import BaseRoute
 
 from fastapi_all_out.code_responses import BaseCodes
 from fastapi_all_out.pydantic import CommaSeparatedOf, lower_camel, CamelModel
-from fastapi_all_out.lazy import get_codes, get_auth_backend
+from fastapi_all_out.lazy_objects import get_global_objects
 from fastapi_all_out.responses import BgHTTPException
 from fastapi_all_out.routers import BaseRepository
 from .exceptions import ItemNotFound, ObjectErrors
 from .filters import BaseFilter
 from .utils import \
     pagination_factory, PAGINATION,\
     filters_factory, FILTERS, \
@@ -35,15 +35,17 @@
 REPO = TypeVar('REPO', bound=BaseRepository)
 DEPENDENCIES = Optional[Sequence[Depends]]
 ROUTE_KWARGS = TypedDict('ROUTE_KWARGS', total=False, fields={
     'dependencies': DEPENDENCIES,
     'access': ACCESS
 })
 ROUTES_KWARGS = dict[str, ROUTE_KWARGS]
-Codes = get_codes()
+global_objects = get_global_objects()
+Codes = global_objects.CODES
+auth_backend = global_objects.AUTH_BACKEND
 
 
 class CRUDRouter(Generic[REPO], APIRouter):
     repo: Type[REPO]
     max_items_get_many_routes: Optional[int]
     max_items_delete_many_routes: Optional[int]
     filters: list[Type[BaseFilter]]
@@ -170,19 +172,19 @@
             elif route_name in self.DELETE_names():
                 check_perms_dep = Depends(self.repo.with_model_permissions('delete'))
             else:
                 raise Exception('If access is check_perms, permissions must be passed '
                                 'or route_name must be in GET_names, CREATE_names, EDIT_names or DELETE_names')
             return *dependencies, check_perms_dep
         elif access == LOAD_USER:
-            return *dependencies, Depends(get_auth_backend().load_user_dependency())
+            return *dependencies, Depends(auth_backend.load_user_dependency())
         elif access == AUTH_REQUIRED:
-            return *dependencies, Depends(get_auth_backend().auth_required_dependency())
+            return *dependencies, Depends(auth_backend.auth_required_dependency())
         elif access == LOAD_USER_OPTIONALLY:
-            return *dependencies, Depends(get_auth_backend().load_user_optionally_dependency())
+            return *dependencies, Depends(auth_backend.load_user_optionally_dependency())
         return *dependencies,
 
     def get_read_schema(self) -> Type[CamelModel]:
         return self.read_schema
 
     def get_read_many_schema(self) -> Type[CamelModel]:
         return self.read_many_schema
```

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/routers/exceptions.py` & `fastapi_all_out-0.4.0/fastapi_all_out/routers/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/routers/utils.py` & `fastapi_all_out-0.4.0/fastapi_all_out/routers/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/base.py` & `fastapi_all_out-0.4.0/fastapi_all_out/routers/filters/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/bool.py` & `fastapi_all_out-0.4.0/fastapi_all_out/routers/filters/bool.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/int.py` & `fastapi_all_out-0.4.0/fastapi_all_out/routers/filters/int.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/int_btw.py` & `fastapi_all_out-0.4.0/fastapi_all_out/routers/filters/int_btw.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/str.py` & `fastapi_all_out-0.4.0/fastapi_all_out/routers/filters/str.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/templates/activation.html` & `fastapi_all_out-0.4.0/fastapi_all_out/templates/activation.html`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/templates/email_change.html` & `fastapi_all_out-0.4.0/fastapi_all_out/templates/email_change.html`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/fastapi_all_out/templates/password_reset.html` & `fastapi_all_out-0.4.0/fastapi_all_out/templates/password_reset.html`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/LICENSE.md` & `fastapi_all_out-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.3.0/pyproject.toml` & `fastapi_all_out-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.hatch.build]
 ignore-vcs = true
 include = ["fastapi_all_out"]
 
 [project]
 name = "fastapi-all-out"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="Alexandr Tamrazov", email="alta77@mail.ru" },
 ]
 maintainers = [
   { name="Alexandr Tamrazov", email="alta77@mail.ru" },
 ]
 keywords = ["DDD", "Domain-driven design", "Database", "WEB", "Architecture", "Backend"]
```

### Comparing `fastapi_all_out-0.3.0/PKG-INFO` & `fastapi_all_out-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-all-out
-Version: 0.3.0
+Version: 0.4.0
 Summary: Makes fastapi much easier and stronger, then Django
 Project-URL: Github, https://github.com/alta7700/fastapi_all_out/
 Author-email: Alexandr Tamrazov <alta77@mail.ru>
 Maintainer-email: Alexandr Tamrazov <alta77@mail.ru>
 License: Copyright © 2023 Alexandr Tamrazov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

