# Comparing `tmp/soniox-1.8.0.tar.gz` & `tmp/soniox-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soniox-1.8.0.tar", last modified: Fri Jun 16 11:03:11 2023, max compression
+gzip compressed data, was "soniox-1.8.1.tar", last modified: Fri Jun 16 15:22:38 2023, max compression
```

## Comparing `soniox-1.8.0.tar` & `soniox-1.8.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 ambroz    (1001) ambroz    (1001)        0 2023-06-16 11:03:11.161706 soniox-1.8.0/
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     1053 2022-06-20 18:06:39.000000 soniox-1.8.0/LICENSE
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     1168 2023-06-16 11:03:11.161706 soniox-1.8.0/PKG-INFO
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      745 2023-03-29 10:56:40.000000 soniox-1.8.0/README.md
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)       38 2023-06-16 11:03:11.161706 soniox-1.8.0/setup.cfg
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      740 2023-06-16 11:02:20.000000 soniox-1.8.0/setup.py
-drwxrwxr-x   0 ambroz    (1001) ambroz    (1001)        0 2023-06-16 11:03:11.161706 soniox-1.8.0/soniox/
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)        0 2022-06-20 18:06:39.000000 soniox-1.8.0/soniox/__init__.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     3815 2023-05-17 12:09:38.000000 soniox-1.8.0/soniox/capture_device.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      304 2022-09-01 10:40:05.000000 soniox-1.8.0/soniox/conversion.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     6512 2022-08-31 07:52:52.000000 soniox-1.8.0/soniox/manage_speakers.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     5586 2022-08-31 07:53:02.000000 soniox-1.8.0/soniox/manage_speech_contexts.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     3808 2022-06-21 13:02:45.000000 soniox-1.8.0/soniox/multi_channel_utils.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)    13420 2023-06-16 10:55:12.000000 soniox-1.8.0/soniox/speech_service.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)    26555 2023-06-16 10:55:45.000000 soniox-1.8.0/soniox/speech_service_pb2.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)    44301 2023-06-16 10:55:45.000000 soniox-1.8.0/soniox/speech_service_pb2_grpc.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     5885 2023-04-25 11:52:59.000000 soniox-1.8.0/soniox/storage.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)    16186 2023-03-31 09:29:12.000000 soniox-1.8.0/soniox/transcribe_file.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     8821 2023-05-17 12:09:43.000000 soniox-1.8.0/soniox/transcribe_live.py
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      312 2023-06-16 11:00:40.000000 soniox-1.8.0/soniox/utils.py
-drwxrwxr-x   0 ambroz    (1001) ambroz    (1001)        0 2023-06-16 11:03:11.161706 soniox-1.8.0/soniox.egg-info/
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     1168 2023-06-16 11:03:11.000000 soniox-1.8.0/soniox.egg-info/PKG-INFO
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      503 2023-06-16 11:03:11.000000 soniox-1.8.0/soniox.egg-info/SOURCES.txt
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)        1 2023-06-16 11:03:11.000000 soniox-1.8.0/soniox.egg-info/dependency_links.txt
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)       48 2023-06-16 11:03:11.000000 soniox-1.8.0/soniox.egg-info/requires.txt
--rw-rw-r--   0 ambroz    (1001) ambroz    (1001)        7 2023-06-16 11:03:11.000000 soniox-1.8.0/soniox.egg-info/top_level.txt
+drwxrwxr-x   0 ambroz    (1001) ambroz    (1001)        0 2023-06-16 15:22:38.443229 soniox-1.8.1/
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     1053 2022-06-20 18:06:39.000000 soniox-1.8.1/LICENSE
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     1168 2023-06-16 15:22:38.443229 soniox-1.8.1/PKG-INFO
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      745 2023-03-29 10:56:40.000000 soniox-1.8.1/README.md
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)       38 2023-06-16 15:22:38.443229 soniox-1.8.1/setup.cfg
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      740 2023-06-16 15:22:03.000000 soniox-1.8.1/setup.py
+drwxrwxr-x   0 ambroz    (1001) ambroz    (1001)        0 2023-06-16 15:22:38.443229 soniox-1.8.1/soniox/
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)        0 2022-06-20 18:06:39.000000 soniox-1.8.1/soniox/__init__.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     3815 2023-05-17 12:09:38.000000 soniox-1.8.1/soniox/capture_device.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      304 2022-09-01 10:40:05.000000 soniox-1.8.1/soniox/conversion.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     6512 2022-08-31 07:52:52.000000 soniox-1.8.1/soniox/manage_speakers.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     5586 2022-08-31 07:53:02.000000 soniox-1.8.1/soniox/manage_speech_contexts.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     3808 2022-06-21 13:02:45.000000 soniox-1.8.1/soniox/multi_channel_utils.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)    13491 2023-06-16 15:10:47.000000 soniox-1.8.1/soniox/speech_service.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)    26602 2023-06-16 15:09:51.000000 soniox-1.8.1/soniox/speech_service_pb2.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)    44301 2023-06-16 15:09:51.000000 soniox-1.8.1/soniox/speech_service_pb2_grpc.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     5885 2023-04-25 11:52:59.000000 soniox-1.8.1/soniox/storage.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)    16186 2023-03-31 09:29:12.000000 soniox-1.8.1/soniox/transcribe_file.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     8821 2023-05-17 12:09:43.000000 soniox-1.8.1/soniox/transcribe_live.py
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      312 2023-06-16 11:00:40.000000 soniox-1.8.1/soniox/utils.py
+drwxrwxr-x   0 ambroz    (1001) ambroz    (1001)        0 2023-06-16 15:22:38.443229 soniox-1.8.1/soniox.egg-info/
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)     1168 2023-06-16 15:22:38.000000 soniox-1.8.1/soniox.egg-info/PKG-INFO
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)      503 2023-06-16 15:22:38.000000 soniox-1.8.1/soniox.egg-info/SOURCES.txt
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)        1 2023-06-16 15:22:38.000000 soniox-1.8.1/soniox.egg-info/dependency_links.txt
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)       48 2023-06-16 15:22:38.000000 soniox-1.8.1/soniox.egg-info/requires.txt
+-rw-rw-r--   0 ambroz    (1001) ambroz    (1001)        7 2023-06-16 15:22:38.000000 soniox-1.8.1/soniox.egg-info/top_level.txt
```

### Comparing `soniox-1.8.0/LICENSE` & `soniox-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `soniox-1.8.0/PKG-INFO` & `soniox-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soniox
-Version: 1.8.0
+Version: 1.8.1
 Summary: Soniox speech recognition service client library
 Home-page: https://soniox.com/
 Author: Soniox Inc
 Author-email: support@soniox.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `soniox-1.8.0/README.md` & `soniox-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `soniox-1.8.0/setup.py` & `soniox-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="soniox",
-    version="1.8.0",
+    version="1.8.1",
     author="Soniox Inc",
     author_email="support@soniox.com",
     description="Soniox speech recognition service client library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://soniox.com/",
     packages=setuptools.find_packages(),
```

### Comparing `soniox-1.8.0/soniox/capture_device.py` & `soniox-1.8.1/soniox/capture_device.py`

 * *Files identical despite different names*

