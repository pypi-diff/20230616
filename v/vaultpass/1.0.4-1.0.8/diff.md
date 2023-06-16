# Comparing `tmp/vaultpass-1.0.4.tar.gz` & `tmp/vaultpass-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vaultpass-1.0.4.tar", last modified: Tue Apr  4 23:51:17 2023, max compression
+gzip compressed data, was "dist/vaultpass-1.0.8.tar", last modified: Fri Jun 16 19:19:06 2023, max compression
```

## Comparing `vaultpass-1.0.4.tar` & `vaultpass-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-x---   0 mjstew   (99386308) mcomm      (985)        0 2023-04-04 23:51:17.000000 vaultpass-1.0.4/
--rw-r-----   0 mjstew   (99386308) mcomm      (985)      709 2023-04-04 23:51:17.000000 vaultpass-1.0.4/PKG-INFO
-drwxr-x---   0 mjstew   (99386308) mcomm      (985)        0 2023-04-04 23:51:17.000000 vaultpass-1.0.4/scripts/
--rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)     9492 2023-04-04 23:50:11.000000 vaultpass-1.0.4/scripts/vaultpass.py
--rw-r-----   0 mjstew   (99386308) mcomm      (985)       38 2023-04-04 23:51:17.000000 vaultpass-1.0.4/setup.cfg
--rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)     1026 2023-04-04 23:51:14.000000 vaultpass-1.0.4/setup.py
-drwxr-x---   0 mjstew   (99386308) mcomm      (985)        0 2023-04-04 23:51:17.000000 vaultpass-1.0.4/vaultpass/
--rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)      306 2023-04-04 23:51:14.000000 vaultpass-1.0.4/vaultpass/__init__.py
--rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)     9492 2023-04-04 23:50:11.000000 vaultpass-1.0.4/vaultpass/vaultpass.py
-drwxr-x---   0 mjstew   (99386308) mcomm      (985)        0 2023-04-04 23:51:17.000000 vaultpass-1.0.4/vaultpass.egg-info/
--rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)      709 2023-04-04 23:51:17.000000 vaultpass-1.0.4/vaultpass.egg-info/PKG-INFO
--rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)      238 2023-04-04 23:51:17.000000 vaultpass-1.0.4/vaultpass.egg-info/SOURCES.txt
--rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)        1 2023-04-04 23:51:17.000000 vaultpass-1.0.4/vaultpass.egg-info/dependency_links.txt
--rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)       97 2023-04-04 23:51:17.000000 vaultpass-1.0.4/vaultpass.egg-info/requires.txt
--rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)       10 2023-04-04 23:51:17.000000 vaultpass-1.0.4/vaultpass.egg-info/top_level.txt
+drwx------   0 mjstew   (99386308) mcomm      (985)        0 2023-06-16 19:19:06.000000 vaultpass-1.0.8/
+-rw-------   0 mjstew   (99386308) mcomm      (985)      731 2023-06-16 19:19:06.000000 vaultpass-1.0.8/PKG-INFO
+drwx------   0 mjstew   (99386308) mcomm      (985)        0 2023-06-16 19:19:06.000000 vaultpass-1.0.8/scripts/
+-rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)     9372 2023-04-15 17:06:35.000000 vaultpass-1.0.8/scripts/vaultpass.py
+-rw-------   0 mjstew   (99386308) mcomm      (985)       38 2023-06-16 19:19:06.000000 vaultpass-1.0.8/setup.cfg
+-rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)     1105 2023-06-16 19:19:03.000000 vaultpass-1.0.8/setup.py
+drwx------   0 mjstew   (99386308) mcomm      (985)        0 2023-06-16 19:19:06.000000 vaultpass-1.0.8/vaultpass/
+-rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)      322 2023-06-16 19:19:03.000000 vaultpass-1.0.8/vaultpass/__init__.py
+-rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)     9492 2023-04-04 23:50:11.000000 vaultpass-1.0.8/vaultpass/vaultpass.py
+drwx------   0 mjstew   (99386308) mcomm      (985)        0 2023-06-16 19:19:06.000000 vaultpass-1.0.8/vaultpass.egg-info/
+-rw-------   0 mjstew   (99386308) mcomm      (985)      731 2023-06-16 19:19:06.000000 vaultpass-1.0.8/vaultpass.egg-info/PKG-INFO
+-rw-------   0 mjstew   (99386308) mcomm      (985)      238 2023-06-16 19:19:06.000000 vaultpass-1.0.8/vaultpass.egg-info/SOURCES.txt
+-rw-------   0 mjstew   (99386308) mcomm      (985)        1 2023-06-16 19:19:06.000000 vaultpass-1.0.8/vaultpass.egg-info/dependency_links.txt
+-rw-------   0 mjstew   (99386308) mcomm      (985)      142 2023-06-16 19:19:06.000000 vaultpass-1.0.8/vaultpass.egg-info/requires.txt
+-rw-------   0 mjstew   (99386308) mcomm      (985)       10 2023-06-16 19:19:06.000000 vaultpass-1.0.8/vaultpass.egg-info/top_level.txt
```

### Comparing `vaultpass-1.0.4/PKG-INFO` & `vaultpass-1.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.1
 Name: vaultpass
