# Comparing `tmp/bl_hector-0.1.1.tar.gz` & `tmp/bl_hector-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bl_hector-0.1.1.tar", max compression
+gzip compressed data, was "bl_hector-0.1.2.tar", max compression
```

## Comparing `bl_hector-0.1.1.tar` & `bl_hector-0.1.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0    34523 2023-06-15 06:52:14.608155 bl_hector-0.1.1/LICENSE
--rw-r--r--   0        0        0     1854 2023-06-15 06:52:14.608155 bl_hector-0.1.1/README.md
--rw-r--r--   0        0        0      807 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/__init__.py
--rw-r--r--   0        0        0      721 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/application/__init__.py
--rw-r--r--   0        0        0      721 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/application/use_cases/__init__.py
--rw-r--r--   0        0        0     3803 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/application/use_cases/add_book.py
--rw-r--r--   0        0        0     2048 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/application/use_cases/display_book.py
--rw-r--r--   0        0        0     1975 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/application/use_cases/look_up_book.py
--rw-r--r--   0        0        0     3751 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/application/use_cases/search_books.py
--rw-r--r--   0        0        0     3801 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/application/use_cases/update_book.py
--rw-r--r--   0        0        0      944 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/configuration/__init__.py
--rw-r--r--   0        0        0      981 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/configuration/cli.py
--rw-r--r--   0        0        0      986 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/configuration/wsgi.py
--rw-r--r--   0        0        0      721 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/__init__.py
--rw-r--r--   0        0        0      721 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/administration/__init__.py
--rw-r--r--   0        0        0     1272 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/administration/entities.py
--rw-r--r--   0        0        0      808 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/administration/enumerations.py
--rw-r--r--   0        0        0     1659 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/administration/repositories.py
--rw-r--r--   0        0        0     1196 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/administration/services.py
--rw-r--r--   0        0        0      931 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/administration/value_objects.py
--rw-r--r--   0        0        0      721 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/collection_management/__init__.py
--rw-r--r--   0        0        0     1563 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/collection_management/entities.py
--rw-r--r--   0        0        0      996 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/collection_management/errors.py
--rw-r--r--   0        0        0     1509 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/collection_management/repositories.py
--rw-r--r--   0        0        0     1173 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/collection_management/services.py
--rw-r--r--   0        0        0     1800 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/collection_management/validators.py
--rw-r--r--   0        0        0     3325 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/domain/collection_management/value_objects.py
--rw-r--r--   0        0        0     1453 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/__init__.py
--rw-r--r--   0        0        0     3738 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/__init__.py
--rw-r--r--   0        0        0     1064 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/aliases/__init__.py
--rw-r--r--   0        0        0     1693 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/auth/__init__.py
--rw-r--r--   0        0        0     4116 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/books/__init__.py
--rw-r--r--   0        0        0     3466 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/services.py
--rw-r--r--   0        0        0   207302 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
--rw-r--r--   0        0        0    73117 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
--rw-r--r--   0        0        0      664 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/css/hector.css
--rw-r--r--   0        0        0      655 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/favicon.svg
--rw-r--r--   0        0        0     1502 2023-06-15 06:52:14.608155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
--rw-r--r--   0        0        0    42819 2023-06-15 06:52:14.612155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
--rw-r--r--   0        0        0    97249 2023-06-15 06:52:14.612155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
--rw-r--r--   0        0        0     6828 2023-06-15 06:52:14.612155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
--rw-r--r--   0        0        0   186112 2023-06-15 06:52:14.612155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   107460 2023-06-15 06:52:14.612155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    62048 2023-06-15 06:52:14.612155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25096 2023-06-15 06:52:14.612155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   397728 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   150472 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     2363 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/flask/totp/__init__.py
--rw-r--r--   0        0        0     1265 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/flask/utils.py
--rw-r--r--   0        0        0     4544 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/flask/webauthn/__init__.py
--rw-r--r--   0        0        0     3282 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/flask/webauthn/security.py
--rw-r--r--   0        0        0     1789 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/isbnlib/__init__.py
--rw-r--r--   0        0        0     1729 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/requests/__init__.py
--rw-r--r--   0        0        0     2615 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/settings.py
--rw-r--r--   0        0        0      721 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     8336 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/sqlalchemy/repositories.py
--rw-r--r--   0        0        0     2058 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/typer/__init__.py
--rw-r--r--   0        0        0     2886 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/typer/books.py
--rw-r--r--   0        0        0     2099 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/infrastructure/typer/services.py
--rw-r--r--   0        0        0     1845 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/interfaces/__init__.py
--rw-r--r--   0        0        0      761 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/interfaces/exceptions.py
--rw-r--r--   0        0        0     3371 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/interfaces/from_dict.py
--rw-r--r--   0        0        0     1659 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/interfaces/from_json.py
--rw-r--r--   0        0        0     1435 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/interfaces/l10n/__init__.py
--rw-r--r--   0        0        0     4792 2023-06-15 13:06:54.302159 bl_hector-0.1.1/bl_hector/interfaces/l10n/en-GB/main.ftl
--rw-r--r--   0        0        0     5330 2023-06-15 13:06:54.302159 bl_hector-0.1.1/bl_hector/interfaces/l10n/fr-FR/main.ftl
--rw-r--r--   0        0        0     1407 2023-06-15 06:52:14.616155 bl_hector-0.1.1/bl_hector/interfaces/to_http/__init__.py
--rw-r--r--   0        0        0    14758 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/__init__.py
--rw-r--r--   0        0        0     1247 2023-06-15 13:06:54.302159 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
--rw-r--r--   0        0        0     4296 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
--rw-r--r--   0        0        0     2100 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
--rw-r--r--   0        0        0     2043 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug
--rw-r--r--   0        0        0     5727 2023-06-15 13:06:54.302159 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
--rw-r--r--   0        0        0     3589 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
--rw-r--r--   0        0        0      982 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/error.pug
--rw-r--r--   0        0        0     2028 2023-06-15 13:06:54.302159 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/layout.pug
--rw-r--r--   0        0        0     1127 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
--rw-r--r--   0        0        0     4129 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
--rw-r--r--   0        0        0     1992 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
--rw-r--r--   0        0        0     1678 2023-06-15 13:06:54.302159 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug
--rw-r--r--   0        0        0     2010 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
--rw-r--r--   0        0        0     2045 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
--rw-r--r--   0        0        0     1310 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_http/as_json/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_terminal/__init__.py
--rw-r--r--   0        0        0     1885 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_terminal/as_json.py
--rw-r--r--   0        0        0     5280 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/to_terminal/as_text.py
--rw-r--r--   0        0        0     1519 2023-06-15 06:52:14.620154 bl_hector-0.1.1/bl_hector/interfaces/utils.py
--rw-r--r--   0        0        0     1570 2023-06-15 13:06:54.302159 bl_hector-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4676 2023-06-15 13:07:06.618553 bl_hector-0.1.1/setup.py
--rw-r--r--   0        0        0     3048 2023-06-15 13:07:06.618820 bl_hector-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-14 14:53:28.100751 bl_hector-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1854 2023-06-14 14:53:28.100751 bl_hector-0.1.2/README.md
+-rw-r--r--   0        0        0      807 2023-06-14 14:53:28.100751 bl_hector-0.1.2/bl_hector/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.100751 bl_hector-0.1.2/bl_hector/application/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.100751 bl_hector-0.1.2/bl_hector/application/use_cases/__init__.py
+-rw-r--r--   0        0        0     3803 2023-06-14 14:53:28.100751 bl_hector-0.1.2/bl_hector/application/use_cases/add_book.py
+-rw-r--r--   0        0        0     2048 2023-06-14 14:53:28.100751 bl_hector-0.1.2/bl_hector/application/use_cases/display_book.py
+-rw-r--r--   0        0        0     1975 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/application/use_cases/look_up_book.py
+-rw-r--r--   0        0        0     3751 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/application/use_cases/search_books.py
+-rw-r--r--   0        0        0     3801 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/application/use_cases/update_book.py
+-rw-r--r--   0        0        0      944 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/configuration/__init__.py
+-rw-r--r--   0        0        0      981 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/configuration/cli.py
+-rw-r--r--   0        0        0      986 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/configuration/wsgi.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/administration/__init__.py
+-rw-r--r--   0        0        0     1272 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/administration/entities.py
+-rw-r--r--   0        0        0      808 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/administration/enumerations.py
+-rw-r--r--   0        0        0     1659 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/administration/repositories.py
+-rw-r--r--   0        0        0     1196 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/administration/services.py
+-rw-r--r--   0        0        0      931 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/administration/value_objects.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/collection_management/__init__.py
+-rw-r--r--   0        0        0     1563 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/collection_management/entities.py
+-rw-r--r--   0        0        0      996 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/collection_management/errors.py
+-rw-r--r--   0        0        0     1509 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/collection_management/repositories.py
+-rw-r--r--   0        0        0     1173 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/collection_management/services.py
+-rw-r--r--   0        0        0     1800 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/collection_management/validators.py
+-rw-r--r--   0        0        0     3325 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/collection_management/value_objects.py
+-rw-r--r--   0        0        0     1453 2023-06-14 14:53:28.108751 bl_hector-0.1.2/bl_hector/infrastructure/__init__.py
+-rw-r--r--   0        0        0     3982 2023-06-16 08:33:27.027305 bl_hector-0.1.2/bl_hector/infrastructure/flask/__init__.py
+-rw-r--r--   0        0        0     1064 2023-06-14 14:53:28.108751 bl_hector-0.1.2/bl_hector/infrastructure/flask/aliases/__init__.py
+-rw-r--r--   0        0        0     1693 2023-06-14 14:53:28.108751 bl_hector-0.1.2/bl_hector/infrastructure/flask/auth/__init__.py
+-rw-r--r--   0        0        0     4282 2023-06-16 08:55:18.414785 bl_hector-0.1.2/bl_hector/infrastructure/flask/books/__init__.py
+-rw-r--r--   0        0        0     3466 2023-06-14 14:53:28.108751 bl_hector-0.1.2/bl_hector/infrastructure/flask/services.py
+-rw-r--r--   0        0        0   207302 2023-06-14 14:53:28.108751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
+-rw-r--r--   0        0        0    73117 2023-06-14 14:53:28.112751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
+-rw-r--r--   0        0        0      664 2023-06-14 14:53:28.112751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/css/hector.css
+-rw-r--r--   0        0        0      655 2023-06-14 14:53:28.112751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/favicon.svg
+-rw-r--r--   0        0        0     1502 2023-06-14 14:53:28.112751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
+-rw-r--r--   0        0        0    42819 2023-06-14 14:53:28.112751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
+-rw-r--r--   0        0        0    97249 2023-06-14 14:53:28.112751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
+-rw-r--r--   0        0        0     6828 2023-06-14 14:53:28.112751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
+-rw-r--r--   0        0        0   186112 2023-06-14 14:53:28.116751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   107460 2023-06-14 14:53:28.116751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    62048 2023-06-14 14:53:28.116751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25096 2023-06-14 14:53:28.116751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   397728 2023-06-14 14:53:28.120751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   150472 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     2363 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/flask/totp/__init__.py
+-rw-r--r--   0        0        0     1265 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/flask/utils.py
+-rw-r--r--   0        0        0     4544 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/flask/webauthn/__init__.py
+-rw-r--r--   0        0        0     3282 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/flask/webauthn/security.py
+-rw-r--r--   0        0        0     1789 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/isbnlib/__init__.py
+-rw-r--r--   0        0        0     1729 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/requests/__init__.py
+-rw-r--r--   0        0        0     2615 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/settings.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     8336 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0     2058 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/typer/__init__.py
+-rw-r--r--   0        0        0     2886 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/typer/books.py
+-rw-r--r--   0        0        0     2099 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/typer/services.py
+-rw-r--r--   0        0        0     1845 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/interfaces/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/interfaces/exceptions.py
+-rw-r--r--   0        0        0     3371 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/interfaces/from_dict.py
+-rw-r--r--   0        0        0     1659 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/interfaces/from_json.py
+-rw-r--r--   0        0        0     1435 2023-06-14 14:53:28.128751 bl_hector-0.1.2/bl_hector/interfaces/l10n/__init__.py
+-rw-r--r--   0        0        0     4792 2023-06-16 06:26:43.520346 bl_hector-0.1.2/bl_hector/interfaces/l10n/en-GB/main.ftl
+-rw-r--r--   0        0        0     5330 2023-06-16 06:26:43.520346 bl_hector-0.1.2/bl_hector/interfaces/l10n/fr-FR/main.ftl
+-rw-r--r--   0        0        0     1407 2023-06-14 14:53:28.128751 bl_hector-0.1.2/bl_hector/interfaces/to_http/__init__.py
+-rw-r--r--   0        0        0    14822 2023-06-16 08:56:31.481861 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/__init__.py
+-rw-r--r--   0        0        0     1247 2023-06-16 06:26:43.520346 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
+-rw-r--r--   0        0        0     4288 2023-06-16 09:51:27.024346 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
+-rw-r--r--   0        0        0     2116 2023-06-16 09:56:40.596445 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
+-rw-r--r--   0        0        0     2043 2023-06-14 14:53:28.128751 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug
+-rw-r--r--   0        0        0     5680 2023-06-16 09:53:48.126592 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
+-rw-r--r--   0        0        0     3628 2023-06-16 09:55:40.101198 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
+-rw-r--r--   0        0        0      982 2023-06-14 14:53:28.128751 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/error.pug
+-rw-r--r--   0        0        0     2028 2023-06-16 06:26:43.520346 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/layout.pug
+-rw-r--r--   0        0        0     1127 2023-06-14 14:53:28.132751 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
+-rw-r--r--   0        0        0     4129 2023-06-14 14:53:28.132751 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
+-rw-r--r--   0        0        0     2008 2023-06-16 08:59:37.299508 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
+-rw-r--r--   0        0        0     1678 2023-06-16 06:26:43.524346 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug
+-rw-r--r--   0        0        0     2010 2023-06-14 14:53:28.132751 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
+-rw-r--r--   0        0        0     2045 2023-06-14 14:53:28.132751 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
+-rw-r--r--   0        0        0     1310 2023-06-14 14:53:28.132751 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_json/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-14 14:53:28.132751 bl_hector-0.1.2/bl_hector/interfaces/to_terminal/__init__.py
+-rw-r--r--   0        0        0     1885 2023-06-14 14:53:28.132751 bl_hector-0.1.2/bl_hector/interfaces/to_terminal/as_json.py
+-rw-r--r--   0        0        0     5280 2023-06-14 14:53:28.132751 bl_hector-0.1.2/bl_hector/interfaces/to_terminal/as_text.py
+-rw-r--r--   0        0        0     1519 2023-06-14 14:53:28.132751 bl_hector-0.1.2/bl_hector/interfaces/utils.py
+-rw-r--r--   0        0        0     1570 2023-06-16 10:00:00.357940 bl_hector-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4676 2023-06-16 10:00:45.217874 bl_hector-0.1.2/setup.py
+-rw-r--r--   0        0        0     3048 2023-06-16 10:00:45.218990 bl_hector-0.1.2/PKG-INFO
```

### Comparing `bl_hector-0.1.1/LICENSE` & `bl_hector-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/README.md` & `bl_hector-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/__init__.py` & `bl_hector-0.1.2/bl_hector/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/application/__init__.py` & `bl_hector-0.1.2/bl_hector/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/application/use_cases/__init__.py` & `bl_hector-0.1.2/bl_hector/application/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/application/use_cases/add_book.py` & `bl_hector-0.1.2/bl_hector/application/use_cases/add_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/application/use_cases/display_book.py` & `bl_hector-0.1.2/bl_hector/application/use_cases/display_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/application/use_cases/look_up_book.py` & `bl_hector-0.1.2/bl_hector/application/use_cases/look_up_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/application/use_cases/search_books.py` & `bl_hector-0.1.2/bl_hector/application/use_cases/search_books.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/application/use_cases/update_book.py` & `bl_hector-0.1.2/bl_hector/application/use_cases/update_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/configuration/__init__.py` & `bl_hector-0.1.2/bl_hector/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/configuration/cli.py` & `bl_hector-0.1.2/bl_hector/configuration/cli.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/configuration/wsgi.py` & `bl_hector-0.1.2/bl_hector/configuration/wsgi.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/domain/__init__.py` & `bl_hector-0.1.2/bl_hector/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/domain/administration/__init__.py` & `bl_hector-0.1.2/bl_hector/domain/administration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/domain/administration/entities.py` & `bl_hector-0.1.2/bl_hector/domain/administration/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/domain/administration/enumerations.py` & `bl_hector-0.1.2/bl_hector/domain/administration/enumerations.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/domain/administration/repositories.py` & `bl_hector-0.1.2/bl_hector/domain/administration/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/domain/administration/services.py` & `bl_hector-0.1.2/bl_hector/domain/administration/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/domain/administration/value_objects.py` & `bl_hector-0.1.2/bl_hector/domain/administration/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/domain/collection_management/__init__.py` & `bl_hector-0.1.2/bl_hector/domain/collection_management/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/domain/collection_management/entities.py` & `bl_hector-0.1.2/bl_hector/domain/collection_management/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/domain/collection_management/errors.py` & `bl_hector-0.1.2/bl_hector/domain/collection_management/errors.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/domain/collection_management/repositories.py` & `bl_hector-0.1.2/bl_hector/domain/collection_management/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/domain/collection_management/services.py` & `bl_hector-0.1.2/bl_hector/domain/collection_management/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/domain/collection_management/validators.py` & `bl_hector-0.1.2/bl_hector/domain/collection_management/validators.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/domain/collection_management/value_objects.py` & `bl_hector-0.1.2/bl_hector/domain/collection_management/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/__init__.py` & `bl_hector-0.1.2/bl_hector/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/__init__.py` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from http import HTTPStatus as HTTP
 from typing import Any
 
-from flask import Flask, g, get_flashed_messages, request, url_for
+from flask import Flask, Response, g, get_flashed_messages, request, url_for
 from werkzeug.middleware.proxy_fix import ProxyFix
 
 from bl_hector import __version__
 from bl_hector.infrastructure.flask import services
 from bl_hector.infrastructure.flask.aliases import blueprint as aliases
 from bl_hector.infrastructure.flask.auth import blueprint as auth
 from bl_hector.infrastructure.flask.books import blueprint as books
@@ -53,14 +53,20 @@
 
     @app.before_request
     def guess_locale() -> None:
         g.locale = (
             request.accept_languages.best_match(l10n.LOCALES) or l10n.DEFAULT_LOCALE
         )
 
+    @app.after_request
+    def disable_cache_for_htmx_requests(response: Response) -> Response:
+        if "Hx-Target" in request.headers:
+            response.headers["Cache-Control"] = "no-store, max-age=0"
+        return response
+
     @app.errorhandler(BadRequest)  # type: ignore[type-var]
     @presenter_to_response
     def handle_bad_request(e: Exception) -> Any:
         presenter = JinjaPresenter(
             "error",
             message="You submitted a bad request! This should have never happened!?",
         )
```

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/aliases/__init__.py` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/aliases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/auth/__init__.py` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/books/__init__.py` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/books/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 
 @blueprint.get("")
 @presenter_to_response
 def search() -> Any:
     presenter = presenters.SearchBooks(
         request.args,
-        fragment=request.headers.get("Hx-Target", ""),
+        fragment=request.headers.get("HX-Target", ""),
         user=services.get_user(),
     )
     interactor = search_books.Interactor(presenter, services.get_books())
     controller = controllers.SearchBooks(
         request.args, page_size=presenters.SearchBooks.PAGE_SIZE
     )
     controller.call(interactor)
@@ -59,15 +59,20 @@
 def add() -> Any:
     return presenters.AddBook(request.form, user=services.get_user())
 
 
 @blueprint.post("__new__")
 @presenter_to_response
 def add_POST() -> Any:
-    presenter = presenters.AddBook(request.form, notify=notify, user=services.get_user())
+    presenter = presenters.AddBook(
+        request.form,
+        notify=notify,
+        fragment=request.headers.get("HX-Target", ""),
+        user=services.get_user(),
+    )
     interactor = add_book.Interactor(
         presenter,
         services.get_books(),
         services.get_calendar(),
         services.get_permissions(),
     )
     controller = controllers.AddBook(request.form, str(services.get_user().id))
@@ -106,15 +111,19 @@
     return presenter
 
 
 @blueprint.post("<string:isbn>/__edit__")
 @presenter_to_response
 def update_POST(isbn: str) -> Any:
     presenter = presenters.UpdateBook(
-        isbn, request.form, notify=notify, user=services.get_user()
+        isbn,
+        request.form,
+        notify=notify,
+        fragment=request.headers.get("HX-Target", ""),
+        user=services.get_user(),
     )
     interactor = update_book.Interactor(
         presenter,
         services.get_books(),
         services.get_calendar(),
         services.get_permissions(),
     )
```

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/services.py` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/css/hector.css` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/css/hector.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/favicon.svg` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/totp/__init__.py` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/totp/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/utils.py` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/webauthn/__init__.py` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/webauthn/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/flask/webauthn/security.py` & `bl_hector-0.1.2/bl_hector/infrastructure/flask/webauthn/security.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/isbnlib/__init__.py` & `bl_hector-0.1.2/bl_hector/infrastructure/isbnlib/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/requests/__init__.py` & `bl_hector-0.1.2/bl_hector/infrastructure/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/settings.py` & `bl_hector-0.1.2/bl_hector/infrastructure/settings.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/sqlalchemy/__init__.py` & `bl_hector-0.1.2/bl_hector/infrastructure/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/sqlalchemy/repositories.py` & `bl_hector-0.1.2/bl_hector/infrastructure/sqlalchemy/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/typer/__init__.py` & `bl_hector-0.1.2/bl_hector/infrastructure/typer/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/typer/books.py` & `bl_hector-0.1.2/bl_hector/infrastructure/typer/books.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/infrastructure/typer/services.py` & `bl_hector-0.1.2/bl_hector/infrastructure/typer/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/__init__.py` & `bl_hector-0.1.2/bl_hector/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/exceptions.py` & `bl_hector-0.1.2/bl_hector/interfaces/exceptions.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/from_dict.py` & `bl_hector-0.1.2/bl_hector/interfaces/from_dict.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/from_json.py` & `bl_hector-0.1.2/bl_hector/interfaces/from_json.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/l10n/__init__.py` & `bl_hector-0.1.2/bl_hector/interfaces/l10n/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/l10n/en-GB/main.ftl` & `bl_hector-0.1.2/bl_hector/interfaces/l10n/en-GB/main.ftl`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/l10n/fr-FR/main.ftl` & `bl_hector-0.1.2/bl_hector/interfaces/l10n/fr-FR/main.ftl`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_http/__init__.py` & `bl_hector-0.1.2/bl_hector/interfaces/to_http/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/__init__.py` & `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,18 @@
     def error(self, message: str, status_code: HTTP) -> None:
         self.__error = message
         self.set_status_code(status_code)
 
     def redirect(self, url: str, status_code: HTTP = HTTP.SEE_OTHER) -> None:
         if "Content-Type" in self.__headers:
             del self.__headers["Content-Type"]