### Comparing `soniox-1.8.0/soniox/manage_speakers.py` & `soniox-1.8.1/soniox/manage_speakers.py`

 * *Files identical despite different names*

### Comparing `soniox-1.8.0/soniox/manage_speech_contexts.py` & `soniox-1.8.1/soniox/manage_speech_contexts.py`

 * *Files identical despite different names*

### Comparing `soniox-1.8.0/soniox/multi_channel_utils.py` & `soniox-1.8.1/soniox/multi_channel_utils.py`

 * *Files identical despite different names*

### Comparing `soniox-1.8.0/soniox/speech_service.py` & `soniox-1.8.1/soniox/speech_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,19 +357,21 @@
         request.file_id = file_id
 
         self._client.DeleteTranscribeAsyncFile(request)
 
     def CreateTemporaryApiKey(
         self,
         usage_type: str,
+        expires_in_s: int,
         client_request_reference: str = "",
     ) -> CreateTemporaryApiKeyResponse:
         request = speech_service_pb2.CreateTemporaryApiKeyRequest()
         request.api_key = self.api_key
         request.usage_type = usage_type
+        request.expires_in_s = expires_in_s
         request.client_request_reference = client_request_reference
 
         return self._client.CreateTemporaryApiKey(request)
 
 
 def update_result(result: Result, new_result: Result) -> None:
     assert result.channel == new_result.channel
