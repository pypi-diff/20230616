# Comparing `tmp/rpa_cooperativa-1.0.55.tar.gz` & `tmp/rpa_cooperativa-1.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.55.tar", last modified: Thu Jun  1 16:55:33 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.56.tar", last modified: Fri Jun 16 13:27:15 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.55.tar` & `rpa_cooperativa-1.0.56.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 16:55:33.933443 rpa_cooperativa-1.0.55/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.55/LICENSE
--rw-rw-rw-   0        0        0     6875 2023-06-01 16:55:33.928457 rpa_cooperativa-1.0.55/PKG-INFO
--rw-rw-rw-   0        0        0     5730 2023-05-19 18:58:05.000000 rpa_cooperativa-1.0.55/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 16:55:33.683986 rpa_cooperativa-1.0.55/rpa_coop/
--rw-rw-rw-   0        0        0      585 2023-05-22 15:25:02.000000 rpa_cooperativa-1.0.55/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 16:55:33.868452 rpa_cooperativa-1.0.55/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.55/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.55/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.55/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.55/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.55/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.55/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.55/rpa_coop/img/siac_branco.PNG
--rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.55/rpa_coop/img/siat_amarelo.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.55/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.55/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.55/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0    87333 2023-06-01 16:51:46.000000 rpa_cooperativa-1.0.55/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-06-01 16:55:33.918993 rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6875 2023-06-01 16:55:32.000000 rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-06-01 16:55:33.000000 rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 16:55:32.000000 rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-01 16:55:32.000000 rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      559 2023-06-01 16:55:32.000000 rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 16:55:32.000000 rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 16:55:33.935447 rpa_cooperativa-1.0.55/setup.cfg
--rw-rw-rw-   0        0        0     2325 2023-06-01 16:53:22.000000 rpa_cooperativa-1.0.55/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 13:27:15.467083 rpa_cooperativa-1.0.56/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.56/LICENSE
+-rw-rw-rw-   0        0        0     6875 2023-06-16 13:27:15.464563 rpa_cooperativa-1.0.56/PKG-INFO
+-rw-rw-rw-   0        0        0     5730 2023-05-19 18:58:05.000000 rpa_cooperativa-1.0.56/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 13:27:15.230706 rpa_cooperativa-1.0.56/rpa_coop/
+-rw-rw-rw-   0        0        0      585 2023-05-22 15:25:02.000000 rpa_cooperativa-1.0.56/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 13:27:15.420188 rpa_cooperativa-1.0.56/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.56/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.56/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.56/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.56/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.56/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.56/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.56/rpa_coop/img/siac_branco.PNG
+-rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.56/rpa_coop/img/siat_amarelo.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.56/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.56/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.56/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0    87556 2023-06-16 13:17:06.000000 rpa_cooperativa-1.0.56/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-06-16 13:27:15.458887 rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6875 2023-06-16 13:27:14.000000 rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-06-16 13:27:14.000000 rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 13:27:14.000000 rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-16 13:27:14.000000 rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      567 2023-06-16 13:27:14.000000 rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-16 13:27:14.000000 rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 13:27:15.468601 rpa_cooperativa-1.0.56/setup.cfg
+-rw-rw-rw-   0        0        0     2336 2023-06-16 13:09:25.000000 rpa_cooperativa-1.0.56/setup.py
```

### Comparing `rpa_cooperativa-1.0.55/LICENSE` & `rpa_cooperativa-1.0.56/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.55/PKG-INFO` & `rpa_cooperativa-1.0.56/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.55
+Version: 1.0.56
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.55/README.md` & `rpa_cooperativa-1.0.56/README.md`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.55/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.56/rpa_coop/__init__.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.55/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.56/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.55/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.56/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.55/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.56/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.55/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.56/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.55/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.56/rpa_coop/rpa_coop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1396,15 +1396,15 @@
             self.p.sleep(1)
             self.p.typewrite(letras[6])
             self.p.sleep(1)
         else:
             print('ops funcao entende apenas 2, 3, 4, 5, 6 ou 7 letras')
             
                   
-    def get_text(self, ini_linha=22, fim_linha=632, topo1=410, topo2=415, nome_janela=None):
+    def get_text(self, ini_linha: int=22, fim_linha: int=632, topo1: int=410, topo2: int=415, tempo_arrastar_soltar: float=1.5, nome_janela: str | None=None):
         ''' acc.get_text('Retorna ao Sistema')\n
          acc.get_text('Retorna ao Sistema', nome_janela = 'sacg')'''
         time.sleep(1)
         nome_janela = str(nome_janela).upper()
         if nome_janela == 'SIAT':
             janela = self.janela_siat
         elif nome_janela == 'SIAC':
@@ -1414,35 +1414,36 @@
         else:
             janela = self.p.getWindowsWithTitle('teoff-exe')[0]
   
         time.sleep(1)
         janela.activate()
         self.p.moveTo(janela.left + ini_linha, janela.top + topo1)
         self.p.sleep(1)
-        self.p.dragTo(janela.left + fim_linha, janela.top + topo2, 1.5, button='left')
+        self.p.dragTo(janela.left + fim_linha, janela.top + topo2, tempo_arrastar_soltar, button='left')
         self.p.moveTo(janela.left + ini_linha, janela.top + topo2)
         self.p.rightClick()
         capturado = self.pyperclip.paste()
         print(f'texto capturado:{capturado}')
         return capturado            
             
             
-    def exist_text(self, texto_esperado, max_tentativas=7, segundos_entre_tentativas=3, ini_linha=22, fim_linha=632, topo1=412, topo2=412, continua_seerro=False, nome_janela=None):
+     
+    def exist_text(self, texto_esperado: str, max_tentativas: int=7, segundos_entre_tentativas: int=3, ini_linha: int=22, fim_linha: int=632, topo1: int=412, topo2: int=412, tempo_arrastar_soltar: float=1.5, continua_seerro: bool=False, nome_janela: str |None=None):
         ''' acc.exist_text('Retorna ao Sistema')\n
          acc.exist_text('Retorna ao Sistema', nome_janela = 'sacg')'''
         time.sleep(1)
         self.pyperclip.copy('')
         tentativas = 0
         time.sleep(1)
-        captura = self.get_text(ini_linha, fim_linha, topo1, topo2, nome_janela = nome_janela)
+        captura = self.get_text(ini_linha, fim_linha, topo1, topo2, tempo_arrastar_soltar, nome_janela = nome_janela)
         resultado = True
         while not texto_esperado in captura and tentativas < max_tentativas:
             print('esperando texto: ', texto_esperado)
             self.p.sleep(segundos_entre_tentativas)
-            captura = self.get_text(ini_linha, fim_linha, topo1, topo2, nome_janela = nome_janela)
+            captura = self.get_text(ini_linha, fim_linha, topo1, topo2, tempo_arrastar_soltar, nome_janela = nome_janela)
             tentativas += 1
             if tentativas == max_tentativas:
                 resultado = False
         print(resultado)
         if resultado == False and continua_seerro == False:
             raise Exception(f'Execução pausada. O texto: "{texto_esperado}" não foi localizado durante a execução do robô.')
         return resultado
```