-        self.__headers["Location"] = url
+        if self.__fragment:
+            self.__headers["HX-Location"] = url
+        else:
+            self.__headers["Location"] = url
         self.set_status_code(status_code)
 
     def not_authorized(self) -> None:
         if self.__user:
             self.set_status_code(HTTP.FORBIDDEN)
             self.__error = self._("access-forbidden")
         else:
@@ -212,17 +215,17 @@
 class AddBook(JinjaPresenter, add_book.Presenter):
     def __init__(
         self,
         data: MultiDict[str, Any],
         /,
         *,
         notify: Callable[[str, str], None] = lambda m, t: None,
-        user: Optional[User] = None,
+        **kwargs: Any,
     ) -> None:
-        super().__init__("books/add", user=user)
+        super().__init__("books/add", **kwargs)
         self.set_status_code(HTTP.OK)
         self.__data = data
         self.__notify = notify
         self.__context: dict[str, Any] = {"errors": {}}
 
     def render(self, **context: Any) -> str:
         return super().render(**self.__context, **context, data=self.__data)
@@ -368,17 +371,17 @@
     def __init__(
         self,
         isbn: str,
         data: MultiDict[str, Any],
         /,
         *,
         notify: Callable[[str, str], None] = lambda m, t: None,
-        user: Optional[User] = None,
+        **kwargs: Any,
     ) -> None:
-        super().__init__("books/update", user=user)
+        super().__init__("books/update", **kwargs)
         self.set_status_code(HTTP.FORBIDDEN)
         self.__data = data
         self.__notify = notify
         self.__context: dict[str, Any] = {"isbn": isbn, "errors": {}}
 
     def render(self, **context: Any) -> str:
         return super().render(**self.__context, **context, data=self.__data)
```

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug` & `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/add.pug` & `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/add.pug`

 * *Files 2% similar despite different names*

```diff
@@ -39,65 +39,69 @@
     }
 
 block content
   section.section
     .container
       h1.title.is-3= _("add-book-title")
 
-      #form
-        block form
-          include mixins/form
-          form(method="POST")
-            .columns
-              .column.is-one-quarter
-                input#coverUploader.is-hidden(
-                  accept="image/*"
-                  type="file"
-                  _="on change set img to #cover then set inp to #coverInput then js(me, img, inp) loadIntoImage(me, img, inp)"
-                )
-                img#cover.cover.is-2by3(
-                  src="#{data.cover or url_for('static', filename='img/placeholders/320x480.png')}"
-                  alt="Book cover"
-                  title=_("add-book-cover-help")
-                  style="cursor: pointer"
-                  _="on click set target to #coverUploader js(target) target.click()"
-                )
-                input#coverInput.is-hidden(
-                  name="cover"
-                  type="text"
-                  value="#{data.cover}"
-                )
-              .column
-                block isbn
-                  .field.is-horizontal(_="on load remove @disabled from .button")
-                    .field-body
-                      include books/mixins/render_isbn
-                      +isbn_field(data.isbn, errors.isbn, required="1")
-
-                      .field.is-narrow
-                        p.control
-                          button.button.is-info(
-                            hx-post="#{url_for('books.look_up')}"
-                            hx-target="#form"
-                            disabled
-                            _="on htmx:beforeSend add .is-loading add @disabled"
-                          )
-                            span.icon: i.fas.fa-search
-                            span= _("search-books-action")
-
-                +text_field("title", data.title, errors.title, required="1", description=_("book-title-description"), icon="file", placeholder=_('book-title'))
-                +number_field("year", data.year, errors.year, required="1", description=_("book-year-description"), icon="calendar", placeholder=_('book-year'))
-                +text_field("authors", data.authors, errors.authors, required="1", description=_("book-authors-description"), icon="users", placeholder=_('book-authors'))
-                +text_field("genres", data.genres, errors.genres, description=_("book-genres-description"), icon="crown", placeholder=_('book-genres'))
-
-                .field
-                  p.control
-                    a.button.is-light(href="#{url_for('books.search')}")
-                      span.icon: i.fas.fa-times
-                      span= _("add-book-cancel")
-                    button.button.is-primary
-                      span.icon: i.fas.fa-plus
-                      span= _("add-book-add")
-
-          if error is defined
-            article.message.is-danger
-              .message-body= error
+      block form
+        include mixins/form
+        form#form(
+          method="POST"
+          action=""
+          hx-post=""
+          hx-target="#form"
+        )
+          .columns
+            .column.is-one-quarter
+              input#coverUploader.is-hidden(
+                accept="image/*"
+                type="file"
+                _="on change set img to #cover then set inp to #coverInput then js(me, img, inp) loadIntoImage(me, img, inp)"
+              )
+              img#cover.cover.is-2by3(
+                src="#{data.cover or url_for('static', filename='img/placeholders/320x480.png')}"
+                alt="Book cover"
+                title=_("add-book-cover-help")
+                style="cursor: pointer"
+                _="on click set target to #coverUploader js(target) target.click()"
+              )
+              input#coverInput.is-hidden(
+                name="cover"
+                type="text"
+                value="#{data.cover}"
+              )
+            .column
+              block isbn
+                .field.is-horizontal(_="on load remove @disabled from .button")
+                  .field-body
+                    include books/mixins/render_isbn
+                    +isbn_field(data.isbn, errors.isbn, required="1")
+
+                    .field.is-narrow
+                      p.control
+                        button.button.is-info(
+                          hx-post="#{url_for('books.look_up')}"
+                          hx-target="#form"
+                          disabled
+                          _="on htmx:beforeSend add .is-loading add @disabled"
+                        )
+                          span.icon: i.fas.fa-search
+                          span= _("search-books-action")
+
+              +text_field("title", data.title, errors.title, required="1", description=_("book-title-description"), icon="file", placeholder=_('book-title'))
+              +number_field("year", data.year, errors.year, required="1", description=_("book-year-description"), icon="calendar", placeholder=_('book-year'))
+              +text_field("authors", data.authors, errors.authors, required="1", description=_("book-authors-description"), icon="users", placeholder=_('book-authors'))
+              +text_field("genres", data.genres, errors.genres, description=_("book-genres-description"), icon="crown", placeholder=_('book-genres'))
+
+              .field
+                p.control
+                  a.button.is-light(href="#{url_for('books.search')}" hx-boost="true")
+                    span.icon: i.fas.fa-times
+                    span= _("add-book-cancel")
+                  button.button.is-primary
+                    span.icon: i.fas.fa-plus
+                    span= _("add-book-add")
+
+        if error is defined
+          article.message.is-danger
+            .message-body= error
```

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/display.pug` & `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/display.pug`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 block content
   section.section
     .container
       //- Fixes a spacing problem.
       .buttons.is-pulled-right(style="margin-bottom: -1rem")
         if user.can_update_book
-          a.button.is-link(href="#{url_for('books.update', isbn=book.isbn)}")
+          a.button.is-link(href="#{url_for('books.update', isbn=book.isbn)}" hx-boost="true")
             span.icon: i.fas.fa-edit
             span= _("update-book-action")
         else
           button.button.is-link.is-disabled(disabled title=_("update-book-requires-authentification"))
             span.icon: i.fas.fa-edit
             span= _("update-book-action")
```

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug` & `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/search.pug` & `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/search.pug`

 * *Files 5% similar despite different names*

```diff
@@ -20,108 +20,109 @@
   title= _("hector") + " – " + _("search-books-title")
 
 block content
   section.section
     .container
       .buttons.is-pulled-right
         if user.can_add_book
