# Comparing `tmp/neon-skill-audio_record-0.1.1a1.tar.gz` & `tmp/neon-skill-audio_record-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-audio_record-0.1.1a1.tar", last modified: Thu Jun 15 22:34:41 2023, max compression
+gzip compressed data, was "neon-skill-audio_record-0.1.1a2.tar", last modified: Thu Jun 15 22:38:39 2023, max compression
```

## Comparing `neon-skill-audio_record-0.1.1a1.tar` & `neon-skill-audio_record-0.1.1a2.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.648545 neon-skill-audio_record-0.1.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-15 22:34:41.648545 neon-skill-audio_record-0.1.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    25739 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.628544 neon-skill-audio_record-0.1.1a1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.628544 neon-skill-audio_record-0.1.1a1/locale/ca-es/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/ca-es/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/ca-es/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/ca-es/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/ca-es/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/ca-es/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/ca-es/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/ca-es/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/ca-es/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/ca-es/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.632545 neon-skill-audio_record-0.1.1a1/locale/cs-cz/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/cs-cz/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/cs-cz/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/cs-cz/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/cs-cz/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/cs-cz/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/cs-cz/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/cs-cz/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/cs-cz/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/cs-cz/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.632545 neon-skill-audio_record-0.1.1a1/locale/da-dk/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/da-dk/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/da-dk/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/da-dk/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/da-dk/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/da-dk/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/da-dk/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/da-dk/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/da-dk/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/da-dk/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.632545 neon-skill-audio_record-0.1.1a1/locale/de-de/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/de-de/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/de-de/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/de-de/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/de-de/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/de-de/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/de-de/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/de-de/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/de-de/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/de-de/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.632545 neon-skill-audio_record-0.1.1a1/locale/el-gr/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/el-gr/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/el-gr/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/el-gr/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/el-gr/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/el-gr/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/el-gr/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/el-gr/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/el-gr/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/el-gr/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.636545 neon-skill-audio_record-0.1.1a1/locale/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/Audio.voc
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/AudioRecordSkillDeleteVerb.voc
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/AudioRecordSkillKeyword.voc
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/AudioRecordSkillListKeyword.voc
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/AudioRecordSkillPlayVerb.voc
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/AudioRecordSkillStopVerb.voc
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/ConfirmFilename.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/ConfirmNo.voc
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/ConfirmYes.voc
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/FileExists.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/Neon.voc
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/Record.voc
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/ResumeKeyword.voc
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/audio.record.start.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/audio.record.start.duration.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/audio.record.stop.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/en-us/audio.record.stop.play.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.636545 neon-skill-audio_record-0.1.1a1/locale/es-es/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/es-es/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/es-es/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/es-es/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/es-es/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/es-es/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/es-es/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/es-es/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/es-es/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/es-es/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.640545 neon-skill-audio_record-0.1.1a1/locale/es-lm/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/es-lm/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/es-lm/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/es-lm/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/es-lm/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/es-lm/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/es-lm/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/es-lm/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/es-lm/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/es-lm/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.640545 neon-skill-audio_record-0.1.1a1/locale/eu-eu/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/eu-eu/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/eu-eu/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/eu-eu/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/eu-eu/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/eu-eu/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/eu-eu/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/eu-eu/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/eu-eu/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/eu-eu/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.640545 neon-skill-audio_record-0.1.1a1/locale/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/fr-fr/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/fr-fr/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/fr-fr/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/fr-fr/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/fr-fr/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/fr-fr/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/fr-fr/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/fr-fr/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/fr-fr/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.640545 neon-skill-audio_record-0.1.1a1/locale/gl-es/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/gl-es/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/gl-es/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/gl-es/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/gl-es/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/gl-es/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/gl-es/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/gl-es/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/gl-es/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/gl-es/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.644545 neon-skill-audio_record-0.1.1a1/locale/hu-hu/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/hu-hu/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/hu-hu/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/hu-hu/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/hu-hu/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/hu-hu/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/hu-hu/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/hu-hu/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/hu-hu/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/hu-hu/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.644545 neon-skill-audio_record-0.1.1a1/locale/it-it/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/it-it/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/it-it/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/it-it/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/it-it/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/it-it/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/it-it/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/it-it/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/it-it/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/it-it/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.644545 neon-skill-audio_record-0.1.1a1/locale/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/nl-nl/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/nl-nl/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/nl-nl/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/nl-nl/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/nl-nl/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/nl-nl/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/nl-nl/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/nl-nl/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/nl-nl/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.644545 neon-skill-audio_record-0.1.1a1/locale/pt-br/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/pt-br/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/pt-br/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/pt-br/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/pt-br/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/pt-br/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/pt-br/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/pt-br/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/pt-br/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/pt-br/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.648545 neon-skill-audio_record-0.1.1a1/locale/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/ru-ru/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/ru-ru/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/ru-ru/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/ru-ru/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/ru-ru/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/ru-ru/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/ru-ru/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/ru-ru/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/ru-ru/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.648545 neon-skill-audio_record-0.1.1a1/locale/sv-se/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/sv-se/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/sv-se/Play.voc
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/sv-se/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/sv-se/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/sv-se/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/sv-se/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/sv-se/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/sv-se/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/locale/sv-se/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:34:41.648545 neon-skill-audio_record-0.1.1a1/neon_skill_audio_record.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-15 22:34:41.000000 neon-skill-audio_record-0.1.1a1/neon_skill_audio_record.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-06-15 22:34:41.000000 neon-skill-audio_record-0.1.1a1/neon_skill_audio_record.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:34:41.000000 neon-skill-audio_record-0.1.1a1/neon_skill_audio_record.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-15 22:34:41.000000 neon-skill-audio_record-0.1.1a1/neon_skill_audio_record.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 22:34:41.000000 neon-skill-audio_record-0.1.1a1/neon_skill_audio_record.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 22:34:41.000000 neon-skill-audio_record-0.1.1a1/neon_skill_audio_record.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:34:41.648545 neon-skill-audio_record-0.1.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/skill.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 22:34:37.000000 neon-skill-audio_record-0.1.1a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.890163 neon-skill-audio_record-0.1.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-15 22:38:39.890163 neon-skill-audio_record-0.1.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    25739 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.870163 neon-skill-audio_record-0.1.1a2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.874163 neon-skill-audio_record-0.1.1a2/locale/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/ca-es/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/ca-es/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/ca-es/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/ca-es/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/ca-es/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/ca-es/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/ca-es/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/ca-es/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/ca-es/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.874163 neon-skill-audio_record-0.1.1a2/locale/cs-cz/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/cs-cz/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/cs-cz/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/cs-cz/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/cs-cz/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/cs-cz/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/cs-cz/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/cs-cz/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/cs-cz/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/cs-cz/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.874163 neon-skill-audio_record-0.1.1a2/locale/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/da-dk/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/da-dk/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/da-dk/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/da-dk/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/da-dk/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/da-dk/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/da-dk/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/da-dk/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/da-dk/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.874163 neon-skill-audio_record-0.1.1a2/locale/de-de/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/de-de/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/de-de/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/de-de/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/de-de/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/de-de/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/de-de/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/de-de/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/de-de/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/de-de/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.874163 neon-skill-audio_record-0.1.1a2/locale/el-gr/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/el-gr/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/el-gr/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/el-gr/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/el-gr/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/el-gr/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/el-gr/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/el-gr/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/el-gr/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/el-gr/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.878163 neon-skill-audio_record-0.1.1a2/locale/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/Audio.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/AudioRecordSkillDeleteVerb.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/AudioRecordSkillKeyword.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/AudioRecordSkillListKeyword.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/AudioRecordSkillPlayVerb.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/AudioRecordSkillStopVerb.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/ConfirmFilename.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/ConfirmNo.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/ConfirmYes.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/FileExists.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/Neon.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/Record.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/ResumeKeyword.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/audio.record.start.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/audio.record.start.duration.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/audio.record.stop.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/en-us/audio.record.stop.play.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.878163 neon-skill-audio_record-0.1.1a2/locale/es-es/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/es-es/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/es-es/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/es-es/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/es-es/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/es-es/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/es-es/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/es-es/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/es-es/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/es-es/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.878163 neon-skill-audio_record-0.1.1a2/locale/es-lm/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/es-lm/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/es-lm/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/es-lm/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/es-lm/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/es-lm/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/es-lm/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/es-lm/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/es-lm/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/es-lm/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.882163 neon-skill-audio_record-0.1.1a2/locale/eu-eu/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/eu-eu/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/eu-eu/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/eu-eu/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/eu-eu/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/eu-eu/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/eu-eu/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/eu-eu/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/eu-eu/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/eu-eu/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.882163 neon-skill-audio_record-0.1.1a2/locale/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/fr-fr/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/fr-fr/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/fr-fr/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/fr-fr/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/fr-fr/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/fr-fr/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/fr-fr/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/fr-fr/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/fr-fr/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.882163 neon-skill-audio_record-0.1.1a2/locale/gl-es/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/gl-es/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/gl-es/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/gl-es/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/gl-es/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/gl-es/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/gl-es/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/gl-es/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/gl-es/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/gl-es/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.882163 neon-skill-audio_record-0.1.1a2/locale/hu-hu/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/hu-hu/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/hu-hu/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/hu-hu/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/hu-hu/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/hu-hu/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/hu-hu/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/hu-hu/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/hu-hu/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/hu-hu/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.882163 neon-skill-audio_record-0.1.1a2/locale/it-it/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/it-it/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/it-it/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/it-it/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/it-it/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/it-it/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/it-it/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/it-it/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/it-it/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/it-it/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.886163 neon-skill-audio_record-0.1.1a2/locale/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/nl-nl/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/nl-nl/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/nl-nl/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/nl-nl/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/nl-nl/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/nl-nl/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/nl-nl/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/nl-nl/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/nl-nl/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.886163 neon-skill-audio_record-0.1.1a2/locale/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/pt-br/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/pt-br/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/pt-br/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/pt-br/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/pt-br/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/pt-br/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/pt-br/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/pt-br/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/pt-br/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.890163 neon-skill-audio_record-0.1.1a2/locale/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/ru-ru/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/ru-ru/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/ru-ru/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/ru-ru/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/ru-ru/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/ru-ru/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/ru-ru/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/ru-ru/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/ru-ru/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.890163 neon-skill-audio_record-0.1.1a2/locale/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/sv-se/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/sv-se/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/sv-se/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/sv-se/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/sv-se/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/sv-se/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/sv-se/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/sv-se/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/locale/sv-se/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:39.890163 neon-skill-audio_record-0.1.1a2/neon_skill_audio_record.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-15 22:38:39.000000 neon-skill-audio_record-0.1.1a2/neon_skill_audio_record.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-06-15 22:38:39.000000 neon-skill-audio_record-0.1.1a2/neon_skill_audio_record.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:38:39.000000 neon-skill-audio_record-0.1.1a2/neon_skill_audio_record.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-15 22:38:39.000000 neon-skill-audio_record-0.1.1a2/neon_skill_audio_record.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 22:38:39.000000 neon-skill-audio_record-0.1.1a2/neon_skill_audio_record.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 22:38:39.000000 neon-skill-audio_record-0.1.1a2/neon_skill_audio_record.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:38:39.890163 neon-skill-audio_record-0.1.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/skill.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 22:38:35.000000 neon-skill-audio_record-0.1.1a2/version.py
```

### Comparing `neon-skill-audio_record-0.1.1a1/LICENSE` & `neon-skill-audio_record-0.1.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-audio_record-0.1.1a1/LICENSE.md` & `neon-skill-audio_record-0.1.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-audio_record-0.1.1a1/PKG-INFO` & `neon-skill-audio_record-0.1.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-audio_record
-Version: 0.1.1a1
+Version: 0.1.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-audio_record
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-audio_record-0.1.1a1/README.md` & `neon-skill-audio_record-0.1.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-audio_record-0.1.1a1/__init__.py` & `neon-skill-audio_record-0.1.1a2/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-audio_record-0.1.1a1/locale/eu-eu/PlayRecording.intent` & `neon-skill-audio_record-0.1.1a2/locale/eu-eu/PlayRecording.intent`

 * *Files identical despite different names*

### Comparing `neon-skill-audio_record-0.1.1a1/neon_skill_audio_record.egg-info/PKG-INFO` & `neon-skill-audio_record-0.1.1a2/neon_skill_audio_record.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-audio-record
-Version: 0.1.1a1
+Version: 0.1.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-audio_record
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-audio_record-0.1.1a1/neon_skill_audio_record.egg-info/SOURCES.txt` & `neon-skill-audio_record-0.1.1a2/neon_skill_audio_record.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-audio_record-0.1.1a1/setup.py` & `neon-skill-audio_record-0.1.1a2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 from setuptools import setup
 from os import getenv, path, walk
 
 SKILL_NAME = "skill-audio_record"
 SKILL_PKG = SKILL_NAME.replace('-', '_')
 # skill_id=package_name:SkillClass
 PLUGIN_ENTRY_POINT = f'{SKILL_NAME}.neongeckocom={SKILL_PKG}:AudioRecordSkill'
