# Comparing `tmp/dopplrSDK-2.0.0-py3-none-any.whl.zip` & `tmp/dopplrSDK-2.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4392 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     6805 b- defN 23-Jun-15 15:33 dopplrSDK/__init__.py
--rw-rw-rw-  2.0 fat     1077 b- defN 23-Jun-15 17:00 dopplrSDK-2.0.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      530 b- defN 23-Jun-15 17:00 dopplrSDK-2.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-15 17:00 dopplrSDK-2.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-15 17:00 dopplrSDK-2.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      477 b- defN 23-Jun-15 17:00 dopplrSDK-2.0.0.dist-info/RECORD
-6 files, 8991 bytes uncompressed, 3526 bytes compressed:  60.8%
+Zip file size: 4232 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     6113 b- defN 23-Jun-16 05:45 dopplrSDK/__init__.py
+-rw-rw-rw-  2.0 fat     1077 b- defN 23-Jun-16 05:47 dopplrSDK-2.1.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      530 b- defN 23-Jun-16 05:47 dopplrSDK-2.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-16 05:47 dopplrSDK-2.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-16 05:47 dopplrSDK-2.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      477 b- defN 23-Jun-16 05:47 dopplrSDK-2.1.0.dist-info/RECORD
+6 files, 8299 bytes uncompressed, 3366 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: dopplrSDK/__init__.py
 Comment: 
 
-Filename: dopplrSDK-2.0.0.dist-info/LICENSE.txt
+Filename: dopplrSDK-2.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dopplrSDK-2.0.0.dist-info/METADATA
+Filename: dopplrSDK-2.1.0.dist-info/METADATA
 Comment: 
 
-Filename: dopplrSDK-2.0.0.dist-info/WHEEL
+Filename: dopplrSDK-2.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: dopplrSDK-2.0.0.dist-info/top_level.txt
+Filename: dopplrSDK-2.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dopplrSDK-2.0.0.dist-info/RECORD
+Filename: dopplrSDK-2.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dopplrSDK/__init__.py