-          a.button.is-link(href="#{url_for('books.add')}")
+          a.button.is-link(href="#{url_for('books.add')}" hx-boost="true")
             span.icon: i.fas.fa-plus
             span= _("add-book-action")
         else
           button.button.is-link.is-disabled(disabled title=_("add-book-requires-authentification"))
             span.icon: i.fas.fa-plus
             span= _("add-book-action")
 
       h1.title.is-3= _("search-books-title")
 
-      #form
-        block form
-          include mixins/form
-          form(
-            method="GET"
-            action="#{url_for('books.search')}"
-            hx-target="#form"
-          )
-            +hidden_input("page", data.page or "1")
-
-            block isbn
-              include books/mixins/render_isbn
-              +isbn_field(data.isbn, errors.isbn)
-
-            +text_field("title", data.title, errors.title, description=_("book-title-description"), icon="file", placeholder=_('book-title'))
-            +number_field("year", data.year, errors.year, description=_("book-year-description"), icon="calendar", placeholder=_('book-year'))
-            +text_field("author", data.author, errors.author, description=_("book-author-description"), icon="users", placeholder=_('book-author'))
-            +text_field("genre", data.genre, errors.genre, description=_("book-genre-description"), icon="crown", placeholder=_('book-genre'))
-
-            .field
-              p.control
-                a.button.is-light(href="#{url_for('books.search')}")
-                  span.icon: i.fas.fa-trash
-                  span= _("search-books-clear")
-                button.button.is-primary(_="on click add .is-loading")
-                  span.icon: i.fas.fa-search
-                  span= _("search-books-search")
-
-          if books is defined
-            if books|length > 0
-              #books.books
-                block books
-                  mixin book_content(book)
-                    .card-content
-                      .media
-                        .media-left(style="width: 5em")
-                          figure.image.cover.is-2by3
-                            img(src="#{book.cover or url_for('static', filename='img/placeholders/320x480.png')}" alt="Book cover")
-                        .media-content
-                          h2.title.is-4(title="#{book.title}")= book.title|truncate(20)
-                          p.subtitle.is-6
-                            each author in book.authors
-                              if author == book.authors[-1]
-                                | #[a(href="#{url_for('books.search', author=author)}") #{author}]
+      block form
+        include mixins/form
+        form#form(
+          method="GET"
+          action="#{url_for('books.search')}"
+          hx-get="#{url_for('books.search')}"
+          hx-target="#form"
+          hx-push-url="true"
+        )
+          +hidden_input("page", data.page or "1")
+
+          block isbn
+            include books/mixins/render_isbn
+            +isbn_field(data.isbn, errors.isbn)
+
+          +text_field("title", data.title, errors.title, description=_("book-title-description"), icon="file", placeholder=_('book-title'))
+          +number_field("year", data.year, errors.year, description=_("book-year-description"), icon="calendar", placeholder=_('book-year'))
+          +text_field("author", data.author, errors.author, description=_("book-author-description"), icon="users", placeholder=_('book-author'))
+          +text_field("genre", data.genre, errors.genre, description=_("book-genre-description"), icon="crown", placeholder=_('book-genre'))
+
+          .field
+            p.control
+              a.button.is-light(href="#{url_for('books.search')}" hx-boost="true" hx-target="body")
+                span.icon: i.fas.fa-trash
+                span= _("search-books-clear")
+              button.button.is-primary(_="on click add .is-loading")
+                span.icon: i.fas.fa-search
+                span= _("search-books-search")
+
+        if books is defined
+          if books|length > 0
+            #books.books
+              block books
+                mixin book_content(book)
+                  .card-content
+                    .media
+                      .media-left(style="width: 5em")
+                        figure.image.cover.is-2by3
+                          img(src="#{book.cover or url_for('static', filename='img/placeholders/320x480.png')}" alt="Book cover")
+                      .media-content
+                        h2.title.is-4(title="#{book.title}")= book.title|truncate(20)
+                        p.subtitle.is-6
+                          each author in book.authors
+                            if author == book.authors[-1]
+                              | #[a(href="#{url_for('books.search', author=author)}") #{author}]
+                            else
+                              | #[a(href="#{url_for('books.search', author=author)}") #{author}], 
+                        p
+                          small
+                            | #[time(datetime="#{book.year}-01-01") #{book.year}] / 
+                            a(href="#{url_for('books.display', isbn=book.isbn)}") #{book.isbn}
+                            br
+                            each genre in book.genres
+                              if genre == book.genres[-1]
+                                | #[a(href="#{url_for('books.search', genre=genre)}") #{genre}]
                               else
