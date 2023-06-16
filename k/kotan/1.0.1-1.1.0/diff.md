# Comparing `tmp/kotan-1.0.1.tar.gz` & `tmp/kotan-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kotan-1.0.1.tar", max compression
+gzip compressed data, was "kotan-1.1.0.tar", max compression
```

## Comparing `kotan-1.0.1.tar` & `kotan-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-06-13 08:18:12.690062 kotan-1.0.1/README.md
--rw-r--r--   0        0        0       45 2023-06-13 08:18:12.690062 kotan-1.0.1/kotan/__init__.py
--rw-r--r--   0        0        0      749 2023-06-13 08:18:12.690062 kotan-1.0.1/kotan/const.py
--rw-r--r--   0        0        0     2727 2023-06-13 08:18:12.690062 kotan-1.0.1/kotan/job.py
--rw-r--r--   0        0        0      168 2023-06-13 08:18:12.690062 kotan-1.0.1/kotan/tasks/__init__.py
--rw-r--r--   0        0        0     4300 2023-06-13 08:18:12.690062 kotan-1.0.1/kotan/tasks/data_augmentation.py
--rw-r--r--   0        0        0     2063 2023-06-13 08:18:12.690062 kotan-1.0.1/kotan/tasks/machine_translation.py
--rw-r--r--   0        0        0     2208 2023-06-13 08:18:12.690062 kotan-1.0.1/kotan/tasks/style_convert.py
--rw-r--r--   0        0        0      327 2023-06-13 08:19:28.813300 kotan-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 kotan-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-16 06:27:17.818625 kotan-1.1.0/README.md
+-rw-r--r--   0        0        0       45 2023-06-16 06:28:13.158078 kotan-1.1.0/kotan/__init__.py
+-rw-r--r--   0        0        0      749 2023-06-16 06:27:17.818625 kotan-1.1.0/kotan/const.py
+-rw-r--r--   0        0        0     2727 2023-06-16 06:27:17.818625 kotan-1.1.0/kotan/job.py
+-rw-r--r--   0        0        0      168 2023-06-16 06:27:17.818625 kotan-1.1.0/kotan/tasks/__init__.py
+-rw-r--r--   0        0        0     5018 2023-06-16 06:27:17.818625 kotan-1.1.0/kotan/tasks/data_augmentation.py
+-rw-r--r--   0        0        0     3586 2023-06-16 06:27:17.818625 kotan-1.1.0/kotan/tasks/machine_translation.py
+-rw-r--r--   0        0        0     2208 2023-06-16 06:27:17.818625 kotan-1.1.0/kotan/tasks/style_convert.py
+-rw-r--r--   0        0        0      344 2023-06-16 06:28:07.658132 kotan-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 kotan-1.1.0/PKG-INFO
```

### Comparing `kotan-1.0.1/kotan/const.py` & `kotan-1.1.0/kotan/const.py`

 * *Files identical despite different names*

### Comparing `kotan-1.0.1/kotan/job.py` & `kotan-1.1.0/kotan/job.py`

 * *Files identical despite different names*

### Comparing `kotan-1.0.1/kotan/tasks/data_augmentation.py` & `kotan-1.1.0/kotan/tasks/data_augmentation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from transformers import AutoTokenizer, AutoModelForSeq2SeqLM
-from transformers import pipeline
+from konlpy.tag import Twitter
+import numpy as np
 
 class KoTANAugmentationFactory:
     """
     Text augmentation using facebook/nllb-200-distilled-600M Meta model
 
     - dataset: Train
 
@@ -17,21 +18,20 @@
         >>> mt = KoTAN(task="augmentation", level="fine")
     """
 
     def __init__(self, 
                  task, 
                  tgt, 
                  level,
-                 style = None,
+                 style
                  ):
         super().__init__()
         self.task = task
         self.tgt = tgt
         self.level = level
-        self.style = style
 
     def load(self, device):
         if self.level == "fine":
             ko2en_tokenizer = AutoTokenizer.from_pretrained("NHNDQ/nllb-finetuned-ko2en")
             en2ko_tokenizer = AutoTokenizer.from_pretrained("NHNDQ/nllb-finetuned-en2ko")
 
             ko2en_model = AutoModelForSeq2SeqLM.from_pretrained("NHNDQ/nllb-finetuned-ko2en").to(device)
@@ -40,92 +40,124 @@
         
         elif self.level == "origin":
             ko2en_tokenizer = AutoTokenizer.from_pretrained("facebook/nllb-200-distilled-600M", src_lang="kor_Hang", tgt_lang="eng_Latn")
             en2ko_tokenizer = AutoTokenizer.from_pretrained("facebook/nllb-200-distilled-600M", src_lang="eng_Latn", tgt_lang="kor_Hang")
 
             ko2en_model = AutoModelForSeq2SeqLM.from_pretrained("facebook/nllb-200-distilled-600M").to(device)
             en2ko_model = AutoModelForSeq2SeqLM.from_pretrained("facebook/nllb-200-distilled-600M").to(device)