```

### Comparing `soniox-1.8.0/soniox/speech_service_pb2.py` & `soniox-1.8.1/soniox/speech_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bsoniox/speech_service.proto\x12\x15soniox.speech_service\x1a\x1fgoogle/protobuf/timestamp.proto\"o\n\x11TranscribeRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12:\n\x06\x63onfig\x18\x04 \x01(\x0b\x32*.soniox.speech_service.TranscriptionConfig\x12\r\n\x05\x61udio\x18\x03 \x01(\x0c\"\xbb\x01\n\x12TranscribeResponse\x12-\n\x06result\x18\x01 \x01(\x0b\x32\x1d.soniox.speech_service.Result\x12\x36\n\x0f\x63hannel_results\x18\x02 \x03(\x0b\x32\x1d.soniox.speech_service.Result\x12>\n\x08metadata\x18\x03 \x01(\x0b\x32,.soniox.speech_service.TranscriptionMetadata\"u\n\x17TranscribeStreamRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12:\n\x06\x63onfig\x18\x04 \x01(\x0b\x32*.soniox.speech_service.TranscriptionConfig\x12\r\n\x05\x61udio\x18\x03 \x01(\x0c\"\x89\x01\n\x18TranscribeStreamResponse\x12-\n\x06result\x18\x01 \x01(\x0b\x32\x1d.soniox.speech_service.Result\x12>\n\x08metadata\x18\x02 \x01(\x0b\x32,.soniox.speech_service.TranscriptionMetadata\"\xcc\x01\n\x18TranscribeMeetingRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12:\n\x06\x63onfig\x18\n \x01(\x0b\x32*.soniox.speech_service.TranscriptionConfig\x12\x0f\n\x07seq_num\x18\x03 \x01(\x05\x12\x11\n\tstream_id\x18\x04 \x01(\x05\x12\x18\n\x10start_of_segment\x18\x05 \x01(\x08\x12\r\n\x05\x61udio\x18\x06 \x01(\x0c\x12\x16\n\x0e\x65nd_of_segment\x18\x07 \x01(\x08\"\xef\x01\n\x19TranscribeMeetingResponse\x12\x0f\n\x07seq_num\x18\x01 \x01(\x05\x12\x11\n\tstream_id\x18\x02 \x01(\x05\x12\x18\n\x10start_of_segment\x18\x03 \x01(\x08\x12\x16\n\x0e\x65nd_of_segment\x18\x04 \x01(\x08\x12-\n\x06result\x18\x05 \x01(\x0b\x32\x1d.soniox.speech_service.Result\x12\r\n\x05\x65rror\x18\x06 \x01(\t\x12>\n\x08metadata\x18\x07 \x01(\x0b\x32,.soniox.speech_service.TranscriptionMetadata\"\xad\x01\n\x16TranscribeAsyncRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x16\n\x0ereference_name\x18\x03 \x01(\t\x12:\n\x06\x63onfig\x18\x05 \x01(\x0b\x32*.soniox.speech_service.TranscriptionConfig\x12\x12\n\nenable_eof\x18\x06 \x01(\x08\x12\x0b\n\x03\x65of\x18\x07 \x01(\x08\x12\r\n\x05\x61udio\x18\x04 \x01(\x0c\"*\n\x17TranscribeAsyncResponse\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\"C\n\x1fGetTranscribeAsyncStatusRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"c\n GetTranscribeAsyncStatusResponse\x12?\n\x05\x66iles\x18\x01 \x03(\x0b\x32\x30.soniox.speech_service.TranscribeAsyncFileStatus\"\x9d\x01\n\x19TranscribeAsyncFileStatus\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x16\n\x0ereference_name\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x30\n\x0c\x63reated_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rerror_message\x18\x05 \x01(\t\"C\n\x1fGetTranscribeAsyncResultRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"\xbb\x01\n GetTranscribeAsyncResultResponse\x12(\n separate_recognition_per_channel\x18\x02 \x01(\x08\x12-\n\x06result\x18\x01 \x01(\x0b\x32\x1d.soniox.speech_service.Result\x12>\n\x08metadata\x18\x03 \x01(\x0b\x32,.soniox.speech_service.TranscriptionMetadata\"D\n DeleteTranscribeAsyncFileRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"#\n!DeleteTranscribeAsyncFileResponse\"\xad\x05\n\x13TranscriptionConfig\x12 \n\x18\x63lient_request_reference\x18\x13 \x01(\t\x12\x14\n\x0c\x61udio_format\x18\x01 \x01(\t\x12\x19\n\x11sample_rate_hertz\x18\x02 \x01(\x05\x12\x1a\n\x12num_audio_channels\x18\x03 \x01(\x05\x12\x18\n\x10include_nonfinal\x18\x04 \x01(\x08\x12/\n\'enable_separate_recognition_per_channel\x18\x10 \x01(\x08\x12!\n\x19\x65nable_endpoint_detection\x18\x12 \x01(\x08\x12<\n\x0espeech_context\x18\x05 \x01(\x0b\x32$.soniox.speech_service.SpeechContext\x12\x1f\n\x17\x65nable_profanity_filter\x18\x06 \x01(\x08\x12\"\n\x1a\x63ontent_moderation_phrases\x18\x07 \x03(\t\x12,\n$enable_streaming_speaker_diarization\x18\x08 \x01(\x08\x12)\n!enable_global_speaker_diarization\x18\t \x01(\x08\x12\x18\n\x10min_num_speakers\x18\n \x01(\x05\x12\x18\n\x10max_num_speakers\x18\x0b \x01(\x05\x12%\n\x1d\x65nable_speaker_identification\x18\x0c \x01(\x08\x12\x1a\n\x12\x63\x61nd_speaker_names\x18\r \x03(\t\x12\r\n\x05model\x18\x0e \x01(\t\x12\x18\n\x10\x65nable_dictation\x18\x0f \x01(\x08\x12=\n\x0estorage_config\x18\xee\x07 \x01(\x0b\x32$.soniox.speech_service.StorageConfig\"0\n\x15TranscriptionMetadata\x12\x17\n\x0fpackage_version\x18\x01 \x01(\t\"\xb5\x01\n\x06Result\x12*\n\x05words\x18\x01 \x03(\x0b\x32\x1b.soniox.speech_service.Word\x12\x1a\n\x12\x66inal_proc_time_ms\x18\x02 \x01(\x05\x12\x1a\n\x12total_proc_time_ms\x18\x03 \x01(\x05\x12\x36\n\x08speakers\x18\x06 \x03(\x0b\x32$.soniox.speech_service.ResultSpeaker\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\x05\"\x85\x01\n\x04Word\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x10\n\x08start_ms\x18\x02 \x01(\x05\x12\x13\n\x0b\x64uration_ms\x18\x03 \x01(\x05\x12\x10\n\x08is_final\x18\x04 \x01(\x08\x12\x0f\n\x07speaker\x18\x05 \x01(\x05\x12\x11\n\torig_text\x18\x08 \x01(\t\x12\x12\n\nconfidence\x18\t \x01(\x01\".\n\rResultSpeaker\x12\x0f\n\x07speaker\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\"Y\n\rSpeechContext\x12:\n\x07\x65ntries\x18\x01 \x03(\x0b\x32).soniox.speech_service.SpeechContextEntry\x12\x0c\n\x04name\x18\x02 \x01(\t\"4\n\x12SpeechContextEntry\x12\x0f\n\x07phrases\x18\x01 \x03(\t\x12\r\n\x05\x62oost\x18\x02 \x01(\x01\"k\n\x1a\x43reateSpeechContextRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12<\n\x0espeech_context\x18\x02 \x01(\x0b\x32$.soniox.speech_service.SpeechContext\"\x1d\n\x1b\x43reateSpeechContextResponse\";\n\x1a\x44\x65leteSpeechContextRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x1d\n\x1b\x44\x65leteSpeechContextResponse\"0\n\x1dListSpeechContextNamesRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\"/\n\x1eListSpeechContextNamesResponse\x12\r\n\x05names\x18\x01 \x03(\t\"8\n\x17GetSpeechContextRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"X\n\x18GetSpeechContextResponse\x12<\n\x0espeech_context\x18\x01 \x01(\x0b\x32$.soniox.speech_service.SpeechContext\"k\n\x1aUpdateSpeechContextRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12<\n\x0espeech_context\x18\x02 \x01(\x0b\x32$.soniox.speech_service.SpeechContext\"\x1d\n\x1bUpdateSpeechContextResponse\"2\n\x11\x41\x64\x64SpeakerRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"O\n\x12\x41\x64\x64SpeakerResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\x07\x63reated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"2\n\x11GetSpeakerRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x8f\x01\n\x12GetSpeakerResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\x07\x63reated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12>\n\x06\x61udios\x18\x03 \x03(\x0b\x32..soniox.speech_service.GetSpeakerResponseAudio\"o\n\x17GetSpeakerResponseAudio\x12\x12\n\naudio_name\x18\x01 \x01(\t\x12+\n\x07\x63reated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64uration_ms\x18\x03 \x01(\x05\"5\n\x14RemoveSpeakerRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x17\n\x15RemoveSpeakerResponse\"&\n\x13ListSpeakersRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\"\\\n\x14ListSpeakersResponse\x12\x44\n\x08speakers\x18\x01 \x03(\x0b\x32\x32.soniox.speech_service.ListSpeakersResponseSpeaker\"l\n\x1bListSpeakersResponseSpeaker\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\x07\x63reated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nnum_audios\x18\x03 \x01(\x05\"b\n\x16\x41\x64\x64SpeakerAudioRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x14\n\x0cspeaker_name\x18\x02 \x01(\t\x12\x12\n\naudio_name\x18\x03 \x01(\t\x12\r\n\x05\x61udio\x18\x04 \x01(\x0c\"\x85\x01\n\x17\x41\x64\x64SpeakerAudioResponse\x12\x14\n\x0cspeaker_name\x18\x01 \x01(\t\x12\x12\n\naudio_name\x18\x02 \x01(\t\x12+\n\x07\x63reated\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64uration_ms\x18\x04 \x01(\x05\"S\n\x16GetSpeakerAudioRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x14\n\x0cspeaker_name\x18\x02 \x01(\t\x12\x12\n\naudio_name\x18\x03 \x01(\t\"\x94\x01\n\x17GetSpeakerAudioResponse\x12\x14\n\x0cspeaker_name\x18\x01 \x01(\t\x12\x12\n\naudio_name\x18\x02 \x01(\t\x12+\n\x07\x63reated\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64uration_ms\x18\x04 \x01(\x05\x12\r\n\x05\x61udio\x18\x05 \x01(\x0c\"V\n\x19RemoveSpeakerAudioRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x14\n\x0cspeaker_name\x18\x02 \x01(\t\x12\x12\n\naudio_name\x18\x03 \x01(\t\"\x1c\n\x1aRemoveSpeakerAudioResponse\"\x95\x02\n\rStorageConfig\x12\x11\n\tobject_id\x18\x01 \x01(\t\x12\x44\n\x08metadata\x18\x02 \x03(\x0b\x32\x32.soniox.speech_service.StorageConfig.MetadataEntry\x12\r\n\x05title\x18\x03 \x01(\t\x12,\n\x08\x64\x61tetime\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x13\x64isable_store_audio\x18\x05 \x01(\x08\x12 \n\x18\x64isable_store_transcript\x18\x06 \x01(\x08\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xa8\x01\n\x05Token\x12\x0b\n\x03idx\x18\x01 \x01(\x05\x12\x12\n\ntext_start\x18\x02 \x01(\x05\x12\x10\n\x08text_end\x18\x03 \x01(\x05\x12\x0c\n\x04text\x18\x04 \x01(\t\x12\x10\n\x08start_ms\x18\x05 \x01(\x05\x12\x13\n\x0b\x64uration_ms\x18\x06 \x01(\x05\x12\x12\n\nconfidence\x18\x07 \x01(\x01\x12\x12\n\nspeaker_id\x18\x08 \x01(\x05\x12\x0f\n\x07profane\x18\t \x01(\x08\"2\n\x08Sentence\x12\x13\n\x0btoken_start\x18\x01 \x01(\x05\x12\x11\n\ttoken_end\x18\x02 \x01(\x05\"9\n\tParagraph\x12\x16\n\x0esentence_start\x18\x01 \x01(\x05\x12\x14\n\x0csentence_end\x18\x02 \x01(\x05\"C\n\x07Keyterm\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\r\n\x05score\x18\x02 \x01(\x01\x12\x1b\n\x13token_start_indexes\x18\x03 \x03(\x05\"\xe5\x02\n\nTranscript\x12\x0c\n\x04text\x18\x01 \x01(\t\x12,\n\x06tokens\x18\x02 \x03(\x0b\x32\x1c.soniox.speech_service.Token\x12\x32\n\tsentences\x18\x03 \x03(\x0b\x32\x1f.soniox.speech_service.Sentence\x12\x34\n\nparagraphs\x18\x04 \x03(\x0b\x32 .soniox.speech_service.Paragraph\x12\x30\n\x08keyterms\x18\x06 \x03(\x0b\x32\x1e.soniox.speech_service.Keyterm\x12J\n\rspeaker_names\x18\x07 \x03(\x0b\x32\x33.soniox.speech_service.Transcript.SpeakerNamesEntry\x1a\x33\n\x11SpeakerNamesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x87\x03\n\x0cStoredObject\x12\x11\n\tobject_id\x18\x01 \x01(\t\x12\x43\n\x08metadata\x18\x02 \x03(\x0b\x32\x31.soniox.speech_service.StoredObject.MetadataEntry\x12\r\n\x05title\x18\x03 \x01(\t\x12,\n\x08\x64\x61tetime\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0fstored_datetime\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64uration_ms\x18\x06 \x01(\x05\x12\x1a\n\x12num_audio_channels\x18\n \x01(\x05\x12\x14\n\x0c\x61udio_stored\x18\x0b \x01(\x08\x12\x35\n\ntranscript\x18\x07 \x01(\x0b\x32!.soniox.speech_service.Transcript\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xdf\x01\n\rSearchRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x11\n\tobject_id\x18\x02 \x01(\t\x12\x16\n\x0emetadata_query\x18\x03 \x01(\t\x12\x31\n\rdatetime_from\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0b\x64\x61tetime_to\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ntext_query\x18\x06 \x01(\t\x12\r\n\x05start\x18\x07 \x01(\x05\x12\x0b\n\x03num\x18\x08 \x01(\x05\"\xfa\x01\n\x0cSearchResult\x12\x11\n\tobject_id\x18\x01 \x01(\t\x12\x43\n\x08metadata\x18\x02 \x03(\x0b\x32\x31.soniox.speech_service.SearchResult.MetadataEntry\x12\r\n\x05title\x18\x03 \x01(\t\x12,\n\x08\x64\x61tetime\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64uration_ms\x18\x05 \x01(\x05\x12\x0f\n\x07preview\x18\x06 \x01(\t\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"h\n\x0eSearchResponse\x12\x11\n\tnum_found\x18\x01 \x01(\x05\x12\r\n\x05start\x18\x02 \x01(\x05\x12\x34\n\x07results\x18\x03 \x03(\x0b\x32#.soniox.speech_service.SearchResult\"6\n\x10GetObjectRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x11\n\tobject_id\x18\x02 \x01(\t\"H\n\x11GetObjectResponse\x12\x33\n\x06object\x18\x01 \x01(\x0b\x32#.soniox.speech_service.StoredObject\"\xb3\x01\n\x12ListObjectsRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x38\n\x14stored_datetime_from\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x36\n\x12stored_datetime_to\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05start\x18\x04 \x01(\x03\x12\x0b\n\x03num\x18\x05 \x01(\x03\"g\n\x13ListObjectsResponse\x12\r\n\x05start\x18\x01 \x01(\x03\x12\x41\n\x07objects\x18\x02 \x03(\x0b\x32\x30.soniox.speech_service.ListObjectsResponseObject\"\xc8\x01\n\x19ListObjectsResponseObject\x12\x11\n\tobject_id\x18\x01 \x01(\t\x12\x33\n\x0fstored_datetime\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0c\x61udio_stored\x18\x03 \x01(\x08\x12\x19\n\x11transcript_stored\x18\x04 \x01(\x08\x12\x19\n\x11\x61udio_duration_ms\x18\x05 \x01(\x05\x12\x17\n\x0fstored_audio_ms\x18\x06 \x01(\x05\"9\n\x13\x44\x65leteObjectRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x11\n\tobject_id\x18\x02 \x01(\t\"\x16\n\x14\x44\x65leteObjectResponse\"\xea\x02\n\x0fGetAudioRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x11\n\tobject_id\x18\x02 \x01(\t\x12J\n\x0ctime_segment\x18\x03 \x01(\x0b\x32\x32.soniox.speech_service.GetAudioRequest.TimeSegmentH\x00\x12L\n\rtoken_segment\x18\x04 \x01(\x0b\x32\x33.soniox.speech_service.GetAudioRequest.TokenSegmentH\x00\x12\x1a\n\x12\x61udio_bytes_format\x18\x05 \x01(\t\x1a\x34\n\x0bTimeSegment\x12\x10\n\x08start_ms\x18\x01 \x01(\x05\x12\x13\n\x0b\x64uration_ms\x18\x02 \x01(\x05\x1a\x36\n\x0cTokenSegment\x12\x13\n\x0btoken_start\x18\x01 \x01(\x05\x12\x11\n\ttoken_end\x18\x02 \x01(\x05\x42\x0f\n\roneof_segment\"\x91\x01\n\x10GetAudioResponse\x12\x11\n\tobject_id\x18\x01 \x01(\t\x12\x10\n\x08start_ms\x18\x02 \x01(\x05\x12\x13\n\x0b\x64uration_ms\x18\x03 \x01(\x05\x12\x19\n\x11total_duration_ms\x18\x04 \x01(\x05\x12\x1a\n\x12num_audio_channels\x18\x06 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\x0c\"e\n\x1c\x43reateTemporaryApiKeyRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x12\n\nusage_type\x18\x02 \x01(\t\x12 \n\x18\x63lient_request_reference\x18\x03 \x01(\t\"b\n\x1d\x43reateTemporaryApiKeyResponse\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x10\x65xpires_datetime\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp2\x97\x17\n\rSpeechService\x12\x63\n\nTranscribe\x12(.soniox.speech_service.TranscribeRequest\x1a).soniox.speech_service.TranscribeResponse\"\x00\x12y\n\x10TranscribeStream\x12..soniox.speech_service.TranscribeStreamRequest\x1a/.soniox.speech_service.TranscribeStreamResponse\"\x00(\x01\x30\x01\x12|\n\x11TranscribeMeeting\x12/.soniox.speech_service.TranscribeMeetingRequest\x1a\x30.soniox.speech_service.TranscribeMeetingResponse\"\x00(\x01\x30\x01\x12t\n\x0fTranscribeAsync\x12-.soniox.speech_service.TranscribeAsyncRequest\x1a..soniox.speech_service.TranscribeAsyncResponse\"\x00(\x01\x12\x8d\x01\n\x18GetTranscribeAsyncStatus\x12\x36.soniox.speech_service.GetTranscribeAsyncStatusRequest\x1a\x37.soniox.speech_service.GetTranscribeAsyncStatusResponse\"\x00\x12\x8f\x01\n\x18GetTranscribeAsyncResult\x12\x36.soniox.speech_service.GetTranscribeAsyncResultRequest\x1a\x37.soniox.speech_service.GetTranscribeAsyncResultResponse\"\x00\x30\x01\x12\x90\x01\n\x19\x44\x65leteTranscribeAsyncFile\x12\x37.soniox.speech_service.DeleteTranscribeAsyncFileRequest\x1a\x38.soniox.speech_service.DeleteTranscribeAsyncFileResponse\"\x00\x12~\n\x13\x43reateSpeechContext\x12\x31.soniox.speech_service.CreateSpeechContextRequest\x1a\x32.soniox.speech_service.CreateSpeechContextResponse\"\x00\x12~\n\x13\x44\x65leteSpeechContext\x12\x31.soniox.speech_service.DeleteSpeechContextRequest\x1a\x32.soniox.speech_service.DeleteSpeechContextResponse\"\x00\x12\x87\x01\n\x16ListSpeechContextNames\x12\x34.soniox.speech_service.ListSpeechContextNamesRequest\x1a\x35.soniox.speech_service.ListSpeechContextNamesResponse\"\x00\x12u\n\x10GetSpeechContext\x12..soniox.speech_service.GetSpeechContextRequest\x1a/.soniox.speech_service.GetSpeechContextResponse\"\x00\x12~\n\x13UpdateSpeechContext\x12\x31.soniox.speech_service.UpdateSpeechContextRequest\x1a\x32.soniox.speech_service.UpdateSpeechContextResponse\"\x00\x12\x63\n\nAddSpeaker\x12(.soniox.speech_service.AddSpeakerRequest\x1a).soniox.speech_service.AddSpeakerResponse\"\x00\x12\x63\n\nGetSpeaker\x12(.soniox.speech_service.GetSpeakerRequest\x1a).soniox.speech_service.GetSpeakerResponse\"\x00\x12l\n\rRemoveSpeaker\x12+.soniox.speech_service.RemoveSpeakerRequest\x1a,.soniox.speech_service.RemoveSpeakerResponse\"\x00\x12i\n\x0cListSpeakers\x12*.soniox.speech_service.ListSpeakersRequest\x1a+.soniox.speech_service.ListSpeakersResponse\"\x00\x12r\n\x0f\x41\x64\x64SpeakerAudio\x12-.soniox.speech_service.AddSpeakerAudioRequest\x1a..soniox.speech_service.AddSpeakerAudioResponse\"\x00\x12r\n\x0fGetSpeakerAudio\x12-.soniox.speech_service.GetSpeakerAudioRequest\x1a..soniox.speech_service.GetSpeakerAudioResponse\"\x00\x12{\n\x12RemoveSpeakerAudio\x12\x30.soniox.speech_service.RemoveSpeakerAudioRequest\x1a\x31.soniox.speech_service.RemoveSpeakerAudioResponse\"\x00\x12W\n\x06Search\x12$.soniox.speech_service.SearchRequest\x1a%.soniox.speech_service.SearchResponse\"\x00\x12`\n\tGetObject\x12\'.soniox.speech_service.GetObjectRequest\x1a(.soniox.speech_service.GetObjectResponse\"\x00\x12\x66\n\x0bListObjects\x12).soniox.speech_service.ListObjectsRequest\x1a*.soniox.speech_service.ListObjectsResponse\"\x00\x12i\n\x0c\x44\x65leteObject\x12*.soniox.speech_service.DeleteObjectRequest\x1a+.soniox.speech_service.DeleteObjectResponse\"\x00\x12_\n\x08GetAudio\x12&.soniox.speech_service.GetAudioRequest\x1a\'.soniox.speech_service.GetAudioResponse\"\x00\x30\x01\x12\x84\x01\n\x15\x43reateTemporaryApiKey\x12\x33.soniox.speech_service.CreateTemporaryApiKeyRequest\x1a\x34.soniox.speech_service.CreateTemporaryApiKeyResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bsoniox/speech_service.proto\x12\x15soniox.speech_service\x1a\x1fgoogle/protobuf/timestamp.proto\"o\n\x11TranscribeRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12:\n\x06\x63onfig\x18\x04 \x01(\x0b\x32*.soniox.speech_service.TranscriptionConfig\x12\r\n\x05\x61udio\x18\x03 \x01(\x0c\"\xbb\x01\n\x12TranscribeResponse\x12-\n\x06result\x18\x01 \x01(\x0b\x32\x1d.soniox.speech_service.Result\x12\x36\n\x0f\x63hannel_results\x18\x02 \x03(\x0b\x32\x1d.soniox.speech_service.Result\x12>\n\x08metadata\x18\x03 \x01(\x0b\x32,.soniox.speech_service.TranscriptionMetadata\"u\n\x17TranscribeStreamRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12:\n\x06\x63onfig\x18\x04 \x01(\x0b\x32*.soniox.speech_service.TranscriptionConfig\x12\r\n\x05\x61udio\x18\x03 \x01(\x0c\"\x89\x01\n\x18TranscribeStreamResponse\x12-\n\x06result\x18\x01 \x01(\x0b\x32\x1d.soniox.speech_service.Result\x12>\n\x08metadata\x18\x02 \x01(\x0b\x32,.soniox.speech_service.TranscriptionMetadata\"\xcc\x01\n\x18TranscribeMeetingRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12:\n\x06\x63onfig\x18\n \x01(\x0b\x32*.soniox.speech_service.TranscriptionConfig\x12\x0f\n\x07seq_num\x18\x03 \x01(\x05\x12\x11\n\tstream_id\x18\x04 \x01(\x05\x12\x18\n\x10start_of_segment\x18\x05 \x01(\x08\x12\r\n\x05\x61udio\x18\x06 \x01(\x0c\x12\x16\n\x0e\x65nd_of_segment\x18\x07 \x01(\x08\"\xef\x01\n\x19TranscribeMeetingResponse\x12\x0f\n\x07seq_num\x18\x01 \x01(\x05\x12\x11\n\tstream_id\x18\x02 \x01(\x05\x12\x18\n\x10start_of_segment\x18\x03 \x01(\x08\x12\x16\n\x0e\x65nd_of_segment\x18\x04 \x01(\x08\x12-\n\x06result\x18\x05 \x01(\x0b\x32\x1d.soniox.speech_service.Result\x12\r\n\x05\x65rror\x18\x06 \x01(\t\x12>\n\x08metadata\x18\x07 \x01(\x0b\x32,.soniox.speech_service.TranscriptionMetadata\"\xad\x01\n\x16TranscribeAsyncRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x16\n\x0ereference_name\x18\x03 \x01(\t\x12:\n\x06\x63onfig\x18\x05 \x01(\x0b\x32*.soniox.speech_service.TranscriptionConfig\x12\x12\n\nenable_eof\x18\x06 \x01(\x08\x12\x0b\n\x03\x65of\x18\x07 \x01(\x08\x12\r\n\x05\x61udio\x18\x04 \x01(\x0c\"*\n\x17TranscribeAsyncResponse\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\"C\n\x1fGetTranscribeAsyncStatusRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"c\n GetTranscribeAsyncStatusResponse\x12?\n\x05\x66iles\x18\x01 \x03(\x0b\x32\x30.soniox.speech_service.TranscribeAsyncFileStatus\"\x9d\x01\n\x19TranscribeAsyncFileStatus\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x16\n\x0ereference_name\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x30\n\x0c\x63reated_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rerror_message\x18\x05 \x01(\t\"C\n\x1fGetTranscribeAsyncResultRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"\xbb\x01\n GetTranscribeAsyncResultResponse\x12(\n separate_recognition_per_channel\x18\x02 \x01(\x08\x12-\n\x06result\x18\x01 \x01(\x0b\x32\x1d.soniox.speech_service.Result\x12>\n\x08metadata\x18\x03 \x01(\x0b\x32,.soniox.speech_service.TranscriptionMetadata\"D\n DeleteTranscribeAsyncFileRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"#\n!DeleteTranscribeAsyncFileResponse\"\xad\x05\n\x13TranscriptionConfig\x12 \n\x18\x63lient_request_reference\x18\x13 \x01(\t\x12\x14\n\x0c\x61udio_format\x18\x01 \x01(\t\x12\x19\n\x11sample_rate_hertz\x18\x02 \x01(\x05\x12\x1a\n\x12num_audio_channels\x18\x03 \x01(\x05\x12\x18\n\x10include_nonfinal\x18\x04 \x01(\x08\x12/\n\'enable_separate_recognition_per_channel\x18\x10 \x01(\x08\x12!\n\x19\x65nable_endpoint_detection\x18\x12 \x01(\x08\x12<\n\x0espeech_context\x18\x05 \x01(\x0b\x32$.soniox.speech_service.SpeechContext\x12\x1f\n\x17\x65nable_profanity_filter\x18\x06 \x01(\x08\x12\"\n\x1a\x63ontent_moderation_phrases\x18\x07 \x03(\t\x12,\n$enable_streaming_speaker_diarization\x18\x08 \x01(\x08\x12)\n!enable_global_speaker_diarization\x18\t \x01(\x08\x12\x18\n\x10min_num_speakers\x18\n \x01(\x05\x12\x18\n\x10max_num_speakers\x18\x0b \x01(\x05\x12%\n\x1d\x65nable_speaker_identification\x18\x0c \x01(\x08\x12\x1a\n\x12\x63\x61nd_speaker_names\x18\r \x03(\t\x12\r\n\x05model\x18\x0e \x01(\t\x12\x18\n\x10\x65nable_dictation\x18\x0f \x01(\x08\x12=\n\x0estorage_config\x18\xee\x07 \x01(\x0b\x32$.soniox.speech_service.StorageConfig\"0\n\x15TranscriptionMetadata\x12\x17\n\x0fpackage_version\x18\x01 \x01(\t\"\xb5\x01\n\x06Result\x12*\n\x05words\x18\x01 \x03(\x0b\x32\x1b.soniox.speech_service.Word\x12\x1a\n\x12\x66inal_proc_time_ms\x18\x02 \x01(\x05\x12\x1a\n\x12total_proc_time_ms\x18\x03 \x01(\x05\x12\x36\n\x08speakers\x18\x06 \x03(\x0b\x32$.soniox.speech_service.ResultSpeaker\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\x05\"\x85\x01\n\x04Word\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x10\n\x08start_ms\x18\x02 \x01(\x05\x12\x13\n\x0b\x64uration_ms\x18\x03 \x01(\x05\x12\x10\n\x08is_final\x18\x04 \x01(\x08\x12\x0f\n\x07speaker\x18\x05 \x01(\x05\x12\x11\n\torig_text\x18\x08 \x01(\t\x12\x12\n\nconfidence\x18\t \x01(\x01\".\n\rResultSpeaker\x12\x0f\n\x07speaker\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\"Y\n\rSpeechContext\x12:\n\x07\x65ntries\x18\x01 \x03(\x0b\x32).soniox.speech_service.SpeechContextEntry\x12\x0c\n\x04name\x18\x02 \x01(\t\"4\n\x12SpeechContextEntry\x12\x0f\n\x07phrases\x18\x01 \x03(\t\x12\r\n\x05\x62oost\x18\x02 \x01(\x01\"k\n\x1a\x43reateSpeechContextRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12<\n\x0espeech_context\x18\x02 \x01(\x0b\x32$.soniox.speech_service.SpeechContext\"\x1d\n\x1b\x43reateSpeechContextResponse\";\n\x1a\x44\x65leteSpeechContextRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x1d\n\x1b\x44\x65leteSpeechContextResponse\"0\n\x1dListSpeechContextNamesRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\"/\n\x1eListSpeechContextNamesResponse\x12\r\n\x05names\x18\x01 \x03(\t\"8\n\x17GetSpeechContextRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"X\n\x18GetSpeechContextResponse\x12<\n\x0espeech_context\x18\x01 \x01(\x0b\x32$.soniox.speech_service.SpeechContext\"k\n\x1aUpdateSpeechContextRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12<\n\x0espeech_context\x18\x02 \x01(\x0b\x32$.soniox.speech_service.SpeechContext\"\x1d\n\x1bUpdateSpeechContextResponse\"2\n\x11\x41\x64\x64SpeakerRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"O\n\x12\x41\x64\x64SpeakerResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\x07\x63reated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"2\n\x11GetSpeakerRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x8f\x01\n\x12GetSpeakerResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\x07\x63reated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12>\n\x06\x61udios\x18\x03 \x03(\x0b\x32..soniox.speech_service.GetSpeakerResponseAudio\"o\n\x17GetSpeakerResponseAudio\x12\x12\n\naudio_name\x18\x01 \x01(\t\x12+\n\x07\x63reated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64uration_ms\x18\x03 \x01(\x05\"5\n\x14RemoveSpeakerRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x17\n\x15RemoveSpeakerResponse\"&\n\x13ListSpeakersRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\"\\\n\x14ListSpeakersResponse\x12\x44\n\x08speakers\x18\x01 \x03(\x0b\x32\x32.soniox.speech_service.ListSpeakersResponseSpeaker\"l\n\x1bListSpeakersResponseSpeaker\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\x07\x63reated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nnum_audios\x18\x03 \x01(\x05\"b\n\x16\x41\x64\x64SpeakerAudioRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x14\n\x0cspeaker_name\x18\x02 \x01(\t\x12\x12\n\naudio_name\x18\x03 \x01(\t\x12\r\n\x05\x61udio\x18\x04 \x01(\x0c\"\x85\x01\n\x17\x41\x64\x64SpeakerAudioResponse\x12\x14\n\x0cspeaker_name\x18\x01 \x01(\t\x12\x12\n\naudio_name\x18\x02 \x01(\t\x12+\n\x07\x63reated\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64uration_ms\x18\x04 \x01(\x05\"S\n\x16GetSpeakerAudioRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x14\n\x0cspeaker_name\x18\x02 \x01(\t\x12\x12\n\naudio_name\x18\x03 \x01(\t\"\x94\x01\n\x17GetSpeakerAudioResponse\x12\x14\n\x0cspeaker_name\x18\x01 \x01(\t\x12\x12\n\naudio_name\x18\x02 \x01(\t\x12+\n\x07\x63reated\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64uration_ms\x18\x04 \x01(\x05\x12\r\n\x05\x61udio\x18\x05 \x01(\x0c\"V\n\x19RemoveSpeakerAudioRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x14\n\x0cspeaker_name\x18\x02 \x01(\t\x12\x12\n\naudio_name\x18\x03 \x01(\t\"\x1c\n\x1aRemoveSpeakerAudioResponse\"\x95\x02\n\rStorageConfig\x12\x11\n\tobject_id\x18\x01 \x01(\t\x12\x44\n\x08metadata\x18\x02 \x03(\x0b\x32\x32.soniox.speech_service.StorageConfig.MetadataEntry\x12\r\n\x05title\x18\x03 \x01(\t\x12,\n\x08\x64\x61tetime\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x13\x64isable_store_audio\x18\x05 \x01(\x08\x12 \n\x18\x64isable_store_transcript\x18\x06 \x01(\x08\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xa8\x01\n\x05Token\x12\x0b\n\x03idx\x18\x01 \x01(\x05\x12\x12\n\ntext_start\x18\x02 \x01(\x05\x12\x10\n\x08text_end\x18\x03 \x01(\x05\x12\x0c\n\x04text\x18\x04 \x01(\t\x12\x10\n\x08start_ms\x18\x05 \x01(\x05\x12\x13\n\x0b\x64uration_ms\x18\x06 \x01(\x05\x12\x12\n\nconfidence\x18\x07 \x01(\x01\x12\x12\n\nspeaker_id\x18\x08 \x01(\x05\x12\x0f\n\x07profane\x18\t \x01(\x08\"2\n\x08Sentence\x12\x13\n\x0btoken_start\x18\x01 \x01(\x05\x12\x11\n\ttoken_end\x18\x02 \x01(\x05\"9\n\tParagraph\x12\x16\n\x0esentence_start\x18\x01 \x01(\x05\x12\x14\n\x0csentence_end\x18\x02 \x01(\x05\"C\n\x07Keyterm\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\r\n\x05score\x18\x02 \x01(\x01\x12\x1b\n\x13token_start_indexes\x18\x03 \x03(\x05\"\xe5\x02\n\nTranscript\x12\x0c\n\x04text\x18\x01 \x01(\t\x12,\n\x06tokens\x18\x02 \x03(\x0b\x32\x1c.soniox.speech_service.Token\x12\x32\n\tsentences\x18\x03 \x03(\x0b\x32\x1f.soniox.speech_service.Sentence\x12\x34\n\nparagraphs\x18\x04 \x03(\x0b\x32 .soniox.speech_service.Paragraph\x12\x30\n\x08keyterms\x18\x06 \x03(\x0b\x32\x1e.soniox.speech_service.Keyterm\x12J\n\rspeaker_names\x18\x07 \x03(\x0b\x32\x33.soniox.speech_service.Transcript.SpeakerNamesEntry\x1a\x33\n\x11SpeakerNamesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x87\x03\n\x0cStoredObject\x12\x11\n\tobject_id\x18\x01 \x01(\t\x12\x43\n\x08metadata\x18\x02 \x03(\x0b\x32\x31.soniox.speech_service.StoredObject.MetadataEntry\x12\r\n\x05title\x18\x03 \x01(\t\x12,\n\x08\x64\x61tetime\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0fstored_datetime\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64uration_ms\x18\x06 \x01(\x05\x12\x1a\n\x12num_audio_channels\x18\n \x01(\x05\x12\x14\n\x0c\x61udio_stored\x18\x0b \x01(\x08\x12\x35\n\ntranscript\x18\x07 \x01(\x0b\x32!.soniox.speech_service.Transcript\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xdf\x01\n\rSearchRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x11\n\tobject_id\x18\x02 \x01(\t\x12\x16\n\x0emetadata_query\x18\x03 \x01(\t\x12\x31\n\rdatetime_from\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0b\x64\x61tetime_to\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ntext_query\x18\x06 \x01(\t\x12\r\n\x05start\x18\x07 \x01(\x05\x12\x0b\n\x03num\x18\x08 \x01(\x05\"\xfa\x01\n\x0cSearchResult\x12\x11\n\tobject_id\x18\x01 \x01(\t\x12\x43\n\x08metadata\x18\x02 \x03(\x0b\x32\x31.soniox.speech_service.SearchResult.MetadataEntry\x12\r\n\x05title\x18\x03 \x01(\t\x12,\n\x08\x64\x61tetime\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64uration_ms\x18\x05 \x01(\x05\x12\x0f\n\x07preview\x18\x06 \x01(\t\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"h\n\x0eSearchResponse\x12\x11\n\tnum_found\x18\x01 \x01(\x05\x12\r\n\x05start\x18\x02 \x01(\x05\x12\x34\n\x07results\x18\x03 \x03(\x0b\x32#.soniox.speech_service.SearchResult\"6\n\x10GetObjectRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x11\n\tobject_id\x18\x02 \x01(\t\"H\n\x11GetObjectResponse\x12\x33\n\x06object\x18\x01 \x01(\x0b\x32#.soniox.speech_service.StoredObject\"\xb3\x01\n\x12ListObjectsRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x38\n\x14stored_datetime_from\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x36\n\x12stored_datetime_to\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05start\x18\x04 \x01(\x03\x12\x0b\n\x03num\x18\x05 \x01(\x03\"g\n\x13ListObjectsResponse\x12\r\n\x05start\x18\x01 \x01(\x03\x12\x41\n\x07objects\x18\x02 \x03(\x0b\x32\x30.soniox.speech_service.ListObjectsResponseObject\"\xc8\x01\n\x19ListObjectsResponseObject\x12\x11\n\tobject_id\x18\x01 \x01(\t\x12\x33\n\x0fstored_datetime\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0c\x61udio_stored\x18\x03 \x01(\x08\x12\x19\n\x11transcript_stored\x18\x04 \x01(\x08\x12\x19\n\x11\x61udio_duration_ms\x18\x05 \x01(\x05\x12\x17\n\x0fstored_audio_ms\x18\x06 \x01(\x05\"9\n\x13\x44\x65leteObjectRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x11\n\tobject_id\x18\x02 \x01(\t\"\x16\n\x14\x44\x65leteObjectResponse\"\xea\x02\n\x0fGetAudioRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x11\n\tobject_id\x18\x02 \x01(\t\x12J\n\x0ctime_segment\x18\x03 \x01(\x0b\x32\x32.soniox.speech_service.GetAudioRequest.TimeSegmentH\x00\x12L\n\rtoken_segment\x18\x04 \x01(\x0b\x32\x33.soniox.speech_service.GetAudioRequest.TokenSegmentH\x00\x12\x1a\n\x12\x61udio_bytes_format\x18\x05 \x01(\t\x1a\x34\n\x0bTimeSegment\x12\x10\n\x08start_ms\x18\x01 \x01(\x05\x12\x13\n\x0b\x64uration_ms\x18\x02 \x01(\x05\x1a\x36\n\x0cTokenSegment\x12\x13\n\x0btoken_start\x18\x01 \x01(\x05\x12\x11\n\ttoken_end\x18\x02 \x01(\x05\x42\x0f\n\roneof_segment\"\x91\x01\n\x10GetAudioResponse\x12\x11\n\tobject_id\x18\x01 \x01(\t\x12\x10\n\x08start_ms\x18\x02 \x01(\x05\x12\x13\n\x0b\x64uration_ms\x18\x03 \x01(\x05\x12\x19\n\x11total_duration_ms\x18\x04 \x01(\x05\x12\x1a\n\x12num_audio_channels\x18\x06 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\x0c\"{\n\x1c\x43reateTemporaryApiKeyRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x12\n\nusage_type\x18\x02 \x01(\t\x12\x14\n\x0c\x65xpires_in_s\x18\x04 \x01(\x05\x12 \n\x18\x63lient_request_reference\x18\x03 \x01(\t\"b\n\x1d\x43reateTemporaryApiKeyResponse\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x10\x65xpires_datetime\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp2\x97\x17\n\rSpeechService\x12\x63\n\nTranscribe\x12(.soniox.speech_service.TranscribeRequest\x1a).soniox.speech_service.TranscribeResponse\"\x00\x12y\n\x10TranscribeStream\x12..soniox.speech_service.TranscribeStreamRequest\x1a/.soniox.speech_service.TranscribeStreamResponse\"\x00(\x01\x30\x01\x12|\n\x11TranscribeMeeting\x12/.soniox.speech_service.TranscribeMeetingRequest\x1a\x30.soniox.speech_service.TranscribeMeetingResponse\"\x00(\x01\x30\x01\x12t\n\x0fTranscribeAsync\x12-.soniox.speech_service.TranscribeAsyncRequest\x1a..soniox.speech_service.TranscribeAsyncResponse\"\x00(\x01\x12\x8d\x01\n\x18GetTranscribeAsyncStatus\x12\x36.soniox.speech_service.GetTranscribeAsyncStatusRequest\x1a\x37.soniox.speech_service.GetTranscribeAsyncStatusResponse\"\x00\x12\x8f\x01\n\x18GetTranscribeAsyncResult\x12\x36.soniox.speech_service.GetTranscribeAsyncResultRequest\x1a\x37.soniox.speech_service.GetTranscribeAsyncResultResponse\"\x00\x30\x01\x12\x90\x01\n\x19\x44\x65leteTranscribeAsyncFile\x12\x37.soniox.speech_service.DeleteTranscribeAsyncFileRequest\x1a\x38.soniox.speech_service.DeleteTranscribeAsyncFileResponse\"\x00\x12~\n\x13\x43reateSpeechContext\x12\x31.soniox.speech_service.CreateSpeechContextRequest\x1a\x32.soniox.speech_service.CreateSpeechContextResponse\"\x00\x12~\n\x13\x44\x65leteSpeechContext\x12\x31.soniox.speech_service.DeleteSpeechContextRequest\x1a\x32.soniox.speech_service.DeleteSpeechContextResponse\"\x00\x12\x87\x01\n\x16ListSpeechContextNames\x12\x34.soniox.speech_service.ListSpeechContextNamesRequest\x1a\x35.soniox.speech_service.ListSpeechContextNamesResponse\"\x00\x12u\n\x10GetSpeechContext\x12..soniox.speech_service.GetSpeechContextRequest\x1a/.soniox.speech_service.GetSpeechContextResponse\"\x00\x12~\n\x13UpdateSpeechContext\x12\x31.soniox.speech_service.UpdateSpeechContextRequest\x1a\x32.soniox.speech_service.UpdateSpeechContextResponse\"\x00\x12\x63\n\nAddSpeaker\x12(.soniox.speech_service.AddSpeakerRequest\x1a).soniox.speech_service.AddSpeakerResponse\"\x00\x12\x63\n\nGetSpeaker\x12(.soniox.speech_service.GetSpeakerRequest\x1a).soniox.speech_service.GetSpeakerResponse\"\x00\x12l\n\rRemoveSpeaker\x12+.soniox.speech_service.RemoveSpeakerRequest\x1a,.soniox.speech_service.RemoveSpeakerResponse\"\x00\x12i\n\x0cListSpeakers\x12*.soniox.speech_service.ListSpeakersRequest\x1a+.soniox.speech_service.ListSpeakersResponse\"\x00\x12r\n\x0f\x41\x64\x64SpeakerAudio\x12-.soniox.speech_service.AddSpeakerAudioRequest\x1a..soniox.speech_service.AddSpeakerAudioResponse\"\x00\x12r\n\x0fGetSpeakerAudio\x12-.soniox.speech_service.GetSpeakerAudioRequest\x1a..soniox.speech_service.GetSpeakerAudioResponse\"\x00\x12{\n\x12RemoveSpeakerAudio\x12\x30.soniox.speech_service.RemoveSpeakerAudioRequest\x1a\x31.soniox.speech_service.RemoveSpeakerAudioResponse\"\x00\x12W\n\x06Search\x12$.soniox.speech_service.SearchRequest\x1a%.soniox.speech_service.SearchResponse\"\x00\x12`\n\tGetObject\x12\'.soniox.speech_service.GetObjectRequest\x1a(.soniox.speech_service.GetObjectResponse\"\x00\x12\x66\n\x0bListObjects\x12).soniox.speech_service.ListObjectsRequest\x1a*.soniox.speech_service.ListObjectsResponse\"\x00\x12i\n\x0c\x44\x65leteObject\x12*.soniox.speech_service.DeleteObjectRequest\x1a+.soniox.speech_service.DeleteObjectResponse\"\x00\x12_\n\x08GetAudio\x12&.soniox.speech_service.GetAudioRequest\x1a\'.soniox.speech_service.GetAudioResponse\"\x00\x30\x01\x12\x84\x01\n\x15\x43reateTemporaryApiKey\x12\x33.soniox.speech_service.CreateTemporaryApiKeyRequest\x1a\x34.soniox.speech_service.CreateTemporaryApiKeyResponse\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'soniox.speech_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _STORAGECONFIG_METADATAENTRY._options = None
@@ -172,13 +172,13 @@
   _GETAUDIOREQUEST_TIMESEGMENT._serialized_start=8153
   _GETAUDIOREQUEST_TIMESEGMENT._serialized_end=8205
   _GETAUDIOREQUEST_TOKENSEGMENT._serialized_start=8207
   _GETAUDIOREQUEST_TOKENSEGMENT._serialized_end=8261
   _GETAUDIORESPONSE._serialized_start=8281
   _GETAUDIORESPONSE._serialized_end=8426
   _CREATETEMPORARYAPIKEYREQUEST._serialized_start=8428
-  _CREATETEMPORARYAPIKEYREQUEST._serialized_end=8529
-  _CREATETEMPORARYAPIKEYRESPONSE._serialized_start=8531
-  _CREATETEMPORARYAPIKEYRESPONSE._serialized_end=8629
-  _SPEECHSERVICE._serialized_start=8632
-  _SPEECHSERVICE._serialized_end=11599
+  _CREATETEMPORARYAPIKEYREQUEST._serialized_end=8551
+  _CREATETEMPORARYAPIKEYRESPONSE._serialized_start=8553
+  _CREATETEMPORARYAPIKEYRESPONSE._serialized_end=8651
+  _SPEECHSERVICE._serialized_start=8654
+  _SPEECHSERVICE._serialized_end=11621
 # @@protoc_insertion_point(module_scope)
```

### Comparing `soniox-1.8.0/soniox/speech_service_pb2_grpc.py` & `soniox-1.8.1/soniox/speech_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `soniox-1.8.0/soniox/storage.py` & `soniox-1.8.1/soniox/storage.py`

 * *Files identical despite different names*

### Comparing `soniox-1.8.0/soniox/transcribe_file.py` & `soniox-1.8.1/soniox/transcribe_file.py`

 * *Files identical despite different names*

### Comparing `soniox-1.8.0/soniox/transcribe_live.py` & `soniox-1.8.1/soniox/transcribe_live.py`

 * *Files identical despite different names*

### Comparing `soniox-1.8.0/soniox.egg-info/PKG-INFO` & `soniox-1.8.1/soniox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soniox
-Version: 1.8.0
+Version: 1.8.1
 Summary: Soniox speech recognition service client library
 Home-page: https://soniox.com/
 Author: Soniox Inc
 Author-email: support@soniox.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