-                                | #[a(href="#{url_for('books.search', author=author)}") #{author}], 
-                          p
-                            small
-                              | #[time(datetime="#{book.year}-01-01") #{book.year}] / 
-                              a(href="#{url_for('books.display', isbn=book.isbn)}") #{book.isbn}
-                              br
-                              each genre in book.genres
-                                if genre == book.genres[-1]
-                                  | #[a(href="#{url_for('books.search', genre=genre)}") #{genre}]
-                                else
-                                  | #[a(href="#{url_for('books.search', genre=genre)}") #{genre}], 
-
-                  each book in books
-                    if loop.last
-                      article.book.card(
-                        hx-get=next_page_url
-                        hx-trigger="revealed"
-                        hx-swap="beforeend"
-                        hx-target="#books"
-                        hx-indicator="#indicator"
-                      )
-                        +book_content(book)
-                    else
-                      article.book.card
-                        +book_content(book)
-
-              #indicator.buttons.is-centered.mt-3.htmx-indicator.is-hidden(_="on load remove .is-hidden")
-                  button.button.is-white.is-loading Loading indicator
-
-              if previous_page_url or next_page_url:
-                .buttons.is-centered.mt-3(_="on load remove me")
-                  if previous_page_url:
-                    a#previous-page.button.is-link(href="#{previous_page_url}")
-                      span.icon: i.fa.fa-step-backward
-                      span= _("search-books-previous-page")
-                  if next_page_url:
-                    a#next-page.button.is-link(href="#{next_page_url}")
-                      span= _("search-books-next-page")
-                      span.icon: i.fa.fa-step-forward
-            else
-              article.message.is-info
-                .message-body= _("search-books-no-result")
-
-          if error is defined
-            article.message.is-danger
-              .message-body= error
+                                | #[a(href="#{url_for('books.search', genre=genre)}") #{genre}], 
+
+                each book in books
+                  if loop.last
+                    article.book.card(
+                      hx-get=next_page_url
+                      hx-trigger="revealed"
+                      hx-swap="beforeend"
+                      hx-target="#books"
+                      hx-indicator="#indicator"
+                    )
+                      +book_content(book)
+                  else
+                    article.book.card
+                      +book_content(book)
+
+            #indicator.buttons.is-centered.mt-3.htmx-indicator.is-hidden(_="on load remove .is-hidden")
+                button.button.is-white.is-loading Loading indicator
+
+            if previous_page_url or next_page_url:
+              .buttons.is-centered.mt-3(_="on load remove me")
+                if previous_page_url:
+                  a#previous-page.button.is-link(href="#{previous_page_url}")
+                    span.icon: i.fa.fa-step-backward
+                    span= _("search-books-previous-page")
+                if next_page_url:
+                  a#next-page.button.is-link(href="#{next_page_url}")
+                    span= _("search-books-next-page")
+                    span.icon: i.fa.fa-step-forward
+          else
+            article.message.is-info
+              .message-body= _("search-books-no-result")
+
+        if error is defined
+          article.message.is-danger
+            .message-body= error
```

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/books/update.pug` & `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/update.pug`

 * *Files 9% similar despite different names*