-
-        if self.style == None:
-            style = None
-            style_transfer_pipeline = None
-        else:
-            style = self.style
-            style_checkpoint = "NHNDQ/bart-speech-style-converter"
-            style_tokenizer = AutoTokenizer.from_pretrained(style_checkpoint)
-            style_transfer_pipeline = pipeline('text2text-generation',model=style_checkpoint, tokenizer=style_tokenizer)
-
+        
 
         return KoTANAugmentation(
             ko2en_tokenizer, en2ko_tokenizer,
             ko2en_model, en2ko_model, 
-            style, style_transfer_pipeline,
             device
         )
 
 
 class KoTANAugmentation:
     def __init__(self, 
                  ko2en_tokenizer, en2ko_tokenizer,
                  ko2en_model, en2ko_model, 
-                 style, style_transfer_pipeline,
                  device):
         self.ko2en_tokenizer = ko2en_tokenizer
         self.en2ko_tokenizer = en2ko_tokenizer
 
         self.ko2en_model = ko2en_model
         self.en2ko_model = en2ko_model
 
-        self.style = style
-        self.style_transfer_pipeline = style_transfer_pipeline
-
         self.device = device
 
     def predict(self, text):
         """
         Predict a backtranslation result
 
         Args:
             text (str): input text
 
         Returns:
             output (list): Backtranslation results
-        """
-
-        # ko2en
-        translation = self._translate(text, 'eng_Latn', self.ko2en_tokenizer, self.ko2en_model)
+        """       
 
-        # en2ko
-        backtranslation = self._translate(translation, 'kor_Hang', self.en2ko_tokenizer, self.en2ko_model)
+        # post-processing
+        post_process_output = []
+        
+        for i in range(len(text)):
+            emojiList, textList = self._post_process(text[i])
+            # ko2en
+            translation = self._translate(textList, 'eng_Latn', self.ko2en_tokenizer, self.ko2en_model)
+            # en2ko
+            augList = self._translate(translation, 'kor_Hang', self.en2ko_tokenizer, self.en2ko_model)
+            outList = []
+            for emo, txt in zip(emojiList, augList):
+                output = txt + emo
+                outList.append(output)
+                output = ''.join(outList).strip()
+            post_process_output.append(output)
 
-        # style transfer
-        if self.style_transfer_pipeline != None:
-            style_transfer = self._style_transfer(backtranslation, self.style_transfer_pipeline, self.style)
-            return style_transfer
-        else:
-            return backtranslation
+        return post_process_output
 
 
     def _translate(self, text, tgt, tokenizer, model):
 
         # translation
         inputs = tokenizer(text, padding=True, truncation=True, return_tensors="pt")
         inputs = inputs.to(self.device)
         translated_tokens = model.generate(
             inputs['input_ids'], forced_bos_token_id=tokenizer.lang_code_to_id[tgt], max_length=128
         )
 
         translation = tokenizer.batch_decode(translated_tokens, skip_special_tokens=True)
-        
-        return translation
-    
-    def _style_transfer(self, text, pipeline, style):
-        text = [f"{style} 형식으로 변환:{sentence}" for sentence in text]
-        out = pipeline(text, max_length=100)
-        out = [ sentence['generated_text'] for sentence in out ]
-        return out
-
-
-
 
+        post_output = []
 
+        for inp, outp in zip(text, translation):
+            if inp == '':
+                post_output.append('')
+            else:
+                post_output.append(outp)
         
+        return post_output
+
+    
+    def _post_process(self, text):
+        textList = []
+        emojiList = []
+        twit = Twitter()
+
+        posText = twit.pos(text)
+        posArray = np.array(posText)
+
+        for i in range(len(posArray)):
+            if posArray[i][1] == 'KoreanParticle':
+                emojiList.append(posArray[i][0])
+
+        for i in range(len(emojiList)):
+            splitText = text.split(emojiList[i], maxsplit=1)
+
+            if splitText[0] == '':
+                textList.append('')
+            else:
+                textList.append(splitText[0])
+
+            try:
+                if len(splitText[1:]) > 1:
+                    text = ''.join(splitText[1:]).strip()
+                else:
+                    text = splitText[1:][0].strip()
+
+            except:
+                break
+
+            try:
+                if text in emojiList[i+1]:
+                    pass
+            except:
+                textList.append(splitText[-1])
+                emojiList.append('')
+                break
+
+        ## 이모지 없는 경우            
+        if len(emojiList) < 1:
+            emojiList.append('')
+            textList.append(text)
+                
+        return emojiList, textList
```

### Comparing `kotan-1.0.1/kotan/tasks/style_convert.py` & `kotan-1.1.0/kotan/tasks/style_convert.py`

 * *Files identical despite different names*

### Comparing `kotan-1.0.1/PKG-INFO` & `kotan-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: kotan
-Version: 1.0.1
+Version: 1.1.0
 Summary: 
 Author: jisukim
 Author-email: jisukim8873@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: konlpy (==0.6.0)
 Requires-Dist: sentencepiece (>=0.1.99,<0.2.0)
 Requires-Dist: torch (==2.0.0)
 Requires-Dist: transformers (>=4.29.1,<5.0.0)
 Description-Content-Type: text/markdown
```