-Version: 1.0.4
-Summary: CyberArk Search: Search for accounts and retrieve their passwords in the CyberArk elevated access management application. You can only retrieve accounts that you are able to view.
-Home-page: https://github.com/mjackstewart1/vaultpass
+Version: 1.0.8
+Summary: VaultPass: A CyberArk search CLI. Search for accounts and retrieve their passwords in the CyberArk elevated access management application. You can only retrieve accounts that you are able to view.
+Home-page: https://github.com/mjackstewart/vaultpass
 Author: Jack Stewart
-Author-email: mjstew@umich.edu
+Author-email: mjackstewart@gmail.com
 License: Unilicense
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `vaultpass-1.0.4/scripts/vaultpass.py` & `vaultpass-1.0.8/vaultpass/vaultpass.py`

 * *Files identical despite different names*

### Comparing `vaultpass-1.0.4/setup.py` & `vaultpass-1.0.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,26 +5,29 @@
 	'charset-normalizer',
 	'click',
 	'colorama',
 	'enum34',
 	'idna',
 	'pexpect',
 	'ptyprocess',
-	'urllib3',
 	'pypass',
+	'typing_extensions',
+	'urllib3==1.26.6',
+	'rich==12.0.0',
+	'twine',
 	'requests',
 ]
 
 setup(
 	name='vaultpass',
-    	version='1.0.4',    
-    	description='CyberArk Search: Search for accounts and retrieve their passwords in the CyberArk elevated access management application. You can only retrieve accounts that you are able to view.',
-    	url='https://github.com/mjackstewart1/vaultpass',
+    	version='1.0.8',    
+    	description='VaultPass: A CyberArk search CLI. Search for accounts and retrieve their passwords in the CyberArk elevated access management application. You can only retrieve accounts that you are able to view.',
+    	url='https://github.com/mjackstewart/vaultpass',
     	author='Jack Stewart',
-    	author_email='mjstew@umich.edu',
+    	author_email='mjackstewart@gmail.com',
     	license='Unilicense',
     	packages=['vaultpass'],
 	setup_requires=requirements_list,
     	install_requires=requirements_list,
 
 	classifiers=[
 		'Development Status :: 1 - Planning',
```

### Comparing `vaultpass-1.0.4/vaultpass/vaultpass.py` & `vaultpass-1.0.8/scripts/vaultpass.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 
 try:
 	import argparse
 	import getpass
 	import json
-	import platform
 	import requests
 	import sys
 except Exception as e:
 	print()
 	print('Could not import the required modules, exiting script ...')
 	print()
 	exit(1)
@@ -21,15 +20,15 @@
 
 def cyberark_choose_account(cyberark_accounts_list: list):
 	print('>> Choose Account <<')
 	print()
 
 	cyberark_accounts_dict = {}
 	
-	for account in cyberark_accounts_list:	
+	for account in cyberark_accounts_list:  
 		cyberark_accounts_id = account['id']
 		
 		try:
 			cyberark_accounts_name = account['name']
 		except:
 			cyberark_accounts_name = 'No Name'
 			
@@ -39,15 +38,15 @@
 			cyberark_accounts_username = 'No Username'
 			
 		cyberark_accounts_dict[cyberark_accounts_username] = []
 		cyberark_accounts_dict[cyberark_accounts_username] = [cyberark_accounts_id, cyberark_accounts_name]
 			
 	cyberark_accounts_id_list = []
 	
-	for username in sorted(cyberark_accounts_dict):	
+	for username in sorted(cyberark_accounts_dict): 
 		cyberark_accounts_id, cyberark_accounts_name = cyberark_accounts_dict[username]
 		cyberark_accounts_id_list.append(cyberark_accounts_id)
 
 	if len(cyberark_accounts_list) == 1:
 		print('Good news! Account found ...')
 		print()
 		
@@ -91,18 +90,17 @@
 					print('Your choice was not a number in the specified range.')
 					print()
 
 def cyberark_output_password(cyberark_auth_header: dict, cyberark_chosen_password: str):
 	print('>> Display or Save Password <<')
 	print()
 				
-	cyberark_response_search_password_dict = do_webservice_request('POST', f'https://cyberark.its.umich.edu/PasswordVault/api/Accounts/{cyberark_chosen_password}/Password/Retrieve', cyberark_auth_header, {})
+	cyberark_password = do_webservice_request('POST', f'https://cyberark.its.umich.edu/PasswordVault/api/Accounts/{cyberark_chosen_password}/Password/Retrieve', cyberark_auth_header, {})
 	
 	script_output_password_quit_flag = False
-	script_output_password_return = False
 	
 	while script_output_password_quit_flag is False:
 		print('d: Display the password on the screen')
 		if pass_available is True: print('s: Save the password in pass')
 		print('r: Return to the main menu')
 		print('!q: Exit the script')
 		print()
@@ -110,68 +108,68 @@
 		script_output_password_choice_input = input('Enter your choice: ')
 		script_output_password_choice = script_output_password_choice_input.lower()
 		print()
 		
 		if script_output_password_choice == 'd':	
 			print(' Display Password '.center(50, "-"))
 		
-			if len(cyberark_response_search_password_dict) > 0:		
+			if len(cyberark_password) > 0:		 
 				print(' Success! '.center(50, '-'))
-				print(f' {cyberark_response_search_password_dict} '.center(50, "-"))
+				print(f' {cyberark_password} '.center(50, "-"))
 				
-			else:		
+			else:	   
 				print(' Error! '.center(50, "-"))
 				
 			print('-' * 50)
 			print()
 			
 			script_output_password_quit_flag = True
-		elif script_output_password_choice == 's':	
+		elif script_output_password_choice == 's':	  
 			cyberark_password_name_input = input('Enter the name of the password: ')
 			print()
 			
 			try:
 				password_store = passpy.Store()
-				password_set = password_store.set_key(cyberark_password_name_input, cyberark_response_search_password_dict, force=True)
+				password_set = password_store.set_key(cyberark_password_name_input, cyberark_password, force=True)
 			
 				print(' Save Password '.center(50, "-"))
 			
 				if password_set is None:		
-					print(' Success! '.center(50, "-"))			
-				else:		
+					print(' Success! '.center(50, "-"))			 
+				else:	   
 					print(' Error! '.center(50, "-"))
 				
 				print('-' * 50)
 				print()
 			except:
 				print('Error ...')
 				print('Message: You do not have pass configured!')
 				print()
 			
 			script_output_password_quit_flag = True
 		elif script_output_password_choice == 'r':
 			script_output_password_quit_flag = True
 		elif script_output_password_choice == '!q':
 			return True
-		else:	
+		else:   
 			print('You did not choose d, s, r, or !q.')
 			print()
 
 def cyberark_search_accounts(cyberark_auth_header: dict):
 	print('>> Search for Account <<')
 	print()
 
 	print('Search accounts: Enter a search term')
 	print('r: Return to the main menu')
 	print()
 	
 	script_search_accounts_input = input('Enter your choice: ')
 	print()
 	
-	if script_search_accounts_input == '':	
+	if script_search_accounts_input == '':  
 		print('You did not enter a search term.')
 		print()
 	elif script_search_accounts_input == 'r':
 		pass
 	else:
 		cyberark_response_search_accounts_dict = do_webservice_request('GET', f'https://cyberark.its.umich.edu/PasswordVault/api/Accounts?search={script_search_accounts_input}', cyberark_auth_header, {})
 		
@@ -182,36 +180,36 @@
 			
 		return cyberark_search_accounts_return
 
 def do_webservice_request(requests_method: str, requests_url: str, requests_headers: dict, requests_json: dict or None):
 	try:	
 		webservice_response = requests.request(
 				method=requests_method,
-				url=requests_url,					
+				url=requests_url,					   
 				headers=requests_headers,
 				json=requests_json
 			)
 		
 		webservice_response.raise_for_status()
 
-		return json.loads(webservice_response.text)	
-	except (ConnectionError, requests.exceptions.HTTPError, Timeout, Exception) as e:	
+		return json.loads(webservice_response.text)	 
+	except (ConnectionError, requests.exceptions.HTTPError, Exception) as e:	   
 		print('Error ...')
 		print(f'Message: {str(e)}')
 		print()
 		
 		exit(1)
 	
 def get_auth_userinfo_from_commandline():
 	print()
 	print('>>> VaultPass: A CyberArk Search Script <<<')
 	print()
 	
 	print('>> Provide Credentials <<')
-	print()	
+	print() 
 	
 	parser = argparse.ArgumentParser(description='VaultPass: Search CyberArk for elevated accounts and retrieve their passwords. You can only retrieve accounts that you are able to view.')
 	
 	parser.add_argument('--uniqname', '-u', type=str, required=True, help='Your uniqname')
 	parser.add_argument('--password', '-p', type=str, required=True, help='Your UMICH Level 1 password')
 	
 	args = parser.parse_args()
@@ -223,15 +221,15 @@
 	
 def get_auth_userinfo_from_directinput():
 	print()
 	print('>>> VaultPass: A CyberArk Search Script <<<')
 	print()
 	
 	print('>> Provide Credentials <<')
-	print()	
+	print() 
 	
 	print('>> Enter your uniqname and UMICH Level 1 Password <<')
 	print()
 	
 	username = input('uniqname: ')
 	print()
 	
@@ -259,44 +257,44 @@
 		
 		cyberark_auth_header = cyberark_generic_header
 		cyberark_auth_header['Authorization'] = cyberark_auth_token_string
 		
 		print('Success!')
 		print()
 		
-		return cyberark_auth_header		
-	except:	
+		return cyberark_auth_header		 
+	except: 
 		print('Error ...')
 		print('Message: There was an error retrieving the authentication token.')
 		print()
 		
 		exit(1)
 
-def main():	
+def main():	 
 	if len(sys.argv) > 1:
-		username, password = get_auth_userinfo_from_commandline()		
-	else:	
+		username, password = get_auth_userinfo_from_commandline()		   
+	else:   
 		username, password = get_auth_userinfo_from_directinput()
 
 	cyberark_auth_header = get_cyberark_auth_header(username, password)
 	
 	script_quit_choice = 's'
 	script_quit_flag = False
 	
 	while script_quit_flag is False:
-		if script_quit_choice == 's':			
+		if script_quit_choice == 's':		   
 			cyberark_accounts_list = cyberark_search_accounts(cyberark_auth_header)
 			
 			if cyberark_accounts_list is None:
 				pass
 			else:
 				if len(cyberark_accounts_list) == 0:
 					print('Your search produced no results.')
 					print()
-				else:				
+				else:			   
 					cyberark_chosen_account = cyberark_choose_account(cyberark_accounts_list)
 					
 					if not(cyberark_chosen_account is None):
 						script_output_password_quit_flag = cyberark_output_password(cyberark_auth_header, cyberark_chosen_account)
 						
 						if script_output_password_quit_flag is True:
 							script_quit_flag = True
@@ -305,15 +303,15 @@
 			script_quit_flag = True
 		else:
 			print('You did not choose s or !q.')
 			print()
 			
 		if script_quit_flag is False:
 			print('Do you want to search again for another account or exit the script?')
-			print()			
+			print()		 
 			print('s: Search again')
 			print('!q: Exit the script')
 			print()
 			
 			script_quit_choice_input = input('Enter your choice: ')
 			script_quit_choice = script_quit_choice_input.lower()
 			
@@ -322,10 +320,9 @@
 	print('>> Exiting VaultPass ... <<')
 	print()
 			
 	print('Buh-Bye Now! Y\'all have a GREAT DAY!')
 	print()
 
 if __name__ == "__main__":
-
 	main()
```

### Comparing `vaultpass-1.0.4/vaultpass.egg-info/PKG-INFO` & `vaultpass-1.0.8/vaultpass.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.1
 Name: vaultpass
-Version: 1.0.4
-Summary: CyberArk Search: Search for accounts and retrieve their passwords in the CyberArk elevated access management application. You can only retrieve accounts that you are able to view.
-Home-page: https://github.com/mjackstewart1/vaultpass
+Version: 1.0.8
+Summary: VaultPass: A CyberArk search CLI. Search for accounts and retrieve their passwords in the CyberArk elevated access management application. You can only retrieve accounts that you are able to view.
+Home-page: https://github.com/mjackstewart/vaultpass
 Author: Jack Stewart
-Author-email: mjstew@umich.edu
+Author-email: mjackstewart@gmail.com
 License: Unilicense
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: Microsoft :: Windows
```