```diff
@@ -39,48 +39,52 @@
     }
 
 block content
   section.section
     .container
       h1.title.is-3= _("update-book-title", isbn=isbn)
 
-      #form
-        block form
-          include mixins/form
-          form(method="POST")
-            .columns
-              .column.is-one-quarter
-                input#coverUploader.is-hidden(
-                  accept="image/*"
-                  type="file"
-                  _="on change set img to #cover then set inp to #coverInput then js(me, img, inp) loadIntoImage(me, img, inp)"
-                )
-                img#cover.cover.is-2by3(
-                  src="#{data.cover or url_for('static', filename='img/placeholders/320x480.png')}"
-                  alt="Book cover"
-                  title=_("update-book-cover-help")
-                  style="cursor: pointer"
-                  _="on click set target to #coverUploader js(target) target.click()"
-                )
-                input#coverInput.is-hidden(
-                  name="cover"
-                  type="text"
-                  value="#{data.cover}"
-                )
-              .column
-                +text_field("title", data.title, errors.title, required="1", description=_("book-title-description"), icon="file", placeholder=_('book-title'))
-                +number_field("year", data.year, errors.year, required="1", description=_("book-year-description"), icon="calendar", placeholder=_('book-year'))
-                +text_field("authors", data.authors, errors.authors, required="1", description=_("book-authors-description"), icon="users", placeholder=_('book-authors'))
-                +text_field("genres", data.genres, errors.genres, description=_("book-genres-description"), icon="crown", placeholder=_('book-genres'))
+      block form
+        include mixins/form
+        form#form(
+          method="POST"
+          action=""
+          hx-post=""
+          hx-target="#form"
+        )
+          .columns
+            .column.is-one-quarter
+              input#coverUploader.is-hidden(
+                accept="image/*"
+                type="file"
+                _="on change set img to #cover then set inp to #coverInput then js(me, img, inp) loadIntoImage(me, img, inp)"
+              )
+              img#cover.cover.is-2by3(
+                src="#{data.cover or url_for('static', filename='img/placeholders/320x480.png')}"
+                alt="Book cover"
+                title=_("update-book-cover-help")
+                style="cursor: pointer"
+                _="on click set target to #coverUploader js(target) target.click()"
+              )
+              input#coverInput.is-hidden(
+                name="cover"
+                type="text"
+                value="#{data.cover}"
+              )
+            .column
+              +text_field("title", data.title, errors.title, required="1", description=_("book-title-description"), icon="file", placeholder=_('book-title'))
+              +number_field("year", data.year, errors.year, required="1", description=_("book-year-description"), icon="calendar", placeholder=_('book-year'))
+              +text_field("authors", data.authors, errors.authors, required="1", description=_("book-authors-description"), icon="users", placeholder=_('book-authors'))
+              +text_field("genres", data.genres, errors.genres, description=_("book-genres-description"), icon="crown", placeholder=_('book-genres'))
 
-                .field
-                  p.control
-                    a.button.is-light(href="#{url_for('books.display', isbn=data.isbn)}")
-                      span.icon: i.fas.fa-times
-                      span= _("update-book-cancel")
-                    button.button.is-primary
-                      span.icon: i.fas.fa-plus
-                      span= _("update-book-update")
+              .field
+                p.control
+                  a.button.is-light(href="#{url_for('books.display', isbn=data.isbn)}" hx-boost="true" hx-target="body")
+                    span.icon: i.fas.fa-times
+                    span= _("update-book-cancel")
+                  button.button.is-primary
+                    span.icon: i.fas.fa-plus
+                    span= _("update-book-update")
 
-          if error is defined
-            article.message.is-danger
-              .message-body= error
+        if error is defined
+          article.message.is-danger
+            .message-body= error
```

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/error.pug` & `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/error.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/layout.pug` & `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/layout.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug` & `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug` & `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug` & `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 //- MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 //- GNU Affero General Public License for more details.
 //-
 //- You should have received a copy of the GNU Affero General Public License
 //- along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 mixin navbar()