### Comparing `rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.55
+Version: 1.0.56
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.56/rpa_cooperativa.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 mysql-connector-python==8.0.28
 pymysql
 pyodbc
 sqlalchemy==1.4.37
 psycopg2
 psycopg2-binary
 denodo-sqlalchemy
+pymssql
 pillow
 requests>=2.28.1
 urllib3>=1.26.9
 certifi>=2022.5.18.1
 pyopenssl>=22.0.0
 idna>=3.3
 charset-normalizer>=2.0.12
```

### Comparing `rpa_cooperativa-1.0.55/setup.py` & `rpa_cooperativa-1.0.56/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.55",
+    version="1.0.56",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
@@ -34,13 +34,13 @@
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Topic :: Software Development :: Libraries :: Python Modules"
     ],
     python_requires='>=3.8',
     install_requires=['wheel', 'pandas', 'openpyxl', 'cryptography', 'xlsxwriter', 'xlrd', 'openpyxl','selenium', 'webdriver_manager', 'easygui', 'pyperclip', 'mysql-connector-python==8.0.28',
-                      'pymysql', 'pyodbc', 'sqlalchemy==1.4.37', 'psycopg2', 'psycopg2-binary', 'denodo-sqlalchemy', 'pillow', 'requests>=2.28.1', 'urllib3>=1.26.9', 
+                      'pymysql', 'pyodbc', 'sqlalchemy==1.4.37', 'psycopg2', 'psycopg2-binary', 'denodo-sqlalchemy', 'pymssql', 'pillow', 'requests>=2.28.1', 'urllib3>=1.26.9', 
                       'certifi>=2022.5.18.1', 'pyopenssl>=22.0.0', 'idna>=3.3', 'charset-normalizer>=2.0.12', 'pyautogui',
                       'pyrect', 'pyscreeze', 'pytz', 'graypy', 'reportlab', 'psutil', 'requests-html', 'paramiko','opencv-python',
                       'pytesseract', 'xmltodict', 'pywin32', 'pywinauto', 'beautifulsoup4', 'mechanize', 'matplotlib', 
                       'Unidecode', 'WMI', 'tabulate', 'python-dateutil>=2.8.2', 'secure-smtplib']
 )
```