+BASE_PATH = path.abspath(path.dirname(__file__))
 
 
 def get_requirements(requirements_filename: str):
-    requirements_file = path.join(path.abspath(path.dirname(__file__)),
-                                  requirements_filename)
+    requirements_file = path.join(BASE_PATH, requirements_filename)
     with open(requirements_file, 'r', encoding='utf-8') as r:
         requirements = r.readlines()
     requirements = [r.strip() for r in requirements if r.strip()
                     and not r.strip().startswith("#")]
 
     for i in range(0, len(requirements)):
         r = requirements[i]
@@ -55,31 +55,31 @@
                     r.replace("github.com",
                               f"{getenv('GITHUB_TOKEN')}@github.com")
     return requirements
 
 
 def find_resource_files():
     resource_base_dirs = ("locale", "ui", "vocab", "dialog", "regex")
-    base_dir = path.dirname(__file__)
+    base_dir = BASE_PATH
     package_data = ["skill.json"]
     for res in resource_base_dirs:
         if path.isdir(path.join(base_dir, res)):
             for (directory, _, files) in walk(path.join(base_dir, res)):
                 if files:
                     package_data.append(
                         path.join(directory.replace(base_dir, "").lstrip('/'),
                                   '*'))
 #    print(package_data)
     return package_data
 
 
-with open("README.md", "r") as f:
+with open(path.join(BASE_PATH, "README.md"), "r") as f:
     long_description = f.read()
 
-with open("./version.py", "r", encoding="utf-8") as v:
+with open(path.join(BASE_PATH, "version.py"), "r", encoding="utf-8") as v:
     for line in v.readlines():
         if line.startswith("__version__"):
             if '"' in line:
                 version = line.split('"')[1]
             else:
                 version = line.split("'")[1]
```

### Comparing `neon-skill-audio_record-0.1.1a1/skill.json` & `neon-skill-audio_record-0.1.1a2/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-audio_record-0.1.1a1/version.py` & `neon-skill-audio_record-0.1.1a2/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.1.1a1"
+__version__ = "0.1.1a2"
```