-  nav.navbar(role="navigation" aria-label="main navigation")
+  nav.navbar(role="navigation" aria-label="main navigation" hx-boost="true")
     .container
       .navbar-brand
         a.navbar-item.is-size-5.has-text-weight-semibold(href="#{url_for('aliases.root')}")= _("hector")
         a.navbar-burger(
           role="button"
           aria-label="menu"
           aria-expanded="false"
```

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug` & `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug` & `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug` & `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_http/as_json/__init__.py` & `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_json/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_terminal/__init__.py` & `bl_hector-0.1.2/bl_hector/interfaces/to_terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_terminal/as_json.py` & `bl_hector-0.1.2/bl_hector/interfaces/to_terminal/as_json.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/to_terminal/as_text.py` & `bl_hector-0.1.2/bl_hector/interfaces/to_terminal/as_text.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/bl_hector/interfaces/utils.py` & `bl_hector-0.1.2/bl_hector/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.1/pyproject.toml` & `bl_hector-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bl_hector"
-version = "0.1.1"
+version = "0.1.2"
 description = "A collection manager."
 authors = ["Tanguy Le Carrour <tanguy@bioneland.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://git.easter-eggs.org/bioneland/hector"
 
 exclude = [
```

### Comparing `bl_hector-0.1.1/setup.py` & `bl_hector-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 {'totp': ['pyotp>=2.8.0,<3.0.0'], 'webauthn': ['webauthn>=1.8.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['hector = bl_hector.configuration.cli:cli']}
 
 setup_kwargs = {
     'name': 'bl-hector',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A collection manager.',
     'long_description': '# Hector — a collection manager\n\n## Install\n\nHector is available on PyPI under the name `bl_hector`.\nTo install, just run `python -m pip install bl_hector`.\n\n\n## Configure\n\nHector is configured using environment variables.\nSee [the `settings` module](bl_hector/infrastructure/settings.py) for\na comprehensive list of configuration variables.\n\nAll the variable names must be prefixed with `HECTOR_`. For instance\xa0:\n\n```console\n# The secret can be generated using the `secrets.token_hex()` function.\n$ export HECTOR_SECRET_KEY="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"\n\n# Additional Python database drivers might be required depending on the DSN.\n$ export HECTOR_DSN="sqlite:///data.sqlite"\n```\n\n\n## Authentication\n\nTo enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)\nand enable it explicitly:\n\n```console\n$ export HECTOR_WEBAUTHN_ENABLED=1\n```\n\nTOTP authentication is provided to be able to login on servers that do not (yet) support\nthe `cryptography` module. You must install extra dependencies (`bl-hector[totp]`)\nand enable it explicitly by setting a base32 random secret:\n\n```console\n# The secret can be generated using the `pyotp.random_base32()` function.\n$ export HECTOR_TOTP_SECRET=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX\n```\n\nNote that it is a highly insecure way of authenticating, as anyone gaining access to your\nOTP generator would be able to login.\n\n\n## Initialise\n\nOnce configured, you must initialise Hector\'s database with the dedicated command:\n\n```console\n$ hector init-db\n```\n\n\n## Run\n\nHector being a Flask application, it can be run using any WSGI server,\nfor instance, with [Gunicorn](https://gunicorn.org):\n\n```console\n$ gunicorn --access-logfile="-" -w 4 -b 127.0.0.1:3000 "bl_hector.configuration.wsgi:app()"\n```\n\n\n## Contributing\n\nSee [CONTRIBUTING.md]() to set up a development environment.\n',
     'author': 'Tanguy Le Carrour',
     'author_email': 'tanguy@bioneland.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://git.easter-eggs.org/bioneland/hector',
```

### Comparing `bl_hector-0.1.1/PKG-INFO` & `bl_hector-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bl-hector
-Version: 0.1.1
+Version: 0.1.2
 Summary: A collection manager.
 Home-page: https://git.easter-eggs.org/bioneland/hector
 License: AGPL-3.0-or-later
 Author: Tanguy Le Carrour
 Author-email: tanguy@bioneland.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

