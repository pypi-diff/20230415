# Comparing `tmp/iam_actions-1.2.20230414.tar.gz` & `tmp/iam_actions-1.2.20230415.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230414.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230415.tar", max compression
```

## Comparing `iam_actions-1.2.20230414.tar` & `iam_actions-1.2.20230415.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/LICENSE
--rw-r--r--   0        0        0     2302 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/README.md
--rw-r--r--   0        0        0      228 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/iam_actions/__init__.py
--rw-r--r--   0        0        0  4208597 2023-04-14 02:25:53.397005 iam_actions-1.2.20230414/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-04-14 02:24:25.654019 iam_actions-1.2.20230414/iam_actions/generate/services.py
--rw-r--r--   0        0        0   540398 2023-04-14 02:25:53.397005 iam_actions-1.2.20230414/iam_actions/policies.json
--rw-r--r--   0        0        0   189864 2023-04-14 02:25:53.397005 iam_actions-1.2.20230414/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   524022 2023-04-14 02:25:53.397005 iam_actions-1.2.20230414/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-04-14 02:25:54.452994 iam_actions-1.2.20230414/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230414/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230414/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-15 02:25:07.722088 iam_actions-1.2.20230415/LICENSE
+-rw-r--r--   0        0        0     2302 2023-04-15 02:25:07.722088 iam_actions-1.2.20230415/README.md
+-rw-r--r--   0        0        0      228 2023-04-15 02:25:07.722088 iam_actions-1.2.20230415/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4212929 2023-04-15 02:26:54.304003 iam_actions-1.2.20230415/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-04-15 02:25:07.722088 iam_actions-1.2.20230415/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-04-15 02:25:07.722088 iam_actions-1.2.20230415/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-04-15 02:25:07.722088 iam_actions-1.2.20230415/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-04-15 02:25:07.722088 iam_actions-1.2.20230415/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-04-15 02:25:07.722088 iam_actions-1.2.20230415/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-04-15 02:25:07.722088 iam_actions-1.2.20230415/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-04-15 02:25:07.722088 iam_actions-1.2.20230415/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-04-15 02:25:07.722088 iam_actions-1.2.20230415/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   540625 2023-04-15 02:26:54.304003 iam_actions-1.2.20230415/iam_actions/policies.json
+-rw-r--r--   0        0        0   190432 2023-04-15 02:26:54.304003 iam_actions-1.2.20230415/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   524216 2023-04-15 02:26:54.304003 iam_actions-1.2.20230415/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-04-15 02:26:55.100017 iam_actions-1.2.20230415/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230415/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230415/PKG-INFO
```

### Comparing `iam_actions-1.2.20230414/LICENSE` & `iam_actions-1.2.20230415/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230414/README.md` & `iam_actions-1.2.20230415/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230414/iam_actions/actions.json` & `iam_actions-1.2.20230415/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991748335584714%*

 * *Differences: {"'chime'": "{'AssociatePhoneNumbersWithVoiceConnector': {'resources': ['voice-connector']}, "*

 * *            "'CreateProxySession': {'resources': ['voice-connector']}, "*

 * *            "'CreateSipMediaApplication': {'condition_keys': ['aws:RequestTag/${TagKey}', "*

 * *            "'aws:TagKeys']}, 'CreateSipMediaApplicationCall': {'resources': "*

 * *            "['sip-media-application']}, 'CreateSipRule': {'resources': "*

 * *            "['sip-media-application']}, 'CreateVoiceConnector': {'condition_keys': "*

 * *            " […]*

```diff
@@ -13991,15 +13991,17 @@
         },
         "AssociatePhoneNumbersWithVoiceConnector": {
             "access_level": "Write",
             "action": "AssociatePhoneNumbersWithVoiceConnector",
             "condition_keys": [],
             "description": "Grants permission to associate multiple phone numbers with an Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "AssociatePhoneNumbersWithVoiceConnectorGroup": {
             "access_level": "Write",
             "action": "AssociatePhoneNumbersWithVoiceConnectorGroup",
             "condition_keys": [],
             "description": "Grants permission to associate multiple phone numbers with an Amazon Chime Voice Connector Group",
             "orphan": false,
@@ -14378,15 +14380,17 @@
         },
         "CreateProxySession": {
             "access_level": "Write",
             "action": "CreateProxySession",
             "condition_keys": [],
             "description": "Grants permission to create a proxy session for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "CreateRoom": {
             "access_level": "Write",
             "action": "CreateRoom",
             "condition_keys": [],
             "description": "Grants permission to create a room",
             "orphan": false,
@@ -14399,58 +14403,70 @@
             "description": "Grants permission to add a room member",
             "orphan": false,
             "resources": []
         },
         "CreateSipMediaApplication": {
             "access_level": "Write",
             "action": "CreateSipMediaApplication",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
             "description": "Grants permission to create an Amazon Chime SIP media application under the administrator's AWS account",
             "orphan": false,
             "resources": []
         },
         "CreateSipMediaApplicationCall": {
             "access_level": "Write",
             "action": "CreateSipMediaApplicationCall",
             "condition_keys": [],
             "description": "Grants permission to create outbound call for Amazon Chime SIP media application under the administrator's AWS account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sip-media-application"
+            ]
         },
         "CreateSipRule": {
             "access_level": "Write",
             "action": "CreateSipRule",
             "condition_keys": [],
             "description": "Grants permission to create an Amazon Chime SIP rule under the administrator's AWS account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sip-media-application"
+            ]
         },
         "CreateUser": {
             "access_level": "Write",
             "action": "CreateUser",
             "condition_keys": [],
             "description": "Grants permission to create a user under the specified Amazon Chime account",
             "orphan": false,
             "resources": []
         },
         "CreateVoiceConnector": {
             "access_level": "Write",
             "action": "CreateVoiceConnector",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
             "description": "Grants permission to create a Amazon Chime Voice Connector under the administrator's AWS account",
             "orphan": false,
             "resources": []
         },
         "CreateVoiceConnectorGroup": {
             "access_level": "Write",
             "action": "CreateVoiceConnectorGroup",
             "condition_keys": [],
             "description": "Grants permission to create a Amazon Chime Voice Connector Group under the administrator's AWS account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "CreateVoiceProfile": {
             "access_level": "Write",
             "action": "CreateVoiceProfile",
             "condition_keys": [],
             "description": "Grants permission to create a voice profile",
             "orphan": false,
@@ -14723,15 +14739,17 @@
         },
         "DeleteProxySession": {
             "access_level": "Write",
             "action": "DeleteProxySession",
             "condition_keys": [],
             "description": "Grants permission to delete a proxy session for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "DeleteRoom": {
             "access_level": "Write",
             "action": "DeleteRoom",
             "condition_keys": [],
             "description": "Grants permission to delete a room",
             "orphan": false,
@@ -14747,15 +14765,17 @@
         },
         "DeleteSipMediaApplication": {
             "access_level": "Write",
             "action": "DeleteSipMediaApplication",
             "condition_keys": [],
             "description": "Grants permission to delete Amazon Chime SIP media application under the administrator's AWS account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sip-media-application"
+            ]
         },
         "DeleteSipRule": {
             "access_level": "Write",
             "action": "DeleteSipRule",
             "condition_keys": [],
             "description": "Grants permission to delete Amazon Chime SIP rule under the administrator's AWS account",
             "orphan": false,
@@ -14763,23 +14783,27 @@
         },
         "DeleteVoiceConnector": {
             "access_level": "Write",
             "action": "DeleteVoiceConnector",
             "condition_keys": [],
             "description": "Grants permission to delete the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "DeleteVoiceConnectorEmergencyCallingConfiguration": {
             "access_level": "Write",
             "action": "DeleteVoiceConnectorEmergencyCallingConfiguration",
             "condition_keys": [],
             "description": "Grants permission to delete emergency calling configuration for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "DeleteVoiceConnectorGroup": {
             "access_level": "Write",
             "action": "DeleteVoiceConnectorGroup",
             "condition_keys": [],
             "description": "Grants permission to delete the specified Amazon Chime Voice Connector Group",
             "orphan": false,
@@ -14787,47 +14811,57 @@
         },
         "DeleteVoiceConnectorOrigination": {
             "access_level": "Write",
             "action": "DeleteVoiceConnectorOrigination",
             "condition_keys": [],
             "description": "Grants permission to delete the origination settings for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "DeleteVoiceConnectorProxy": {
             "access_level": "Write",
             "action": "DeleteVoiceConnectorProxy",
             "condition_keys": [],
             "description": "Grants permission to delete proxy configuration for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "DeleteVoiceConnectorStreamingConfiguration": {
             "access_level": "Write",
             "action": "DeleteVoiceConnectorStreamingConfiguration",
             "condition_keys": [],
             "description": "Grants permission to delete streaming configuration for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "DeleteVoiceConnectorTermination": {
             "access_level": "Write",
             "action": "DeleteVoiceConnectorTermination",
             "condition_keys": [],
             "description": "Grants permission to delete the termination settings for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "DeleteVoiceConnectorTerminationCredentials": {
             "access_level": "Write",
             "action": "DeleteVoiceConnectorTerminationCredentials",
             "condition_keys": [],
             "description": "Grants permission to delete SIP termination credentials for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "DeleteVoiceProfile": {
             "access_level": "Write",
             "action": "DeleteVoiceProfile",
             "condition_keys": [],
             "description": "Grants permission to delete a voice profile",
             "orphan": false,
@@ -15012,15 +15046,17 @@
         },
         "DisassociatePhoneNumbersFromVoiceConnector": {
             "access_level": "Write",
             "action": "DisassociatePhoneNumbersFromVoiceConnector",
             "condition_keys": [],
             "description": "Grants permission to disassociate multiple phone numbers from the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "DisassociatePhoneNumbersFromVoiceConnectorGroup": {
             "access_level": "Write",
             "action": "DisassociatePhoneNumbersFromVoiceConnectorGroup",
             "condition_keys": [],
             "description": "Grants permission to disassociate multiple phone numbers from the specified Amazon Chime Voice Connector Group",
             "orphan": false,
@@ -15272,15 +15308,17 @@
         },
         "GetProxySession": {
             "access_level": "Read",
             "action": "GetProxySession",
             "condition_keys": [],
             "description": "Grants permission to get details of the specified proxy session for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "GetRetentionSettings": {
             "access_level": "Read",
             "action": "GetRetentionSettings",
             "condition_keys": [],
             "description": "Grants permission to retrieve the retention settings for the specified Amazon Chime account",
             "orphan": false,
@@ -15296,31 +15334,37 @@
         },
         "GetSipMediaApplication": {
             "access_level": "Read",
             "action": "GetSipMediaApplication",
             "condition_keys": [],
             "description": "Grants permission to get details of Amazon Chime SIP media application under the administrator's AWS account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sip-media-application"
+            ]
         },
         "GetSipMediaApplicationAlexaSkillConfiguration": {
             "access_level": "Read",
             "action": "GetSipMediaApplicationAlexaSkillConfiguration",
             "condition_keys": [],
             "description": "Grants permission to get Alexa Skill configuration settings for Amazon Chime SIP media application under the administrator's AWS account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sip-media-application"
+            ]
         },
         "GetSipMediaApplicationLoggingConfiguration": {
             "access_level": "Read",
             "action": "GetSipMediaApplicationLoggingConfiguration",
             "condition_keys": [],
             "description": "Grants permission to get logging configuration settings for Amazon Chime SIP media application under the administrator's AWS account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sip-media-application"
+            ]
         },
         "GetSipRule": {
             "access_level": "Read",
             "action": "GetSipRule",
             "condition_keys": [],
             "description": "Grants permission to get details of Amazon Chime SIP rule under the administrator's AWS account",
             "orphan": false,
@@ -15328,15 +15372,17 @@
         },
         "GetSpeakerSearchTask": {
             "access_level": "Read",
             "action": "GetSpeakerSearchTask",
             "condition_keys": [],
             "description": "Grants permission to get a speaker search task",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "GetTelephonyLimits": {
             "access_level": "Read",
             "action": "GetTelephonyLimits",
             "condition_keys": [],
             "description": "Grants permission to get telephony limits for the AWS account",
             "orphan": false,
@@ -15376,23 +15422,27 @@
         },
         "GetVoiceConnector": {
             "access_level": "Read",
             "action": "GetVoiceConnector",
             "condition_keys": [],
             "description": "Grants permission to get details for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "GetVoiceConnectorEmergencyCallingConfiguration": {
             "access_level": "Read",
             "action": "GetVoiceConnectorEmergencyCallingConfiguration",
             "condition_keys": [],
             "description": "Grants permission to get details of the emergency calling configuration for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "GetVoiceConnectorGroup": {
             "access_level": "Read",
             "action": "GetVoiceConnectorGroup",
             "condition_keys": [],
             "description": "Grants permission to get details for the specified Amazon Chime Voice Connector Group",
             "orphan": false,
@@ -15400,55 +15450,67 @@
         },
         "GetVoiceConnectorLoggingConfiguration": {
             "access_level": "Read",
             "action": "GetVoiceConnectorLoggingConfiguration",
             "condition_keys": [],
             "description": "Grants permission to get details of the logging configuration for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "GetVoiceConnectorOrigination": {
             "access_level": "Read",
             "action": "GetVoiceConnectorOrigination",
             "condition_keys": [],
             "description": "Grants permission to get details of the origination settings for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "GetVoiceConnectorProxy": {
             "access_level": "Read",
             "action": "GetVoiceConnectorProxy",
             "condition_keys": [],
             "description": "Grants permission to get details of the proxy configuration for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "GetVoiceConnectorStreamingConfiguration": {
             "access_level": "Read",
             "action": "GetVoiceConnectorStreamingConfiguration",
             "condition_keys": [],
             "description": "Grants permission to get details of the streaming configuration for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "GetVoiceConnectorTermination": {
             "access_level": "Read",
             "action": "GetVoiceConnectorTermination",
             "condition_keys": [],
             "description": "Grants permission to get details of the termination settings for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "GetVoiceConnectorTerminationHealth": {
             "access_level": "Read",
             "action": "GetVoiceConnectorTerminationHealth",
             "condition_keys": [],
             "description": "Grants permission to get details of the termination health for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "GetVoiceProfile": {
             "access_level": "Read",
             "action": "GetVoiceProfile",
             "condition_keys": [],
             "description": "Grants permission to get a voice profile",
             "orphan": false,
@@ -15468,15 +15530,17 @@
         },
         "GetVoiceToneAnalysisTask": {
             "access_level": "Read",
             "action": "GetVoiceToneAnalysisTask",
             "condition_keys": [],
             "description": "Grants permission to get a voice tone analysis task",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "InviteDelegate": {
             "access_level": "Write",
             "action": "InviteDelegate",
             "condition_keys": [],
             "description": "Grants permission to send an invitation to accept a request for AWS account delegation for an Amazon Chime account",
             "orphan": false,
@@ -15835,15 +15899,17 @@
         },
         "ListProxySessions": {
             "access_level": "List",
             "action": "ListProxySessions",
             "condition_keys": [],
             "description": "Grants permission to list proxy sessions for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "ListRoomMemberships": {
             "access_level": "List",
             "action": "ListRoomMemberships",
             "condition_keys": [],
             "description": "Grants permission to list all room members",
             "orphan": false,
@@ -15867,15 +15933,17 @@
         },
         "ListSipRules": {
             "access_level": "List",
             "action": "ListSipRules",
             "condition_keys": [],
             "description": "Grants permission to list all Amazon Chime SIP rules under the administrator's AWS account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sip-media-application"
+            ]
         },
         "ListSubChannels": {
             "access_level": "List",
             "action": "ListSubChannels",
             "condition_keys": [],
             "description": "Grants permission to list all the SubChannels under a single Channel",
             "orphan": false,
@@ -15901,14 +15969,16 @@
             "orphan": false,
             "resources": [
                 "app-instance-bot",
                 "channel",
                 "media-insights-pipeline-configuration",
                 "media-pipeline",
                 "meeting",
+                "sip-media-application",
+                "voice-connector",
                 "voice-profile-domain"
             ]
         },
         "ListUsers": {
             "access_level": "List",
             "action": "ListUsers",
             "condition_keys": [],
@@ -15926,15 +15996,17 @@
         },
         "ListVoiceConnectorTerminationCredentials": {
             "access_level": "List",
             "action": "ListVoiceConnectorTerminationCredentials",
             "condition_keys": [],
             "description": "Grants permission to list the SIP termination credentials for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "ListVoiceConnectors": {
             "access_level": "List",
             "action": "ListVoiceConnectors",
             "condition_keys": [],
             "description": "Grants permission to list the Amazon Chime Voice Connectors under the administrator's AWS account",
             "orphan": false,
@@ -16047,81 +16119,98 @@
         },
         "PutSipMediaApplicationAlexaSkillConfiguration": {
             "access_level": "Write",
             "action": "PutSipMediaApplicationAlexaSkillConfiguration",
             "condition_keys": [],
             "description": "Grants permission to update Alexa Skill configuration settings for Amazon Chime SIP media application under the administrator's AWS account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sip-media-application"
+            ]
         },
         "PutSipMediaApplicationLoggingConfiguration": {
             "access_level": "Write",
             "action": "PutSipMediaApplicationLoggingConfiguration",
             "condition_keys": [],
             "description": "Grants permission to update logging configuration settings for Amazon Chime SIP media application under the administrator's AWS account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sip-media-application"
+            ]
         },
         "PutVoiceConnectorEmergencyCallingConfiguration": {
             "access_level": "Write",
             "action": "PutVoiceConnectorEmergencyCallingConfiguration",
             "condition_keys": [],
             "description": "Grants permission to add emergency calling configuration for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "PutVoiceConnectorLoggingConfiguration": {
             "access_level": "Write",
             "action": "PutVoiceConnectorLoggingConfiguration",
             "condition_keys": [],
             "description": "Grants permission to add logging configuration for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "PutVoiceConnectorOrigination": {
             "access_level": "Write",
             "action": "PutVoiceConnectorOrigination",
             "condition_keys": [],
             "description": "Grants permission to update the origination settings for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "PutVoiceConnectorProxy": {
             "access_level": "Write",
             "action": "PutVoiceConnectorProxy",
             "condition_keys": [],
             "description": "Grants permission to add proxy configuration for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "PutVoiceConnectorStreamingConfiguration": {
             "access_level": "Write",
             "action": "PutVoiceConnectorStreamingConfiguration",
             "condition_keys": [],
             "description": "Grants permission to add streaming configuration for the specified Amazon Chime Voice Connector",
             "orphan": false,
             "resources": [
-                "media-insights-pipeline-configuration"
+                "media-insights-pipeline-configuration",
+                "voice-connector"
             ]
         },
         "PutVoiceConnectorTermination": {
             "access_level": "Write",
             "action": "PutVoiceConnectorTermination",
             "condition_keys": [],
             "description": "Grants permission to update the termination settings for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "PutVoiceConnectorTerminationCredentials": {
             "access_level": "Write",
             "action": "PutVoiceConnectorTerminationCredentials",
             "condition_keys": [],
             "description": "Grants permission to add SIP termination credentials for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "RedactChannelMessage": {
             "access_level": "Write",
             "action": "RedactChannelMessage",
             "condition_keys": [],
             "description": "Grants permission to redact message content",
             "orphan": false,
@@ -16262,23 +16351,27 @@
         },
         "StartSpeakerSearchTask": {
             "access_level": "Write",
             "action": "StartSpeakerSearchTask",
             "condition_keys": [],
             "description": "Grants permission to start a speaker search task",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "StartVoiceToneAnalysisTask": {
             "access_level": "Write",
             "action": "StartVoiceToneAnalysisTask",
             "condition_keys": [],
             "description": "Grants permission to start a voice tone analysis task",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "StopMeetingTranscription": {
             "access_level": "Write",
             "action": "StopMeetingTranscription",
             "condition_keys": [],
             "description": "Grants permission to stop transcription for a meeting",
             "orphan": false,
@@ -16286,23 +16379,27 @@
         },
         "StopSpeakerSearchTask": {
             "access_level": "Write",
             "action": "StopSpeakerSearchTask",
             "condition_keys": [],
             "description": "Grants permission to stop a speaker search task",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "StopVoiceToneAnalysisTask": {
             "access_level": "Write",
             "action": "StopVoiceToneAnalysisTask",
             "condition_keys": [],
             "description": "Grants permission to stop a voice tone analysis task",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "SubmitSupportRequest": {
             "access_level": "Write",
             "action": "SubmitSupportRequest",
             "condition_keys": [],
             "description": "Grants permission to submit a customer service support request",
             "orphan": false,
@@ -16355,14 +16452,16 @@
                 "app-instance-bot",
                 "app-instance-user",
                 "channel",
                 "channel-flow",
                 "media-insights-pipeline-configuration",
                 "media-pipeline",
                 "meeting",
+                "sip-media-application",
+                "voice-connector",
                 "voice-profile-domain"
             ]
         },
         "UnauthorizeDirectory": {
             "access_level": "Write",
             "action": "UnauthorizeDirectory",
             "condition_keys": [],
@@ -16403,14 +16502,16 @@
                 "app-instance-bot",
                 "app-instance-user",
                 "channel",
                 "channel-flow",
                 "media-insights-pipeline-configuration",
                 "media-pipeline",
                 "meeting",
+                "sip-media-application",
+                "voice-connector",
                 "voice-profile-domain"
             ]
         },
         "UpdateAccount": {
             "access_level": "Write",
             "action": "UpdateAccount",
             "condition_keys": [],
@@ -16600,15 +16701,17 @@
         },
         "UpdateProxySession": {
             "access_level": "Write",
             "action": "UpdateProxySession",
             "condition_keys": [],
             "description": "Grants permission to update a proxy session for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "UpdateRoom": {
             "access_level": "Write",
             "action": "UpdateRoom",
             "condition_keys": [],
             "description": "Grants permission to update a room",
             "orphan": false,
@@ -16624,31 +16727,37 @@
         },
         "UpdateSipMediaApplication": {
             "access_level": "Write",
             "action": "UpdateSipMediaApplication",
             "condition_keys": [],
             "description": "Grants permission to update properties of Amazon Chime SIP media application under the administrator's AWS account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sip-media-application"
+            ]
         },
         "UpdateSipMediaApplicationCall": {
             "access_level": "Write",
             "action": "UpdateSipMediaApplicationCall",
             "condition_keys": [],
             "description": "Grants permission to update an Amazon Chime SIP media application call under the administrator's AWS account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sip-media-application"
+            ]
         },
         "UpdateSipRule": {
             "access_level": "Write",
             "action": "UpdateSipRule",
             "condition_keys": [],
             "description": "Grants permission to update properties of Amazon Chime SIP rule under the administrator's AWS account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "sip-media-application"
+            ]
         },
         "UpdateSupportedLicenses": {
             "access_level": "Write",
             "action": "UpdateSupportedLicenses",
             "condition_keys": [],
             "description": "Grants permission to update the supported license tiers available for users in your Amazon Chime account",
             "orphan": false,
@@ -16680,23 +16789,27 @@
         },
         "UpdateVoiceConnector": {
             "access_level": "Write",
             "action": "UpdateVoiceConnector",
             "condition_keys": [],
             "description": "Grants permission to update Amazon Chime Voice Connector details for the specified Amazon Chime Voice Connector",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "UpdateVoiceConnectorGroup": {
             "access_level": "Write",
             "action": "UpdateVoiceConnectorGroup",
             "condition_keys": [],
             "description": "Grants permission to update Amazon Chime Voice Connector Group details for the specified Amazon Chime Voice Connector Group",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "voice-connector"
+            ]
         },
         "UpdateVoiceProfile": {
             "access_level": "Write",
             "action": "UpdateVoiceProfile",
             "condition_keys": [],
             "description": "Grants permission to update a voice profile",
             "orphan": false,
@@ -25454,14 +25567,22 @@
             "condition_keys": [],
             "description": "Grants permission to invoke CreateProfile on CodeWhisperer",
             "orphan": false,
             "resources": [
                 "profile"
             ]
         },
+        "DeleteProfile": {
+            "access_level": "Undocumented",
+            "action": "DeleteProfile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GenerateRecommendations": {
             "access_level": "Read",
             "action": "GenerateRecommendations",
             "condition_keys": [],
             "description": "Grants permission to invoke GenerateRecommendations on CodeWhisperer",
             "orphan": false,
             "resources": []
@@ -25470,14 +25591,38 @@
             "access_level": "List",
             "action": "ListProfiles",
             "condition_keys": [],
             "description": "Grants permission to invoke ListProfiles on CodeWhisperer",
             "orphan": false,
             "resources": []
         },
+        "ListTagsForResource": {
+            "access_level": "Undocumented",
+            "action": "ListTagsForResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "TagResource": {
+            "access_level": "Undocumented",
+            "action": "TagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UntagResource": {
+            "access_level": "Undocumented",
+            "action": "UntagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateProfile": {
             "access_level": "Write",
             "action": "UpdateProfile",
             "condition_keys": [],
             "description": "Grants permission to invoke UpdateProfile on CodeWhisperer",
             "orphan": false,
             "resources": [
@@ -57152,14 +57297,24 @@
             "condition_keys": [],
             "description": "Grants permission to view a description of the configuration options and status of an OpenSearch Service domain",
             "orphan": false,
             "resources": [
                 "domain"
             ]
         },
+        "DescribeDomainHealth": {
+            "access_level": "Read",
+            "action": "DescribeDomainHealth",
+            "condition_keys": [],
+            "description": "Grants permission to view information about domain and node health, the standby Availability Zone, number of nodes per Availability Zone, and shard count per node",
+            "orphan": false,
+            "resources": [
+                "domain"
+            ]
+        },
         "DescribeDomains": {
             "access_level": "List",
             "action": "DescribeDomains",
             "condition_keys": [],
             "description": "Grants permission to view a description of the domain configuration for up to five specified OpenSearch Service domains",
             "orphan": false,
             "resources": [
@@ -72634,26 +72789,26 @@
             "action": "BatchGetFreeTrialInfo",
             "condition_keys": [],
             "description": "Grants permission to retrieve free trial period eligibility about Amazon Inspector accounts for an account",
             "orphan": false,
             "resources": []
         },
         "BatchGetMemberEc2DeepInspectionStatus": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "BatchGetMemberEc2DeepInspectionStatus",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delegated administrator to retrieve ec2 deep inspection status of member accounts",
             "orphan": false,
             "resources": []
         },
         "BatchUpdateMemberEc2DeepInspectionStatus": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "BatchUpdateMemberEc2DeepInspectionStatus",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update ec2 deep inspection status by delegated administrator for its associated member accounts",
             "orphan": false,
             "resources": []
         },
         "CancelFindingsReport": {
             "access_level": "Write",
             "action": "CancelFindingsReport",
             "condition_keys": [],
@@ -72753,18 +72908,18 @@
             "action": "GetDelegatedAdminAccount",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about the Amazon Inspector administrator account for an account",
             "orphan": false,
             "resources": []
         },
         "GetEc2DeepInspectionConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetEc2DeepInspectionConfiguration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve ec2 deep inspection configuration for standalone accounts, delegated administrator and member account",
             "orphan": false,
             "resources": []
         },
         "GetFindingsReportStatus": {
             "access_level": "Read",
             "action": "GetFindingsReportStatus",
             "condition_keys": [],
@@ -72887,18 +73042,18 @@
             "action": "UpdateConfiguration",
             "condition_keys": [],
             "description": "Grants permission to update information about the Amazon Inspector configuration settings for an AWS account",
             "orphan": false,
             "resources": []
         },
         "UpdateEc2DeepInspectionConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateEc2DeepInspectionConfiguration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update ec2 deep inspection configuration by delegated administrator, member and standalone account",
             "orphan": false,
             "resources": []
         },
         "UpdateFilter": {
             "access_level": "Write",
             "action": "UpdateFilter",
             "condition_keys": [
@@ -72908,18 +73063,18 @@
             "description": "Grants permission to update the settings for a findings filter",
             "orphan": false,
             "resources": [
                 "Filter"
             ]
         },
         "UpdateOrgEc2DeepInspectionConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateOrgEc2DeepInspectionConfiguration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update ec2 deep inspection configuration by delegated administrator for its associated member accounts",
             "orphan": false,
             "resources": []
         },
         "UpdateOrganizationConfiguration": {
             "access_level": "Write",
             "action": "UpdateOrganizationConfiguration",
             "condition_keys": [],
@@ -91880,28 +92035,32 @@
             "description": "The UpdateQualificationType operation modifies the attributes of an existing Qualification type, which is represented by a QualificationType data structure",
             "orphan": false,
             "resources": []
         }
     },
     "mediaconnect": {
         "AddBridgeOutputs": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AddBridgeOutputs",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to add outputs to an existing bridge",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Bridge"
+            ]
         },
         "AddBridgeSources": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AddBridgeSources",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to add sources to an existing bridge",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Bridge"
+            ]
         },
         "AddFlowMediaStreams": {
             "access_level": "Write",
             "action": "AddFlowMediaStreams",
             "condition_keys": [],
             "description": "Grants permission to add media streams to any flow",
             "orphan": false,
@@ -91928,100 +92087,116 @@
             "action": "AddFlowVpcInterfaces",
             "condition_keys": [],
             "description": "Grants permission to add VPC interfaces to any flow",
             "orphan": false,
             "resources": []
         },
         "CreateBridge": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateBridge",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create bridges",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Bridge"
+            ]
         },
         "CreateFlow": {
             "access_level": "Write",
             "action": "CreateFlow",
             "condition_keys": [],
             "description": "Grants permission to create flows",
             "orphan": false,
             "resources": []
         },
         "CreateGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateGateway",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create gateways",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Gateway"
+            ]
         },
         "DeleteBridge": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteBridge",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete bridges",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Bridge"
+            ]
         },
         "DeleteFlow": {
             "access_level": "Write",
             "action": "DeleteFlow",
             "condition_keys": [],
             "description": "Grants permission to delete flows",
             "orphan": false,
             "resources": []
         },
         "DeleteGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteGateway",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete gateways",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Gateway"
+            ]
         },
         "DeregisterGatewayInstance": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeregisterGatewayInstance",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to deregister gateway instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "GatewayInstance"
+            ]
         },
         "DescribeBridge": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeBridge",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to display the details of a bridge",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Bridge"
+            ]
         },
         "DescribeFlow": {
             "access_level": "Read",
             "action": "DescribeFlow",
             "condition_keys": [],
             "description": "Grants permission to display the details of a flow including the flow ARN, name, and Availability Zone, as well as details about the source, outputs, and entitlements",
             "orphan": false,
             "resources": []
         },
         "DescribeGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeGateway",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to display the details of a gateway including the gateway ARN, name, and CIDR blocks, as well as details about the networks",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Gateway"
+            ]
         },
         "DescribeGatewayInstance": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeGatewayInstance",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to display the details of a gateway instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "GatewayInstance"
+            ]
         },
         "DescribeOffering": {
             "access_level": "Read",
             "action": "DescribeOffering",
             "condition_keys": [],
             "description": "Grants permission to display the details of an offering",
             "orphan": false,
@@ -92032,36 +92207,38 @@
             "action": "DescribeReservation",
             "condition_keys": [],
             "description": "Grants permission to display the details of a reservation",
             "orphan": false,
             "resources": []
         },
         "DiscoverGatewayPollEndpoint": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DiscoverGatewayPollEndpoint",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to discover gateway poll endpoint",
             "orphan": false,
             "resources": []
         },
         "GrantFlowEntitlements": {
             "access_level": "Write",
             "action": "GrantFlowEntitlements",
             "condition_keys": [],
             "description": "Grants permission to grant entitlements on any flow",
             "orphan": false,
             "resources": []
         },
         "ListBridges": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListBridges",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to display a list of bridges that are associated with this account and an optionally specified Arn",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Bridge"
+            ]
         },
         "ListEntitlements": {
             "access_level": "List",
             "action": "ListEntitlements",
             "condition_keys": [],
             "description": "Grants permission to display a list of all entitlements that have been granted to the account",
             "orphan": false,
@@ -92072,26 +92249,28 @@
             "action": "ListFlows",
             "condition_keys": [],
             "description": "Grants permission to display a list of flows that are associated with this account",
             "orphan": false,
             "resources": []
         },
         "ListGatewayInstances": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListGatewayInstances",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to display a list of instances that are associated with this gateway",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "GatewayInstance"
+            ]
         },
         "ListGateways": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListGateways",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to display a list of gateways that are associated with this account",
             "orphan": false,
             "resources": []
         },
         "ListOfferings": {
             "access_level": "List",
             "action": "ListOfferings",
             "condition_keys": [],
@@ -92112,44 +92291,48 @@
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to display a list of all tags associated with a resource",
             "orphan": false,
             "resources": []
         },
         "PollGateway": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PollGateway",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to poll gateway",
             "orphan": false,
             "resources": []
         },
         "PurchaseOffering": {
             "access_level": "Write",
             "action": "PurchaseOffering",
             "condition_keys": [],
             "description": "Grants permission to purchase an offering",
             "orphan": false,
             "resources": []
         },
         "RemoveBridgeOutput": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RemoveBridgeOutput",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to remove an output of an existing bridge",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Bridge"
+            ]
         },
         "RemoveBridgeSource": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RemoveBridgeSource",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to remove a source of an existing bridge",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Bridge"
+            ]
         },
         "RemoveFlowMediaStream": {
             "access_level": "Write",
             "action": "RemoveFlowMediaStream",
             "condition_keys": [],
             "description": "Grants permission to remove media streams from any flow",
             "orphan": false,
@@ -92200,18 +92383,18 @@
             "action": "StopFlow",
             "condition_keys": [],
             "description": "Grants permission to stop flows",
             "orphan": false,
             "resources": []
         },
         "SubmitGatewayStateChange": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "SubmitGatewayStateChange",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to submit gateway state change",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [],
@@ -92224,44 +92407,52 @@
             "action": "UntagResource",
             "condition_keys": [],
             "description": "Grants permission to remove tags from resources",
             "orphan": false,
             "resources": []
         },
         "UpdateBridge": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateBridge",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update bridges",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Bridge"
+            ]
         },
         "UpdateBridgeOutput": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateBridgeOutput",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update an output of an existing bridge",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Bridge"
+            ]
         },
         "UpdateBridgeSource": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateBridgeSource",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update a source of an existing bridge",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Bridge"
+            ]
         },
         "UpdateBridgeState": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateBridgeState",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update the state of an existing bridge",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Bridge"
+            ]
         },
         "UpdateFlow": {
             "access_level": "Write",
             "action": "UpdateFlow",
             "condition_keys": [],
             "description": "Grants permission to update flows",
             "orphan": false,
@@ -135851,20 +136042,22 @@
             "description": "Grants permission to list all receipts of a page",
             "orphan": false,
             "resources": [
                 "page"
             ]
         },
         "ListPageResolutions": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListPageResolutions",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list the resolution path of an engagement",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "page"
+            ]
         },
         "ListPagesByContact": {
             "access_level": "List",
             "action": "ListPagesByContact",
             "condition_keys": [],
             "description": "Grants permission to list all pages sent to a contact",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20230414/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230415/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230414/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230415/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230414/iam_actions/generate/generate.py` & `iam_actions-1.2.20230415/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230414/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230415/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230414/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230415/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230414/iam_actions/generate/services.py` & `iam_actions-1.2.20230415/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230414/iam_actions/policies.json` & `iam_actions-1.2.20230415/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999717174070621%*

 * *Differences: {"'serviceMap'": "{'Amazon OpenSearch Service': {'Actions': {insert: [(28, "*

 * *                 "'DescribeDomainHealth')]}}, 'Amazon CodeWhisperer': {'Actions': {insert: [(1, "*

 * *                 "'DeleteProfile'), (4, 'ListTagsForResource'), (5, 'TagResource'), (6, "*

 * *                 "'UntagResource')]}, 'conditionKeys': ['aws:RequestTag/${TagKey}', "*

 * *                 "'aws:ResourceTag/${TagKey}', 'aws:TagKeys']}}"}*

```diff
@@ -10748,20 +10748,29 @@
             "StringPrefix": "codeguru-security"
         },
         "Amazon CodeWhisperer": {
             "ARNFormat": "arn:aws:codewhisperer:${Region}:${Account}:${ResourceType}/${ResourceId}",
             "ARNRegex": "^arn:aws:codewhisperer:.+:[0-9]+:.+",
             "Actions": [
                 "CreateProfile",
+                "DeleteProfile",
                 "GenerateRecommendations",
                 "ListProfiles",
+                "ListTagsForResource",
+                "TagResource",
+                "UntagResource",
                 "UpdateProfile"
             ],
             "HasResource": true,
-            "StringPrefix": "codewhisperer"
+            "StringPrefix": "codewhisperer",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ]
         },
         "Amazon Cognito Identity": {
             "ARNFormat": "arn:aws:cognito-identity:${Region}:${Account}:${ResourceType}/${ResourcePath}",
             "ARNRegex": "^arn:aws:cognito-identity:.+",
             "Actions": [
                 "CreateIdentityPool",
                 "DeleteIdentities",
@@ -15880,14 +15889,15 @@
                 "DeleteOutboundCrossClusterSearchConnection",
                 "DeletePackage",
                 "DeleteVpcEndpoint",
                 "DescribeDomain",
                 "DescribeDomainAutoTunes",
                 "DescribeDomainChangeProgress",
                 "DescribeDomainConfig",
+                "DescribeDomainHealth",
                 "DescribeDomains",
                 "DescribeDryRunProgress",
                 "DescribeElasticsearchDomain",
                 "DescribeElasticsearchDomainConfig",
                 "DescribeElasticsearchDomains",
                 "DescribeElasticsearchInstanceTypeLimits",
                 "DescribeInboundConnections",
```

### Comparing `iam_actions-1.2.20230414/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230415/iam_actions/resourcetypes.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991568865506543%*

 * *Differences: {"'chime'": "{'voice-connector': OrderedDict([('arn_pattern', 'arn:*:chime:*:*:vc/*'), "*

 * *            "('condition_keys', 'aws:ResourceTag/${TagKey}')]), 'sip-media-application': "*

 * *            "OrderedDict([('arn_pattern', 'arn:*:chime:*:*:sma/*'), ('condition_keys', "*

 * *            "'aws:ResourceTag/${TagKey}')])}",*

 * * "'mediaconnect'": "{'Gateway': OrderedDict([('arn_pattern', "*

 * *                   "'arn:*:mediaconnect:*:*:gateway:*:*'), ('condition_keys', None)]), 'Bridge': "*

 * *                   "OrderedDict([( […]*

```diff
@@ -911,14 +911,22 @@
             "arn_pattern": "arn:*:chime:*:*:media-pipeline/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "meeting": {
             "arn_pattern": "arn:*:chime::*:meeting/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "sip-media-application": {
+            "arn_pattern": "arn:*:chime:*:*:sma/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
+        "voice-connector": {
+            "arn_pattern": "arn:*:chime:*:*:vc/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "voice-profile": {
             "arn_pattern": "arn:*:chime:*:*:voice-profile/*",
             "condition_keys": null
         },
         "voice-profile-domain": {
             "arn_pattern": "arn:*:chime:*:*:voice-profile-domain/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
@@ -4005,22 +4013,34 @@
             "arn_pattern": "arn:*:managedblockchain:*::proposals/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "marketplacecommerceanalytics": {},
     "mechanicalturk": {},
     "mediaconnect": {
+        "Bridge": {
+            "arn_pattern": "arn:*:mediaconnect:*:*:bridge:*:*",
+            "condition_keys": null
+        },
         "Entitlement": {
             "arn_pattern": "arn:*:mediaconnect:*:*:entitlement:*:*",
             "condition_keys": null
         },
         "Flow": {
             "arn_pattern": "arn:*:mediaconnect:*:*:flow:*:*",
             "condition_keys": null
         },
+        "Gateway": {
+            "arn_pattern": "arn:*:mediaconnect:*:*:gateway:*:*",
+            "condition_keys": null
+        },
+        "GatewayInstance": {
+            "arn_pattern": "arn:*:mediaconnect:*:*:gateway:*:*:instance:*",
+            "condition_keys": null
+        },
         "Output": {
             "arn_pattern": "arn:*:mediaconnect:*:*:output:*:*",
             "condition_keys": null
         },
         "Source": {
             "arn_pattern": "arn:*:mediaconnect:*:*:source:*:*",
             "condition_keys": null
```

### Comparing `iam_actions-1.2.20230414/iam_actions/services.json` & `iam_actions-1.2.20230415/iam_actions/services.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998215894413511%*

 * *Differences: {"'codewhisperer'": "{'Actions': {insert: [(1, 'DeleteProfile'), (4, 'ListTagsForResource'), (5, "*

 * *                    "'TagResource'), (6, 'UntagResource')]}, 'ConditionKeys': "*

 * *                    "['aws:RequestTag/${TagKey}', 'aws:ResourceTag/${TagKey}', 'aws:TagKeys']}",*

 * * "'es'": "{'Actions': {insert: [(28, 'DescribeDomainHealth')]}}"}*

```diff
@@ -3971,19 +3971,27 @@
             "arn:aws:codewhisperer:${Region}:${Account}:${ResourceType}/${ResourceId}"
         ],
         "ARNRegexes": [
             "^arn:aws:codewhisperer:.+:[0-9]+:.+"
         ],
         "Actions": [
             "CreateProfile",
+            "DeleteProfile",
             "GenerateRecommendations",
             "ListProfiles",
+            "ListTagsForResource",
+            "TagResource",
+            "UntagResource",
             "UpdateProfile"
         ],
-        "ConditionKeys": [],
+        "ConditionKeys": [
+            "aws:RequestTag/${TagKey}",
+            "aws:ResourceTag/${TagKey}",
+            "aws:TagKeys"
+        ],
         "HasResource": true,
         "ServiceNames": [
             "Amazon CodeWhisperer"
         ]
     },
     "cognito-identity": {
         "ARNFormats": [
@@ -7833,14 +7841,15 @@
             "DeleteOutboundCrossClusterSearchConnection",
             "DeletePackage",
             "DeleteVpcEndpoint",
             "DescribeDomain",
             "DescribeDomainAutoTunes",
             "DescribeDomainChangeProgress",
             "DescribeDomainConfig",
+            "DescribeDomainHealth",
             "DescribeDomains",
             "DescribeDryRunProgress",
             "DescribeElasticsearchDomain",
             "DescribeElasticsearchDomainConfig",
             "DescribeElasticsearchDomains",
             "DescribeElasticsearchInstanceTypeLimits",
             "DescribeInboundConnections",
```

### Comparing `iam_actions-1.2.20230414/pyproject.toml` & `iam_actions-1.2.20230415/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230414"
+version = "1.2.20230415"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230414/setup.py` & `iam_actions-1.2.20230415/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230414',
+    'version': '1.2.20230415',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230414/PKG-INFO` & `iam_actions-1.2.20230415/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230414
+Version: 1.2.20230415
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