```diff
@@ -45,130 +45,113 @@
     return keys,db,s3
 
 def putFileTomywrkspace(filePath,file_type,loginName,s_key):
     try:
         keys,db,s3=decrypt_keys("zvkPurRjZz0ptGnEIxMq0tu3062oChYVkuUwkk7RG7pigQttPVQFkoHBQp+hb5dcYuGeb8asmxKv9XkaI9EnTTTT3YT4UvOF9cT46kotQRceh4oRzPwwKSWFUswJmtBBb2NNlUBFBae6qZqoozBn5g==",s_key)
         
         query="select DOR.\"OrgName\",Du.\"UserKey\",DOR.\"ContainerName\",DOR.\"AwsAccessKey\",DOR.\"AwsSecretKey\" FROM doppler.\"DopplerUser\" Du join doppler.\"DopplerOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" where Du.\"LoginName\"="+"'"+loginName+"'"+""
-        #print(query)
+
         ContainerName = keys['Bucket']
         cnxn = psycopg2.connect(host=db['host'],database=db['database'],user=db['user'],password=db['password'],port=db['port'])
     
         cur=cnxn.cursor()
         cur.execute(query)
         results = cur.fetchone()
         
 
-        #ContainerName=results[2]
-        #AwsAccessKey=results[3]
-        #AwsSecretKey=results[4]
         UserKey=results[1]
         OrgName=results[0]
         
-        
-
         cur=cnxn.cursor()
         file_name = os.path.basename(filePath)
-        file_name=file_name.replace('.csv','')
-        query="select count(\"TableName\") from doppler.\"DopplerLake\" where \"Source\"='MLStudio' and \"TableName\"="+"'"+file_name+"'"
+        file_name1=file_name.split('.')
+        query="select count(\"TableName\") from doppler.\"DopplerLake\" where \"Source\"='MLStudio' and \"TableName\"="+"'"+file_name1[0]+"'"
+ 
         cur.execute(query)
         results = cur.fetchone()
         if results[0]<1:
-            insert_query = "INSERT INTO doppler.\"DopplerLake\"(\"UserKey\", \"TableName\",\"ResourceType\",\"DopplerConnectionDetailsKey\",\"Projectid\",\"Status\") VALUES ("+str(UserKey)+",'"+file_name+"','"+file_type+"',null,'','Uploaded')"
+            insert_query = "INSERT INTO doppler.\"DopplerLake\"(\"UserKey\", \"TableName\",\"ResourceType\",\"DopplerConnectionDetailsKey\",\"Projectid\",\"Status\") VALUES ("+str(UserKey)+",'"+file_name1[0]+"','"+file_type+"',null,'','Uploaded')"
             cur.execute(insert_query)
             cnxn.commit()
         else:
             pass
             
         
         cur1=cnxn.cursor()
-        insert_query1 = "SELECT max(\"SourceKey\") as \"SourceKey\" FROM doppler.\"DopplerLake\" where \"UserKey\"="+str(UserKey)+" and \"TableName\"='"+file_name+"'"
+        insert_query1 = "SELECT max(\"SourceKey\") as \"SourceKey\" FROM doppler.\"DopplerLake\" where \"UserKey\"="+str(UserKey)+" and \"TableName\"='"+file_name1[0]+"'"
         
         cur1.execute(insert_query1)
         results = cur1.fetchone()
         SourceKey=results[0]
         SourceKey=str(SourceKey)
 
 
-        ConnectionString = str(OrgName)+"/"+str(loginName).upper()+"/"+(str(SourceKey).lstrip()+'/SOURCE/'+file_name+'.csv')
-
-        update_query = "UPDATE doppler.\"DopplerLake\" set \"ConnectionString\"='"+str(OrgName)+"/"+str(loginName).upper()+'/'+(str(SourceKey).lstrip()+'/SOURCE/'+file_name+".csv',\"Source\"= 'MLStudio' ,\"CreatedTs\"=CURRENT_TIMESTAMP where \"SourceKey\"="+str(SourceKey))
+        ConnectionString = str(OrgName)+"/"+str(loginName).upper()+"/"+(str(SourceKey).lstrip()+'/SOURCE/'+file_name)
+        update_query = "UPDATE doppler.\"DopplerLake\" set \"ConnectionString\"='"+str(OrgName)+"/"+str(loginName).upper()+'/'+(str(SourceKey).lstrip()+'/SOURCE/'+file_name+"',\"Source\"= 'MLStudio' ,\"CreatedTs\"=CURRENT_TIMESTAMP where \"SourceKey\"="+str(SourceKey))
         cur2=cnxn.cursor()
-        #print("update_query ",update_query)
+
         cur2.execute(update_query)
         cnxn.commit()
-        if '.csv' in filePath:
-            filePath=filePath
-        else:
-            filePath=filePath+'.csv'
         s3.upload_file(filePath, ContainerName, ConnectionString)
          # Generate a pre-signed URL
         
         s3.put_object_acl(ACL='public-read',
                           Bucket=ContainerName,
                           Key=ConnectionString)
-        #url = f"https://{ContainerName}.s3.ap-south-1.amazonaws.com/{ConnectionString}"
+        
         url = f"s3://{ContainerName}/{ConnectionString}"
         print("uri : ",url)
         cnxn.close()
         #print("done")
     except Exception as error:
         if 'NoneType' in str(error):
             dopplrsource= 'File does not exists'
             print("Error : ", dopplrsource)
             sys.exit()
         else:
             print("Error : ",error)
 
 
 def getWorkspaceFile(fileName,destination,loginName,s_key):
-    #type = 1 then get file (Actual file) 
-    #type = 2 then get file* (file pattern)
-
 
     keys,db,s3=decrypt_keys("zvkPurRjZz0ptGnEIxMq0tu3062oChYVkuUwkk7RG7pigQttPVQFkoHBQp+hb5dcYuGeb8asmxKv9XkaI9EnTTTT3YT4UvOF9cT46kotQRceh4oRzPwwKSWFUswJmtBBb2NNlUBFBae6qZqoozBn5g==",s_key)
 
     
     query="select DOR.\"OrgName\",Du.\"UserKey\",DOR.\"ContainerName\",DOR.\"AwsAccessKey\",DOR.\"AwsSecretKey\" FROM doppler.\"DopplerUser\" Du join doppler.\"DopplerOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" where Du.\"LoginName\"="+"'"+loginName+"'"+""
     ContainerName = keys['Bucket']
     cnxn = psycopg2.connect(host=db['host'],database=db['database'],user=db['user'],password=db['password'],port=db['port'])
 
     cur=cnxn.cursor()
     cur.execute(query)
     results = cur.fetchone()
         
 
-    #ContainerName=results[2]
-    #AwsAccessKey=results[3]
-    #AwsSecretKey=results[4]
+
     UserKey=results[1]
     OrgName=results[0]
     folder_prefix = OrgName+'/'+loginName.upper()+'/'
         
-    #s3 = boto3.client('s3', aws_access_key_id=AwsAccessKey, aws_secret_access_key=AwsSecretKey)
 
     # Check if the file exists
     if os.path.exists(destination):
         print('folder exists')
     else:
         os.mkdir(destination)
 
     response = s3.list_objects_v2(Bucket=ContainerName, Prefix=folder_prefix)
     # Iterate through the objects
     destination=destination+'/'+fileName
     for obj in response['Contents']:
         key = obj['Key']
-        #print(key,fileName)
+
             
         is_same = is_file_name_same(key, fileName)
 
         if(is_same):                
             s3.download_file(ContainerName, key, destination)
             print("download")
 
 def is_file_name_same(file_path, expected_file_name):
         file_name = os.path.basename(file_path)
         return file_name == expected_file_name
 
 
-
-
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `dopplrSDK-2.0.0.dist-info/LICENSE.txt` & `dopplrSDK-2.1.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dopplrSDK-2.0.0.dist-info/METADATA` & `dopplrSDK-2.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dopplrSDK
-Version: 2.0.0
+Version: 2.1.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Anand
 Author-email: anandt@systechusa.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

