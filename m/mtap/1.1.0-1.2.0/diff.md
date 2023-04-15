# Comparing `tmp/mtap-1.1.0.tar.gz` & `tmp/mtap-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtap-1.1.0.tar", last modified: Thu Mar 16 17:28:32 2023, max compression
+gzip compressed data, was "mtap-1.2.0.tar", last modified: Sat Apr 15 17:37:51 2023, max compression
```

## Comparing `mtap-1.1.0.tar` & `mtap-1.2.0.tar`

### file list

```diff
@@ -1,308 +1,315 @@
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.810363 mtap-1.1.0/
--rw-r--r--   0 knol0061   (501) staff       (20)       94 2022-10-20 17:05:59.000000 mtap-1.1.0/.dockerignore
--rw-r--r--   0 knol0061   (501) staff       (20)      122 2022-12-16 21:10:42.000000 mtap-1.1.0/.flake8
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.735421 mtap-1.1.0/.github/
--rw-r--r--   0 knol0061   (501) staff       (20)      273 2023-03-09 21:39:14.000000 mtap-1.1.0/.github/dependabot.yml
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.741165 mtap-1.1.0/.github/workflows/
--rw-r--r--   0 knol0061   (501) staff       (20)     2820 2023-02-06 20:02:45.000000 mtap-1.1.0/.github/workflows/ci.yml
--rw-r--r--   0 knol0061   (501) staff       (20)     5326 2023-03-09 18:01:06.000000 mtap-1.1.0/.gitignore
--rw-r--r--   0 knol0061   (501) staff       (20)      708 2023-02-23 20:20:04.000000 mtap-1.1.0/Dockerfile-dev
--rw-r--r--   0 knol0061   (501) staff       (20)    11358 2020-05-14 14:53:51.000000 mtap-1.1.0/LICENSE.txt
--rw-r--r--   0 knol0061   (501) staff       (20)    17357 2023-03-16 17:28:32.809639 mtap-1.1.0/PKG-INFO
--rw-r--r--   0 knol0061   (501) staff       (20)     2786 2023-03-16 17:26:11.000000 mtap-1.1.0/README.md
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.755008 mtap-1.1.0/go/
--rw-r--r--   0 knol0061   (501) staff       (20)     1343 2020-05-14 14:53:51.000000 mtap-1.1.0/go/Makefile
--rw-r--r--   0 knol0061   (501) staff       (20)     1611 2023-03-16 17:26:11.000000 mtap-1.1.0/go/doc.go
--rw-r--r--   0 knol0061   (501) staff       (20)     1943 2023-03-16 17:26:11.000000 mtap-1.1.0/go/go.mod
--rw-r--r--   0 knol0061   (501) staff       (20)    65987 2023-03-16 17:26:11.000000 mtap-1.1.0/go/go.sum
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.681890 mtap-1.1.0/go/mtap/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.681320 mtap-1.1.0/go/mtap/api/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.810604 mtap-1.1.0/go/mtap/api/v1/
--rw-r--r--   0 knol0061   (501) staff       (20)    94278 2023-03-16 17:14:50.000000 mtap-1.1.0/go/mtap/api/v1/events.pb.go
--rw-r--r--   0 knol0061   (501) staff       (20)    61461 2023-03-16 17:14:50.000000 mtap-1.1.0/go/mtap/api/v1/events.pb.gw.go
--rw-r--r--   0 knol0061   (501) staff       (20)    30458 2023-03-16 17:14:50.000000 mtap-1.1.0/go/mtap/api/v1/events.swagger.json
--rw-r--r--   0 knol0061   (501) staff       (20)    27349 2023-03-16 17:14:50.000000 mtap-1.1.0/go/mtap/api/v1/processing.pb.go
--rw-r--r--   0 knol0061   (501) staff       (20)    14459 2023-03-16 17:14:50.000000 mtap-1.1.0/go/mtap/api/v1/processing.pb.gw.go
--rw-r--r--   0 knol0061   (501) staff       (20)     8603 2023-03-16 17:14:50.000000 mtap-1.1.0/go/mtap/api/v1/processing.swagger.json
--rw-r--r--   0 knol0061   (501) staff       (20)    43110 2023-03-16 17:14:51.000000 mtap-1.1.0/go/mtap/api/v1/swaggers.go
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.814453 mtap-1.1.0/go/mtap/consul/
--rw-r--r--   0 knol0061   (501) staff       (20)     2981 2022-12-07 20:42:08.000000 mtap-1.1.0/go/mtap/consul/resolver.go
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.819680 mtap-1.1.0/go/mtap/processors/
--rw-r--r--   0 knol0061   (501) staff       (20)     7775 2022-12-07 20:42:08.000000 mtap-1.1.0/go/mtap/processors/processors.go
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.760440 mtap-1.1.0/go/mtap-gateway/
--rw-r--r--   0 knol0061   (501) staff       (20)     5520 2023-03-16 17:05:40.000000 mtap-1.1.0/go/mtap-gateway/mtap-gateway.go
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.823198 mtap-1.1.0/go/store-swaggers/
--rw-r--r--   0 knol0061   (501) staff       (20)     1359 2022-12-07 20:42:08.000000 mtap-1.1.0/go/store-swaggers/main.go
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.682739 mtap-1.1.0/go/third_party/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.682966 mtap-1.1.0/go/third_party/googleapis/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.683253 mtap-1.1.0/go/third_party/googleapis/google/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.827247 mtap-1.1.0/go/third_party/googleapis/google/api/
--rw-r--r--   0 knol0061   (501) staff       (20)     1045 2023-03-16 17:26:11.000000 mtap-1.1.0/go/third_party/googleapis/google/api/annotations.proto
--rw-r--r--   0 knol0061   (501) staff       (20)     3604 2023-03-16 17:26:11.000000 mtap-1.1.0/go/third_party/googleapis/google/api/field_behavior.proto
--rw-r--r--   0 knol0061   (501) staff       (20)    15140 2023-03-16 17:26:11.000000 mtap-1.1.0/go/third_party/googleapis/google/api/http.proto
--rw-r--r--   0 knol0061   (501) staff       (20)     2693 2023-03-16 17:26:11.000000 mtap-1.1.0/go/third_party/googleapis/google/api/httpbody.proto
--rw-r--r--   0 knol0061   (501) staff       (20)      215 2020-05-14 14:53:51.000000 mtap-1.1.0/go/tools.go
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.853969 mtap-1.1.0/java/
--rw-r--r--   0 knol0061   (501) staff       (20)     7714 2023-03-16 17:26:11.000000 mtap-1.1.0/java/build.gradle
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.684143 mtap-1.1.0/java/gradle/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.866459 mtap-1.1.0/java/gradle/wrapper/
--rw-r--r--   0 knol0061   (501) staff       (20)    60756 2023-03-09 18:01:06.000000 mtap-1.1.0/java/gradle/wrapper/gradle-wrapper.jar
--rw-r--r--   0 knol0061   (501) staff       (20)      202 2023-03-09 18:01:06.000000 mtap-1.1.0/java/gradle/wrapper/gradle-wrapper.properties
--rwxr-xr-x   0 knol0061   (501) staff       (20)     8188 2023-03-09 18:01:06.000000 mtap-1.1.0/java/gradlew
--rw-r--r--   0 knol0061   (501) staff       (20)     2838 2023-03-09 18:01:06.000000 mtap-1.1.0/java/gradlew.bat
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.870615 mtap-1.1.0/java/log_resources/
--rw-r--r--   0 knol0061   (501) staff       (20)      396 2021-08-30 15:58:40.000000 mtap-1.1.0/java/log_resources/log4j2.xml
--rw-r--r--   0 knol0061   (501) staff       (20)      650 2020-05-14 14:53:51.000000 mtap-1.1.0/java/settings.gradle
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.691681 mtap-1.1.0/java/src/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.689923 mtap-1.1.0/java/src/main/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.685797 mtap-1.1.0/java/src/main/java/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.686151 mtap-1.1.0/java/src/main/java/edu/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.686435 mtap-1.1.0/java/src/main/java/edu/umn/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.686749 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.903217 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/
--rw-r--r--   0 knol0061   (501) staff       (20)    32081 2023-02-23 20:20:04.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/EventsServer.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1042 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/ExperimentalApi.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1046 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/Internal.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1438 2021-08-30 15:58:40.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/MTAP.java
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.953370 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/common/
--rw-r--r--   0 knol0061   (501) staff       (20)    11652 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/common/AbstractJsonObject.java
--rw-r--r--   0 knol0061   (501) staff       (20)     3187 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/common/Config.java
--rw-r--r--   0 knol0061   (501) staff       (20)     6838 2022-08-03 15:52:44.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/common/ConfigImpl.java
--rw-r--r--   0 knol0061   (501) staff       (20)     2688 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObject.java
--rw-r--r--   0 knol0061   (501) staff       (20)     3324 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObjectBuilder.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1745 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObjectImpl.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1583 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/common/Server.java
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.982074 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/
--rw-r--r--   0 knol0061   (501) staff       (20)     3269 2022-12-07 20:42:08.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/ConsulDiscoveryMechanism.java
--rw-r--r--   0 knol0061   (501) staff       (20)     4068 2022-12-07 20:42:08.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/ConsulNameResolverProvider.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1192 2022-12-07 20:42:08.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/Discovery.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1057 2022-12-07 20:42:08.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/DiscoveryMechanism.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1446 2022-12-07 20:42:08.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/ServiceInfo.java
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.001584 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/examples/
--rw-r--r--   0 knol0061   (501) staff       (20)     2282 2020-09-28 17:50:36.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/examples/HelloWorldExample.java
--rw-r--r--   0 knol0061   (501) staff       (20)     5628 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/examples/ReferenceLabelsExampleProcessor.java
--rw-r--r--   0 knol0061   (501) staff       (20)     4406 2022-12-07 20:42:08.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/examples/WordOccurrencesExampleProcessor.java
--rw-r--r--   0 knol0061   (501) staff       (20)      711 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/examples/package-info.java
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.014129 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/exc/
--rw-r--r--   0 knol0061   (501) staff       (20)     1280 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/exc/EventExistsException.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1003 2022-08-03 15:52:44.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/exc/FailedToConnectToEventsException.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1149 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/exc/MtapException.java
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.098962 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/
--rw-r--r--   0 knol0061   (501) staff       (20)     2110 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/AbstractLabelIndex.java
--rw-r--r--   0 knol0061   (501) staff       (20)      872 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/Builder.java
--rw-r--r--   0 knol0061   (501) staff       (20)      775 2021-08-30 15:58:40.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/ChannelFactory.java
--rw-r--r--   0 knol0061   (501) staff       (20)    14937 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/DistinctLabelIndex.java
--rw-r--r--   0 knol0061   (501) staff       (20)    16528 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/Document.java
--rw-r--r--   0 knol0061   (501) staff       (20)    16546 2021-08-30 15:58:40.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/Event.java
--rw-r--r--   0 knol0061   (501) staff       (20)    13871 2022-08-03 15:52:44.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/EventsClient.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1978 2023-03-09 14:17:39.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/EventsClientPool.java
--rw-r--r--   0 knol0061   (501) staff       (20)    13061 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/GenericLabel.java
--rw-r--r--   0 knol0061   (501) staff       (20)     5777 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/GenericLabelAdapter.java
--rw-r--r--   0 knol0061   (501) staff       (20)     5921 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/Label.java
--rw-r--r--   0 knol0061   (501) staff       (20)    10132 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/LabelIndex.java
--rw-r--r--   0 knol0061   (501) staff       (20)     2361 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/LabelIndexInfo.java
--rw-r--r--   0 knol0061   (501) staff       (20)     2030 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/Labeler.java
--rw-r--r--   0 knol0061   (501) staff       (20)     2108 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/ProtoLabelAdapter.java
--rw-r--r--   0 knol0061   (501) staff       (20)     2632 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/Span.java
--rw-r--r--   0 knol0061   (501) staff       (20)    19216 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/StandardLabelIndex.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1454 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/TextSpan.java
--rw-r--r--   0 knol0061   (501) staff       (20)      864 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/package-info.java
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.191306 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/
--rw-r--r--   0 knol0061   (501) staff       (20)     7200 2023-01-25 20:34:46.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/DefaultProcessorService.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1404 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/DefaultTimingService.java
--rw-r--r--   0 knol0061   (501) staff       (20)     2388 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/DocumentProcessor.java
--rw-r--r--   0 knol0061   (501) staff       (20)     3801 2020-09-25 12:43:54.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/EventProcessor.java
--rw-r--r--   0 knol0061   (501) staff       (20)      803 2022-10-20 17:05:59.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/HSMHealthService.java
--rw-r--r--   0 knol0061   (501) staff       (20)      288 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/HealthService.java
--rw-r--r--   0 knol0061   (501) staff       (20)      277 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/KeyValue.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1892 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/LabelIndexDescription.java
--rw-r--r--   0 knol0061   (501) staff       (20)     2522 2021-08-30 15:58:40.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/LocalProcessorRunner.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1542 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ParameterDescription.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1438 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessingResult.java
--rw-r--r--   0 knol0061   (501) staff       (20)     2217 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/Processor.java
--rw-r--r--   0 knol0061   (501) staff       (20)     6864 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorBase.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1003 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorContext.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1212 2021-08-30 15:58:40.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorRunner.java
--rw-r--r--   0 knol0061   (501) staff       (20)    16591 2023-01-25 20:34:46.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorServer.java
--rw-r--r--   0 knol0061   (501) staff       (20)      773 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorService.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1489 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/PropertyDescription.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1877 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/RunningVariance.java
--rw-r--r--   0 knol0061   (501) staff       (20)     2773 2022-12-07 20:42:08.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/StandardChannelFactory.java
--rw-r--r--   0 knol0061   (501) staff       (20)     2369 2022-10-20 17:05:59.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/Stopwatch.java
--rw-r--r--   0 knol0061   (501) staff       (20)      381 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/TimingService.java
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.199082 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/utilities/
--rw-r--r--   0 knol0061   (501) staff       (20)     1132 2020-09-25 12:43:54.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/utilities/Helpers.java
--rw-r--r--   0 knol0061   (501) staff       (20)     3089 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/utilities/PrintProcessorMetadata.java
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.690221 mtap-1.1.0/java/src/main/resources/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.690590 mtap-1.1.0/java/src/main/resources/edu/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.690978 mtap-1.1.0/java/src/main/resources/edu/umn/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.691280 mtap-1.1.0/java/src/main/resources/edu/umn/nlpie/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.202276 mtap-1.1.0/java/src/main/resources/edu/umn/nlpie/mtap/
--rw-r--r--   0 knol0061   (501) staff       (20)      980 2023-01-25 16:53:29.000000 mtap-1.1.0/java/src/main/resources/edu/umn/nlpie/mtap/defaultConfig.yml
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.695799 mtap-1.1.0/java/src/test/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.692416 mtap-1.1.0/java/src/test/java/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.692754 mtap-1.1.0/java/src/test/java/edu/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.693100 mtap-1.1.0/java/src/test/java/edu/umn/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.693456 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.695293 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.205846 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/common/
--rw-r--r--   0 knol0061   (501) staff       (20)     2937 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/common/ConfigTest.java
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.246995 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/
--rw-r--r--   0 knol0061   (501) staff       (20)     9334 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexAscendingViewTest.java
--rw-r--r--   0 knol0061   (501) staff       (20)     9496 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexDescendingViewTest.java
--rw-r--r--   0 knol0061   (501) staff       (20)    13774 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexTest.java
--rw-r--r--   0 knol0061   (501) staff       (20)     9602 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/DocumentTest.java
--rw-r--r--   0 knol0061   (501) staff       (20)     6141 2021-08-30 15:58:40.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/EventTest.java
--rw-r--r--   0 knol0061   (501) staff       (20)    14423 2022-08-03 15:52:44.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/EventsClientTest.java
--rw-r--r--   0 knol0061   (501) staff       (20)     3668 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/GenericLabelAdapterTest.java
--rw-r--r--   0 knol0061   (501) staff       (20)     5091 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/GenericLabelTest.java
--rw-r--r--   0 knol0061   (501) staff       (20)    23583 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexAscendingViewTest.java
--rw-r--r--   0 knol0061   (501) staff       (20)    23618 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexDescendingViewTest.java
--rw-r--r--   0 knol0061   (501) staff       (20)    21240 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexTest.java
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.277818 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/processing/
--rw-r--r--   0 knol0061   (501) staff       (20)     9165 2022-12-07 20:42:08.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/processing/DefaultProcessorServiceTest.java
--rw-r--r--   0 knol0061   (501) staff       (20)     1337 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/processing/DefaultTimingServiceTest.java
--rw-r--r--   0 knol0061   (501) staff       (20)     3958 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/processing/EventProcessorTest.java
--rw-r--r--   0 knol0061   (501) staff       (20)     2514 2021-08-30 15:58:40.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/processing/LocalProcessorRunnerTest.java
--rw-r--r--   0 knol0061   (501) staff       (20)     3624 2022-10-25 15:05:59.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/processing/ProcessorServerBuilderTest.java
--rw-r--r--   0 knol0061   (501) staff       (20)     2471 2023-01-25 16:29:06.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/processing/ProcessorServerTest.java
--rw-r--r--   0 knol0061   (501) staff       (20)     2378 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/processing/RunningVarianceTest.java
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.281294 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/utilities/
--rw-r--r--   0 knol0061   (501) staff       (20)     1429 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/utilities/PrintProcessorMetadataTest.java
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.696208 mtap-1.1.0/java/src/test/resources/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.696577 mtap-1.1.0/java/src/test/resources/edu/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.696950 mtap-1.1.0/java/src/test/resources/edu/umn/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.697315 mtap-1.1.0/java/src/test/resources/edu/umn/nlpie/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.284454 mtap-1.1.0/java/src/test/resources/edu/umn/nlpie/mtap/
--rw-r--r--   0 knol0061   (501) staff       (20)      613 2020-05-14 14:53:51.000000 mtap-1.1.0/java/src/test/resources/edu/umn/nlpie/mtap/ExampleMeta.yaml
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.698303 mtap-1.1.0/proto/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.698718 mtap-1.1.0/proto/mtap/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.699074 mtap-1.1.0/proto/mtap/api/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.292713 mtap-1.1.0/proto/mtap/api/v1/
--rw-r--r--   0 knol0061   (501) staff       (20)    12780 2021-08-30 15:58:40.000000 mtap-1.1.0/proto/mtap/api/v1/events.proto
--rw-r--r--   0 knol0061   (501) staff       (20)     4729 2021-08-30 15:58:40.000000 mtap-1.1.0/proto/mtap/api/v1/processing.proto
--rw-r--r--   0 knol0061   (501) staff       (20)     2318 2023-03-16 15:24:46.000000 mtap-1.1.0/pyproject.toml
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:31.706513 mtap-1.1.0/python/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.324729 mtap-1.1.0/python/docs/
--rw-r--r--   0 knol0061   (501) staff       (20)      582 2020-05-14 14:53:51.000000 mtap-1.1.0/python/docs/Makefile
--rw-r--r--   0 knol0061   (501) staff       (20)     6672 2023-02-23 21:37:12.000000 mtap-1.1.0/python/docs/conf.py
--rw-r--r--   0 knol0061   (501) staff       (20)       64 2023-02-23 21:37:12.000000 mtap-1.1.0/python/docs/deployment.rst
--rw-r--r--   0 knol0061   (501) staff       (20)      371 2023-02-23 21:37:12.000000 mtap-1.1.0/python/docs/index.rst
--rw-r--r--   0 knol0061   (501) staff       (20)      787 2020-05-14 14:53:51.000000 mtap-1.1.0/python/docs/make.bat
--rw-r--r--   0 knol0061   (501) staff       (20)     2827 2020-09-25 12:43:54.000000 mtap-1.1.0/python/docs/mtap.rst
--rw-r--r--   0 knol0061   (501) staff       (20)      253 2023-02-23 21:37:12.000000 mtap-1.1.0/python/docs/serialization.rst
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.378025 mtap-1.1.0/python/mtap/
--rw-r--r--   0 knol0061   (501) staff       (20)     1195 2022-12-16 21:10:42.000000 mtap-1.1.0/python/mtap/__init__.py
--rw-r--r--   0 knol0061   (501) staff       (20)     3179 2023-01-17 19:04:27.000000 mtap-1.1.0/python/mtap/__main__.py
--rw-r--r--   0 knol0061   (501) staff       (20)     5388 2023-01-17 19:04:27.000000 mtap-1.1.0/python/mtap/_config.py
--rw-r--r--   0 knol0061   (501) staff       (20)     4104 2022-12-07 20:42:08.000000 mtap-1.1.0/python/mtap/_discovery.py
--rw-r--r--   0 knol0061   (501) staff       (20)    15253 2023-02-06 20:02:45.000000 mtap-1.1.0/python/mtap/_events_service.py
--rw-r--r--   0 knol0061   (501) staff       (20)     3229 2022-12-16 21:10:42.000000 mtap-1.1.0/python/mtap/_structs.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.388274 mtap-1.1.0/python/mtap/api/
--rw-r--r--   0 knol0061   (501) staff       (20)      636 2020-05-14 14:53:51.000000 mtap-1.1.0/python/mtap/api/__init__.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.417955 mtap-1.1.0/python/mtap/api/v1/
--rw-r--r--   0 knol0061   (501) staff       (20)      646 2020-05-14 14:53:51.000000 mtap-1.1.0/python/mtap/api/v1/__init__.py
--rw-r--r--   0 knol0061   (501) staff       (20)    14226 2023-03-16 16:17:00.000000 mtap-1.1.0/python/mtap/api/v1/events_pb2.py
--rw-r--r--   0 knol0061   (501) staff       (20)    25839 2023-03-16 16:17:00.000000 mtap-1.1.0/python/mtap/api/v1/events_pb2_grpc.py
--rw-r--r--   0 knol0061   (501) staff       (20)     5254 2023-03-16 16:17:00.000000 mtap-1.1.0/python/mtap/api/v1/processing_pb2.py
--rw-r--r--   0 knol0061   (501) staff       (20)     6181 2023-03-16 16:17:00.000000 mtap-1.1.0/python/mtap/api/v1/processing_pb2_grpc.py
--rw-r--r--   0 knol0061   (501) staff       (20)      812 2020-05-14 14:53:51.000000 mtap-1.1.0/python/mtap/constants.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.456653 mtap-1.1.0/python/mtap/data/
--rw-r--r--   0 knol0061   (501) staff       (20)     1397 2022-12-15 19:04:02.000000 mtap-1.1.0/python/mtap/data/__init__.py
--rw-r--r--   0 knol0061   (501) staff       (20)     1565 2020-09-25 12:43:54.000000 mtap-1.1.0/python/mtap/data/_base.py
--rw-r--r--   0 knol0061   (501) staff       (20)    40001 2023-02-23 20:20:04.000000 mtap-1.1.0/python/mtap/data/_events.py
--rw-r--r--   0 knol0061   (501) staff       (20)     8321 2021-08-30 15:58:40.000000 mtap-1.1.0/python/mtap/data/_label_adapters.py
--rw-r--r--   0 knol0061   (501) staff       (20)    28162 2022-12-16 21:10:42.000000 mtap-1.1.0/python/mtap/data/_label_indices.py
--rw-r--r--   0 knol0061   (501) staff       (20)    17582 2022-12-16 21:10:42.000000 mtap-1.1.0/python/mtap/data/_labels.py
--rw-r--r--   0 knol0061   (501) staff       (20)      980 2022-12-07 20:42:08.000000 mtap-1.1.0/python/mtap/defaultConfig.yml
--rw-r--r--   0 knol0061   (501) staff       (20)    31561 2023-02-23 21:37:12.000000 mtap-1.1.0/python/mtap/deployment.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.491879 mtap-1.1.0/python/mtap/examples/
--rw-r--r--   0 knol0061   (501) staff       (20)      635 2020-05-14 14:53:51.000000 mtap-1.1.0/python/mtap/examples/__init__.py
--rw-r--r--   0 knol0061   (501) staff       (20)     2737 2022-10-25 15:05:59.000000 mtap-1.1.0/python/mtap/examples/exampleDeploymentConfiguration.yml
--rw-r--r--   0 knol0061   (501) staff       (20)     1018 2022-10-25 15:05:59.000000 mtap-1.1.0/python/mtap/examples/examplePipelineConfiguration.yml
--rw-r--r--   0 knol0061   (501) staff       (20)     3435 2022-12-16 21:10:42.000000 mtap-1.1.0/python/mtap/examples/example_pipeline.py
--rw-r--r--   0 knol0061   (501) staff       (20)     2263 2023-01-25 20:34:46.000000 mtap-1.1.0/python/mtap/examples/example_processor.py
--rw-r--r--   0 knol0061   (501) staff       (20)     2549 2020-09-25 12:43:54.000000 mtap-1.1.0/python/mtap/examples/example_references_processor.py
--rw-r--r--   0 knol0061   (501) staff       (20)     1829 2020-09-25 12:43:54.000000 mtap-1.1.0/python/mtap/examples/print_processor_meta.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.503591 mtap-1.1.0/python/mtap/examples/serialization/
--rw-r--r--   0 knol0061   (501) staff       (20)      603 2022-12-16 21:10:42.000000 mtap-1.1.0/python/mtap/examples/serialization/__init__.py
--rw-r--r--   0 knol0061   (501) staff       (20)     3366 2022-12-16 21:10:42.000000 mtap-1.1.0/python/mtap/examples/serialization/brat_converter.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.517699 mtap-1.1.0/python/mtap/examples/tutorial/
--rw-r--r--   0 knol0061   (501) staff       (20)      635 2020-05-14 14:53:51.000000 mtap-1.1.0/python/mtap/examples/tutorial/__init__.py
--rw-r--r--   0 knol0061   (501) staff       (20)     1004 2020-09-25 12:43:54.000000 mtap-1.1.0/python/mtap/examples/tutorial/hello.py
--rw-r--r--   0 knol0061   (501) staff       (20)     1241 2022-12-16 21:10:42.000000 mtap-1.1.0/python/mtap/examples/tutorial/pipeline.py
--rw-r--r--   0 knol0061   (501) staff       (20)    14203 2022-12-16 21:10:42.000000 mtap-1.1.0/python/mtap/metrics.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.567381 mtap-1.1.0/python/mtap/processing/
--rw-r--r--   0 knol0061   (501) staff       (20)     1185 2022-12-15 19:04:02.000000 mtap-1.1.0/python/mtap/processing/__init__.py
--rw-r--r--   0 knol0061   (501) staff       (20)    15515 2023-02-23 21:37:12.000000 mtap-1.1.0/python/mtap/processing/_base.py
--rw-r--r--   0 knol0061   (501) staff       (20)    43244 2023-02-06 20:02:45.000000 mtap-1.1.0/python/mtap/processing/_pipeline.py
--rw-r--r--   0 knol0061   (501) staff       (20)     5730 2023-02-23 20:20:04.000000 mtap-1.1.0/python/mtap/processing/_runners.py
--rw-r--r--   0 knol0061   (501) staff       (20)    19503 2023-02-06 20:02:45.000000 mtap-1.1.0/python/mtap/processing/_service.py
--rw-r--r--   0 knol0061   (501) staff       (20)     2213 2022-12-16 21:10:42.000000 mtap-1.1.0/python/mtap/processing/_timing.py
--rw-r--r--   0 knol0061   (501) staff       (20)    11368 2021-08-30 15:58:40.000000 mtap-1.1.0/python/mtap/processing/descriptions.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.579127 mtap-1.1.0/python/mtap/processors/
--rw-r--r--   0 knol0061   (501) staff       (20)      615 2022-12-16 21:10:42.000000 mtap-1.1.0/python/mtap/processors/__init__.py
--rw-r--r--   0 knol0061   (501) staff       (20)     3426 2021-08-30 15:58:40.000000 mtap-1.1.0/python/mtap/processors/copy_document.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.599388 mtap-1.1.0/python/mtap/serialization/
--rw-r--r--   0 knol0061   (501) staff       (20)      939 2022-12-16 21:10:42.000000 mtap-1.1.0/python/mtap/serialization/__init__.py
--rw-r--r--   0 knol0061   (501) staff       (20)    11476 2023-02-01 21:10:45.000000 mtap-1.1.0/python/mtap/serialization/_serialization.py
--rw-r--r--   0 knol0061   (501) staff       (20)     6748 2022-12-16 21:17:09.000000 mtap-1.1.0/python/mtap/serialization/brat.py
--rw-r--r--   0 knol0061   (501) staff       (20)     2348 2022-12-16 21:10:42.000000 mtap-1.1.0/python/mtap/serialization/event.schema.json
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.610223 mtap-1.1.0/python/mtap/utilities/
--rw-r--r--   0 knol0061   (501) staff       (20)     4546 2023-02-06 20:02:45.000000 mtap-1.1.0/python/mtap/utilities/__init__.py
--rw-r--r--   0 knol0061   (501) staff       (20)     1231 2020-09-25 12:43:54.000000 mtap-1.1.0/python/mtap/utilities/tokenization.py
--rw-r--r--   0 knol0061   (501) staff       (20)      160 2023-03-16 17:28:31.000000 mtap-1.1.0/python/mtap/version.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.383289 mtap-1.1.0/python/mtap.egg-info/
--rw-r--r--   0 knol0061   (501) staff       (20)    17357 2023-03-16 17:28:31.000000 mtap-1.1.0/python/mtap.egg-info/PKG-INFO
--rw-r--r--   0 knol0061   (501) staff       (20)    10553 2023-03-16 17:28:31.000000 mtap-1.1.0/python/mtap.egg-info/SOURCES.txt
--rw-r--r--   0 knol0061   (501) staff       (20)        1 2023-03-16 17:28:31.000000 mtap-1.1.0/python/mtap.egg-info/dependency_links.txt
--rw-r--r--   0 knol0061   (501) staff       (20)      303 2023-03-16 17:28:31.000000 mtap-1.1.0/python/mtap.egg-info/requires.txt
--rw-r--r--   0 knol0061   (501) staff       (20)        5 2023-03-16 17:28:31.000000 mtap-1.1.0/python/mtap.egg-info/top_level.txt
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.644107 mtap-1.1.0/python/tests/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.656867 mtap-1.1.0/python/tests/config/
--rw-r--r--   0 knol0061   (501) staff       (20)       26 2022-12-07 20:42:08.000000 mtap-1.1.0/python/tests/config/brokenConfig.yaml
--rw-r--r--   0 knol0061   (501) staff       (20)     2001 2022-12-07 20:42:08.000000 mtap-1.1.0/python/tests/config/test_config.py
--rw-r--r--   0 knol0061   (501) staff       (20)       45 2022-12-07 20:42:08.000000 mtap-1.1.0/python/tests/config/workingConfig.yaml
--rwxr-xr-x   0 knol0061   (501) staff       (20)     3956 2023-01-17 19:04:27.000000 mtap-1.1.0/python/tests/conftest.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.667353 mtap-1.1.0/python/tests/consul/
--rw-r--r--   0 knol0061   (501) staff       (20)     1149 2022-12-07 20:42:08.000000 mtap-1.1.0/python/tests/consul/integrationConfig.yaml
--rw-r--r--   0 knol0061   (501) staff       (20)     5340 2023-02-06 20:02:45.000000 mtap-1.1.0/python/tests/consul/test_discovery.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.710235 mtap-1.1.0/python/tests/data/
--rw-r--r--   0 knol0061   (501) staff       (20)     4486 2021-08-30 15:58:40.000000 mtap-1.1.0/python/tests/data/test_document.py
--rw-r--r--   0 knol0061   (501) staff       (20)     5570 2022-12-16 21:10:42.000000 mtap-1.1.0/python/tests/data/test_event.py
--rw-r--r--   0 knol0061   (501) staff       (20)     6066 2021-08-30 15:58:40.000000 mtap-1.1.0/python/tests/data/test_events_client.py
--rw-r--r--   0 knol0061   (501) staff       (20)     4611 2020-09-25 12:43:54.000000 mtap-1.1.0/python/tests/data/test_generic_label.py
--rw-r--r--   0 knol0061   (501) staff       (20)     1460 2020-09-25 12:43:54.000000 mtap-1.1.0/python/tests/data/test_labels.py
--rw-r--r--   0 knol0061   (501) staff       (20)    15073 2020-09-25 12:43:54.000000 mtap-1.1.0/python/tests/data/test_standard_ascending_label_index.py
--rw-r--r--   0 knol0061   (501) staff       (20)    14164 2020-09-25 12:43:54.000000 mtap-1.1.0/python/tests/data/test_standard_descending_label_index.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.717246 mtap-1.1.0/python/tests/deployment/
--rw-r--r--   0 knol0061   (501) staff       (20)     3031 2023-02-06 20:02:45.000000 mtap-1.1.0/python/tests/deployment/test_deployment.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.728105 mtap-1.1.0/python/tests/integration/
--rw-r--r--   0 knol0061   (501) staff       (20)     2374 2022-10-25 15:05:59.000000 mtap-1.1.0/python/tests/integration/test_hello_world_tutorial.py
--rw-r--r--   0 knol0061   (501) staff       (20)    11892 2023-02-06 20:02:45.000000 mtap-1.1.0/python/tests/integration/test_integration.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.761857 mtap-1.1.0/python/tests/processing/
--rw-r--r--   0 knol0061   (501) staff       (20)      271 2022-10-25 15:05:59.000000 mtap-1.1.0/python/tests/processing/pipeline.yml
--rw-r--r--   0 knol0061   (501) staff       (20)     1565 2020-09-25 12:43:54.000000 mtap-1.1.0/python/tests/processing/test_event_processor.py
--rw-r--r--   0 knol0061   (501) staff       (20)     3745 2022-10-25 15:05:59.000000 mtap-1.1.0/python/tests/processing/test_pipeline.py
--rw-r--r--   0 knol0061   (501) staff       (20)     1188 2020-09-25 12:43:54.000000 mtap-1.1.0/python/tests/processing/test_pipeline_result.py
--rw-r--r--   0 knol0061   (501) staff       (20)     1057 2022-12-16 21:10:42.000000 mtap-1.1.0/python/tests/processing/test_processor.py
--rw-r--r--   0 knol0061   (501) staff       (20)     3909 2022-12-07 20:42:08.000000 mtap-1.1.0/python/tests/processing/test_processor_service.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.766754 mtap-1.1.0/python/tests/processors/
--rw-r--r--   0 knol0061   (501) staff       (20)     1338 2020-09-25 12:43:54.000000 mtap-1.1.0/python/tests/processors/test_copy_document.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.773277 mtap-1.1.0/python/tests/references/
--rw-r--r--   0 knol0061   (501) staff       (20)     4497 2022-10-25 15:05:59.000000 mtap-1.1.0/python/tests/references/test_references.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.799550 mtap-1.1.0/python/tests/serialization/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 17:28:32.808401 mtap-1.1.0/python/tests/serialization/brat/
--rw-r--r--   0 knol0061   (501) staff       (20)      452 2022-12-16 21:10:42.000000 mtap-1.1.0/python/tests/serialization/brat/100_1442.ann
--rw-r--r--   0 knol0061   (501) staff       (20)     2583 2022-12-16 21:10:42.000000 mtap-1.1.0/python/tests/serialization/brat/100_1442.txt
--rw-r--r--   0 knol0061   (501) staff       (20)     1484 2022-12-16 21:10:42.000000 mtap-1.1.0/python/tests/serialization/test_brat.py
--rw-r--r--   0 knol0061   (501) staff       (20)     2292 2022-12-16 21:10:42.000000 mtap-1.1.0/python/tests/serialization/test_json.py
--rw-r--r--   0 knol0061   (501) staff       (20)     2800 2022-12-16 21:10:42.000000 mtap-1.1.0/python/tests/serialization/test_pickle.py
--rw-r--r--   0 knol0061   (501) staff       (20)     1796 2022-12-16 21:10:42.000000 mtap-1.1.0/python/tests/serialization/test_serialization.py
--rw-r--r--   0 knol0061   (501) staff       (20)     2296 2022-12-16 21:10:42.000000 mtap-1.1.0/python/tests/serialization/test_yml.py
--rw-r--r--   0 knol0061   (501) staff       (20)    14905 2022-12-07 20:42:08.000000 mtap-1.1.0/python/tests/slf4j-simple-2.0.3.jar
--rwxr-xr-x   0 knol0061   (501) staff       (20)    30744 2022-10-25 15:05:59.000000 mtap-1.1.0/python/tests/test_events_service.py
--rw-r--r--   0 knol0061   (501) staff       (20)     6115 2022-12-16 21:10:42.000000 mtap-1.1.0/python/tests/test_metrics.py
--rw-r--r--   0 knol0061   (501) staff       (20)     7727 2020-05-14 14:53:51.000000 mtap-1.1.0/python/tests/test_structs.py
--rw-r--r--   0 knol0061   (501) staff       (20)       38 2023-03-16 17:28:32.810512 mtap-1.1.0/setup.cfg
--rw-r--r--   0 knol0061   (501) staff       (20)     1797 2023-03-09 21:36:13.000000 mtap-1.1.0/setup.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/
+-rw-r--r--   0 ben       (1000) ben       (1000)       94 2023-03-11 15:03:25.000000 mtap-1.2.0/.dockerignore
+-rw-r--r--   0 ben       (1000) ben       (1000)      122 2023-03-11 15:03:25.000000 mtap-1.2.0/.flake8
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/.github/
+-rw-r--r--   0 ben       (1000) ben       (1000)      273 2023-03-11 15:03:25.000000 mtap-1.2.0/.github/dependabot.yml
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/.github/workflows/
+-rw-r--r--   0 ben       (1000) ben       (1000)     2820 2023-03-11 15:03:25.000000 mtap-1.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 ben       (1000) ben       (1000)     5326 2023-03-30 15:59:37.000000 mtap-1.2.0/.gitignore
+-rw-r--r--   0 ben       (1000) ben       (1000)      434 2023-03-30 15:59:37.000000 mtap-1.2.0/.readthedocs.yaml
+-rw-r--r--   0 ben       (1000) ben       (1000)      708 2023-03-11 15:03:25.000000 mtap-1.2.0/Dockerfile-dev
+-rw-r--r--   0 ben       (1000) ben       (1000)    11358 2023-03-11 15:03:25.000000 mtap-1.2.0/LICENSE.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)    17047 2023-04-15 17:37:51.555431 mtap-1.2.0/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)     2476 2023-04-15 15:21:56.000000 mtap-1.2.0/README.md
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/go/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1343 2023-03-11 15:03:25.000000 mtap-1.2.0/go/Makefile
+-rw-r--r--   0 ben       (1000) ben       (1000)     1477 2023-03-30 15:59:37.000000 mtap-1.2.0/go/doc.go
+-rw-r--r--   0 ben       (1000) ben       (1000)     1835 2023-03-30 15:59:37.000000 mtap-1.2.0/go/go.mod
+-rw-r--r--   0 ben       (1000) ben       (1000)    65077 2023-03-30 15:59:37.000000 mtap-1.2.0/go/go.sum
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/go/mtap/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/go/mtap/api/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/go/mtap/api/v1/
+-rw-r--r--   0 ben       (1000) ben       (1000)   104710 2023-04-14 22:53:36.000000 mtap-1.2.0/go/mtap/api/v1/events.pb.go
+-rw-r--r--   0 ben       (1000) ben       (1000)    71157 2023-04-14 22:53:36.000000 mtap-1.2.0/go/mtap/api/v1/events.pb.gw.go
+-rw-r--r--   0 ben       (1000) ben       (1000)    26240 2023-04-14 22:53:36.000000 mtap-1.2.0/go/mtap/api/v1/events_grpc.pb.go
+-rw-r--r--   0 ben       (1000) ben       (1000)    33560 2023-04-14 22:53:36.000000 mtap-1.2.0/go/mtap/api/v1/processing.pb.go
+-rw-r--r--   0 ben       (1000) ben       (1000)    16594 2023-04-14 22:53:36.000000 mtap-1.2.0/go/mtap/api/v1/processing.pb.gw.go
+-rw-r--r--   0 ben       (1000) ben       (1000)     7483 2023-04-14 22:53:36.000000 mtap-1.2.0/go/mtap/api/v1/processing_grpc.pb.go
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/go/mtap/consul/
+-rw-r--r--   0 ben       (1000) ben       (1000)     2981 2023-03-11 15:03:25.000000 mtap-1.2.0/go/mtap/consul/resolver.go
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/go/mtap/processors/
+-rw-r--r--   0 ben       (1000) ben       (1000)     7921 2023-03-30 15:59:37.000000 mtap-1.2.0/go/mtap/processors/processors.go
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/go/mtap-gateway/
+-rw-r--r--   0 ben       (1000) ben       (1000)     4732 2023-04-14 22:47:09.000000 mtap-1.2.0/go/mtap-gateway/mtap-gateway.go
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/go/store-swaggers/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1359 2023-03-11 15:03:25.000000 mtap-1.2.0/go/store-swaggers/main.go
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/go/third_party/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/go/third_party/googleapis/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/go/third_party/googleapis/google/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/go/third_party/googleapis/google/api/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1045 2023-03-17 16:24:15.000000 mtap-1.2.0/go/third_party/googleapis/google/api/annotations.proto
+-rw-r--r--   0 ben       (1000) ben       (1000)     3604 2023-03-17 16:24:15.000000 mtap-1.2.0/go/third_party/googleapis/google/api/field_behavior.proto
+-rw-r--r--   0 ben       (1000) ben       (1000)    15140 2023-03-17 16:24:15.000000 mtap-1.2.0/go/third_party/googleapis/google/api/http.proto
+-rw-r--r--   0 ben       (1000) ben       (1000)     2693 2023-03-17 16:24:15.000000 mtap-1.2.0/go/third_party/googleapis/google/api/httpbody.proto
+-rw-r--r--   0 ben       (1000) ben       (1000)      283 2023-03-30 15:59:37.000000 mtap-1.2.0/go/tools.go
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/java/
+-rw-r--r--   0 ben       (1000) ben       (1000)     7975 2023-04-15 15:21:56.000000 mtap-1.2.0/java/build.gradle
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/gradle/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/java/gradle/wrapper/
+-rw-r--r--   0 ben       (1000) ben       (1000)    61608 2023-04-14 22:47:09.000000 mtap-1.2.0/java/gradle/wrapper/gradle-wrapper.jar
+-rw-r--r--   0 ben       (1000) ben       (1000)      221 2023-04-14 22:47:09.000000 mtap-1.2.0/java/gradle/wrapper/gradle-wrapper.properties
+-rwxr-xr-x   0 ben       (1000) ben       (1000)     8495 2023-04-14 22:47:09.000000 mtap-1.2.0/java/gradlew
+-rw-r--r--   0 ben       (1000) ben       (1000)     2868 2023-04-14 22:47:09.000000 mtap-1.2.0/java/gradlew.bat
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/java/log_resources/
+-rw-r--r--   0 ben       (1000) ben       (1000)      396 2023-03-11 15:03:25.000000 mtap-1.2.0/java/log_resources/log4j2.xml
+-rw-r--r--   0 ben       (1000) ben       (1000)      650 2023-03-11 15:03:25.000000 mtap-1.2.0/java/settings.gradle
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/main/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/main/java/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/main/java/edu/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/main/java/edu/umn/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/
+-rw-r--r--   0 ben       (1000) ben       (1000)    32081 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/EventsServer.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1042 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/ExperimentalApi.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1046 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/Internal.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1438 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/MTAP.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/
+-rw-r--r--   0 ben       (1000) ben       (1000)    11652 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/AbstractJsonObject.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     3187 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/Config.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     6838 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/ConfigImpl.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2688 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObject.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     3324 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObjectBuilder.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1745 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObjectImpl.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1583 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/Server.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/
+-rw-r--r--   0 ben       (1000) ben       (1000)     3269 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/ConsulDiscoveryMechanism.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     4068 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/ConsulNameResolverProvider.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1192 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/Discovery.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1057 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/DiscoveryMechanism.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1446 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/ServiceInfo.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/
+-rw-r--r--   0 ben       (1000) ben       (1000)      829 2023-04-14 22:47:09.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/ErrorThrower.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2282 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/HelloWorldExample.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     5628 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/ReferenceLabelsExampleProcessor.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     4406 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/WordOccurrencesExampleProcessor.java
+-rw-r--r--   0 ben       (1000) ben       (1000)      711 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/package-info.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.525431 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/exc/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1280 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/exc/EventExistsException.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1003 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/exc/FailedToConnectToEventsException.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1149 2023-04-14 01:30:11.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/exc/MtapException.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.535431 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/
+-rw-r--r--   0 ben       (1000) ben       (1000)     2110 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/AbstractLabelIndex.java
+-rw-r--r--   0 ben       (1000) ben       (1000)      872 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Builder.java
+-rw-r--r--   0 ben       (1000) ben       (1000)      775 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/ChannelFactory.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    14937 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/DistinctLabelIndex.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    16528 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Document.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    16546 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Event.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    13871 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/EventsClient.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1978 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/EventsClientPool.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    13061 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/GenericLabel.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     5777 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/GenericLabelAdapter.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     5921 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Label.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    10132 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/LabelIndex.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2361 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/LabelIndexInfo.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2030 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Labeler.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2108 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/ProtoLabelAdapter.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2632 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Span.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    19216 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/StandardLabelIndex.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1454 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/TextSpan.java
+-rw-r--r--   0 ben       (1000) ben       (1000)      864 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/package-info.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.535431 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/
+-rw-r--r--   0 ben       (1000) ben       (1000)     9045 2023-04-14 22:47:09.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/DefaultProcessorService.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1404 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/DefaultTimingService.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2388 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/DocumentProcessor.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     3801 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/EventProcessor.java
+-rw-r--r--   0 ben       (1000) ben       (1000)      803 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/HSMHealthService.java
+-rw-r--r--   0 ben       (1000) ben       (1000)      288 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/HealthService.java
+-rw-r--r--   0 ben       (1000) ben       (1000)      277 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/KeyValue.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1892 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/LabelIndexDescription.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2522 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/LocalProcessorRunner.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1542 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ParameterDescription.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1438 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessingResult.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2217 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/Processor.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     6864 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorBase.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1003 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorContext.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1212 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorRunner.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    17320 2023-04-14 22:47:09.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorServer.java
+-rw-r--r--   0 ben       (1000) ben       (1000)      773 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorService.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1489 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/PropertyDescription.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1877 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/RunningVariance.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2773 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/StandardChannelFactory.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2369 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/Stopwatch.java
+-rw-r--r--   0 ben       (1000) ben       (1000)      381 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/TimingService.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.535431 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/utilities/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1132 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/utilities/Helpers.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     3089 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/utilities/PrintProcessorMetadata.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/main/resources/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/main/resources/edu/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/main/resources/edu/umn/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/main/resources/edu/umn/nlpie/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.535431 mtap-1.2.0/java/src/main/resources/edu/umn/nlpie/mtap/
+-rw-r--r--   0 ben       (1000) ben       (1000)      980 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/main/resources/edu/umn/nlpie/mtap/defaultConfig.yml
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/java/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/java/edu/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/java/edu/umn/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.535431 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/common/
+-rw-r--r--   0 ben       (1000) ben       (1000)     2937 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/common/ConfigTest.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/
+-rw-r--r--   0 ben       (1000) ben       (1000)     9334 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexAscendingViewTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     9496 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexDescendingViewTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    13774 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     9602 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/DocumentTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     6141 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/EventTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    14423 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/EventsClientTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     3668 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/GenericLabelAdapterTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     5091 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/GenericLabelTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    23583 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexAscendingViewTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    23618 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexDescendingViewTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)    21240 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexTest.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/
+-rw-r--r--   0 ben       (1000) ben       (1000)     9161 2023-04-14 22:47:09.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/DefaultProcessorServiceTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     1337 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/DefaultTimingServiceTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     3958 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/EventProcessorTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2514 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/LocalProcessorRunnerTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     3624 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/ProcessorServerBuilderTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2471 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/ProcessorServerTest.java
+-rw-r--r--   0 ben       (1000) ben       (1000)     2378 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/RunningVarianceTest.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/utilities/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1429 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/utilities/PrintProcessorMetadataTest.java
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/resources/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/resources/edu/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/resources/edu/umn/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/java/src/test/resources/edu/umn/nlpie/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/java/src/test/resources/edu/umn/nlpie/mtap/
+-rw-r--r--   0 ben       (1000) ben       (1000)      613 2023-03-11 15:03:25.000000 mtap-1.2.0/java/src/test/resources/edu/umn/nlpie/mtap/ExampleMeta.yaml
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/proto/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/proto/mtap/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/proto/mtap/api/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/proto/mtap/api/v1/
+-rw-r--r--   0 ben       (1000) ben       (1000)    12815 2023-03-30 15:59:37.000000 mtap-1.2.0/proto/mtap/api/v1/events.proto
+-rw-r--r--   0 ben       (1000) ben       (1000)     4764 2023-03-30 15:59:37.000000 mtap-1.2.0/proto/mtap/api/v1/processing.proto
+-rw-r--r--   0 ben       (1000) ben       (1000)     2356 2023-04-15 15:21:56.000000 mtap-1.2.0/pyproject.toml
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.515432 mtap-1.2.0/python/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/docs/
+-rw-r--r--   0 ben       (1000) ben       (1000)      582 2023-03-11 15:03:25.000000 mtap-1.2.0/python/docs/Makefile
+-rw-r--r--   0 ben       (1000) ben       (1000)     6800 2023-04-14 22:47:09.000000 mtap-1.2.0/python/docs/conf.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      311 2023-04-14 22:47:09.000000 mtap-1.2.0/python/docs/deployment.rst
+-rw-r--r--   0 ben       (1000) ben       (1000)      371 2023-03-30 15:59:37.000000 mtap-1.2.0/python/docs/index.rst
+-rw-r--r--   0 ben       (1000) ben       (1000)      787 2023-03-11 15:03:25.000000 mtap-1.2.0/python/docs/make.bat
+-rw-r--r--   0 ben       (1000) ben       (1000)     3733 2023-04-14 22:47:09.000000 mtap-1.2.0/python/docs/mtap.rst
+-rw-r--r--   0 ben       (1000) ben       (1000)      549 2023-04-14 22:47:09.000000 mtap-1.2.0/python/docs/serialization.rst
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1195 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     3578 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/__main__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     5388 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/_config.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    15511 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/_events_service.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     3229 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/_structs.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/api/
+-rw-r--r--   0 ben       (1000) ben       (1000)      636 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/api/__init__.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/api/v1/
+-rw-r--r--   0 ben       (1000) ben       (1000)      646 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/api/v1/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    14255 2023-04-15 17:37:15.000000 mtap-1.2.0/python/mtap/api/v1/events_pb2.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    25839 2023-04-15 17:37:15.000000 mtap-1.2.0/python/mtap/api/v1/events_pb2_grpc.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     5283 2023-04-15 17:37:15.000000 mtap-1.2.0/python/mtap/api/v1/processing_pb2.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     6181 2023-04-15 17:37:15.000000 mtap-1.2.0/python/mtap/api/v1/processing_pb2_grpc.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      812 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/constants.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/data/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1191 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/data/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1565 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/data/_base.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    44144 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/data/_events.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     8321 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/data/_label_adapters.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    28162 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/data/_label_indices.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    16370 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/data/_labels.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      980 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/defaultConfig.yml
+-rw-r--r--   0 ben       (1000) ben       (1000)    23527 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/deployment.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     7405 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/discovery.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/examples/
+-rw-r--r--   0 ben       (1000) ben       (1000)      635 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/examples/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     2737 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/examples/exampleDeploymentConfiguration.yml
+-rw-r--r--   0 ben       (1000) ben       (1000)     1017 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/examples/examplePipelineConfiguration.yml
+-rw-r--r--   0 ben       (1000) ben       (1000)     3617 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/examples/example_pipeline.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     2514 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/examples/example_processor.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     2549 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/examples/example_references_processor.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1829 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/examples/print_processor_meta.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/examples/serialization/
+-rw-r--r--   0 ben       (1000) ben       (1000)      603 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/examples/serialization/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     3366 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/examples/serialization/brat_converter.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/examples/tutorial/
+-rw-r--r--   0 ben       (1000) ben       (1000)      635 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/examples/tutorial/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1004 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/examples/tutorial/hello.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1278 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/examples/tutorial/pipeline.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    14203 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/metrics.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/processing/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1782 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    10093 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_base.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    17462 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_error_handling.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      709 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_exc.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1911 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_mp_config.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     8733 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_mp_pipeline.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    14813 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_pipeline.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     5578 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_pipeline_components.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     9279 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_pipeline_results.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     8025 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_runners.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    18871 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_service.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     6317 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/_sources.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     8105 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/processing/descriptions.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/processors/
+-rw-r--r--   0 ben       (1000) ben       (1000)      615 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/processors/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     3426 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/processors/copy_document.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/serialization/
+-rw-r--r--   0 ben       (1000) ben       (1000)      987 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/serialization/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    12775 2023-04-14 22:47:09.000000 mtap-1.2.0/python/mtap/serialization/_serialization.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     6748 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/serialization/brat.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     2348 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/serialization/event.schema.json
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap/utilities/
+-rw-r--r--   0 ben       (1000) ben       (1000)     4546 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/utilities/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1231 2023-03-11 15:03:25.000000 mtap-1.2.0/python/mtap/utilities/tokenization.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      160 2023-04-15 17:37:51.000000 mtap-1.2.0/python/mtap/version.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.545431 mtap-1.2.0/python/mtap.egg-info/
+-rw-r--r--   0 ben       (1000) ben       (1000)    17047 2023-04-15 17:37:51.000000 mtap-1.2.0/python/mtap.egg-info/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)    10845 2023-04-15 17:37:51.000000 mtap-1.2.0/python/mtap.egg-info/SOURCES.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)        1 2023-04-15 17:37:51.000000 mtap-1.2.0/python/mtap.egg-info/dependency_links.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)      334 2023-04-15 17:37:51.000000 mtap-1.2.0/python/mtap.egg-info/requires.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)        5 2023-04-15 17:37:51.000000 mtap-1.2.0/python/mtap.egg-info/top_level.txt
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/config/
+-rw-r--r--   0 ben       (1000) ben       (1000)       26 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/config/brokenConfig.yaml
+-rw-r--r--   0 ben       (1000) ben       (1000)     2001 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/config/test_config.py
+-rw-r--r--   0 ben       (1000) ben       (1000)       45 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/config/workingConfig.yaml
+-rwxr-xr-x   0 ben       (1000) ben       (1000)     3990 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/conftest.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/consul/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1149 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/consul/integrationConfig.yaml
+-rw-r--r--   0 ben       (1000) ben       (1000)     5796 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/consul/test_discovery.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/data/
+-rw-r--r--   0 ben       (1000) ben       (1000)     4486 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/data/test_document.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     5570 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/data/test_event.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     6066 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/data/test_events_client.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     4611 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/data/test_generic_label.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1460 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/data/test_labels.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    15073 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/data/test_standard_ascending_label_index.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    14164 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/data/test_standard_descending_label_index.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/deployment/
+-rw-r--r--   0 ben       (1000) ben       (1000)     3212 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/deployment/test_deployment.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/integration/
+-rw-r--r--   0 ben       (1000) ben       (1000)     2386 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/integration/test_hello_world_tutorial.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    12156 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/integration/test_integration.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/processing/
+-rw-r--r--   0 ben       (1000) ben       (1000)      342 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/processing/pipeline.yml
+-rw-r--r--   0 ben       (1000) ben       (1000)     1565 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/processing/test_event_processor.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     3850 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/processing/test_pipeline.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1186 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/processing/test_pipeline_result.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1057 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/processing/test_processor.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     4036 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/processing/test_processor_service.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/processors/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1338 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/processors/test_copy_document.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/references/
+-rw-r--r--   0 ben       (1000) ben       (1000)     4584 2023-04-14 22:47:09.000000 mtap-1.2.0/python/tests/references/test_references.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/serialization/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-15 17:37:51.555431 mtap-1.2.0/python/tests/serialization/brat/
+-rw-r--r--   0 ben       (1000) ben       (1000)      452 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/serialization/brat/100_1442.ann
+-rw-r--r--   0 ben       (1000) ben       (1000)     2583 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/serialization/brat/100_1442.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)     1484 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/serialization/test_brat.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     2292 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/serialization/test_json.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     2800 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/serialization/test_pickle.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1796 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/serialization/test_serialization.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     2296 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/serialization/test_yml.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    14905 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/slf4j-simple-2.0.3.jar
+-rwxr-xr-x   0 ben       (1000) ben       (1000)    30744 2023-03-17 16:26:09.000000 mtap-1.2.0/python/tests/test_events_service.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     6115 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/test_metrics.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     7727 2023-03-11 15:03:25.000000 mtap-1.2.0/python/tests/test_structs.py
+-rw-r--r--   0 ben       (1000) ben       (1000)       38 2023-04-15 17:37:51.555431 mtap-1.2.0/setup.cfg
+-rw-r--r--   0 ben       (1000) ben       (1000)     1797 2023-03-11 15:03:25.000000 mtap-1.2.0/setup.py
```

### Comparing `mtap-1.1.0/.github/workflows/ci.yml` & `mtap-1.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/.gitignore` & `mtap-1.2.0/.gitignore`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -368,16 +368,16 @@
 # gradle/wrapper/gradle-wrapper.properties
 
 # go release folder
 /go/release/
 
 # generated code
 python/mtap/version.py
-python/mtap/api/v1/
 !python/mtap/api/v1/__init__.py
+python/mtap/api/v1/
 
 python/docs/_build
 
 .project
 .classpath
 
 Pipfile
```

### Comparing `mtap-1.1.0/Dockerfile-dev` & `mtap-1.2.0/Dockerfile-dev`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/LICENSE.txt` & `mtap-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/PKG-INFO` & `mtap-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtap
-Version: 1.1.0
+Version: 1.2.0
 Summary: A framework for distributed text analysis using gRPC and microservices-based architecture.
 Author-email: University of Minnesota NLP/IE Group <nlp-ie@umn.edu>, Ben Knoll <benknoll@umn.edu>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -235,15 +235,15 @@
 Provides-Extra: docs
 Provides-Extra: consul
 License-File: LICENSE.txt
 
 <p align="center">
   <a href="https://pypi.org/project/mtap/">
     <img src="https://img.shields.io/pypi/v/mtap" /></a>
-  <a href="https://central.sonatype.com/artifact/edu.umn.nlpie/mtap/1.1.0">
+  <a href="https://mvnrepository.com/artifact/edu.umn.nlpie/mtap">
     <img src="https://img.shields.io/maven-central/v/edu.umn.nlpie/mtap" /></a>
 </p>
 
 # MTAP
 
 [nlpie.github.io/mtap](https://nlpie.github.io/mtap)
 
@@ -270,48 +270,21 @@
 
 By using the microservice pattern, text analysis components can be deployed once and then mixed and matched in different pipelines. Components written in different languages can interoperate without hassle. We also provide a RESTful API gateway that lets you call components using HTTP.
 
 ### Scalability
 
 MTAP is designed to bridge the gap between prototyping new ideas and deploying them into a production environment. It supports calling components locally without using any network infastructure all the way up to deploying services and using service discovery via Consul to build pipelines.
 
-## Getting started
-
-### Installation
-
-#### Python
-```bash
-pip install mtap
-```
-
-#### Java
-
-Gradle:
-
-```groovy
-implementation 'edu.umn.nlpie:mtap:1.1.0'
-```
-
-Maven:
-
-```xml
-<dependency>
-  <groupId>edu.umn.nlpie</groupId>
-  <artifactId>mtap</artifactId>
-  <version>1.1.0</version>
-</dependency>
-```
-
-### Instructions
+## Instructions
 
 We make getting started tutorials available on our project website for both [Python](https://nlpie.github.io/mtap/docs/tutorials/python.html) and [Java](https://nlpie.github.io/mtap/docs/tutorials/java.html).
 
-### About Us
+## About Us
 
 MTAP is developed at the University of Minnesota by the [NLP/IE Group in the Institute for Health Informatics](https://healthinformatics.umn.edu/research/nlpie-group).
 
-### Acknowledgements
+## Acknowledgements
 Funding for this work was provided by:
 
 - 1 R01 LM011364-01 NIH-NLM
 - 1 R01 GM102282-01A1 NIH-NIGMS
 - U54 RR026066-01A2 NIH-NCRR
```

### Comparing `mtap-1.1.0/README.md` & `mtap-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <p align="center">
   <a href="https://pypi.org/project/mtap/">
     <img src="https://img.shields.io/pypi/v/mtap" /></a>
-  <a href="https://central.sonatype.com/artifact/edu.umn.nlpie/mtap/1.1.0">
+  <a href="https://mvnrepository.com/artifact/edu.umn.nlpie/mtap">
     <img src="https://img.shields.io/maven-central/v/edu.umn.nlpie/mtap" /></a>
 </p>
 
 # MTAP
 
 [nlpie.github.io/mtap](https://nlpie.github.io/mtap)
 
@@ -32,48 +32,21 @@
 
 By using the microservice pattern, text analysis components can be deployed once and then mixed and matched in different pipelines. Components written in different languages can interoperate without hassle. We also provide a RESTful API gateway that lets you call components using HTTP.
 
 ### Scalability
 
 MTAP is designed to bridge the gap between prototyping new ideas and deploying them into a production environment. It supports calling components locally without using any network infastructure all the way up to deploying services and using service discovery via Consul to build pipelines.
 
-## Getting started
-
-### Installation
-
-#### Python
-```bash
-pip install mtap
-```
-
-#### Java
-
-Gradle:
-
-```groovy
-implementation 'edu.umn.nlpie:mtap:1.1.0'
-```
-
-Maven:
-
-```xml
-<dependency>
-  <groupId>edu.umn.nlpie</groupId>
-  <artifactId>mtap</artifactId>
-  <version>1.1.0</version>
-</dependency>
-```
-
-### Instructions
+## Instructions
 
 We make getting started tutorials available on our project website for both [Python](https://nlpie.github.io/mtap/docs/tutorials/python.html) and [Java](https://nlpie.github.io/mtap/docs/tutorials/java.html).
 
-### About Us
+## About Us
 
 MTAP is developed at the University of Minnesota by the [NLP/IE Group in the Institute for Health Informatics](https://healthinformatics.umn.edu/research/nlpie-group).
 
-### Acknowledgements
+## Acknowledgements
 Funding for this work was provided by:
 
 - 1 R01 LM011364-01 NIH-NLM
 - 1 R01 GM102282-01A1 NIH-NIGMS
 - U54 RR026066-01A2 NIH-NCRR
```

#### html2text {}

```diff
@@ -17,18 +17,15 @@
 components can be deployed once and then mixed and matched in different
 pipelines. Components written in different languages can interoperate without
 hassle. We also provide a RESTful API gateway that lets you call components
 using HTTP. ### Scalability MTAP is designed to bridge the gap between
 prototyping new ideas and deploying them into a production environment. It
 supports calling components locally without using any network infastructure all
 the way up to deploying services and using service discovery via Consul to
-build pipelines. ## Getting started ### Installation #### Python ```bash pip
-install mtap ``` #### Java Gradle: ```groovy implementation 'edu.umn.nlpie:
-mtap:1.1.0' ``` Maven: ```xml  edu.umn.nlpie mtap 1.1.0  ``` ### Instructions
-We make getting started tutorials available on our project website for both
-[Python](https://nlpie.github.io/mtap/docs/tutorials/python.html) and [Java]
-(https://nlpie.github.io/mtap/docs/tutorials/java.html). ### About Us MTAP is
-developed at the University of Minnesota by the [NLP/IE Group in the Institute
-for Health Informatics](https://healthinformatics.umn.edu/research/nlpie-
-group). ### Acknowledgements Funding for this work was provided by: - 1 R01
-LM011364-01 NIH-NLM - 1 R01 GM102282-01A1 NIH-NIGMS - U54 RR026066-01A2 NIH-
-NCRR
+build pipelines. ## Instructions We make getting started tutorials available on
+our project website for both [Python](https://nlpie.github.io/mtap/docs/
+tutorials/python.html) and [Java](https://nlpie.github.io/mtap/docs/tutorials/
+java.html). ## About Us MTAP is developed at the University of Minnesota by the
+[NLP/IE Group in the Institute for Health Informatics](https://
+healthinformatics.umn.edu/research/nlpie-group). ## Acknowledgements Funding
+for this work was provided by: - 1 R01 LM011364-01 NIH-NLM - 1 R01 GM102282-
+01A1 NIH-NIGMS - U54 RR026066-01A2 NIH-NCRR
```

### Comparing `mtap-1.1.0/go/Makefile` & `mtap-1.2.0/go/Makefile`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/go/doc.go` & `mtap-1.2.0/go/doc.go`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,12 @@
  * Unless required by applicable law or agreed to in writing, software
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
-//go:generate protoc -I/usr/local/include -I../proto -Ithird_party/googleapis --go_out=plugins=grpc,paths=source_relative:. ../proto/mtap/api/v1/events.proto
-//go:generate protoc -I/usr/local/include -I../proto -Ithird_party/googleapis --grpc-gateway_out=logtostderr=true:. ../proto/mtap/api/v1/events.proto
-//go:generate protoc -I/usr/local/include -I../proto -Ithird_party/googleapis --swagger_out=logtostderr=true:. ../proto/mtap/api/v1/events.proto
-//go:generate protoc -I/usr/local/include -I../proto -Ithird_party/googleapis --go_out=plugins=grpc,paths=source_relative:. ../proto/mtap/api/v1/processing.proto
-//go:generate protoc -I/usr/local/include -I../proto -Ithird_party/googleapis --grpc-gateway_out=logtostderr=true:. ../proto/mtap/api/v1/processing.proto
-//go:generate protoc -I/usr/local/include -I../proto -Ithird_party/googleapis --swagger_out=logtostderr=true:. ../proto/mtap/api/v1/processing.proto
-//go:generate go run store-swaggers/main.go mtap/api/v1
+//go:generate protoc -I/usr/local/include -I../proto -Ithird_party/googleapis --go_out . --go_opt paths=source_relative --go-grpc_out . --go-grpc_opt paths=source_relative ../proto/mtap/api/v1/events.proto
+//go:generate protoc -I/usr/local/include -I../proto -Ithird_party/googleapis --grpc-gateway_out . --grpc-gateway_opt logtostderr=true --grpc-gateway_opt paths=source_relative ../proto/mtap/api/v1/events.proto
+//go:generate protoc -I/usr/local/include -I../proto -Ithird_party/googleapis --go_out . --go_opt paths=source_relative --go-grpc_out . --go-grpc_opt paths=source_relative ../proto/mtap/api/v1/processing.proto
+//go:generate protoc -I/usr/local/include -I../proto -Ithird_party/googleapis --grpc-gateway_out . --grpc-gateway_opt logtostderr=true --grpc-gateway_opt paths=source_relative ../proto/mtap/api/v1/processing.proto
 package mtap
```

### Comparing `mtap-1.1.0/go/go.mod` & `mtap-1.2.0/go/go.mod`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 module github.com/nlpie/mtap/go
 
 go 1.20
 
 require (
-	github.com/golang/glog v1.1.0
-	github.com/golang/protobuf v1.5.3
-	github.com/gorilla/handlers v1.5.1
+	github.com/golang/glog v1.1.1
 	github.com/gorilla/mux v1.8.0
-	github.com/grpc-ecosystem/grpc-gateway v1.16.0
+	github.com/grpc-ecosystem/grpc-gateway/v2 v2.15.2
 	github.com/hashicorp/consul/api v1.20.0
 	github.com/spf13/cast v1.5.0
 	github.com/spf13/viper v1.15.0
 	golang.org/x/sync v0.1.0
-	google.golang.org/grpc v1.53.0
-	google.golang.org/protobuf v1.29.1
+	google.golang.org/genproto v0.0.0-20230320184635-7606e756e683
+	google.golang.org/grpc v1.54.0
+	google.golang.org/grpc/cmd/protoc-gen-go-grpc v1.3.0
+	google.golang.org/protobuf v1.30.0
 )
 
 require (
 	github.com/armon/go-metrics v0.4.0 // indirect
 	github.com/fatih/color v1.13.0 // indirect
-	github.com/felixge/httpsnoop v1.0.1 // indirect
 	github.com/fsnotify/fsnotify v1.6.0 // indirect
-	github.com/ghodss/yaml v1.0.0 // indirect
+	github.com/golang/protobuf v1.5.3 // indirect
 	github.com/hashicorp/go-cleanhttp v0.5.2 // indirect
 	github.com/hashicorp/go-hclog v1.3.1 // indirect
 	github.com/hashicorp/go-immutable-radix v1.3.1 // indirect
 	github.com/hashicorp/go-msgpack v0.5.5 // indirect
 	github.com/hashicorp/go-multierror v1.1.1 // indirect
 	github.com/hashicorp/go-rootcerts v1.0.2 // indirect
 	github.com/hashicorp/golang-lru v0.5.4 // indirect
@@ -37,15 +36,13 @@
 	github.com/mitchellh/go-homedir v1.1.0 // indirect
 	github.com/mitchellh/mapstructure v1.5.0 // indirect
 	github.com/pelletier/go-toml/v2 v2.0.6 // indirect
 	github.com/spf13/afero v1.9.3 // indirect
 	github.com/spf13/jwalterweatherman v1.1.0 // indirect
 	github.com/spf13/pflag v1.0.5 // indirect
 	github.com/subosito/gotenv v1.4.2 // indirect
-	golang.org/x/net v0.7.0 // indirect
-	golang.org/x/sys v0.5.0 // indirect
-	golang.org/x/text v0.7.0 // indirect
-	google.golang.org/genproto v0.0.0-20230306155012-7f2fa6fef1f4 // indirect
+	golang.org/x/net v0.8.0 // indirect
+	golang.org/x/sys v0.6.0 // indirect
+	golang.org/x/text v0.8.0 // indirect
 	gopkg.in/ini.v1 v1.67.0 // indirect
-	gopkg.in/yaml.v2 v2.4.0 // indirect
 	gopkg.in/yaml.v3 v3.0.1 // indirect
 )
```

### Comparing `mtap-1.1.0/go/go.sum` & `mtap-1.2.0/go/go.sum`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 github.com/BurntSushi/toml v0.3.1/go.mod h1:xHWCNGjB5oqiDr8zfno3MHue2Ht5sIBksp03qcyfWMU=
 github.com/BurntSushi/xgb v0.0.0-20160522181843-27f122750802/go.mod h1:IVnqGOEym/WlBOVXweHU+Q+/VP0lqqI8lqeDx9IjBqo=
 github.com/DataDog/datadog-go v3.2.0+incompatible/go.mod h1:LButxg5PwREeZtORoXG3tL4fMGNddJ+vMq1mwgfaqoQ=
 github.com/alecthomas/template v0.0.0-20160405071501-a0175ee3bccc/go.mod h1:LOuyumcjzFXgccqObfd/Ljyb9UuFJ6TxHnclSeseNhc=
 github.com/alecthomas/template v0.0.0-20190718012654-fb15b899a751/go.mod h1:LOuyumcjzFXgccqObfd/Ljyb9UuFJ6TxHnclSeseNhc=
 github.com/alecthomas/units v0.0.0-20151022065526-2efee857e7cf/go.mod h1:ybxpYRFXyAe+OPACYpWeL0wqObRcbAqCMya13uyzqw0=
 github.com/alecthomas/units v0.0.0-20190717042225-c3de453c63f4/go.mod h1:ybxpYRFXyAe+OPACYpWeL0wqObRcbAqCMya13uyzqw0=
-github.com/antihax/optional v1.0.0/go.mod h1:uupD/76wgC+ih3iEmQUL+0Ugr19nfwCT1kdvxnR2qWY=
 github.com/armon/circbuf v0.0.0-20150827004946-bbbad097214e/go.mod h1:3U/XgcO3hCbHZ8TKRvWD2dDTCfh9M9ya+I9JpbB7O8o=
 github.com/armon/go-metrics v0.0.0-20180917152333-f0300d1749da/go.mod h1:Q73ZrmVTwzkszR9V5SSuryQ31EELlFMUz1kKyl939pY=
 github.com/armon/go-metrics v0.4.0 h1:yCQqn7dwca4ITXb+CbubHmedzaQYHhNhrEXLYUeEe8Q=
 github.com/armon/go-metrics v0.4.0/go.mod h1:E6amYzXo6aW1tqzoZGT755KkbgrJsSdpwZ+3JqfkOG4=
 github.com/armon/go-radix v0.0.0-20180808171621-7fddfc383310/go.mod h1:ufUuZ+zHj4x4TnLV4JWEpy2hxWSpsRywHrMgIH9cCH8=
 github.com/armon/go-radix v1.0.0/go.mod h1:ufUuZ+zHj4x4TnLV4JWEpy2hxWSpsRywHrMgIH9cCH8=
 github.com/beorn7/perks v0.0.0-20180321164747-3a771d992973/go.mod h1:Dwedo/Wpr24TaqPxmxbtue+5NUziq4I4S80YR8gNf3Q=
@@ -74,33 +73,29 @@
 github.com/envoyproxy/go-control-plane v0.9.7/go.mod h1:cwu0lG7PUMfa9snN8LXBig5ynNVH9qI8YYLbd1fK2po=
 github.com/envoyproxy/go-control-plane v0.9.9-0.20201210154907-fd9021fe5dad/go.mod h1:cXg6YxExXjJnVBQHBLXeUAgxn2UodCpnH306RInaBQk=
 github.com/envoyproxy/protoc-gen-validate v0.1.0/go.mod h1:iSmxcyjqTsJpI2R4NaDN7+kN2VEUnK/pcBlmesArF7c=
 github.com/fatih/color v1.7.0/go.mod h1:Zm6kSWBoL9eyXnKyktHP6abPY2pDugNf5KwzbycvMj4=
 github.com/fatih/color v1.9.0/go.mod h1:eQcE1qtQxscV5RaZvpXrrb8Drkc3/DdQ+uUYCNjL+zU=
 github.com/fatih/color v1.13.0 h1:8LOYc1KYPPmyKMuN8QV2DNRWNbLo6LZ0iLs8+mlH53w=
 github.com/fatih/color v1.13.0/go.mod h1:kLAiJbzzSOZDVNGyDpeOxJ47H46qBXwg5ILebYFFOfk=
-github.com/felixge/httpsnoop v1.0.1 h1:lvB5Jl89CsZtGIWuTcDM1E/vkVs49/Ml7JJe07l8SPQ=
-github.com/felixge/httpsnoop v1.0.1/go.mod h1:m8KPJKqk1gH5J9DgRY2ASl2lWCfGKXixSwevea8zH2U=
 github.com/frankban/quicktest v1.14.3 h1:FJKSZTDHjyhriyC81FLQ0LY93eSai0ZyR/ZIkd3ZUKE=
 github.com/fsnotify/fsnotify v1.6.0 h1:n+5WquG0fcWoWp6xPWfHdbskMCQaFnG6PfBrh1Ky4HY=
 github.com/fsnotify/fsnotify v1.6.0/go.mod h1:sl3t1tCWJFWoRz9R8WJCbQihKKwmorjAbSClcnxKAGw=
-github.com/ghodss/yaml v1.0.0 h1:wQHKEahhL6wmXdzwWG11gIVCkOv05bNOh+Rxn0yngAk=
-github.com/ghodss/yaml v1.0.0/go.mod h1:4dBDuWmgqj2HViK6kFavaiC9ZROes6MMH2rRYeMEF04=
 github.com/go-gl/glfw v0.0.0-20190409004039-e6da0acd62b1/go.mod h1:vR7hzQXu2zJy9AVAgeJqvqgH9Q5CA+iKCZ2gyEVpxRU=
 github.com/go-gl/glfw/v3.3/glfw v0.0.0-20191125211704-12ad95a8df72/go.mod h1:tQ2UAYgL5IevRw8kRxooKSPJfGvJ9fJQFa0TUsXzTg8=
 github.com/go-gl/glfw/v3.3/glfw v0.0.0-20200222043503-6f7a984d4dc4/go.mod h1:tQ2UAYgL5IevRw8kRxooKSPJfGvJ9fJQFa0TUsXzTg8=
 github.com/go-kit/kit v0.8.0/go.mod h1:xBxKIO96dXMWWy0MnWVtmwkA9/13aqxPnvrjFYMA2as=
 github.com/go-kit/kit v0.9.0/go.mod h1:xBxKIO96dXMWWy0MnWVtmwkA9/13aqxPnvrjFYMA2as=
 github.com/go-logfmt/logfmt v0.3.0/go.mod h1:Qt1PoO58o5twSAckw1HlFXLmHsOX5/0LbT9GBnD5lWE=
 github.com/go-logfmt/logfmt v0.4.0/go.mod h1:3RMwSq7FuexP4Kalkev3ejPJsZTpXXBr9+V4qmtdjCk=
 github.com/go-stack/stack v1.8.0/go.mod h1:v0f6uXyyMGvRgIKkXu+yp6POWl0qKG85gN/melR3HDY=
 github.com/gogo/protobuf v1.1.1/go.mod h1:r8qH/GZQm5c6nD/R0oafs1akxWv10x8SbQlK7atdtwQ=
 github.com/golang/glog v0.0.0-20160126235308-23def4e6c14b/go.mod h1:SBH7ygxi8pfUlaOkMMuAQtPIUF8ecWP5IEl/CR7VP2Q=
-github.com/golang/glog v1.1.0 h1:/d3pCKDPWNnvIWe0vVUpNP32qc8U3PDVxySP/y360qE=
-github.com/golang/glog v1.1.0/go.mod h1:pfYeQZ3JWZoXTV5sFc986z3HTpwQs9At6P4ImfuP3NQ=
+github.com/golang/glog v1.1.1 h1:jxpi2eWoU84wbX9iIEyAeeoac3FLuifZpY9tcNUD9kw=
+github.com/golang/glog v1.1.1/go.mod h1:zR+okUeTbrL6EL3xHUDxZuEtGv04p5shwip1+mL/rLQ=
 github.com/golang/groupcache v0.0.0-20190702054246-869f871628b6/go.mod h1:cIg4eruTrX1D+g88fzRXU5OdNfaM+9IcxsU14FzY7Hc=
 github.com/golang/groupcache v0.0.0-20191227052852-215e87163ea7/go.mod h1:cIg4eruTrX1D+g88fzRXU5OdNfaM+9IcxsU14FzY7Hc=
 github.com/golang/groupcache v0.0.0-20200121045136-8c9f03a8e57e/go.mod h1:cIg4eruTrX1D+g88fzRXU5OdNfaM+9IcxsU14FzY7Hc=
 github.com/golang/mock v1.1.1/go.mod h1:oTYuIxOrZwtPieC+H1uAHpcLFnEyAGVDL/k47Jfbm0A=
 github.com/golang/mock v1.2.0/go.mod h1:oTYuIxOrZwtPieC+H1uAHpcLFnEyAGVDL/k47Jfbm0A=
 github.com/golang/mock v1.3.1/go.mod h1:sBzyDLLjw3U8JLTeZvSv8jJB+tU5PVekmnlKIyFUx0Y=
 github.com/golang/mock v1.4.0/go.mod h1:UOMv5ysSaYNkG+OFQykRIcU/QvvxJf3p21QfJ2Bt3cw=
@@ -153,20 +148,18 @@
 github.com/google/pprof v0.0.0-20201203190320-1bf35d6f28c2/go.mod h1:kpwsk12EmLew5upagYY7GY0pfYCcupk39gWOCRROcvE=
 github.com/google/pprof v0.0.0-20201218002935-b9804c9f04c2/go.mod h1:kpwsk12EmLew5upagYY7GY0pfYCcupk39gWOCRROcvE=
 github.com/google/renameio v0.1.0/go.mod h1:KWCgfxg9yswjAJkECMjeO8J8rahYeXnNhOm40UhjYkI=
 github.com/google/uuid v1.1.2/go.mod h1:TIyPZe4MgqvfeYDBFedMoGGpEw/LqOeaOT+nhxU+yHo=
 github.com/googleapis/gax-go/v2 v2.0.4/go.mod h1:0Wqv26UfaUD9n4G6kQubkQ+KchISgw+vpHVxEJEs9eg=
 github.com/googleapis/gax-go/v2 v2.0.5/go.mod h1:DWXyrwAJ9X0FpwwEdw+IPEYBICEFu5mhpdKc/us6bOk=
 github.com/googleapis/google-cloud-go-testing v0.0.0-20200911160855-bcd43fbb19e8/go.mod h1:dvDLG8qkwmyD9a/MJJN3XJcT3xFxOKAvTZGvuZmac9g=
-github.com/gorilla/handlers v1.5.1 h1:9lRY6j8DEeeBT10CvO9hGW0gmky0BprnvDI5vfhUHH4=
-github.com/gorilla/handlers v1.5.1/go.mod h1:t8XrUpc4KVXb7HGyJ4/cEnwQiaxrX/hz1Zv/4g96P1Q=
 github.com/gorilla/mux v1.8.0 h1:i40aqfkR1h2SlN9hojwV5ZA91wcXFOvkdNIeFDP5koI=
 github.com/gorilla/mux v1.8.0/go.mod h1:DVbg23sWSpFRCP0SfiEN6jmj59UnW/n46BH5rLB71So=
-github.com/grpc-ecosystem/grpc-gateway v1.16.0 h1:gmcG1KaJ57LophUzW0Hy8NmPhnMZb4M0+kPpLofRdBo=
-github.com/grpc-ecosystem/grpc-gateway v1.16.0/go.mod h1:BDjrQk3hbvj6Nolgz8mAMFbcEtjT1g+wF4CSlocrBnw=
+github.com/grpc-ecosystem/grpc-gateway/v2 v2.15.2 h1:gDLXvp5S9izjldquuoAhDzccbskOL6tDC5jMSyx3zxE=
+github.com/grpc-ecosystem/grpc-gateway/v2 v2.15.2/go.mod h1:7pdNwVWBBHGiCxa9lAszqCJMbfTISJ7oMftp8+UGV08=
 github.com/hashicorp/consul/api v1.20.0 h1:9IHTjNVSZ7MIwjlW3N3a7iGiykCMDpxZu8jsxFJh0yc=
 github.com/hashicorp/consul/api v1.20.0/go.mod h1:nR64eD44KQ59Of/ECwt2vUmIK2DKsDzAwTmwmLl8Wpo=
 github.com/hashicorp/consul/sdk v0.13.1 h1:EygWVWWMczTzXGpO93awkHFzfUka6hLYJ0qhETd+6lY=
 github.com/hashicorp/errwrap v1.0.0 h1:hLrqtEDnRye3+sgx6z4qVLNuviH3MR5aQ0ykNJa/UYA=
 github.com/hashicorp/errwrap v1.0.0/go.mod h1:YH+1FKiLXxHSkmPseP+kNlulaMuP3n2brvKWEqk/Jc4=
 github.com/hashicorp/go-cleanhttp v0.5.0/go.mod h1:JpRdi6/HCYpAwUzNwuwqhbovhLtngrth3wmdIIUrZ80=
 github.com/hashicorp/go-cleanhttp v0.5.2 h1:035FKYIWjmULyFRBKPs8TBQoi0x6d9G4xc9neXJWAZQ=
@@ -274,15 +267,14 @@
 github.com/prometheus/client_model v0.0.0-20190812154241-14fe0d1b01d4/go.mod h1:xMI15A0UPsDsEKsMN9yxemIoYk6Tm2C1GtYGdfGttqA=
 github.com/prometheus/client_model v0.2.0/go.mod h1:xMI15A0UPsDsEKsMN9yxemIoYk6Tm2C1GtYGdfGttqA=
 github.com/prometheus/common v0.4.1/go.mod h1:TNfzLD0ON7rHzMJeJkieUDPYmFC7Snx/y86RQel1bk4=
 github.com/prometheus/common v0.9.1/go.mod h1:yhUN8i9wzaXS3w1O07YhxHEBxD+W35wd8bs7vj7HSQ4=
 github.com/prometheus/procfs v0.0.0-20181005140218-185b4288413d/go.mod h1:c3At6R/oaqEKCNdg8wHV1ftS6bRYblBhIjjI8uT2IGk=
 github.com/prometheus/procfs v0.0.2/go.mod h1:TjEm7ze935MbeOT/UhFTIMYKhuLP4wbCsTZCD3I8kEA=
 github.com/prometheus/procfs v0.0.8/go.mod h1:7Qr8sr6344vo1JqZ6HhLceV9o3AJ1Ff+GxbHq6oeK9A=
-github.com/rogpeppe/fastuuid v1.2.0/go.mod h1:jVj6XXZzXRy/MSR5jhDC/2q6DgLz+nrA6LYCDYWNEvQ=
 github.com/rogpeppe/go-internal v1.3.0/go.mod h1:M8bDsm7K2OlrFYOpmOWEs/qY81heoFRclV5y23lUDJ4=
 github.com/rogpeppe/go-internal v1.6.1 h1:/FiVV8dS/e+YqF2JvO3yXRFbBLTIuSDkuC7aBOAvL+k=
 github.com/ryanuber/columnize v0.0.0-20160712163229-9b3edd62028f/go.mod h1:sm1tb6uqfes/u+d4ooFouqFdy9/2g9QGwK3SQygK0Ts=
 github.com/sean-/seed v0.0.0-20170313163322-e2103e2c3529 h1:nn5Wsu0esKSJiIVhscUtVbo7ada43DJhG55ua/hjS5I=
 github.com/sean-/seed v0.0.0-20170313163322-e2103e2c3529/go.mod h1:DxrIzT+xaE7yg65j358z/aeFdxmN0P9QXhEzd20vsDc=
 github.com/sirupsen/logrus v1.2.0/go.mod h1:LxeOpSwHxABJmUn/MG1IvRgCAasNZTLOkJPxbbu5VWo=
 github.com/sirupsen/logrus v1.4.2/go.mod h1:tLMulIdttU9McNUspp0xgXVQah82FyeX6MwdIuYE2rE=
@@ -397,16 +389,16 @@
 golang.org/x/net v0.0.0-20200822124328-c89045814202/go.mod h1:/O7V0waA8r7cgGh81Ro3o1hOxt32SMVPicZroKQ2sZA=
 golang.org/x/net v0.0.0-20201021035429-f5854403a974/go.mod h1:sp8m0HH+o8qH0wwXwYZr8TS3Oi6o0r6Gce1SSxlDquU=
 golang.org/x/net v0.0.0-20201031054903-ff519b6c9102/go.mod h1:sp8m0HH+o8qH0wwXwYZr8TS3Oi6o0r6Gce1SSxlDquU=
 golang.org/x/net v0.0.0-20201209123823-ac852fbbde11/go.mod h1:m0MpNAwzfU5UDzcl9v0D8zg8gWTRqZa9RBIspLL5mdg=
 golang.org/x/net v0.0.0-20201224014010-6772e930b67b/go.mod h1:m0MpNAwzfU5UDzcl9v0D8zg8gWTRqZa9RBIspLL5mdg=
 golang.org/x/net v0.0.0-20210226172049-e18ecbb05110/go.mod h1:m0MpNAwzfU5UDzcl9v0D8zg8gWTRqZa9RBIspLL5mdg=
 golang.org/x/net v0.0.0-20210410081132-afb366fc7cd1/go.mod h1:9tjilg8BloeKEkVJvy7fQ90B1CfIiPueXVOjqfkSzI8=
-golang.org/x/net v0.7.0 h1:rJrUqqhjsgNp7KqAIc25s9pZnjU7TUcSY7HcVZjdn1g=
-golang.org/x/net v0.7.0/go.mod h1:2Tu9+aMcznHK/AK1HMvgo6xiTLG5rD5rZLDS+rp2Bjs=
+golang.org/x/net v0.8.0 h1:Zrh2ngAOFYneWTAIAPethzeaQLuHwhuBkuV6ZiRnUaQ=
+golang.org/x/net v0.8.0/go.mod h1:QVkue5JL9kW//ek3r6jTKnTFis1tRmNAW2P1shuFdJc=
 golang.org/x/oauth2 v0.0.0-20180821212333-d2e6202438be/go.mod h1:N/0e6XlmueqKjAGxoOufVs8QHGRruUQn6yWY3a++T0U=
 golang.org/x/oauth2 v0.0.0-20190226205417-e64efc72b421/go.mod h1:gOpvHmFTYa4IltrdGE7lF6nIHvwfUNPOp7c8zoXwtLw=
 golang.org/x/oauth2 v0.0.0-20190604053449-0f29369cfe45/go.mod h1:gOpvHmFTYa4IltrdGE7lF6nIHvwfUNPOp7c8zoXwtLw=
 golang.org/x/oauth2 v0.0.0-20191202225959-858c2ad4c8b6/go.mod h1:gOpvHmFTYa4IltrdGE7lF6nIHvwfUNPOp7c8zoXwtLw=
 golang.org/x/oauth2 v0.0.0-20200107190931-bf48bf16ab8d/go.mod h1:gOpvHmFTYa4IltrdGE7lF6nIHvwfUNPOp7c8zoXwtLw=
 golang.org/x/oauth2 v0.0.0-20200902213428-5d25da1a8d43/go.mod h1:KelEdhl1UZF7XfJ4dDtk6s++YSgaE7mD/BuKKDLBl4A=
 golang.org/x/oauth2 v0.0.0-20201109201403-9fd604954f58/go.mod h1:KelEdhl1UZF7XfJ4dDtk6s++YSgaE7mD/BuKKDLBl4A=
@@ -472,26 +464,26 @@
 golang.org/x/sys v0.0.0-20210615035016-665e8c7367d1/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.0.0-20210630005230-0f9fa26af87c/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.0.0-20210927094055-39ccf1dd6fa6/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.0.0-20220503163025-988cb79eb6c6/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.0.0-20220728004956-3c1f35247d10/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.0.0-20220811171246-fbc7d0a398ab/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.0.0-20220908164124-27713097b956/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
-golang.org/x/sys v0.5.0 h1:MUK/U/4lj1t1oPg0HfuXDN/Z1wv31ZJ/YcPiGccS4DU=
-golang.org/x/sys v0.5.0/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
+golang.org/x/sys v0.6.0 h1:MVltZSvRTcU2ljQOhs94SXPftV6DCNnZViHeQps87pQ=
+golang.org/x/sys v0.6.0/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/term v0.0.0-20201126162022-7de9c90e9dd1/go.mod h1:bj7SfCRtBDWHUb9snDiAeCFNEtKQo2Wmx5Cou7ajbmo=
 golang.org/x/text v0.0.0-20170915032832-14c0d48ead0c/go.mod h1:NqM8EUOU14njkJ3fqMW+pc6Ldnwhi/IjpwHt7yyuwOQ=
 golang.org/x/text v0.3.0/go.mod h1:NqM8EUOU14njkJ3fqMW+pc6Ldnwhi/IjpwHt7yyuwOQ=
 golang.org/x/text v0.3.1-0.20180807135948-17ff2d5776d2/go.mod h1:NqM8EUOU14njkJ3fqMW+pc6Ldnwhi/IjpwHt7yyuwOQ=
 golang.org/x/text v0.3.2/go.mod h1:bEr9sfX3Q8Zfm5fL9x+3itogRgK3+ptLWKqgva+5dAk=
 golang.org/x/text v0.3.3/go.mod h1:5Zoc/QRtKVWzQhOtBMvqHzDpF6irO9z98xDceosuGiQ=
 golang.org/x/text v0.3.4/go.mod h1:5Zoc/QRtKVWzQhOtBMvqHzDpF6irO9z98xDceosuGiQ=
 golang.org/x/text v0.3.6/go.mod h1:5Zoc/QRtKVWzQhOtBMvqHzDpF6irO9z98xDceosuGiQ=
-golang.org/x/text v0.7.0 h1:4BRB4x83lYWy72KwLD/qYDuTu7q9PjSagHvijDw7cLo=
-golang.org/x/text v0.7.0/go.mod h1:mrYo+phRRbMaCq/xk9113O4dZlRixOauAjOtrjsXDZ8=
+golang.org/x/text v0.8.0 h1:57P1ETyNKtuIjB4SRd15iJxuhj8Gc416Y78H3qgMh68=
+golang.org/x/text v0.8.0/go.mod h1:e1OnstbJyHTd6l/uOt8jFFHp6TRDWZR/bV3emEE/zU8=
 golang.org/x/time v0.0.0-20181108054448-85acf8d2951c/go.mod h1:tRJNPiyCQ0inRvYxbN9jk5I+vvW/OXSQhTDSoE431IQ=
 golang.org/x/time v0.0.0-20190308202827-9d24e82272b4/go.mod h1:tRJNPiyCQ0inRvYxbN9jk5I+vvW/OXSQhTDSoE431IQ=
 golang.org/x/time v0.0.0-20191024005414-555d28b269f0/go.mod h1:tRJNPiyCQ0inRvYxbN9jk5I+vvW/OXSQhTDSoE431IQ=
 golang.org/x/tools v0.0.0-20180917221912-90fa682c2a6e/go.mod h1:n7NCudcB/nEzxVGmLbDWY5pfWTLqBcC2KZ6jyYvM4mQ=
 golang.org/x/tools v0.0.0-20190114222345-bf090417da8b/go.mod h1:n7NCudcB/nEzxVGmLbDWY5pfWTLqBcC2KZ6jyYvM4mQ=
 golang.org/x/tools v0.0.0-20190226205152-f727befe758c/go.mod h1:9Yl7xja0Znq3iFh3HoIrodX9oNMXvdceNzlUR8zjMvY=
 golang.org/x/tools v0.0.0-20190311212946-11955173bddd/go.mod h1:LCzVGOaR6xXOjkQ3onu1FJEFr0SW1gC7cKk1uF8kGRs=
@@ -588,78 +580,75 @@
 google.golang.org/genproto v0.0.0-20200224152610-e50cd9704f63/go.mod h1:55QSHmfGQM9UVYDPBsyGGes0y52j32PQ3BqQfXhyH3c=
 google.golang.org/genproto v0.0.0-20200228133532-8c2c7df3a383/go.mod h1:55QSHmfGQM9UVYDPBsyGGes0y52j32PQ3BqQfXhyH3c=
 google.golang.org/genproto v0.0.0-20200305110556-506484158171/go.mod h1:55QSHmfGQM9UVYDPBsyGGes0y52j32PQ3BqQfXhyH3c=
 google.golang.org/genproto v0.0.0-20200312145019-da6875a35672/go.mod h1:55QSHmfGQM9UVYDPBsyGGes0y52j32PQ3BqQfXhyH3c=
 google.golang.org/genproto v0.0.0-20200331122359-1ee6d9798940/go.mod h1:55QSHmfGQM9UVYDPBsyGGes0y52j32PQ3BqQfXhyH3c=
 google.golang.org/genproto v0.0.0-20200430143042-b979b6f78d84/go.mod h1:55QSHmfGQM9UVYDPBsyGGes0y52j32PQ3BqQfXhyH3c=
 google.golang.org/genproto v0.0.0-20200511104702-f5ebc3bea380/go.mod h1:55QSHmfGQM9UVYDPBsyGGes0y52j32PQ3BqQfXhyH3c=
-google.golang.org/genproto v0.0.0-20200513103714-09dca8ec2884/go.mod h1:55QSHmfGQM9UVYDPBsyGGes0y52j32PQ3BqQfXhyH3c=
 google.golang.org/genproto v0.0.0-20200515170657-fc4c6c6a6587/go.mod h1:YsZOwe1myG/8QRHRsmBRE1LrgQY60beZKjly0O1fX9U=
 google.golang.org/genproto v0.0.0-20200526211855-cb27e3aa2013/go.mod h1:NbSheEEYHJ7i3ixzK3sjbqSGDJWnxyFXZblF3eUsNvo=
 google.golang.org/genproto v0.0.0-20200618031413-b414f8b61790/go.mod h1:jDfRM7FcilCzHH/e9qn6dsT145K34l5v+OpcnNgKAAA=
 google.golang.org/genproto v0.0.0-20200729003335-053ba62fc06f/go.mod h1:FWY/as6DDZQgahTzZj3fqbO1CbirC29ZNUFHwi0/+no=
 google.golang.org/genproto v0.0.0-20200804131852-c06518451d9c/go.mod h1:FWY/as6DDZQgahTzZj3fqbO1CbirC29ZNUFHwi0/+no=
 google.golang.org/genproto v0.0.0-20200825200019-8632dd797987/go.mod h1:FWY/as6DDZQgahTzZj3fqbO1CbirC29ZNUFHwi0/+no=
 google.golang.org/genproto v0.0.0-20200904004341-0bd0a958aa1d/go.mod h1:FWY/as6DDZQgahTzZj3fqbO1CbirC29ZNUFHwi0/+no=
 google.golang.org/genproto v0.0.0-20201109203340-2640f1f9cdfb/go.mod h1:FWY/as6DDZQgahTzZj3fqbO1CbirC29ZNUFHwi0/+no=
 google.golang.org/genproto v0.0.0-20201201144952-b05cb90ed32e/go.mod h1:FWY/as6DDZQgahTzZj3fqbO1CbirC29ZNUFHwi0/+no=
 google.golang.org/genproto v0.0.0-20201210142538-e3217bee35cc/go.mod h1:FWY/as6DDZQgahTzZj3fqbO1CbirC29ZNUFHwi0/+no=
 google.golang.org/genproto v0.0.0-20201214200347-8c77b98c765d/go.mod h1:FWY/as6DDZQgahTzZj3fqbO1CbirC29ZNUFHwi0/+no=
 google.golang.org/genproto v0.0.0-20210108203827-ffc7fda8c3d7/go.mod h1:FWY/as6DDZQgahTzZj3fqbO1CbirC29ZNUFHwi0/+no=
 google.golang.org/genproto v0.0.0-20210226172003-ab064af71705/go.mod h1:FWY/as6DDZQgahTzZj3fqbO1CbirC29ZNUFHwi0/+no=
-google.golang.org/genproto v0.0.0-20230306155012-7f2fa6fef1f4 h1:DdoeryqhaXp1LtT/emMP1BRJPHHKFi5akj/nbx/zNTA=
-google.golang.org/genproto v0.0.0-20230306155012-7f2fa6fef1f4/go.mod h1:NWraEVixdDnqcqQ30jipen1STv2r/n24Wb7twVTGR4s=
+google.golang.org/genproto v0.0.0-20230320184635-7606e756e683 h1:khxVcsk/FhnzxMKOyD+TDGwjbEOpcPuIpmafPGFmhMA=
+google.golang.org/genproto v0.0.0-20230320184635-7606e756e683/go.mod h1:NWraEVixdDnqcqQ30jipen1STv2r/n24Wb7twVTGR4s=
 google.golang.org/grpc v1.19.0/go.mod h1:mqu4LbDTu4XGKhr4mRzUsmM4RtVoemTSY81AxZiDr8c=
 google.golang.org/grpc v1.20.1/go.mod h1:10oTOabMzJvdu6/UiuZezV6QK5dSlG84ov/aaiqXj38=
 google.golang.org/grpc v1.21.1/go.mod h1:oYelfM1adQP15Ek0mdvEgi9Df8B9CZIaU1084ijfRaM=
 google.golang.org/grpc v1.23.0/go.mod h1:Y5yQAOtifL1yxbo5wqy6BxZv8vAUGQwXBOALyacEbxg=
 google.golang.org/grpc v1.25.1/go.mod h1:c3i+UQWmh7LiEpx4sFZnkU36qjEYZ0imhYfXVyQciAY=
 google.golang.org/grpc v1.26.0/go.mod h1:qbnxyOmOxrQa7FizSgH+ReBfzJrCY1pSN7KXBS8abTk=
 google.golang.org/grpc v1.27.0/go.mod h1:qbnxyOmOxrQa7FizSgH+ReBfzJrCY1pSN7KXBS8abTk=
 google.golang.org/grpc v1.27.1/go.mod h1:qbnxyOmOxrQa7FizSgH+ReBfzJrCY1pSN7KXBS8abTk=
 google.golang.org/grpc v1.28.0/go.mod h1:rpkK4SK4GF4Ach/+MFLZUBavHOvF2JJB5uozKKal+60=
 google.golang.org/grpc v1.29.1/go.mod h1:itym6AZVZYACWQqET3MqgPpjcuV5QH3BxFS3IjizoKk=
 google.golang.org/grpc v1.30.0/go.mod h1:N36X2cJ7JwdamYAgDz+s+rVMFjt3numwzf/HckM8pak=
 google.golang.org/grpc v1.31.0/go.mod h1:N36X2cJ7JwdamYAgDz+s+rVMFjt3numwzf/HckM8pak=
 google.golang.org/grpc v1.31.1/go.mod h1:N36X2cJ7JwdamYAgDz+s+rVMFjt3numwzf/HckM8pak=
-google.golang.org/grpc v1.33.1/go.mod h1:fr5YgcSWrqhRRxogOsw7RzIpsmvOZ6IcH4kBYTpR3n0=
 google.golang.org/grpc v1.33.2/go.mod h1:JMHMWHQWaTccqQQlmk3MJZS+GWXOdAesneDmEnv2fbc=
 google.golang.org/grpc v1.34.0/go.mod h1:WotjhfgOW/POjDeRt8vscBtXq+2VjORFy659qA51WJ8=
 google.golang.org/grpc v1.35.0/go.mod h1:qjiiYl8FncCW8feJPdyg3v6XW24KsRHe+dy9BAGRRjU=
-google.golang.org/grpc v1.53.0 h1:LAv2ds7cmFV/XTS3XG1NneeENYrXGmorPxsBbptIjNc=
-google.golang.org/grpc v1.53.0/go.mod h1:OnIrk0ipVdj4N5d9IUoFUx72/VlD7+jUsHwZgwSMQpw=
+google.golang.org/grpc v1.54.0 h1:EhTqbhiYeixwWQtAEZAxmV9MGqcjEU2mFx52xCzNyag=
+google.golang.org/grpc v1.54.0/go.mod h1:PUSEXI6iWghWaB6lXM4knEgpJNu2qUcKfDtNci3EC2g=
+google.golang.org/grpc/cmd/protoc-gen-go-grpc v1.3.0 h1:rNBFJjBCOgVr9pWD7rs/knKL4FRTKgpZmsRfV214zcA=
+google.golang.org/grpc/cmd/protoc-gen-go-grpc v1.3.0/go.mod h1:Dk1tviKTvMCz5tvh7t+fh94dhmQVHuCt2OzJB3CTW9Y=
 google.golang.org/protobuf v0.0.0-20200109180630-ec00e32a8dfd/go.mod h1:DFci5gLYBciE7Vtevhsrf46CRTquxDuWsQurQQe4oz8=
 google.golang.org/protobuf v0.0.0-20200221191635-4d8936d0db64/go.mod h1:kwYJMbMJ01Woi6D6+Kah6886xMZcty6N08ah7+eCXa0=
 google.golang.org/protobuf v0.0.0-20200228230310-ab0ca4ff8a60/go.mod h1:cfTl7dwQJ+fmap5saPgwCLgHXTUD7jkjRqWcaiX5VyM=
 google.golang.org/protobuf v1.20.1-0.20200309200217-e05f789c0967/go.mod h1:A+miEFZTKqfCUM6K7xSMQL9OKL/b6hQv+e19PK+JZNE=
 google.golang.org/protobuf v1.21.0/go.mod h1:47Nbq4nVaFHyn7ilMalzfO3qCViNmqZ2kzikPIcrTAo=
 google.golang.org/protobuf v1.22.0/go.mod h1:EGpADcykh3NcUnDUJcl1+ZksZNG86OlYog2l/sGQquU=
 google.golang.org/protobuf v1.23.0/go.mod h1:EGpADcykh3NcUnDUJcl1+ZksZNG86OlYog2l/sGQquU=
 google.golang.org/protobuf v1.23.1-0.20200526195155-81db48ad09cc/go.mod h1:EGpADcykh3NcUnDUJcl1+ZksZNG86OlYog2l/sGQquU=
 google.golang.org/protobuf v1.24.0/go.mod h1:r/3tXBNzIEhYS9I1OUVjXDlt8tc493IdKGjtUeSXeh4=
 google.golang.org/protobuf v1.25.0/go.mod h1:9JNX74DMeImyA3h4bdi1ymwjUzf21/xIlbajtzgsN7c=
 google.golang.org/protobuf v1.26.0-rc.1/go.mod h1:jlhhOSvTdKEhbULTjvd4ARK9grFBp09yW+WbY/TyQbw=
 google.golang.org/protobuf v1.26.0/go.mod h1:9q0QmTI4eRPtz6boOQmLYwt+qCgq0jsYwAQnmE0givc=
-google.golang.org/protobuf v1.29.1 h1:7QBf+IK2gx70Ap/hDsOmam3GE0v9HicjfEdAxE62UoM=
-google.golang.org/protobuf v1.29.1/go.mod h1:HV8QOd/L58Z+nl8r43ehVNZIU/HEI6OcFqwMG9pJV4I=
+google.golang.org/protobuf v1.30.0 h1:kPPoIgf3TsEvrm0PFe15JQ+570QVxYzEvvHqChK+cng=
+google.golang.org/protobuf v1.30.0/go.mod h1:HV8QOd/L58Z+nl8r43ehVNZIU/HEI6OcFqwMG9pJV4I=
 gopkg.in/alecthomas/kingpin.v2 v2.2.6/go.mod h1:FMv+mEhP44yOT+4EoQTLFTRgOQ1FBLkstjWtayDeSgw=
 gopkg.in/check.v1 v0.0.0-20161208181325-20d25e280405/go.mod h1:Co6ibVJAznAaIkqp8huTwlJQCZ016jof/cbN4VW5Yz0=
 gopkg.in/check.v1 v1.0.0-20180628173108-788fd7840127/go.mod h1:Co6ibVJAznAaIkqp8huTwlJQCZ016jof/cbN4VW5Yz0=
 gopkg.in/check.v1 v1.0.0-20190902080502-41f04d3bba15 h1:YR8cESwS4TdDjEe65xsg0ogRM/Nc3DYOhEAlW+xobZo=
 gopkg.in/check.v1 v1.0.0-20190902080502-41f04d3bba15/go.mod h1:Co6ibVJAznAaIkqp8huTwlJQCZ016jof/cbN4VW5Yz0=
 gopkg.in/errgo.v2 v2.1.0/go.mod h1:hNsd1EY+bozCKY1Ytp96fpM3vjJbqLJn88ws8XvfDNI=
 gopkg.in/ini.v1 v1.67.0 h1:Dgnx+6+nfE+IfzjUEISNeydPJh9AXNNsWbGP9KzCsOA=
 gopkg.in/ini.v1 v1.67.0/go.mod h1:pNLf8WUiyNEtQjuu5G5vTm06TEv9tsIgeAvK8hOrP4k=
 gopkg.in/yaml.v2 v2.2.1/go.mod h1:hI93XBmqTisBFMUTm0b8Fm+jr3Dg1NNxqwp+5A1VGuI=
 gopkg.in/yaml.v2 v2.2.2/go.mod h1:hI93XBmqTisBFMUTm0b8Fm+jr3Dg1NNxqwp+5A1VGuI=
-gopkg.in/yaml.v2 v2.2.3/go.mod h1:hI93XBmqTisBFMUTm0b8Fm+jr3Dg1NNxqwp+5A1VGuI=
 gopkg.in/yaml.v2 v2.2.4/go.mod h1:hI93XBmqTisBFMUTm0b8Fm+jr3Dg1NNxqwp+5A1VGuI=
 gopkg.in/yaml.v2 v2.2.5/go.mod h1:hI93XBmqTisBFMUTm0b8Fm+jr3Dg1NNxqwp+5A1VGuI=
-gopkg.in/yaml.v2 v2.4.0 h1:D8xgwECY7CYvx+Y2n4sBz93Jn9JRvxdiyyo8CTfuKaY=
-gopkg.in/yaml.v2 v2.4.0/go.mod h1:RDklbk79AGWmwhnvt/jBztapEOGDOx6ZbXqjP6csGnQ=
 gopkg.in/yaml.v3 v3.0.0-20200313102051-9f266ea9e77c/go.mod h1:K4uyk7z7BCEPqu6E+C64Yfv1cQ7kz7rIZviUmN+EgEM=
 gopkg.in/yaml.v3 v3.0.1 h1:fxVm/GzAzEWqLHuvctI91KS9hhNmmWOoWu0XTYJS7CA=
 gopkg.in/yaml.v3 v3.0.1/go.mod h1:K4uyk7z7BCEPqu6E+C64Yfv1cQ7kz7rIZviUmN+EgEM=
 honnef.co/go/tools v0.0.0-20190102054323-c2f93a96b099/go.mod h1:rf3lG4BRIbNafJWhAfAdb/ePZxsR/4RtNHQocxwk9r4=
 honnef.co/go/tools v0.0.0-20190106161140-3f1c8253044a/go.mod h1:rf3lG4BRIbNafJWhAfAdb/ePZxsR/4RtNHQocxwk9r4=
 honnef.co/go/tools v0.0.0-20190418001031-e561f6794a2a/go.mod h1:rf3lG4BRIbNafJWhAfAdb/ePZxsR/4RtNHQocxwk9r4=
 honnef.co/go/tools v0.0.0-20190523083050-ea95bdfd59fc/go.mod h1:rf3lG4BRIbNafJWhAfAdb/ePZxsR/4RtNHQocxwk9r4=
```

### Comparing `mtap-1.1.0/go/mtap/api/v1/events.pb.gw.go` & `mtap-1.2.0/go/mtap/api/v1/events.pb.gw.go`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 // Code generated by protoc-gen-grpc-gateway. DO NOT EDIT.
 // source: mtap/api/v1/events.proto
 
 /*
-Package mtap_api_v1 is a reverse proxy.
+Package v1 is a reverse proxy.
 
 It translates gRPC into RESTful JSON APIs.
 */
-package mtap_api_v1
+package v1
 
 import (
 	"context"
 	"io"
 	"net/http"
 
-	"github.com/golang/protobuf/descriptor"
-	"github.com/golang/protobuf/proto"
-	"github.com/grpc-ecosystem/grpc-gateway/runtime"
-	"github.com/grpc-ecosystem/grpc-gateway/utilities"
+	"github.com/grpc-ecosystem/grpc-gateway/v2/runtime"
+	"github.com/grpc-ecosystem/grpc-gateway/v2/utilities"
 	"google.golang.org/grpc"
 	"google.golang.org/grpc/codes"
 	"google.golang.org/grpc/grpclog"
+	"google.golang.org/grpc/metadata"
 	"google.golang.org/grpc/status"
+	"google.golang.org/protobuf/proto"
 )
 
 // Suppress "imported and not used" errors
 var _ codes.Code
 var _ io.Reader
 var _ status.Status
 var _ = runtime.String
 var _ = utilities.NewDoubleArray
-var _ = descriptor.ForMessage
+var _ = metadata.Join
 
 func request_Events_GetEventsInstanceId_0(ctx context.Context, marshaler runtime.Marshaler, client EventsClient, req *http.Request, pathParams map[string]string) (proto.Message, runtime.ServerMetadata, error) {
 	var protoReq GetEventsInstanceIdRequest
 	var metadata runtime.ServerMetadata
 
 	msg, err := client.GetEventsInstanceId(ctx, &protoReq, grpc.Header(&metadata.HeaderMD), grpc.Trailer(&metadata.TrailerMD))
 	return msg, metadata, err
@@ -70,15 +70,14 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	msg, err := client.OpenEvent(ctx, &protoReq, grpc.Header(&metadata.HeaderMD), grpc.Trailer(&metadata.TrailerMD))
 	return msg, metadata, err
 
@@ -105,26 +104,25 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	msg, err := server.OpenEvent(ctx, &protoReq)
 	return msg, metadata, err
 
 }
 
 var (
-	filter_Events_CloseEvent_0 = &utilities.DoubleArray{Encoding: map[string]int{"event_id": 0}, Base: []int{1, 1, 0}, Check: []int{0, 1, 2}}
+	filter_Events_CloseEvent_0 = &utilities.DoubleArray{Encoding: map[string]int{"event_id": 0, "eventId": 1}, Base: []int{1, 1, 2, 0, 0}, Check: []int{0, 1, 1, 2, 3}}
 )
 
 func request_Events_CloseEvent_0(ctx context.Context, marshaler runtime.Marshaler, client EventsClient, req *http.Request, pathParams map[string]string) (proto.Message, runtime.ServerMetadata, error) {
 	var protoReq CloseEventRequest
 	var metadata runtime.ServerMetadata
 
 	var (
@@ -136,15 +134,14 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	if err := req.ParseForm(); err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "%v", err)
 	}
@@ -170,20 +167,22 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
-	if err := runtime.PopulateQueryParameters(&protoReq, req.URL.Query(), filter_Events_CloseEvent_0); err != nil {
+	if err := req.ParseForm(); err != nil {
+		return nil, metadata, status.Errorf(codes.InvalidArgument, "%v", err)
+	}
+	if err := runtime.PopulateQueryParameters(&protoReq, req.Form, filter_Events_CloseEvent_0); err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "%v", err)
 	}
 
 	msg, err := server.CloseEvent(ctx, &protoReq)
 	return msg, metadata, err
 
 }
@@ -201,15 +200,14 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	msg, err := client.GetAllMetadata(ctx, &protoReq, grpc.Header(&metadata.HeaderMD), grpc.Trailer(&metadata.TrailerMD))
 	return msg, metadata, err
 
@@ -228,15 +226,14 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	msg, err := server.GetAllMetadata(ctx, &protoReq)
 	return msg, metadata, err
 
@@ -263,26 +260,24 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	val, ok = pathParams["key"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "key")
 	}
 
 	protoReq.Key, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "key", err)
 	}
 
 	msg, err := client.AddMetadata(ctx, &protoReq, grpc.Header(&metadata.HeaderMD), grpc.Trailer(&metadata.TrailerMD))
 	return msg, metadata, err
 
@@ -309,26 +304,24 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	val, ok = pathParams["key"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "key")
 	}
 
 	protoReq.Key, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "key", err)
 	}
 
 	msg, err := server.AddMetadata(ctx, &protoReq)
 	return msg, metadata, err
 
@@ -355,26 +348,24 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	val, ok = pathParams["document_name"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "document_name")
 	}
 
 	protoReq.DocumentName, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "document_name", err)
 	}
 
 	msg, err := client.AddDocument(ctx, &protoReq, grpc.Header(&metadata.HeaderMD), grpc.Trailer(&metadata.TrailerMD))
 	return msg, metadata, err
 
@@ -401,26 +392,24 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	val, ok = pathParams["document_name"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "document_name")
 	}
 
 	protoReq.DocumentName, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "document_name", err)
 	}
 
 	msg, err := server.AddDocument(ctx, &protoReq)
 	return msg, metadata, err
 
@@ -439,15 +428,14 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	msg, err := client.GetAllDocumentNames(ctx, &protoReq, grpc.Header(&metadata.HeaderMD), grpc.Trailer(&metadata.TrailerMD))
 	return msg, metadata, err
 
@@ -466,15 +454,14 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	msg, err := server.GetAllDocumentNames(ctx, &protoReq)
 	return msg, metadata, err
 
@@ -493,26 +480,24 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	val, ok = pathParams["document_name"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "document_name")
 	}
 
 	protoReq.DocumentName, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "document_name", err)
 	}
 
 	msg, err := client.GetDocumentText(ctx, &protoReq, grpc.Header(&metadata.HeaderMD), grpc.Trailer(&metadata.TrailerMD))
 	return msg, metadata, err
 
@@ -531,26 +516,24 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	val, ok = pathParams["document_name"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "document_name")
 	}
 
 	protoReq.DocumentName, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "document_name", err)
 	}
 
 	msg, err := server.GetDocumentText(ctx, &protoReq)
 	return msg, metadata, err
 
@@ -569,26 +552,24 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	val, ok = pathParams["document_name"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "document_name")
 	}
 
 	protoReq.DocumentName, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "document_name", err)
 	}
 
 	msg, err := client.GetLabelIndicesInfo(ctx, &protoReq, grpc.Header(&metadata.HeaderMD), grpc.Trailer(&metadata.TrailerMD))
 	return msg, metadata, err
 
@@ -607,26 +588,24 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	val, ok = pathParams["document_name"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "document_name")
 	}
 
 	protoReq.DocumentName, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "document_name", err)
 	}
 
 	msg, err := server.GetLabelIndicesInfo(ctx, &protoReq)
 	return msg, metadata, err
 
@@ -653,37 +632,34 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	val, ok = pathParams["document_name"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "document_name")
 	}
 
 	protoReq.DocumentName, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "document_name", err)
 	}
 
 	val, ok = pathParams["index_name"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "index_name")
 	}
 
 	protoReq.IndexName, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "index_name", err)
 	}
 
 	msg, err := client.AddLabels(ctx, &protoReq, grpc.Header(&metadata.HeaderMD), grpc.Trailer(&metadata.TrailerMD))
 	return msg, metadata, err
 
@@ -710,37 +686,34 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	val, ok = pathParams["document_name"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "document_name")
 	}
 
 	protoReq.DocumentName, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "document_name", err)
 	}
 
 	val, ok = pathParams["index_name"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "index_name")
 	}
 
 	protoReq.IndexName, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "index_name", err)
 	}
 
 	msg, err := server.AddLabels(ctx, &protoReq)
 	return msg, metadata, err
 
@@ -759,37 +732,34 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	val, ok = pathParams["document_name"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "document_name")
 	}
 
 	protoReq.DocumentName, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "document_name", err)
 	}
 
 	val, ok = pathParams["index_name"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "index_name")
 	}
 
 	protoReq.IndexName, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "index_name", err)
 	}
 
 	msg, err := client.GetLabels(ctx, &protoReq, grpc.Header(&metadata.HeaderMD), grpc.Trailer(&metadata.TrailerMD))
 	return msg, metadata, err
 
@@ -808,37 +778,34 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	val, ok = pathParams["document_name"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "document_name")
 	}
 
 	protoReq.DocumentName, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "document_name", err)
 	}
 
 	val, ok = pathParams["index_name"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "index_name")
 	}
 
 	protoReq.IndexName, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "index_name", err)
 	}
 
 	msg, err := server.GetLabels(ctx, &protoReq)
 	return msg, metadata, err
 
@@ -857,15 +824,14 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	msg, err := client.GetAllBinaryDataNames(ctx, &protoReq, grpc.Header(&metadata.HeaderMD), grpc.Trailer(&metadata.TrailerMD))
 	return msg, metadata, err
 
@@ -884,15 +850,14 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	msg, err := server.GetAllBinaryDataNames(ctx, &protoReq)
 	return msg, metadata, err
 
@@ -919,26 +884,24 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	val, ok = pathParams["binary_data_name"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "binary_data_name")
 	}
 
 	protoReq.BinaryDataName, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "binary_data_name", err)
 	}
 
 	msg, err := client.AddBinaryData(ctx, &protoReq, grpc.Header(&metadata.HeaderMD), grpc.Trailer(&metadata.TrailerMD))
 	return msg, metadata, err
 
@@ -965,26 +928,24 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	val, ok = pathParams["binary_data_name"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "binary_data_name")
 	}
 
 	protoReq.BinaryDataName, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "binary_data_name", err)
 	}
 
 	msg, err := server.AddBinaryData(ctx, &protoReq)
 	return msg, metadata, err
 
@@ -1003,26 +964,24 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	val, ok = pathParams["binary_data_name"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "binary_data_name")
 	}
 
 	protoReq.BinaryDataName, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "binary_data_name", err)
 	}
 
 	msg, err := client.GetBinaryData(ctx, &protoReq, grpc.Header(&metadata.HeaderMD), grpc.Trailer(&metadata.TrailerMD))
 	return msg, metadata, err
 
@@ -1041,327 +1000,396 @@
 
 	val, ok = pathParams["event_id"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "event_id")
 	}
 
 	protoReq.EventId, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "event_id", err)
 	}
 
 	val, ok = pathParams["binary_data_name"]
 	if !ok {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "missing parameter %s", "binary_data_name")
 	}
 
 	protoReq.BinaryDataName, err = runtime.String(val)
-
 	if err != nil {
 		return nil, metadata, status.Errorf(codes.InvalidArgument, "type mismatch, parameter: %s, error: %v", "binary_data_name", err)
 	}
 
 	msg, err := server.GetBinaryData(ctx, &protoReq)
 	return msg, metadata, err
 
 }
 
 // RegisterEventsHandlerServer registers the http handlers for service Events to "mux".
 // UnaryRPC     :call EventsServer directly.
 // StreamingRPC :currently unsupported pending https://github.com/grpc/grpc-go/issues/906.
+// Note that using this registration option will cause many gRPC library features to stop working. Consider using RegisterEventsHandlerFromEndpoint instead.
 func RegisterEventsHandlerServer(ctx context.Context, mux *runtime.ServeMux, server EventsServer) error {
 
 	mux.Handle("GET", pattern_Events_GetEventsInstanceId_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
+		var stream runtime.ServerTransportStream
+		ctx = grpc.NewContextWithServerTransportStream(ctx, &stream)
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateIncomingContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateIncomingContext(ctx, mux, req, "/mtap.api.v1.Events/GetEventsInstanceId", runtime.WithHTTPPathPattern("/v1/events/instance_id"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := local_request_Events_GetEventsInstanceId_0(rctx, inboundMarshaler, server, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := local_request_Events_GetEventsInstanceId_0(annotatedContext, inboundMarshaler, server, req, pathParams)
+		md.HeaderMD, md.TrailerMD = metadata.Join(md.HeaderMD, stream.Header()), metadata.Join(md.TrailerMD, stream.Trailer())
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_GetEventsInstanceId_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_GetEventsInstanceId_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("POST", pattern_Events_OpenEvent_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
+		var stream runtime.ServerTransportStream
+		ctx = grpc.NewContextWithServerTransportStream(ctx, &stream)
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateIncomingContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateIncomingContext(ctx, mux, req, "/mtap.api.v1.Events/OpenEvent", runtime.WithHTTPPathPattern("/v1/events/{event_id}"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := local_request_Events_OpenEvent_0(rctx, inboundMarshaler, server, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := local_request_Events_OpenEvent_0(annotatedContext, inboundMarshaler, server, req, pathParams)
+		md.HeaderMD, md.TrailerMD = metadata.Join(md.HeaderMD, stream.Header()), metadata.Join(md.TrailerMD, stream.Trailer())
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_OpenEvent_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_OpenEvent_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("DELETE", pattern_Events_CloseEvent_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
+		var stream runtime.ServerTransportStream
+		ctx = grpc.NewContextWithServerTransportStream(ctx, &stream)
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateIncomingContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateIncomingContext(ctx, mux, req, "/mtap.api.v1.Events/CloseEvent", runtime.WithHTTPPathPattern("/v1/events/{event_id}"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := local_request_Events_CloseEvent_0(rctx, inboundMarshaler, server, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := local_request_Events_CloseEvent_0(annotatedContext, inboundMarshaler, server, req, pathParams)
+		md.HeaderMD, md.TrailerMD = metadata.Join(md.HeaderMD, stream.Header()), metadata.Join(md.TrailerMD, stream.Trailer())
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_CloseEvent_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_CloseEvent_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("GET", pattern_Events_GetAllMetadata_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
+		var stream runtime.ServerTransportStream
+		ctx = grpc.NewContextWithServerTransportStream(ctx, &stream)
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateIncomingContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateIncomingContext(ctx, mux, req, "/mtap.api.v1.Events/GetAllMetadata", runtime.WithHTTPPathPattern("/v1/events/{event_id}/metadata"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := local_request_Events_GetAllMetadata_0(rctx, inboundMarshaler, server, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := local_request_Events_GetAllMetadata_0(annotatedContext, inboundMarshaler, server, req, pathParams)
+		md.HeaderMD, md.TrailerMD = metadata.Join(md.HeaderMD, stream.Header()), metadata.Join(md.TrailerMD, stream.Trailer())
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_GetAllMetadata_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_GetAllMetadata_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("POST", pattern_Events_AddMetadata_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
+		var stream runtime.ServerTransportStream
+		ctx = grpc.NewContextWithServerTransportStream(ctx, &stream)
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateIncomingContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateIncomingContext(ctx, mux, req, "/mtap.api.v1.Events/AddMetadata", runtime.WithHTTPPathPattern("/v1/events/{event_id}/metadata/{key}"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := local_request_Events_AddMetadata_0(rctx, inboundMarshaler, server, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := local_request_Events_AddMetadata_0(annotatedContext, inboundMarshaler, server, req, pathParams)
+		md.HeaderMD, md.TrailerMD = metadata.Join(md.HeaderMD, stream.Header()), metadata.Join(md.TrailerMD, stream.Trailer())
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_AddMetadata_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_AddMetadata_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("POST", pattern_Events_AddDocument_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
+		var stream runtime.ServerTransportStream
+		ctx = grpc.NewContextWithServerTransportStream(ctx, &stream)
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateIncomingContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateIncomingContext(ctx, mux, req, "/mtap.api.v1.Events/AddDocument", runtime.WithHTTPPathPattern("/v1/events/{event_id}/documents/{document_name}"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := local_request_Events_AddDocument_0(rctx, inboundMarshaler, server, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := local_request_Events_AddDocument_0(annotatedContext, inboundMarshaler, server, req, pathParams)
+		md.HeaderMD, md.TrailerMD = metadata.Join(md.HeaderMD, stream.Header()), metadata.Join(md.TrailerMD, stream.Trailer())
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_AddDocument_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_AddDocument_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("GET", pattern_Events_GetAllDocumentNames_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
+		var stream runtime.ServerTransportStream
+		ctx = grpc.NewContextWithServerTransportStream(ctx, &stream)
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateIncomingContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateIncomingContext(ctx, mux, req, "/mtap.api.v1.Events/GetAllDocumentNames", runtime.WithHTTPPathPattern("/v1/events/{event_id}/documents"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := local_request_Events_GetAllDocumentNames_0(rctx, inboundMarshaler, server, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := local_request_Events_GetAllDocumentNames_0(annotatedContext, inboundMarshaler, server, req, pathParams)
+		md.HeaderMD, md.TrailerMD = metadata.Join(md.HeaderMD, stream.Header()), metadata.Join(md.TrailerMD, stream.Trailer())
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_GetAllDocumentNames_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_GetAllDocumentNames_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("GET", pattern_Events_GetDocumentText_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
+		var stream runtime.ServerTransportStream
+		ctx = grpc.NewContextWithServerTransportStream(ctx, &stream)
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateIncomingContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateIncomingContext(ctx, mux, req, "/mtap.api.v1.Events/GetDocumentText", runtime.WithHTTPPathPattern("/v1/events/{event_id}/documents/{document_name}"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := local_request_Events_GetDocumentText_0(rctx, inboundMarshaler, server, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := local_request_Events_GetDocumentText_0(annotatedContext, inboundMarshaler, server, req, pathParams)
+		md.HeaderMD, md.TrailerMD = metadata.Join(md.HeaderMD, stream.Header()), metadata.Join(md.TrailerMD, stream.Trailer())
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_GetDocumentText_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_GetDocumentText_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("GET", pattern_Events_GetLabelIndicesInfo_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
+		var stream runtime.ServerTransportStream
+		ctx = grpc.NewContextWithServerTransportStream(ctx, &stream)
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateIncomingContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateIncomingContext(ctx, mux, req, "/mtap.api.v1.Events/GetLabelIndicesInfo", runtime.WithHTTPPathPattern("/v1/events/{event_id}/documents/{document_name}/labels"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := local_request_Events_GetLabelIndicesInfo_0(rctx, inboundMarshaler, server, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := local_request_Events_GetLabelIndicesInfo_0(annotatedContext, inboundMarshaler, server, req, pathParams)
+		md.HeaderMD, md.TrailerMD = metadata.Join(md.HeaderMD, stream.Header()), metadata.Join(md.TrailerMD, stream.Trailer())
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_GetLabelIndicesInfo_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_GetLabelIndicesInfo_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("POST", pattern_Events_AddLabels_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
+		var stream runtime.ServerTransportStream
+		ctx = grpc.NewContextWithServerTransportStream(ctx, &stream)
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateIncomingContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateIncomingContext(ctx, mux, req, "/mtap.api.v1.Events/AddLabels", runtime.WithHTTPPathPattern("/v1/events/{event_id}/documents/{document_name}/labels/{index_name}"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := local_request_Events_AddLabels_0(rctx, inboundMarshaler, server, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := local_request_Events_AddLabels_0(annotatedContext, inboundMarshaler, server, req, pathParams)
+		md.HeaderMD, md.TrailerMD = metadata.Join(md.HeaderMD, stream.Header()), metadata.Join(md.TrailerMD, stream.Trailer())
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_AddLabels_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_AddLabels_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("GET", pattern_Events_GetLabels_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
+		var stream runtime.ServerTransportStream
+		ctx = grpc.NewContextWithServerTransportStream(ctx, &stream)
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateIncomingContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateIncomingContext(ctx, mux, req, "/mtap.api.v1.Events/GetLabels", runtime.WithHTTPPathPattern("/v1/events/{event_id}/documents/{document_name}/labels/{index_name}"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := local_request_Events_GetLabels_0(rctx, inboundMarshaler, server, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := local_request_Events_GetLabels_0(annotatedContext, inboundMarshaler, server, req, pathParams)
+		md.HeaderMD, md.TrailerMD = metadata.Join(md.HeaderMD, stream.Header()), metadata.Join(md.TrailerMD, stream.Trailer())
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_GetLabels_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_GetLabels_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("GET", pattern_Events_GetAllBinaryDataNames_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
+		var stream runtime.ServerTransportStream
+		ctx = grpc.NewContextWithServerTransportStream(ctx, &stream)
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateIncomingContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateIncomingContext(ctx, mux, req, "/mtap.api.v1.Events/GetAllBinaryDataNames", runtime.WithHTTPPathPattern("/v1/events/{event_id}/binaries"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := local_request_Events_GetAllBinaryDataNames_0(rctx, inboundMarshaler, server, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := local_request_Events_GetAllBinaryDataNames_0(annotatedContext, inboundMarshaler, server, req, pathParams)
+		md.HeaderMD, md.TrailerMD = metadata.Join(md.HeaderMD, stream.Header()), metadata.Join(md.TrailerMD, stream.Trailer())
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_GetAllBinaryDataNames_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_GetAllBinaryDataNames_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("POST", pattern_Events_AddBinaryData_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
+		var stream runtime.ServerTransportStream
+		ctx = grpc.NewContextWithServerTransportStream(ctx, &stream)
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateIncomingContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateIncomingContext(ctx, mux, req, "/mtap.api.v1.Events/AddBinaryData", runtime.WithHTTPPathPattern("/v1/events/{event_id}/binaries/{binary_data_name}"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := local_request_Events_AddBinaryData_0(rctx, inboundMarshaler, server, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := local_request_Events_AddBinaryData_0(annotatedContext, inboundMarshaler, server, req, pathParams)
+		md.HeaderMD, md.TrailerMD = metadata.Join(md.HeaderMD, stream.Header()), metadata.Join(md.TrailerMD, stream.Trailer())
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_AddBinaryData_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_AddBinaryData_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("GET", pattern_Events_GetBinaryData_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
+		var stream runtime.ServerTransportStream
+		ctx = grpc.NewContextWithServerTransportStream(ctx, &stream)
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateIncomingContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateIncomingContext(ctx, mux, req, "/mtap.api.v1.Events/GetBinaryData", runtime.WithHTTPPathPattern("/v1/events/{event_id}/binaries/{binary_data_name}"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := local_request_Events_GetBinaryData_0(rctx, inboundMarshaler, server, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := local_request_Events_GetBinaryData_0(annotatedContext, inboundMarshaler, server, req, pathParams)
+		md.HeaderMD, md.TrailerMD = metadata.Join(md.HeaderMD, stream.Header()), metadata.Join(md.TrailerMD, stream.Trailer())
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_GetBinaryData_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_GetBinaryData_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	return nil
 }
 
 // RegisterEventsHandlerFromEndpoint is same as RegisterEventsHandler but
 // automatically dials to "endpoint" and closes the connection when "ctx" gets done.
 func RegisterEventsHandlerFromEndpoint(ctx context.Context, mux *runtime.ServeMux, endpoint string, opts []grpc.DialOption) (err error) {
-	conn, err := grpc.Dial(endpoint, opts...)
+	conn, err := grpc.DialContext(ctx, endpoint, opts...)
 	if err != nil {
 		return err
 	}
 	defer func() {
 		if err != nil {
 			if cerr := conn.Close(); cerr != nil {
 				grpclog.Infof("Failed to close conn to %s: %v", endpoint, cerr)
@@ -1392,321 +1420,349 @@
 // "EventsClient" to call the correct interceptors.
 func RegisterEventsHandlerClient(ctx context.Context, mux *runtime.ServeMux, client EventsClient) error {
 
 	mux.Handle("GET", pattern_Events_GetEventsInstanceId_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateContext(ctx, mux, req, "/mtap.api.v1.Events/GetEventsInstanceId", runtime.WithHTTPPathPattern("/v1/events/instance_id"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := request_Events_GetEventsInstanceId_0(rctx, inboundMarshaler, client, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := request_Events_GetEventsInstanceId_0(annotatedContext, inboundMarshaler, client, req, pathParams)
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_GetEventsInstanceId_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_GetEventsInstanceId_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("POST", pattern_Events_OpenEvent_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateContext(ctx, mux, req, "/mtap.api.v1.Events/OpenEvent", runtime.WithHTTPPathPattern("/v1/events/{event_id}"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := request_Events_OpenEvent_0(rctx, inboundMarshaler, client, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := request_Events_OpenEvent_0(annotatedContext, inboundMarshaler, client, req, pathParams)
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_OpenEvent_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_OpenEvent_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("DELETE", pattern_Events_CloseEvent_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateContext(ctx, mux, req, "/mtap.api.v1.Events/CloseEvent", runtime.WithHTTPPathPattern("/v1/events/{event_id}"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := request_Events_CloseEvent_0(rctx, inboundMarshaler, client, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := request_Events_CloseEvent_0(annotatedContext, inboundMarshaler, client, req, pathParams)
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_CloseEvent_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_CloseEvent_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("GET", pattern_Events_GetAllMetadata_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateContext(ctx, mux, req, "/mtap.api.v1.Events/GetAllMetadata", runtime.WithHTTPPathPattern("/v1/events/{event_id}/metadata"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := request_Events_GetAllMetadata_0(rctx, inboundMarshaler, client, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := request_Events_GetAllMetadata_0(annotatedContext, inboundMarshaler, client, req, pathParams)
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_GetAllMetadata_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_GetAllMetadata_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("POST", pattern_Events_AddMetadata_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateContext(ctx, mux, req, "/mtap.api.v1.Events/AddMetadata", runtime.WithHTTPPathPattern("/v1/events/{event_id}/metadata/{key}"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := request_Events_AddMetadata_0(rctx, inboundMarshaler, client, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := request_Events_AddMetadata_0(annotatedContext, inboundMarshaler, client, req, pathParams)
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_AddMetadata_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_AddMetadata_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("POST", pattern_Events_AddDocument_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateContext(ctx, mux, req, "/mtap.api.v1.Events/AddDocument", runtime.WithHTTPPathPattern("/v1/events/{event_id}/documents/{document_name}"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := request_Events_AddDocument_0(rctx, inboundMarshaler, client, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := request_Events_AddDocument_0(annotatedContext, inboundMarshaler, client, req, pathParams)
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_AddDocument_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_AddDocument_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("GET", pattern_Events_GetAllDocumentNames_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateContext(ctx, mux, req, "/mtap.api.v1.Events/GetAllDocumentNames", runtime.WithHTTPPathPattern("/v1/events/{event_id}/documents"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := request_Events_GetAllDocumentNames_0(rctx, inboundMarshaler, client, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := request_Events_GetAllDocumentNames_0(annotatedContext, inboundMarshaler, client, req, pathParams)
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_GetAllDocumentNames_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_GetAllDocumentNames_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("GET", pattern_Events_GetDocumentText_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateContext(ctx, mux, req, "/mtap.api.v1.Events/GetDocumentText", runtime.WithHTTPPathPattern("/v1/events/{event_id}/documents/{document_name}"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := request_Events_GetDocumentText_0(rctx, inboundMarshaler, client, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := request_Events_GetDocumentText_0(annotatedContext, inboundMarshaler, client, req, pathParams)
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_GetDocumentText_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_GetDocumentText_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("GET", pattern_Events_GetLabelIndicesInfo_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateContext(ctx, mux, req, "/mtap.api.v1.Events/GetLabelIndicesInfo", runtime.WithHTTPPathPattern("/v1/events/{event_id}/documents/{document_name}/labels"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := request_Events_GetLabelIndicesInfo_0(rctx, inboundMarshaler, client, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := request_Events_GetLabelIndicesInfo_0(annotatedContext, inboundMarshaler, client, req, pathParams)
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_GetLabelIndicesInfo_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_GetLabelIndicesInfo_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("POST", pattern_Events_AddLabels_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateContext(ctx, mux, req, "/mtap.api.v1.Events/AddLabels", runtime.WithHTTPPathPattern("/v1/events/{event_id}/documents/{document_name}/labels/{index_name}"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := request_Events_AddLabels_0(rctx, inboundMarshaler, client, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := request_Events_AddLabels_0(annotatedContext, inboundMarshaler, client, req, pathParams)
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_AddLabels_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_AddLabels_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("GET", pattern_Events_GetLabels_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateContext(ctx, mux, req, "/mtap.api.v1.Events/GetLabels", runtime.WithHTTPPathPattern("/v1/events/{event_id}/documents/{document_name}/labels/{index_name}"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := request_Events_GetLabels_0(rctx, inboundMarshaler, client, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := request_Events_GetLabels_0(annotatedContext, inboundMarshaler, client, req, pathParams)
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_GetLabels_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_GetLabels_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("GET", pattern_Events_GetAllBinaryDataNames_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateContext(ctx, mux, req, "/mtap.api.v1.Events/GetAllBinaryDataNames", runtime.WithHTTPPathPattern("/v1/events/{event_id}/binaries"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := request_Events_GetAllBinaryDataNames_0(rctx, inboundMarshaler, client, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := request_Events_GetAllBinaryDataNames_0(annotatedContext, inboundMarshaler, client, req, pathParams)
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_GetAllBinaryDataNames_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_GetAllBinaryDataNames_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("POST", pattern_Events_AddBinaryData_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateContext(ctx, mux, req, "/mtap.api.v1.Events/AddBinaryData", runtime.WithHTTPPathPattern("/v1/events/{event_id}/binaries/{binary_data_name}"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := request_Events_AddBinaryData_0(rctx, inboundMarshaler, client, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := request_Events_AddBinaryData_0(annotatedContext, inboundMarshaler, client, req, pathParams)
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_AddBinaryData_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_AddBinaryData_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	mux.Handle("GET", pattern_Events_GetBinaryData_0, func(w http.ResponseWriter, req *http.Request, pathParams map[string]string) {
 		ctx, cancel := context.WithCancel(req.Context())
 		defer cancel()
 		inboundMarshaler, outboundMarshaler := runtime.MarshalerForRequest(mux, req)
-		rctx, err := runtime.AnnotateContext(ctx, mux, req)
+		var err error
+		var annotatedContext context.Context
+		annotatedContext, err = runtime.AnnotateContext(ctx, mux, req, "/mtap.api.v1.Events/GetBinaryData", runtime.WithHTTPPathPattern("/v1/events/{event_id}/binaries/{binary_data_name}"))
 		if err != nil {
 			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
 			return
 		}
-		resp, md, err := request_Events_GetBinaryData_0(rctx, inboundMarshaler, client, req, pathParams)
-		ctx = runtime.NewServerMetadataContext(ctx, md)
+		resp, md, err := request_Events_GetBinaryData_0(annotatedContext, inboundMarshaler, client, req, pathParams)
+		annotatedContext = runtime.NewServerMetadataContext(annotatedContext, md)
 		if err != nil {
-			runtime.HTTPError(ctx, mux, outboundMarshaler, w, req, err)
+			runtime.HTTPError(annotatedContext, mux, outboundMarshaler, w, req, err)
 			return
 		}
 
-		forward_Events_GetBinaryData_0(ctx, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
+		forward_Events_GetBinaryData_0(annotatedContext, mux, outboundMarshaler, w, req, resp, mux.GetForwardResponseOptions()...)
 
 	})
 
 	return nil
 }
 
 var (
-	pattern_Events_GetEventsInstanceId_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 2, 2}, []string{"v1", "events", "instance_id"}, "", runtime.AssumeColonVerbOpt(true)))
+	pattern_Events_GetEventsInstanceId_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 2, 2}, []string{"v1", "events", "instance_id"}, ""))
 
-	pattern_Events_OpenEvent_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2}, []string{"v1", "events", "event_id"}, "", runtime.AssumeColonVerbOpt(true)))
+	pattern_Events_OpenEvent_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2}, []string{"v1", "events", "event_id"}, ""))
 
-	pattern_Events_CloseEvent_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2}, []string{"v1", "events", "event_id"}, "", runtime.AssumeColonVerbOpt(true)))
+	pattern_Events_CloseEvent_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2}, []string{"v1", "events", "event_id"}, ""))
 
-	pattern_Events_GetAllMetadata_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3}, []string{"v1", "events", "event_id", "metadata"}, "", runtime.AssumeColonVerbOpt(true)))
+	pattern_Events_GetAllMetadata_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3}, []string{"v1", "events", "event_id", "metadata"}, ""))
 
-	pattern_Events_AddMetadata_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3, 1, 0, 4, 1, 5, 4}, []string{"v1", "events", "event_id", "metadata", "key"}, "", runtime.AssumeColonVerbOpt(true)))
+	pattern_Events_AddMetadata_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3, 1, 0, 4, 1, 5, 4}, []string{"v1", "events", "event_id", "metadata", "key"}, ""))
 
-	pattern_Events_AddDocument_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3, 1, 0, 4, 1, 5, 4}, []string{"v1", "events", "event_id", "documents", "document_name"}, "", runtime.AssumeColonVerbOpt(true)))
+	pattern_Events_AddDocument_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3, 1, 0, 4, 1, 5, 4}, []string{"v1", "events", "event_id", "documents", "document_name"}, ""))
 
-	pattern_Events_GetAllDocumentNames_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3}, []string{"v1", "events", "event_id", "documents"}, "", runtime.AssumeColonVerbOpt(true)))
+	pattern_Events_GetAllDocumentNames_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3}, []string{"v1", "events", "event_id", "documents"}, ""))
 
-	pattern_Events_GetDocumentText_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3, 1, 0, 4, 1, 5, 4}, []string{"v1", "events", "event_id", "documents", "document_name"}, "", runtime.AssumeColonVerbOpt(true)))
+	pattern_Events_GetDocumentText_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3, 1, 0, 4, 1, 5, 4}, []string{"v1", "events", "event_id", "documents", "document_name"}, ""))
 
-	pattern_Events_GetLabelIndicesInfo_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3, 1, 0, 4, 1, 5, 4, 2, 5}, []string{"v1", "events", "event_id", "documents", "document_name", "labels"}, "", runtime.AssumeColonVerbOpt(true)))
+	pattern_Events_GetLabelIndicesInfo_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3, 1, 0, 4, 1, 5, 4, 2, 5}, []string{"v1", "events", "event_id", "documents", "document_name", "labels"}, ""))
 
-	pattern_Events_AddLabels_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3, 1, 0, 4, 1, 5, 4, 2, 5, 1, 0, 4, 1, 5, 6}, []string{"v1", "events", "event_id", "documents", "document_name", "labels", "index_name"}, "", runtime.AssumeColonVerbOpt(true)))
+	pattern_Events_AddLabels_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3, 1, 0, 4, 1, 5, 4, 2, 5, 1, 0, 4, 1, 5, 6}, []string{"v1", "events", "event_id", "documents", "document_name", "labels", "index_name"}, ""))
 
-	pattern_Events_GetLabels_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3, 1, 0, 4, 1, 5, 4, 2, 5, 1, 0, 4, 1, 5, 6}, []string{"v1", "events", "event_id", "documents", "document_name", "labels", "index_name"}, "", runtime.AssumeColonVerbOpt(true)))
+	pattern_Events_GetLabels_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3, 1, 0, 4, 1, 5, 4, 2, 5, 1, 0, 4, 1, 5, 6}, []string{"v1", "events", "event_id", "documents", "document_name", "labels", "index_name"}, ""))
 
-	pattern_Events_GetAllBinaryDataNames_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3}, []string{"v1", "events", "event_id", "binaries"}, "", runtime.AssumeColonVerbOpt(true)))
+	pattern_Events_GetAllBinaryDataNames_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3}, []string{"v1", "events", "event_id", "binaries"}, ""))
 
-	pattern_Events_AddBinaryData_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3, 1, 0, 4, 1, 5, 4}, []string{"v1", "events", "event_id", "binaries", "binary_data_name"}, "", runtime.AssumeColonVerbOpt(true)))
+	pattern_Events_AddBinaryData_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3, 1, 0, 4, 1, 5, 4}, []string{"v1", "events", "event_id", "binaries", "binary_data_name"}, ""))
 
-	pattern_Events_GetBinaryData_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3, 1, 0, 4, 1, 5, 4}, []string{"v1", "events", "event_id", "binaries", "binary_data_name"}, "", runtime.AssumeColonVerbOpt(true)))
+	pattern_Events_GetBinaryData_0 = runtime.MustPattern(runtime.NewPattern(1, []int{2, 0, 2, 1, 1, 0, 4, 1, 5, 2, 2, 3, 1, 0, 4, 1, 5, 4}, []string{"v1", "events", "event_id", "binaries", "binary_data_name"}, ""))
 )
 
 var (
 	forward_Events_GetEventsInstanceId_0 = runtime.ForwardResponseMessage
 
 	forward_Events_OpenEvent_0 = runtime.ForwardResponseMessage
```

### Comparing `mtap-1.1.0/go/mtap/consul/resolver.go` & `mtap-1.2.0/go/mtap/consul/resolver.go`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/go/mtap/processors/processors.go` & `mtap-1.2.0/go/mtap/processors/processors.go`

 * *Files 4% similar despite different names*

```diff
@@ -17,20 +17,21 @@
 package processors
 
 import (
 	"context"
 	"encoding/json"
 	"github.com/golang/glog"
 	"github.com/gorilla/mux"
-	"github.com/grpc-ecosystem/grpc-gateway/runtime"
+	"github.com/grpc-ecosystem/grpc-gateway/v2/runtime"
 	"github.com/hashicorp/consul/api"
-	"github.com/nlpie/mtap/go/mtap/api/v1"
+	ApiV1 "github.com/nlpie/mtap/go/mtap/api/v1"
 	"golang.org/x/sync/semaphore"
 	"google.golang.org/grpc"
 	"google.golang.org/grpc/credentials/insecure"
+	"google.golang.org/protobuf/encoding/protojson"
 	"net/http"
 	"strconv"
 	"time"
 )
 
 type Gateway struct {
 	mux      *runtime.ServeMux
@@ -246,18 +247,18 @@
 	}
 	ps.processors = processorsCopy
 	glog.V(2).Info("Finished updating processor gateways")
 }
 
 func (ps *Server) newManualProcessorGateway(manualProcessor ManualProcessor) (*Gateway, error) {
 	glog.V(2).Infof("Starting new processor gateway for service: %v with address: %v", manualProcessor.Identifier, manualProcessor.Endpoint)
-	gwmux := runtime.NewServeMux(runtime.WithMarshalerOption(runtime.MIMEWildcard, &runtime.JSONPb{OrigName: true, EmitDefaults: true}))
+	gwmux := runtime.NewServeMux(runtime.WithMarshalerOption(runtime.MIMEWildcard, &runtime.JSONPb{MarshalOptions: protojson.MarshalOptions{EmitUnpopulated: true, UseProtoNames: true}}))
 	ctx, cancel := context.WithCancel(ps.ctx)
 
-	err := mtap_api_v1.RegisterProcessorHandlerFromEndpoint(
+	err := ApiV1.RegisterProcessorHandlerFromEndpoint(
 		ctx,
 		gwmux,
 		manualProcessor.Endpoint,
 		ps.createDialOptions())
 
 	if err != nil {
 		cancel()
@@ -274,18 +275,18 @@
 		dialOptions = append(dialOptions, grpc.WithNoProxy())
 	}
 	return dialOptions
 }
 
 func (ps *Server) newProcessorGateway(pn string) (*Gateway, error) {
 	glog.V(2).Infof("Starting new processor gateway for service: %v", pn)
-	gwmux := runtime.NewServeMux(runtime.WithMarshalerOption(runtime.MIMEWildcard, &runtime.JSONPb{OrigName: true, EmitDefaults: true}))
+	gwmux := runtime.NewServeMux(runtime.WithMarshalerOption(runtime.MIMEWildcard, &runtime.JSONPb{MarshalOptions: protojson.MarshalOptions{EmitUnpopulated: true, UseProtoNames: true}}))
 	ctx, cancel := context.WithCancel(ps.ctx)
 
-	err := mtap_api_v1.RegisterProcessorHandlerFromEndpoint(
+	err := ApiV1.RegisterProcessorHandlerFromEndpoint(
 		ctx,
 		gwmux,
 		"consul://"+ps.authority+"/"+pn+"/v1-mtap-processor",
 		ps.createDialOptions())
 
 	if err != nil {
 		cancel()
```

### Comparing `mtap-1.1.0/go/mtap-gateway/mtap-gateway.go` & `mtap-1.2.0/go/mtap-gateway/mtap-gateway.go`

 * *Files 13% similar despite different names*

```diff
@@ -17,114 +17,77 @@
 package main
 
 import (
 	"context"
 	"flag"
 	"fmt"
 	"github.com/golang/glog"
-	"github.com/gorilla/handlers"
 	"github.com/gorilla/mux"
-	"github.com/grpc-ecosystem/grpc-gateway/runtime"
-	"github.com/nlpie/mtap/go/mtap/api/v1"
+	"github.com/grpc-ecosystem/grpc-gateway/v2/runtime"
+	ApiV1 "github.com/nlpie/mtap/go/mtap/api/v1"
 	_ "github.com/nlpie/mtap/go/mtap/consul"
 	"github.com/nlpie/mtap/go/mtap/processors"
 	"github.com/spf13/cast"
 	"github.com/spf13/viper"
 	"google.golang.org/grpc"
 	"google.golang.org/grpc/credentials/insecure"
-	"io"
+	"google.golang.org/protobuf/encoding/protojson"
 	"net/http"
 	"os"
 	"os/signal"
 	"strconv"
-	"strings"
 	"time"
 )
 
-func serveSwagger(r *mux.Router) {
-	m := mux.NewRouter()
-	m.HandleFunc("/v1/processors/swagger.json",
-		func(w http.ResponseWriter, req *http.Request) {
-			_, err := io.Copy(w, strings.NewReader(mtap_api_v1.Processing))
-			if err != nil {
-				w.WriteHeader(500)
-			}
-			w.Header().Set("Content-Type", "application/json")
-		})
-
-	m.HandleFunc("/v1/events/swagger.json",
-		func(w http.ResponseWriter, req *http.Request) {
-			_, err := io.Copy(w, strings.NewReader(mtap_api_v1.Events))
-			if err != nil {
-				w.WriteHeader(500)
-			}
-			w.Header().Set("Content-Type", "application/json")
-		})
-
-	corsHandler := handlers.CORS(
-		handlers.AllowedOrigins([]string{"*"}),
-		handlers.AllowedMethods([]string{"GET", "POST", "DELETE", "PUT", "PATCH", "OPTIONS"}),
-		handlers.AllowedHeaders([]string{"Content-Type", "api-key", "Authorization"}),
-	)
-	r.Handle("/v1/processors/swagger.json", corsHandler(m))
-	r.Handle("/v1/events/swagger.json", corsHandler(m))
-}
-
 func run() error {
 	glog.V(1).Infoln("Starting MTAP API Gateway")
-	err := viper.ReadInConfig() // Find and read the config file
-	if err != nil {             // Handle errors reading the config file
-		// will use sensible defaults
-		err = nil
-	}
 
 	ctx := context.Background()
 	ctx, cancel := context.WithCancel(ctx)
 	defer cancel()
 
 	consulPort := viper.GetInt("consul.port")
 	consulHost := viper.GetString("consul.host")
 	consulAddr := consulHost + ":" + strconv.Itoa(consulPort)
 
 	m := mux.NewRouter()
 
-	serveSwagger(m)
-
 	config := processors.Config{
 		ConsulAddress:       consulHost,
 		ConsulPort:          consulPort,
 		RefreshInterval:     viper.GetDuration("gateway.refresh_interval"),
 		GrpcEnableHttpProxy: viper.GetBool("grpc.enable_proxy"),
 	}
 
 	var manualProcessors []processors.ManualProcessor
-	err = viper.UnmarshalKey("gateway.processors", &manualProcessors)
+	err := viper.UnmarshalKey("gateway.processors", &manualProcessors)
 	if err != nil {
 		err = nil
 	} else {
 		config.ManualProcessors = manualProcessors
 	}
 
 	server, err := processors.NewProcessorsServer(ctx, &config)
 	if err != nil {
 		return err
 	}
 	m.PathPrefix("/v1/processors").Handler(server.Dispatcher)
 
-	gwmux := runtime.NewServeMux(runtime.WithMarshalerOption(runtime.MIMEWildcard, &runtime.JSONPb{OrigName: true, EmitDefaults: true}))
+	gwmux := runtime.NewServeMux(runtime.WithMarshalerOption(runtime.MIMEWildcard,
+		&runtime.JSONPb{MarshalOptions: protojson.MarshalOptions{EmitUnpopulated: true, UseProtoNames: true}}))
 	eventsLookup := viper.Get("gateway.events")
 	var eventsAddr string
 	if eventsLookup != nil {
 		eventsAddr = cast.ToString(eventsLookup)
 		glog.Infof("Using events address: %s", eventsAddr)
 	} else {
 		eventsAddr = fmt.Sprintf("consul://%s/mtap-events/v1", consulAddr)
 		glog.Info("Using consul service discovery for events: ", eventsAddr)
 	}
-	err = mtap_api_v1.RegisterEventsHandlerFromEndpoint(
+	err = ApiV1.RegisterEventsHandlerFromEndpoint(
 		ctx,
 		gwmux,
 		eventsAddr,
 		[]grpc.DialOption{grpc.WithTransportCredentials(insecure.NewCredentials()),
 			grpc.WithDefaultServiceConfig(`{"loadBalancingPolicy":"round_robin"}`)})
 	if err != nil {
 		return err
@@ -158,16 +121,18 @@
 	_ = srv.Shutdown(ctx2)
 	_ = fmt.Errorf("shutting down")
 	return nil
 }
 
 func main() {
 	var mtapConfigFlag string
+	var port int
 	flag.StringVar(&mtapConfigFlag, "mtap-config", "",
 		"The path to the mtap configuration file")
+	flag.IntVar(&port, "port", -1, "The port to use")
 	flag.Parse()
 	viper.SetDefault("consul.host", "localhost")
 	viper.SetDefault("consul.port", 8500)
 	viper.SetDefault("gateway.port", 8080)
 	viper.SetDefault("gateway.refresh_interval", 10)
 	viper.SetDefault("gateway.events", nil)
 	viper.SetDefault("gateway.processors", []processors.ManualProcessor{})
@@ -184,13 +149,23 @@
 	} else {
 		viper.SetConfigName("mtapConfig")
 		viper.AddConfigPath(".")
 		viper.AddConfigPath("$HOME/.mtap")
 		viper.AddConfigPath("/etc/mtap")
 	}
 
+	err := viper.ReadInConfig() // Find and read the config file
+	if err != nil {             // Handle errors reading the config file
+		// will use sensible defaults
+		err = nil
+	}
+
+	if port != -1 {
+		viper.Set("gateway.port", port)
+	}
+
 	defer glog.Flush()
 
 	if err := run(); err != nil {
 		glog.Fatal(err)
 	}
 }
```

### Comparing `mtap-1.1.0/go/store-swaggers/main.go` & `mtap-1.2.0/go/store-swaggers/main.go`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/go/third_party/googleapis/google/api/annotations.proto` & `mtap-1.2.0/go/third_party/googleapis/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/go/third_party/googleapis/google/api/field_behavior.proto` & `mtap-1.2.0/go/third_party/googleapis/google/api/field_behavior.proto`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/go/third_party/googleapis/google/api/http.proto` & `mtap-1.2.0/go/third_party/googleapis/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/go/third_party/googleapis/google/api/httpbody.proto` & `mtap-1.2.0/go/third_party/googleapis/google/api/httpbody.proto`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/build.gradle` & `mtap-1.2.0/java/build.gradle`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 plugins {
     id 'java-library'
     id 'maven-publish'
     id 'com.google.protobuf' version '0.9.2'
     id 'signing'
-    id 'com.github.johnrengelman.shadow' version '8.1.0'
+    id 'com.github.johnrengelman.shadow' version '8.1.1'
 }
 
 def gitVersion = { ->
     def stdout = new ByteArrayOutputStream()
     def execResult = exec {
         commandLine 'git', 'describe', '--tags', '--dirty'
         standardOutput = stdout
@@ -93,18 +93,19 @@
         runtimeClasspath += sourceSets.main.output
         resources {
             srcDirs 'log_resources'
         }
     }
 }
 
-def grpcVersion = '1.53.0'
-def protobufVersion = '3.22.2'
+def grpcVersion = ['1.53.0', '1.54.0']
+def protobufVersion = '3.22.3'
 def junitVersion = '5.9.2'
 def sl4fjVersion = '2.0.6'
+def log4jVersion = '2.20.0'
 
 dependencies {
     api group: 'org.jetbrains', name: 'annotations', version: ['16.0.2', '24.0.1']
     api group: 'com.google.api.grpc', name: 'proto-google-common-protos', version: ['2.9.0','2.14.2']
     api group: 'args4j', name: 'args4j', version: '2.33'
 
     implementation group: 'com.google.guava', name: 'guava', version: '31.1-jre'
@@ -120,19 +121,21 @@
     implementation group: 'com.google.protobuf', name: 'protobuf-java', version: protobufVersion
     implementation group: 'com.google.protobuf', name: 'protobuf-java-util', version: protobufVersion
 
     implementation group: 'org.apache.tomcat', name: 'tomcat-annotations-api', version: '10.1.7'
 
     compileOnly 'org.apache.tomcat:annotations-api:6.0.53'
 
-    testImplementation group: 'org.mockito', name: 'mockito-core', version: '5.2.0'
+    testImplementation group: 'org.mockito', name: 'mockito-core', version: '5.3.0'
     testImplementation group: 'io.grpc', name: 'grpc-testing', version: grpcVersion
     testImplementation group: 'org.junit.jupiter', name: 'junit-jupiter-api', version: junitVersion
     testRuntimeOnly group: 'org.slf4j', name: 'slf4j-simple', version: sl4fjVersion
     testRuntimeOnly group: 'org.junit.jupiter', name: 'junit-jupiter-engine', version: junitVersion
+    withLogBindingRuntimeOnly group: 'org.apache.logging.log4j', name: 'log4j-slf4j2-impl', version: log4jVersion
+    withLogBindingRuntimeOnly group: 'org.apache.logging.log4j', name: 'log4j-core', version: log4jVersion
 }
 
 protobuf {
     protoc { artifact = "com.google.protobuf:protoc:${protobufVersion}" }
     plugins {
         grpc { artifact = "io.grpc:protoc-gen-grpc-java:${grpcVersion}" }
     }
```

### Comparing `mtap-1.1.0/java/gradle/wrapper/gradle-wrapper.jar` & `mtap-1.2.0/java/gradle/wrapper/gradle-wrapper.jar`

 * *Files 15% similar despite different names*

#### zipinfo {}

```diff
@@ -1,57 +1,57 @@
-Zip file size: 60756 bytes, number of entries: 55
+Zip file size: 61608 bytes, number of entries: 55
 drwxr-xr-x  2.0 unx        0 b- defN 80-Feb-01 00:00 META-INF/
 -rw-r--r--  2.0 unx       63 b- defN 80-Feb-01 00:00 META-INF/MANIFEST.MF
 drwxr-xr-x  2.0 unx        0 b- defN 80-Feb-01 00:00 org/
 drwxr-xr-x  2.0 unx        0 b- defN 80-Feb-01 00:00 org/gradle/
 drwxr-xr-x  2.0 unx        0 b- defN 80-Feb-01 00:00 org/gradle/wrapper/
--rw-r--r--  2.0 unx     5677 b- defN 80-Feb-01 00:00 org/gradle/wrapper/GradleWrapperMain.class
+-rw-r--r--  2.0 unx     5982 b- defN 80-Feb-01 00:00 org/gradle/wrapper/GradleWrapperMain.class
 -rw-r--r--  2.0 unx       51 b- defN 80-Feb-01 00:00 gradle-wrapper-classpath.properties
 -rw-r--r--  2.0 unx        0 b- defN 80-Feb-01 00:00 gradle-wrapper-parameter-names.properties
 drwxr-xr-x  2.0 unx        0 b- defN 80-Feb-01 00:00 org/gradle/cli/
 -rw-r--r--  2.0 unx     1363 b- defN 80-Feb-01 00:00 org/gradle/cli/AbstractCommandLineConverter.class
 -rw-r--r--  2.0 unx     2796 b- defN 80-Feb-01 00:00 org/gradle/cli/AbstractPropertiesCommandLineConverter.class
 -rw-r--r--  2.0 unx      587 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineArgumentException.class
 -rw-r--r--  2.0 unx      615 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineConverter.class
 -rw-r--r--  2.0 unx     3687 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineOption.class
 -rw-r--r--  2.0 unx      229 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineParser$1.class
 -rw-r--r--  2.0 unx     2495 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineParser$AfterFirstSubCommand.class
 -rw-r--r--  2.0 unx     1830 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineParser$AfterOptions.class
 -rw-r--r--  2.0 unx     2933 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineParser$BeforeFirstSubCommand.class
 -rw-r--r--  2.0 unx     1263 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineParser$CaseInsensitiveStringComparator.class
--rw-r--r--  2.0 unx     4390 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineParser$KnownOptionParserState.class
+-rw-r--r--  2.0 unx     4472 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineParser$KnownOptionParserState.class
 -rw-r--r--  2.0 unx     1780 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineParser$MissingOptionArgState.class
 -rw-r--r--  2.0 unx     1732 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineParser$OptionAwareParserState.class
 -rw-r--r--  2.0 unx     1706 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineParser$OptionComparator.class
 -rw-r--r--  2.0 unx      931 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineParser$OptionParserState.class
 -rw-r--r--  2.0 unx     1462 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineParser$OptionString.class
 -rw-r--r--  2.0 unx     1400 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineParser$OptionStringComparator.class
 -rw-r--r--  2.0 unx     1208 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineParser$ParserState.class
 -rw-r--r--  2.0 unx     1899 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineParser$UnknownOptionParserState.class
--rw-r--r--  2.0 unx    10604 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineParser.class
+-rw-r--r--  2.0 unx    10729 b- defN 80-Feb-01 00:00 org/gradle/cli/CommandLineParser.class
 -rw-r--r--  2.0 unx     4608 b- defN 80-Feb-01 00:00 org/gradle/cli/ParsedCommandLine.class
 -rw-r--r--  2.0 unx     1349 b- defN 80-Feb-01 00:00 org/gradle/cli/ParsedCommandLineOption.class
 -rw-r--r--  2.0 unx      779 b- defN 80-Feb-01 00:00 org/gradle/cli/ProjectPropertiesCommandLineConverter.class
 -rw-r--r--  2.0 unx      764 b- defN 80-Feb-01 00:00 org/gradle/cli/SystemPropertiesCommandLineConverter.class
 drwxr-xr-x  2.0 unx        0 b- defN 80-Feb-01 00:00 org/gradle/util/
 drwxr-xr-x  2.0 unx        0 b- defN 80-Feb-01 00:00 org/gradle/util/internal/
--rw-r--r--  2.0 unx     1319 b- defN 80-Feb-01 00:00 org/gradle/util/internal/ZipSlip.class
+-rw-r--r--  2.0 unx     1560 b- defN 80-Feb-01 00:00 org/gradle/util/internal/ZipSlip.class
 -rw-r--r--  2.0 unx      793 b- defN 80-Feb-01 00:00 org/gradle/wrapper/BootstrapMainStarter$1.class
--rw-r--r--  2.0 unx     2596 b- defN 80-Feb-01 00:00 org/gradle/wrapper/BootstrapMainStarter.class
+-rw-r--r--  2.0 unx     2572 b- defN 80-Feb-01 00:00 org/gradle/wrapper/BootstrapMainStarter.class
 -rw-r--r--  2.0 unx      210 b- defN 80-Feb-01 00:00 org/gradle/wrapper/Download$1.class
 -rw-r--r--  2.0 unx     2008 b- defN 80-Feb-01 00:00 org/gradle/wrapper/Download$DefaultDownloadProgressListener.class
 -rw-r--r--  2.0 unx     1918 b- defN 80-Feb-01 00:00 org/gradle/wrapper/Download$ProxyAuthenticator.class
--rw-r--r--  2.0 unx     9896 b- defN 80-Feb-01 00:00 org/gradle/wrapper/Download.class
+-rw-r--r--  2.0 unx    10624 b- defN 80-Feb-01 00:00 org/gradle/wrapper/Download.class
 -rw-r--r--  2.0 unx      202 b- defN 80-Feb-01 00:00 org/gradle/wrapper/DownloadProgressListener.class
 -rw-r--r--  2.0 unx     3204 b- defN 80-Feb-01 00:00 org/gradle/wrapper/ExclusiveFileAccessManager.class
 -rw-r--r--  2.0 unx     1158 b- defN 80-Feb-01 00:00 org/gradle/wrapper/GradleUserHomeLookup.class
 -rw-r--r--  2.0 unx      219 b- defN 80-Feb-01 00:00 org/gradle/wrapper/IDownload.class
--rw-r--r--  2.0 unx     4742 b- defN 80-Feb-01 00:00 org/gradle/wrapper/Install$1.class
+-rw-r--r--  2.0 unx     4754 b- defN 80-Feb-01 00:00 org/gradle/wrapper/Install$1.class
 -rw-r--r--  2.0 unx     1561 b- defN 80-Feb-01 00:00 org/gradle/wrapper/Install$InstallCheck.class
 -rw-r--r--  2.0 unx    11647 b- defN 80-Feb-01 00:00 org/gradle/wrapper/Install.class
 -rw-r--r--  2.0 unx     1332 b- defN 80-Feb-01 00:00 org/gradle/wrapper/Logger.class
 -rw-r--r--  2.0 unx      751 b- defN 80-Feb-01 00:00 org/gradle/wrapper/PathAssembler$LocalDistribution.class
 -rw-r--r--  2.0 unx     3627 b- defN 80-Feb-01 00:00 org/gradle/wrapper/PathAssembler.class
 -rw-r--r--  2.0 unx     2428 b- defN 80-Feb-01 00:00 org/gradle/wrapper/SystemPropertiesHandler.class
--rw-r--r--  2.0 unx     1855 b- defN 80-Feb-01 00:00 org/gradle/wrapper/WrapperConfiguration.class
--rw-r--r--  2.0 unx     5148 b- defN 80-Feb-01 00:00 org/gradle/wrapper/WrapperExecutor.class
-55 files, 114815 bytes uncompressed, 51816 bytes compressed:  54.9%
+-rw-r--r--  2.0 unx     2128 b- defN 80-Feb-01 00:00 org/gradle/wrapper/WrapperConfiguration.class
+-rw-r--r--  2.0 unx     5548 b- defN 80-Feb-01 00:00 org/gradle/wrapper/WrapperExecutor.class
+55 files, 116957 bytes uncompressed, 52668 bytes compressed:  55.0%
```

#### filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v1.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

#### org/gradle/wrapper/GradleWrapperMain.class

##### procyon -ec {}

```diff
@@ -32,15 +32,17 @@
         final ParsedCommandLine options = parser.parse(args);
         final Properties systemProperties = System.getProperties();
         systemProperties.putAll(converter.convert(options, (Map)new HashMap()));
         final File gradleUserHome = gradleUserHome(options);
         addSystemProperties(systemProperties, gradleUserHome, rootDir);
         final Logger logger = logger(options);
         final WrapperExecutor wrapperExecutor = WrapperExecutor.forWrapperPropertiesFile(propertiesFile);
-        wrapperExecutor.execute(args, new Install(logger, (IDownload)new Download(logger, "gradlew", "0"), new PathAssembler(gradleUserHome, rootDir)), new BootstrapMainStarter());
+        final WrapperConfiguration configuration = wrapperExecutor.getConfiguration();
+        final IDownload download = (IDownload)new Download(logger, "gradlew", "0", configuration.getNetworkTimeout());
+        wrapperExecutor.execute(args, new Install(logger, download, new PathAssembler(gradleUserHome, rootDir)), new BootstrapMainStarter());
     }
     
     private static void addSystemProperties(final Properties systemProperties, final File gradleUserHome, final File rootDir) {
         systemProperties.putAll(SystemPropertiesHandler.getSystemProperties(new File(rootDir, "gradle.properties")));
         systemProperties.putAll(SystemPropertiesHandler.getSystemProperties(new File(gradleUserHome, "gradle.properties")));
     }
```

#### org/gradle/cli/CommandLineParser$AfterFirstSubCommand.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 6bcafe26a373d6de7e25cb28602e5133b2630615d3678d3278363f1c46c6ecc1
+  SHA-256 checksum b4d4b42f70aaa68170b48b6738dcdc3cc00773d7234aba5ebf284df0a80791b3
   Compiled from "CommandLineParser.java"
 class org.gradle.cli.CommandLineParser$AfterFirstSubCommand extends org.gradle.cli.CommandLineParser$OptionAwareParserState
   minor version: 0
   major version: 50
   flags: (0x0020) ACC_SUPER
   this_class: #14                         // org/gradle/cli/CommandLineParser$AfterFirstSubCommand
   super_class: #15                        // org/gradle/cli/CommandLineParser$OptionAwareParserState
@@ -103,17 +103,17 @@
          2: putfield      #2                  // Field this$0:Lorg/gradle/cli/CommandLineParser;
          5: aload_0
          6: aload_1
          7: aload_2
          8: invokespecial #3                  // Method org/gradle/cli/CommandLineParser$OptionAwareParserState."<init>":(Lorg/gradle/cli/CommandLineParser;Lorg/gradle/cli/ParsedCommandLine;)V
         11: return
       LineNumberTable:
-        line 327: 0
-        line 328: 5
-        line 329: 11
+        line 330: 0
+        line 331: 5
+        line 332: 11
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      12     0  this   Lorg/gradle/cli/CommandLineParser$AfterFirstSubCommand;
             0      12     2 commandLine   Lorg/gradle/cli/ParsedCommandLine;
 
   public org.gradle.cli.CommandLineParser$OptionParserState onStartOption(java.lang.String, java.lang.String);
     descriptor: (Ljava/lang/String;Ljava/lang/String;)Lorg/gradle/cli/CommandLineParser$OptionParserState;
@@ -150,18 +150,18 @@
         51: aload_0
         52: getfield      #8                  // Field commandLine:Lorg/gradle/cli/ParsedCommandLine;
         55: aload_0
         56: aconst_null
         57: invokespecial #13                 // Method org/gradle/cli/CommandLineParser$KnownOptionParserState."<init>":(Lorg/gradle/cli/CommandLineParser$OptionString;Lorg/gradle/cli/CommandLineOption;Lorg/gradle/cli/ParsedCommandLine;Lorg/gradle/cli/CommandLineParser$ParserState;Lorg/gradle/cli/CommandLineParser$1;)V
         60: areturn
       LineNumberTable:
-        line 333: 0
-        line 334: 17
-        line 335: 21
-        line 337: 36
+        line 336: 0
+        line 337: 17
+        line 338: 21
+        line 340: 36
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      61     0  this   Lorg/gradle/cli/CommandLineParser$AfterFirstSubCommand;
             0      61     1   arg   Ljava/lang/String;
             0      61     2 option   Ljava/lang/String;
            17      44     3 commandLineOption   Lorg/gradle/cli/CommandLineOption;
       StackMapTable: number_of_entries = 1
@@ -176,15 +176,15 @@
       stack=3, locals=4, args_size=4
          0: aload_0
          1: aload_1
          2: aload_2
          3: invokespecial #1                  // Method "<init>":(Lorg/gradle/cli/CommandLineParser;Lorg/gradle/cli/ParsedCommandLine;)V
          6: return
       LineNumberTable:
-        line 326: 0
+        line 329: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lorg/gradle/cli/CommandLineParser$AfterFirstSubCommand;
             0       7     1    x0   Lorg/gradle/cli/CommandLineParser;
             0       7     2    x1   Lorg/gradle/cli/ParsedCommandLine;
             0       7     3    x2   Lorg/gradle/cli/CommandLineParser$1;
 }
```

#### org/gradle/cli/CommandLineParser$AfterOptions.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 724f01b028a2372e72b042015b46c3e87038edb5bfd287eec300df5f846cd309
+  SHA-256 checksum d32916ae0105fb7f5d5d0eca3764a687347c11e390773748364593f7d012793a
   Compiled from "CommandLineParser.java"
 class org.gradle.cli.CommandLineParser$AfterOptions extends org.gradle.cli.CommandLineParser$ParserState
   minor version: 0
   major version: 50
   flags: (0x0020) ACC_SUPER
   this_class: #7                          // org/gradle/cli/CommandLineParser$AfterOptions
   super_class: #8                         // org/gradle/cli/CommandLineParser$ParserState
@@ -79,31 +79,31 @@
          1: aconst_null
          2: invokespecial #2                  // Method org/gradle/cli/CommandLineParser$ParserState."<init>":(Lorg/gradle/cli/CommandLineParser$1;)V
          5: aload_0
          6: aload_1
          7: putfield      #3                  // Field commandLine:Lorg/gradle/cli/ParsedCommandLine;
         10: return
       LineNumberTable:
-        line 344: 0
-        line 345: 5
-        line 346: 10
+        line 347: 0
+        line 348: 5
+        line 349: 10
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lorg/gradle/cli/CommandLineParser$AfterOptions;
             0      11     1 commandLine   Lorg/gradle/cli/ParsedCommandLine;
 
   public boolean maybeStartOption(java.lang.String);
     descriptor: (Ljava/lang/String;)Z
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=2, args_size=2
          0: iconst_0
          1: ireturn
       LineNumberTable:
-        line 350: 0
+        line 353: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       2     0  this   Lorg/gradle/cli/CommandLineParser$AfterOptions;
             0       2     1   arg   Ljava/lang/String;
 
   public org.gradle.cli.CommandLineParser$OptionParserState onStartOption(java.lang.String, java.lang.String);
     descriptor: (Ljava/lang/String;Ljava/lang/String;)Lorg/gradle/cli/CommandLineParser$OptionParserState;
@@ -116,15 +116,15 @@
          5: aload_0
          6: getfield      #3                  // Field commandLine:Lorg/gradle/cli/ParsedCommandLine;
          9: aload_0
         10: aconst_null
         11: invokespecial #5                  // Method org/gradle/cli/CommandLineParser$UnknownOptionParserState."<init>":(Ljava/lang/String;Lorg/gradle/cli/ParsedCommandLine;Lorg/gradle/cli/CommandLineParser$ParserState;Lorg/gradle/cli/CommandLineParser$1;)V
         14: areturn
       LineNumberTable:
-        line 355: 0
+        line 358: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      15     0  this   Lorg/gradle/cli/CommandLineParser$AfterOptions;
             0      15     1   arg   Ljava/lang/String;
             0      15     2 option   Ljava/lang/String;
 
   public org.gradle.cli.CommandLineParser$ParserState onNonOption(java.lang.String);
@@ -135,16 +135,16 @@
          0: aload_0
          1: getfield      #3                  // Field commandLine:Lorg/gradle/cli/ParsedCommandLine;
          4: aload_1
          5: invokevirtual #6                  // Method org/gradle/cli/ParsedCommandLine.addExtraValue:(Ljava/lang/String;)V
          8: aload_0
          9: areturn
       LineNumberTable:
-        line 360: 0
-        line 361: 8
+        line 363: 0
+        line 364: 8
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lorg/gradle/cli/CommandLineParser$AfterOptions;
             0      10     1   arg   Ljava/lang/String;
 
   org.gradle.cli.CommandLineParser$AfterOptions(org.gradle.cli.ParsedCommandLine, org.gradle.cli.CommandLineParser$1);
     descriptor: (Lorg/gradle/cli/ParsedCommandLine;Lorg/gradle/cli/CommandLineParser$1;)V
@@ -152,15 +152,15 @@
     Code:
       stack=2, locals=3, args_size=3
          0: aload_0
          1: aload_1
          2: invokespecial #1                  // Method "<init>":(Lorg/gradle/cli/ParsedCommandLine;)V
          5: return
       LineNumberTable:
-        line 341: 0
+        line 344: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lorg/gradle/cli/CommandLineParser$AfterOptions;
             0       6     1    x0   Lorg/gradle/cli/ParsedCommandLine;
             0       6     2    x1   Lorg/gradle/cli/CommandLineParser$1;
 }
 SourceFile: "CommandLineParser.java"
```

#### org/gradle/cli/CommandLineParser$BeforeFirstSubCommand.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum eb1e23ab046e96e669ede43f3cf07b6fc97b1ddf183d7f5730ddc167519ea649
+  SHA-256 checksum 2d007405af89f2582eac2d9b3962724bcad324bc95839af7b596057ac3a33268
   Compiled from "CommandLineParser.java"
 class org.gradle.cli.CommandLineParser$BeforeFirstSubCommand extends org.gradle.cli.CommandLineParser$OptionAwareParserState
   minor version: 0
   major version: 50
   flags: (0x0020) ACC_SUPER
   this_class: #20                         // org/gradle/cli/CommandLineParser$BeforeFirstSubCommand
   super_class: #21                        // org/gradle/cli/CommandLineParser$OptionAwareParserState
@@ -124,17 +124,17 @@
          2: putfield      #2                  // Field this$0:Lorg/gradle/cli/CommandLineParser;
          5: aload_0
          6: aload_1
          7: aload_2
          8: invokespecial #3                  // Method org/gradle/cli/CommandLineParser$OptionAwareParserState."<init>":(Lorg/gradle/cli/CommandLineParser;Lorg/gradle/cli/ParsedCommandLine;)V
         11: return
       LineNumberTable:
-        line 307: 0
-        line 308: 5
-        line 309: 11
+        line 310: 0
+        line 311: 5
+        line 312: 11
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      12     0  this   Lorg/gradle/cli/CommandLineParser$BeforeFirstSubCommand;
             0      12     2 commandLine   Lorg/gradle/cli/ParsedCommandLine;
 
   public org.gradle.cli.CommandLineParser$OptionParserState onStartOption(java.lang.String, java.lang.String);
     descriptor: (Ljava/lang/String;Ljava/lang/String;)Lorg/gradle/cli/CommandLineParser$OptionParserState;
@@ -189,21 +189,21 @@
         87: aload_0
         88: getfield      #11                 // Field commandLine:Lorg/gradle/cli/ParsedCommandLine;
         91: aload_0
         92: aconst_null
         93: invokespecial #19                 // Method org/gradle/cli/CommandLineParser$KnownOptionParserState."<init>":(Lorg/gradle/cli/CommandLineParser$OptionString;Lorg/gradle/cli/CommandLineOption;Lorg/gradle/cli/ParsedCommandLine;Lorg/gradle/cli/CommandLineParser$ParserState;Lorg/gradle/cli/CommandLineParser$1;)V
         96: areturn
       LineNumberTable:
-        line 313: 0
-        line 314: 11
-        line 315: 29
-        line 316: 34
-        line 317: 44
-        line 319: 59
-        line 322: 80
+        line 316: 0
+        line 317: 11
+        line 318: 29
+        line 319: 34
+        line 320: 44
+        line 322: 59
+        line 325: 80
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      97     0  this   Lorg/gradle/cli/CommandLineParser$BeforeFirstSubCommand;
             0      97     1   arg   Ljava/lang/String;
             0      97     2 option   Ljava/lang/String;
            11      86     3 optionString   Lorg/gradle/cli/CommandLineParser$OptionString;
            29      68     4 commandLineOption   Lorg/gradle/cli/CommandLineOption;
@@ -220,15 +220,15 @@
       stack=3, locals=4, args_size=4
          0: aload_0
          1: aload_1
          2: aload_2
          3: invokespecial #1                  // Method "<init>":(Lorg/gradle/cli/CommandLineParser;Lorg/gradle/cli/ParsedCommandLine;)V
          6: return
       LineNumberTable:
-        line 306: 0
+        line 309: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lorg/gradle/cli/CommandLineParser$BeforeFirstSubCommand;
             0       7     1    x0   Lorg/gradle/cli/CommandLineParser;
             0       7     2    x1   Lorg/gradle/cli/ParsedCommandLine;
             0       7     3    x2   Lorg/gradle/cli/CommandLineParser$1;
 }
```

#### org/gradle/cli/CommandLineParser$CaseInsensitiveStringComparator.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 0d8eb831b12a91187f01758b57f8b3ca8ed22cffdf2017b59e8b38881eea38a0
+  SHA-256 checksum 628b4d52b24a542c50cd2a11d55566f2a55dfd058079ea6cd092065fcfe4bfe2
   Compiled from "CommandLineParser.java"
 final class org.gradle.cli.CommandLineParser$CaseInsensitiveStringComparator extends java.lang.Object implements java.util.Comparator<java.lang.String>
   minor version: 0
   major version: 50
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #7                          // org/gradle/cli/CommandLineParser$CaseInsensitiveStringComparator
   super_class: #8                         // java/lang/Object
@@ -63,15 +63,15 @@
     flags: (0x0002) ACC_PRIVATE
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #2                  // Method java/lang/Object."<init>":()V
          4: return
       LineNumberTable:
-        line 505: 0
+        line 508: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/gradle/cli/CommandLineParser$CaseInsensitiveStringComparator;
 
   public int compare(java.lang.String, java.lang.String);
     descriptor: (Ljava/lang/String;Ljava/lang/String;)I
     flags: (0x0001) ACC_PUBLIC
@@ -86,18 +86,18 @@
         10: iload_3
         11: ireturn
         12: aload_1
         13: aload_2
         14: invokevirtual #4                  // Method java/lang/String.compareTo:(Ljava/lang/String;)I
         17: ireturn
       LineNumberTable:
-        line 507: 0
-        line 508: 6
-        line 509: 10
-        line 511: 12
+        line 510: 0
+        line 511: 6
+        line 512: 10
+        line 514: 12
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      18     0  this   Lorg/gradle/cli/CommandLineParser$CaseInsensitiveStringComparator;
             0      18     1 option1   Ljava/lang/String;
             0      18     2 option2   Ljava/lang/String;
             6      12     3  diff   I
       StackMapTable: number_of_entries = 1
@@ -114,29 +114,29 @@
          1: aload_1
          2: checkcast     #5                  // class java/lang/String
          5: aload_2
          6: checkcast     #5                  // class java/lang/String
          9: invokevirtual #6                  // Method compare:(Ljava/lang/String;Ljava/lang/String;)I
         12: ireturn
       LineNumberTable:
-        line 505: 0
+        line 508: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lorg/gradle/cli/CommandLineParser$CaseInsensitiveStringComparator;
 
   org.gradle.cli.CommandLineParser$CaseInsensitiveStringComparator(org.gradle.cli.CommandLineParser$1);
     descriptor: (Lorg/gradle/cli/CommandLineParser$1;)V
     flags: (0x1000) ACC_SYNTHETIC
     Code:
       stack=1, locals=2, args_size=2
          0: aload_0
          1: invokespecial #1                  // Method "<init>":()V
          4: return
       LineNumberTable:
-        line 505: 0
+        line 508: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/gradle/cli/CommandLineParser$CaseInsensitiveStringComparator;
             0       5     1    x0   Lorg/gradle/cli/CommandLineParser$1;
 }
 Signature: #33                          // Ljava/lang/Object;Ljava/util/Comparator<Ljava/lang/String;>;
 SourceFile: "CommandLineParser.java"
```

#### org/gradle/cli/CommandLineParser$KnownOptionParserState.class

##### procyon -ec {}

```diff
@@ -42,15 +42,15 @@
     
     public boolean getHasArgument() {
         return this.option.getAllowsArguments();
     }
     
     public CommandLineParser.ParserState onComplete() {
         if (this.getHasArgument() && this.values.isEmpty()) {
-            throw new CommandLineArgumentException(String.format("No argument was provided for command-line option '%s'.", this.optionString));
+            throw new CommandLineArgumentException(String.format("No argument was provided for command-line option '%s' with description: '%s'", this.optionString, this.option.getDescription()));
         }
         final ParsedCommandLineOption parsedOption = this.commandLine.addOption(CommandLineParser.OptionString.access$1400(this.optionString), this.option);
         if (this.values.size() + parsedOption.getValues().size() > 1 && !this.option.getAllowsMultipleArguments()) {
             throw new CommandLineArgumentException(String.format("Multiple arguments were provided for command-line option '%s'.", this.optionString));
         }
         for (final String value : this.values) {
             parsedOption.addArgument(value);
```

#### org/gradle/cli/CommandLineParser$MissingOptionArgState.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum c5f36809c37102d35e140cbba4ba5e7903b2da1f09f58d5f04b4e7f5aef083e8
+  SHA-256 checksum 8ddff9b8f077effde8aeacfa0b907c76ff050bd8c945150f375e18f44e699d1c
   Compiled from "CommandLineParser.java"
 class org.gradle.cli.CommandLineParser$MissingOptionArgState extends org.gradle.cli.CommandLineParser$ParserState
   minor version: 0
   major version: 50
   flags: (0x0020) ACC_SUPER
   this_class: #8                          // org/gradle/cli/CommandLineParser$MissingOptionArgState
   super_class: #9                         // org/gradle/cli/CommandLineParser$ParserState
@@ -80,17 +80,17 @@
          1: aconst_null
          2: invokespecial #2                  // Method org/gradle/cli/CommandLineParser$ParserState."<init>":(Lorg/gradle/cli/CommandLineParser$1;)V
          5: aload_0
          6: aload_1
          7: putfield      #3                  // Field option:Lorg/gradle/cli/CommandLineParser$OptionParserState;
         10: return
       LineNumberTable:
-        line 368: 0
-        line 369: 5
-        line 370: 10
+        line 371: 0
+        line 372: 5
+        line 373: 10
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lorg/gradle/cli/CommandLineParser$MissingOptionArgState;
             0      11     1 option   Lorg/gradle/cli/CommandLineParser$OptionParserState;
 
   public boolean maybeStartOption(java.lang.String);
     descriptor: (Ljava/lang/String;)Z
@@ -98,15 +98,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #4                  // Method isOption:(Ljava/lang/String;)Z
          5: ireturn
       LineNumberTable:
-        line 374: 0
+        line 377: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lorg/gradle/cli/CommandLineParser$MissingOptionArgState;
             0       6     1   arg   Ljava/lang/String;
 
   public org.gradle.cli.CommandLineParser$OptionParserState onStartOption(java.lang.String, java.lang.String);
     descriptor: (Ljava/lang/String;Ljava/lang/String;)Lorg/gradle/cli/CommandLineParser$OptionParserState;
@@ -117,15 +117,15 @@
          1: getfield      #3                  // Field option:Lorg/gradle/cli/CommandLineParser$OptionParserState;
          4: invokevirtual #5                  // Method org/gradle/cli/CommandLineParser$OptionParserState.onComplete:()Lorg/gradle/cli/CommandLineParser$ParserState;
          7: aload_1
          8: aload_2
          9: invokevirtual #6                  // Method org/gradle/cli/CommandLineParser$ParserState.onStartOption:(Ljava/lang/String;Ljava/lang/String;)Lorg/gradle/cli/CommandLineParser$OptionParserState;
         12: areturn
       LineNumberTable:
-        line 379: 0
+        line 382: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lorg/gradle/cli/CommandLineParser$MissingOptionArgState;
             0      13     1   arg   Ljava/lang/String;
             0      13     2 option   Ljava/lang/String;
 
   public org.gradle.cli.CommandLineParser$ParserState onNonOption(java.lang.String);
@@ -135,15 +135,15 @@
       stack=2, locals=2, args_size=2
          0: aload_0
          1: getfield      #3                  // Field option:Lorg/gradle/cli/CommandLineParser$OptionParserState;
          4: aload_1
          5: invokevirtual #7                  // Method org/gradle/cli/CommandLineParser$OptionParserState.onArgument:(Ljava/lang/String;)Lorg/gradle/cli/CommandLineParser$ParserState;
          8: areturn
       LineNumberTable:
-        line 384: 0
+        line 387: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0  this   Lorg/gradle/cli/CommandLineParser$MissingOptionArgState;
             0       9     1   arg   Ljava/lang/String;
 
   public void onCommandLineEnd();
     descriptor: ()V
@@ -152,31 +152,31 @@
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #3                  // Field option:Lorg/gradle/cli/CommandLineParser$OptionParserState;
          4: invokevirtual #5                  // Method org/gradle/cli/CommandLineParser$OptionParserState.onComplete:()Lorg/gradle/cli/CommandLineParser$ParserState;
          7: pop
          8: return
       LineNumberTable:
-        line 389: 0
-        line 390: 8
+        line 392: 0
+        line 393: 8
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0  this   Lorg/gradle/cli/CommandLineParser$MissingOptionArgState;
 
   org.gradle.cli.CommandLineParser$MissingOptionArgState(org.gradle.cli.CommandLineParser$OptionParserState, org.gradle.cli.CommandLineParser$1);
     descriptor: (Lorg/gradle/cli/CommandLineParser$OptionParserState;Lorg/gradle/cli/CommandLineParser$1;)V
     flags: (0x1000) ACC_SYNTHETIC
     Code:
       stack=2, locals=3, args_size=3
          0: aload_0
          1: aload_1
          2: invokespecial #1                  // Method "<init>":(Lorg/gradle/cli/CommandLineParser$OptionParserState;)V
          5: return
       LineNumberTable:
-        line 365: 0
+        line 368: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lorg/gradle/cli/CommandLineParser$MissingOptionArgState;
             0       6     1    x0   Lorg/gradle/cli/CommandLineParser$OptionParserState;
             0       6     2    x1   Lorg/gradle/cli/CommandLineParser$1;
 }
 SourceFile: "CommandLineParser.java"
```

#### org/gradle/cli/CommandLineParser$OptionAwareParserState.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 09c3f264fabef42c6b9bd50c3a13a4fafcb023f9db536a5ef514b1bec6d73086
+  SHA-256 checksum 5ec91b36d9d49cdf384052791063a2d16dd66d239d8bff1c63484e0723a7872f
   Compiled from "CommandLineParser.java"
 abstract class org.gradle.cli.CommandLineParser$OptionAwareParserState extends org.gradle.cli.CommandLineParser$ParserState
   minor version: 0
   major version: 50
   flags: (0x0420) ACC_SUPER, ACC_ABSTRACT
   this_class: #11                         // org/gradle/cli/CommandLineParser$OptionAwareParserState
   super_class: #12                        // org/gradle/cli/CommandLineParser$ParserState
@@ -92,17 +92,17 @@
          6: aconst_null
          7: invokespecial #2                  // Method org/gradle/cli/CommandLineParser$ParserState."<init>":(Lorg/gradle/cli/CommandLineParser$1;)V
         10: aload_0
         11: aload_2
         12: putfield      #3                  // Field commandLine:Lorg/gradle/cli/ParsedCommandLine;
         15: return
       LineNumberTable:
-        line 290: 0
-        line 291: 10
-        line 292: 15
+        line 293: 0
+        line 294: 10
+        line 295: 15
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lorg/gradle/cli/CommandLineParser$OptionAwareParserState;
             0      16     2 commandLine   Lorg/gradle/cli/ParsedCommandLine;
 
   public boolean maybeStartOption(java.lang.String);
     descriptor: (Ljava/lang/String;)Z
@@ -110,15 +110,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #4                  // Method isOption:(Ljava/lang/String;)Z
          5: ireturn
       LineNumberTable:
-        line 296: 0
+        line 299: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lorg/gradle/cli/CommandLineParser$OptionAwareParserState;
             0       6     1   arg   Ljava/lang/String;
 
   public org.gradle.cli.CommandLineParser$ParserState onNonOption(java.lang.String);
     descriptor: (Ljava/lang/String;)Lorg/gradle/cli/CommandLineParser$ParserState;
@@ -146,16 +146,16 @@
         40: dup
         41: aload_0
         42: getfield      #3                  // Field commandLine:Lorg/gradle/cli/ParsedCommandLine;
         45: aconst_null
         46: invokespecial #10                 // Method org/gradle/cli/CommandLineParser$AfterOptions."<init>":(Lorg/gradle/cli/ParsedCommandLine;Lorg/gradle/cli/CommandLineParser$1;)V
         49: areturn
       LineNumberTable:
-        line 301: 0
-        line 302: 8
+        line 304: 0
+        line 305: 8
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      50     0  this   Lorg/gradle/cli/CommandLineParser$OptionAwareParserState;
             0      50     1   arg   Ljava/lang/String;
       StackMapTable: number_of_entries = 2
         frame_type = 37 /* same */
         frame_type = 75 /* same_locals_1_stack_item */
```

#### org/gradle/cli/CommandLineParser$OptionComparator.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 148881256a6d29aa381630809702a9c105f4d27ad4bd2e44fddf966f45af45d9
+  SHA-256 checksum 67230cca5e087e7d60117b6b27a7f05a02b2e54172b29596534eac1f2fbf1467
   Compiled from "CommandLineParser.java"
 final class org.gradle.cli.CommandLineParser$OptionComparator extends java.lang.Object implements java.util.Comparator<org.gradle.cli.CommandLineOption>
   minor version: 0
   major version: 50
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #13                         // org/gradle/cli/CommandLineParser$OptionComparator
   super_class: #14                        // java/lang/Object
@@ -80,15 +80,15 @@
     flags: (0x0002) ACC_PRIVATE
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #2                  // Method java/lang/Object."<init>":()V
          4: return
       LineNumberTable:
-        line 497: 0
+        line 500: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/gradle/cli/CommandLineParser$OptionComparator;
 
   public int compare(org.gradle.cli.CommandLineOption, org.gradle.cli.CommandLineOption);
     descriptor: (Lorg/gradle/cli/CommandLineOption;Lorg/gradle/cli/CommandLineOption;)I
     flags: (0x0001) ACC_PUBLIC
@@ -117,17 +117,17 @@
         43: aconst_null
         44: invokespecial #9                  // Method org/gradle/cli/CommandLineParser$CaseInsensitiveStringComparator."<init>":(Lorg/gradle/cli/CommandLineParser$1;)V
         47: aload_3
         48: aload         4
         50: invokevirtual #10                 // Method org/gradle/cli/CommandLineParser$CaseInsensitiveStringComparator.compare:(Ljava/lang/String;Ljava/lang/String;)I
         53: ireturn
       LineNumberTable:
-        line 499: 0
-        line 500: 19
-        line 501: 39
+        line 502: 0
+        line 503: 19
+        line 504: 39
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      54     0  this   Lorg/gradle/cli/CommandLineParser$OptionComparator;
             0      54     1 option1   Lorg/gradle/cli/CommandLineOption;
             0      54     2 option2   Lorg/gradle/cli/CommandLineOption;
            19      35     3  min1   Ljava/lang/String;
            39      15     4  min2   Ljava/lang/String;
@@ -141,29 +141,29 @@
          1: aload_1
          2: checkcast     #11                 // class org/gradle/cli/CommandLineOption
          5: aload_2
          6: checkcast     #11                 // class org/gradle/cli/CommandLineOption
          9: invokevirtual #12                 // Method compare:(Lorg/gradle/cli/CommandLineOption;Lorg/gradle/cli/CommandLineOption;)I
         12: ireturn
       LineNumberTable:
-        line 497: 0
+        line 500: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lorg/gradle/cli/CommandLineParser$OptionComparator;
 
   org.gradle.cli.CommandLineParser$OptionComparator(org.gradle.cli.CommandLineParser$1);
     descriptor: (Lorg/gradle/cli/CommandLineParser$1;)V
     flags: (0x1000) ACC_SYNTHETIC
     Code:
       stack=1, locals=2, args_size=2
          0: aload_0
          1: invokespecial #1                  // Method "<init>":()V
          4: return
       LineNumberTable:
-        line 497: 0
+        line 500: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/gradle/cli/CommandLineParser$OptionComparator;
             0       5     1    x0   Lorg/gradle/cli/CommandLineParser$1;
 }
 Signature: #39                          // Ljava/lang/Object;Ljava/util/Comparator<Lorg/gradle/cli/CommandLineOption;>;
 SourceFile: "CommandLineParser.java"
```

#### org/gradle/cli/CommandLineParser$OptionParserState.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 95c6bb99f47f60ea88ec4eebc519c736f4bac3b40a28f84f0cb3fa6603c576a1
+  SHA-256 checksum 444746197d31a7624234ef351acbad48ef4fe628242f8df3670b80cc1110480b
   Compiled from "CommandLineParser.java"
 abstract class org.gradle.cli.CommandLineParser$OptionParserState
   minor version: 0
   major version: 50
   flags: (0x0420) ACC_SUPER, ACC_ABSTRACT
   this_class: #3                          // org/gradle/cli/CommandLineParser$OptionParserState
   super_class: #4                         // java/lang/Object
@@ -49,15 +49,15 @@
     flags: (0x0002) ACC_PRIVATE
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #2                  // Method java/lang/Object."<init>":()V
          4: return
       LineNumberTable:
-        line 393: 0
+        line 396: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/gradle/cli/CommandLineParser$OptionParserState;
 
   public abstract org.gradle.cli.CommandLineParser$ParserState onStartNextArg();
     descriptor: ()Lorg/gradle/cli/CommandLineParser$ParserState;
     flags: (0x0401) ACC_PUBLIC, ACC_ABSTRACT
@@ -79,15 +79,15 @@
     flags: (0x1000) ACC_SYNTHETIC
     Code:
       stack=1, locals=2, args_size=2
          0: aload_0
          1: invokespecial #1                  // Method "<init>":()V
          4: return
       LineNumberTable:
-        line 393: 0
+        line 396: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/gradle/cli/CommandLineParser$OptionParserState;
             0       5     1    x0   Lorg/gradle/cli/CommandLineParser$1;
 }
 SourceFile: "CommandLineParser.java"
 InnerClasses:
```

#### org/gradle/cli/CommandLineParser$OptionString.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum d0a4951a7442482709b1b599c956297b8914ba984c612a7bca44b1a0ef0c5e96
+  SHA-256 checksum c37fd012617d02398dada2edaa8d5f94d7a68c80e4b5f7f1a847d2f55ad937c9
   Compiled from "CommandLineParser.java"
 class org.gradle.cli.CommandLineParser$OptionString
   minor version: 0
   major version: 50
   flags: (0x0020) ACC_SUPER
   this_class: #13                         // org/gradle/cli/CommandLineParser$OptionString
   super_class: #14                        // java/lang/Object
@@ -91,18 +91,18 @@
          5: aload_1
          6: putfield      #4                  // Field arg:Ljava/lang/String;
          9: aload_0
         10: aload_2
         11: putfield      #1                  // Field option:Ljava/lang/String;
         14: return
       LineNumberTable:
-        line 257: 0
-        line 258: 4
-        line 259: 9
-        line 260: 14
+        line 260: 0
+        line 261: 4
+        line 262: 9
+        line 263: 14
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      15     0  this   Lorg/gradle/cli/CommandLineParser$OptionString;
             0      15     1   arg   Ljava/lang/String;
             0      15     2 option   Ljava/lang/String;
 
   public java.lang.String getDisplayName();
@@ -132,15 +132,15 @@
         46: invokevirtual #9                  // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         49: aload_0
         50: getfield      #1                  // Field option:Ljava/lang/String;
         53: invokevirtual #9                  // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         56: invokevirtual #10                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
         59: areturn
       LineNumberTable:
-        line 263: 0
+        line 266: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      60     0  this   Lorg/gradle/cli/CommandLineParser$OptionString;
       StackMapTable: number_of_entries = 2
         frame_type = 37 /* same */
         frame_type = 85 /* same_locals_1_stack_item */
           stack = [ class java/lang/String ]
@@ -150,15 +150,15 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokevirtual #12                 // Method getDisplayName:()Ljava/lang/String;
          4: areturn
       LineNumberTable:
-        line 268: 0
+        line 271: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/gradle/cli/CommandLineParser$OptionString;
 
   org.gradle.cli.CommandLineParser$OptionString(java.lang.String, java.lang.String, org.gradle.cli.CommandLineParser$1);
     descriptor: (Ljava/lang/String;Ljava/lang/String;Lorg/gradle/cli/CommandLineParser$1;)V
     flags: (0x1000) ACC_SYNTHETIC
@@ -166,15 +166,15 @@
       stack=3, locals=4, args_size=4
          0: aload_0
          1: aload_1
          2: aload_2
          3: invokespecial #2                  // Method "<init>":(Ljava/lang/String;Ljava/lang/String;)V
          6: return
       LineNumberTable:
-        line 253: 0
+        line 256: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lorg/gradle/cli/CommandLineParser$OptionString;
             0       7     1    x0   Ljava/lang/String;
             0       7     2    x1   Ljava/lang/String;
             0       7     3    x2   Lorg/gradle/cli/CommandLineParser$1;
 
@@ -183,15 +183,15 @@
     flags: (0x1008) ACC_STATIC, ACC_SYNTHETIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #1                  // Field option:Ljava/lang/String;
          4: areturn
       LineNumberTable:
-        line 253: 0
+        line 256: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0    x0   Lorg/gradle/cli/CommandLineParser$OptionString;
 }
 SourceFile: "CommandLineParser.java"
 InnerClasses:
   private static #24= #13 of #53;         // OptionString=class org/gradle/cli/CommandLineParser$OptionString of class org/gradle/cli/CommandLineParser
```

#### org/gradle/cli/CommandLineParser$OptionStringComparator.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 353331d14a47f7d8a17a8954c68d51f440397da9ef9a2e5d2d7c5179c359c471
+  SHA-256 checksum 2d60794b1077bca01bda25b8e404aaa17b1a965164a5d110b5937651af216e04
   Compiled from "CommandLineParser.java"
 final class org.gradle.cli.CommandLineParser$OptionStringComparator extends java.lang.Object implements java.util.Comparator<java.lang.String>
   minor version: 0
   major version: 50
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #9                          // org/gradle/cli/CommandLineParser$OptionStringComparator
   super_class: #10                        // java/lang/Object
@@ -67,15 +67,15 @@
     flags: (0x0002) ACC_PRIVATE
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #2                  // Method java/lang/Object."<init>":()V
          4: return
       LineNumberTable:
-        line 515: 0
+        line 518: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/gradle/cli/CommandLineParser$OptionStringComparator;
 
   public int compare(java.lang.String, java.lang.String);
     descriptor: (Ljava/lang/String;Ljava/lang/String;)I
     flags: (0x0001) ACC_PUBLIC
@@ -114,21 +114,21 @@
         55: aconst_null
         56: invokespecial #5                  // Method org/gradle/cli/CommandLineParser$CaseInsensitiveStringComparator."<init>":(Lorg/gradle/cli/CommandLineParser$1;)V
         59: aload_1
         60: aload_2
         61: invokevirtual #6                  // Method org/gradle/cli/CommandLineParser$CaseInsensitiveStringComparator.compare:(Ljava/lang/String;Ljava/lang/String;)I
         64: ireturn
       LineNumberTable:
-        line 517: 0
-        line 518: 14
-        line 519: 29
-        line 520: 38
-        line 522: 40
-        line 523: 49
-        line 525: 51
+        line 520: 0
+        line 521: 14
+        line 522: 29
+        line 523: 38
+        line 525: 40
+        line 526: 49
+        line 528: 51
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      65     0  this   Lorg/gradle/cli/CommandLineParser$OptionStringComparator;
             0      65     1 option1   Ljava/lang/String;
             0      65     2 option2   Ljava/lang/String;
            14      51     3 short1   Z
            29      36     4 short2   Z
@@ -155,29 +155,29 @@
          1: aload_1
          2: checkcast     #7                  // class java/lang/String
          5: aload_2
          6: checkcast     #7                  // class java/lang/String
          9: invokevirtual #8                  // Method compare:(Ljava/lang/String;Ljava/lang/String;)I
         12: ireturn
       LineNumberTable:
-        line 515: 0
+        line 518: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lorg/gradle/cli/CommandLineParser$OptionStringComparator;
 
   org.gradle.cli.CommandLineParser$OptionStringComparator(org.gradle.cli.CommandLineParser$1);
     descriptor: (Lorg/gradle/cli/CommandLineParser$1;)V
     flags: (0x1000) ACC_SYNTHETIC
     Code:
       stack=1, locals=2, args_size=2
          0: aload_0
          1: invokespecial #1                  // Method "<init>":()V
          4: return
       LineNumberTable:
-        line 515: 0
+        line 518: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/gradle/cli/CommandLineParser$OptionStringComparator;
             0       5     1    x0   Lorg/gradle/cli/CommandLineParser$1;
 }
 Signature: #36                          // Ljava/lang/Object;Ljava/util/Comparator<Ljava/lang/String;>;
 SourceFile: "CommandLineParser.java"
```

#### org/gradle/cli/CommandLineParser$ParserState.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum d55198e9ae1b97a3588ab6a2c3608b1670996a6bda068a6e8b25ede31c4a05e3
+  SHA-256 checksum 04f88d8d4a14f3543d1cca3850316ecb7ff7e8219cb67865141b5bb186d172c9
   Compiled from "CommandLineParser.java"
 abstract class org.gradle.cli.CommandLineParser$ParserState
   minor version: 0
   major version: 50
   flags: (0x0420) ACC_SUPER, ACC_ABSTRACT
   this_class: #5                          // org/gradle/cli/CommandLineParser$ParserState
   super_class: #6                         // java/lang/Object
@@ -59,15 +59,15 @@
     flags: (0x0002) ACC_PRIVATE
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #2                  // Method java/lang/Object."<init>":()V
          4: return
       LineNumberTable:
-        line 272: 0
+        line 275: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/gradle/cli/CommandLineParser$ParserState;
 
   public abstract boolean maybeStartOption(java.lang.String);
     descriptor: (Ljava/lang/String;)Z
     flags: (0x0401) ACC_PUBLIC, ACC_ABSTRACT
@@ -78,15 +78,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_1
          1: ldc           #3                  // String (?s)-.+
          3: invokevirtual #4                  // Method java/lang/String.matches:(Ljava/lang/String;)Z
          6: ireturn
       LineNumberTable:
-        line 276: 0
+        line 279: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lorg/gradle/cli/CommandLineParser$ParserState;
             0       7     1   arg   Ljava/lang/String;
 
   public abstract org.gradle.cli.CommandLineParser$OptionParserState onStartOption(java.lang.String, java.lang.String);
     descriptor: (Ljava/lang/String;Ljava/lang/String;)Lorg/gradle/cli/CommandLineParser$OptionParserState;
@@ -99,29 +99,29 @@
   public void onCommandLineEnd();
     descriptor: ()V
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=0, locals=1, args_size=1
          0: return
       LineNumberTable:
-        line 284: 0
+        line 287: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       1     0  this   Lorg/gradle/cli/CommandLineParser$ParserState;
 
   org.gradle.cli.CommandLineParser$ParserState(org.gradle.cli.CommandLineParser$1);
     descriptor: (Lorg/gradle/cli/CommandLineParser$1;)V
     flags: (0x1000) ACC_SYNTHETIC
     Code:
       stack=1, locals=2, args_size=2
          0: aload_0
          1: invokespecial #1                  // Method "<init>":()V
          4: return
       LineNumberTable:
-        line 272: 0
+        line 275: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/gradle/cli/CommandLineParser$ParserState;
             0       5     1    x0   Lorg/gradle/cli/CommandLineParser$1;
 }
 SourceFile: "CommandLineParser.java"
 InnerClasses:
```

#### org/gradle/cli/CommandLineParser$UnknownOptionParserState.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum ae37fa564f99da515cf8ebf49f0af0d256f53aa62c0ea5f563bcc79fbf7a9b29
+  SHA-256 checksum 47ba15647c27f0174e97486fd6fd8ab4ef19ee71020228c6b127edc9404ea082
   Compiled from "CommandLineParser.java"
 class org.gradle.cli.CommandLineParser$UnknownOptionParserState extends org.gradle.cli.CommandLineParser$OptionParserState
   minor version: 0
   major version: 50
   flags: (0x0020) ACC_SUPER
   this_class: #8                          // org/gradle/cli/CommandLineParser$UnknownOptionParserState
   super_class: #9                         // org/gradle/cli/CommandLineParser$OptionParserState
@@ -98,19 +98,19 @@
         11: aload_2
         12: putfield      #4                  // Field commandLine:Lorg/gradle/cli/ParsedCommandLine;
         15: aload_0
         16: aload_3
         17: putfield      #5                  // Field state:Lorg/gradle/cli/CommandLineParser$ParserState;
         20: return
       LineNumberTable:
-        line 469: 0
-        line 470: 5
-        line 471: 10
-        line 472: 15
-        line 473: 20
+        line 472: 0
+        line 473: 5
+        line 474: 10
+        line 475: 15
+        line 476: 20
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      21     0  this   Lorg/gradle/cli/CommandLineParser$UnknownOptionParserState;
             0      21     1   arg   Ljava/lang/String;
             0      21     2 commandLine   Lorg/gradle/cli/ParsedCommandLine;
             0      21     3 state   Lorg/gradle/cli/CommandLineParser$ParserState;
 
@@ -118,43 +118,43 @@
     descriptor: ()Z
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: iconst_1
          1: ireturn
       LineNumberTable:
-        line 477: 0
+        line 480: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       2     0  this   Lorg/gradle/cli/CommandLineParser$UnknownOptionParserState;
 
   public org.gradle.cli.CommandLineParser$ParserState onStartNextArg();
     descriptor: ()Lorg/gradle/cli/CommandLineParser$ParserState;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokevirtual #6                  // Method onComplete:()Lorg/gradle/cli/CommandLineParser$ParserState;
          4: areturn
       LineNumberTable:
-        line 482: 0
+        line 485: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/gradle/cli/CommandLineParser$UnknownOptionParserState;
 
   public org.gradle.cli.CommandLineParser$ParserState onArgument(java.lang.String);
     descriptor: (Ljava/lang/String;)Lorg/gradle/cli/CommandLineParser$ParserState;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=2, args_size=2
          0: aload_0
          1: invokevirtual #6                  // Method onComplete:()Lorg/gradle/cli/CommandLineParser$ParserState;
          4: areturn
       LineNumberTable:
-        line 487: 0
+        line 490: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/gradle/cli/CommandLineParser$UnknownOptionParserState;
             0       5     1 argument   Ljava/lang/String;
 
   public org.gradle.cli.CommandLineParser$ParserState onComplete();
     descriptor: ()Lorg/gradle/cli/CommandLineParser$ParserState;
@@ -166,16 +166,16 @@
          4: aload_0
          5: getfield      #3                  // Field arg:Ljava/lang/String;
          8: invokevirtual #7                  // Method org/gradle/cli/ParsedCommandLine.addExtraValue:(Ljava/lang/String;)V
         11: aload_0
         12: getfield      #5                  // Field state:Lorg/gradle/cli/CommandLineParser$ParserState;
         15: areturn
       LineNumberTable:
-        line 492: 0
-        line 493: 11
+        line 495: 0
+        line 496: 11
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lorg/gradle/cli/CommandLineParser$UnknownOptionParserState;
 
   org.gradle.cli.CommandLineParser$UnknownOptionParserState(java.lang.String, org.gradle.cli.ParsedCommandLine, org.gradle.cli.CommandLineParser$ParserState, org.gradle.cli.CommandLineParser$1);
     descriptor: (Ljava/lang/String;Lorg/gradle/cli/ParsedCommandLine;Lorg/gradle/cli/CommandLineParser$ParserState;Lorg/gradle/cli/CommandLineParser$1;)V
     flags: (0x1000) ACC_SYNTHETIC
@@ -184,15 +184,15 @@
          0: aload_0
          1: aload_1
          2: aload_2
          3: aload_3
          4: invokespecial #1                  // Method "<init>":(Ljava/lang/String;Lorg/gradle/cli/ParsedCommandLine;Lorg/gradle/cli/CommandLineParser$ParserState;)V
          7: return
       LineNumberTable:
-        line 464: 0
+        line 467: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       8     0  this   Lorg/gradle/cli/CommandLineParser$UnknownOptionParserState;
             0       8     1    x0   Ljava/lang/String;
             0       8     2    x1   Lorg/gradle/cli/ParsedCommandLine;
             0       8     3    x2   Lorg/gradle/cli/CommandLineParser$ParserState;
             0       8     4    x3   Lorg/gradle/cli/CommandLineParser$1;
```

#### org/gradle/cli/CommandLineParser.class

##### procyon -ec {}

```diff
@@ -135,14 +135,15 @@
             final String key = join(prefixedStrings, ", ");
             String value = option.getDescription();
             if (value == null || value.length() == 0) {
                 value = "";
             }
             lines.put(key, value);
         }
+        lines.put("--", "Signals the end of built-in options. Gradle parses subsequent parameters as only tasks or task options.");
         int max = 0;
         for (final String optionStr : lines.keySet()) {
             max = Math.max(max, optionStr.length());
         }
         for (final Map.Entry<String, String> entry : lines.entrySet()) {
             if (((String)entry.getValue()).length() == 0) {
                 formatter.format("%s%n", entry.getKey());
```

#### org/gradle/util/internal/ZipSlip.class

##### procyon -ec {}

```diff
@@ -9,14 +9,18 @@
         if (isUnsafeZipEntryName(name)) {
             throw new IllegalArgumentException(String.format("'%s' is not a safe zip entry name.", name));
         }
         return name;
     }
     
     public static boolean isUnsafeZipEntryName(final String name) {
-        return name.isEmpty() || name.startsWith("/") || name.startsWith("\\") || name.contains("..") || (name.contains(":") && isWindows());
+        return name.isEmpty() || name.startsWith("/") || name.startsWith("\\") || containsDirectoryNavigation(name) || (name.contains(":") && isWindows());
+    }
+    
+    private static boolean containsDirectoryNavigation(final String name) {
+        return name.contains("..") && (name.endsWith("\\..") || name.contains("..\\") || name.endsWith("/..") || name.contains("../"));
     }
     
     private static boolean isWindows() {
         return System.getProperty("os.name").toLowerCase(Locale.US).contains("windows");
     }
 }
```

#### org/gradle/wrapper/BootstrapMainStarter$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 84748f2bfb89f0d8b532ebd8db4dd2e74583f16c670b88face4939122e90c0d3
+  SHA-256 checksum 6da055435f3cbb07162ff92af2c7d710bd62524cb1c830872c71d2fbc3876757
   Compiled from "BootstrapMainStarter.java"
 class org.gradle.wrapper.BootstrapMainStarter$1 implements java.io.FilenameFilter
   minor version: 0
   major version: 50
   flags: (0x0020) ACC_SUPER
   this_class: #4                          // org/gradle/wrapper/BootstrapMainStarter$1
   super_class: #5                         // java/lang/Object
@@ -52,30 +52,30 @@
     flags: (0x0000)
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method java/lang/Object."<init>":()V
          4: return
       LineNumberTable:
-        line 44: 0
+        line 42: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lorg/gradle/wrapper/BootstrapMainStarter$1;
 
   public boolean accept(java.io.File, java.lang.String);
     descriptor: (Ljava/io/File;Ljava/lang/String;)Z
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=2, locals=3, args_size=3
          0: aload_2
          1: ldc           #2                  // String gradle-launcher-.*\\.jar
          3: invokevirtual #3                  // Method java/lang/String.matches:(Ljava/lang/String;)Z
          6: ireturn
       LineNumberTable:
-        line 47: 0
+        line 45: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lorg/gradle/wrapper/BootstrapMainStarter$1;
             0       7     1   dir   Ljava/io/File;
             0       7     2  name   Ljava/lang/String;
 }
 SourceFile: "BootstrapMainStarter.java"
```

#### org/gradle/wrapper/BootstrapMainStarter.class

##### procyon -ec {}

```diff
@@ -1,13 +1,12 @@
 
 package org.gradle.wrapper;
 
 import java.io.FilenameFilter;
 import java.lang.reflect.Method;
-import java.io.Closeable;
 import java.net.URLClassLoader;
 import java.net.URL;
 import java.io.File;
 
 public class BootstrapMainStarter
 {
     public void start(final String[] args, final File gradleHome) throws Exception {
@@ -16,17 +15,15 @@
             throw new RuntimeException(String.format("Could not locate the Gradle launcher JAR in Gradle distribution '%s'.", gradleHome));
         }
         final URLClassLoader contextClassLoader = new URLClassLoader(new URL[] { gradleJar.toURI().toURL() }, ClassLoader.getSystemClassLoader().getParent());
         Thread.currentThread().setContextClassLoader(contextClassLoader);
         final Class<?> mainClass = contextClassLoader.loadClass("org.gradle.launcher.GradleMain");
         final Method mainMethod = mainClass.getMethod("main", String[].class);
         mainMethod.invoke(null, args);
-        if (contextClassLoader instanceof Closeable) {
-            contextClassLoader.close();
-        }
+        contextClassLoader.close();
     }
     
     static File findLauncherJar(final File gradleHome) {
         final File libDirectory = new File(gradleHome, "lib");
         if (libDirectory.exists() && libDirectory.isDirectory()) {
             final File[] launcherJars = libDirectory.listFiles((FilenameFilter)new BootstrapMainStarter.BootstrapMainStarter$1());
             if (launcherJars != null && launcherJars.length == 1) {
```

#### org/gradle/wrapper/Download$DefaultDownloadProgressListener.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum bd63b87e52bcd477fca7834c2d4ee9dea7d6a3a55ea6681a6b7f7adeb4502d50
+  SHA-256 checksum e0200d282621d088a9c45fd5a0094512010b2444e28adb126f3d6ed92169abde
   Compiled from "Download.java"
 class org.gradle.wrapper.Download$DefaultDownloadProgressListener implements org.gradle.wrapper.DownloadProgressListener
   minor version: 0
   major version: 50
   flags: (0x0020) ACC_SUPER
   this_class: #19                         // org/gradle/wrapper/Download$DefaultDownloadProgressListener
   super_class: #20                        // java/lang/Object
@@ -128,19 +128,19 @@
         10: aload_2
         11: putfield      #3                  // Field delegate:Lorg/gradle/wrapper/DownloadProgressListener;
         14: aload_0
         15: iconst_0
         16: putfield      #4                  // Field previousDownloadPercent:I
         19: return
       LineNumberTable:
-        line 231: 0
-        line 232: 4
-        line 233: 9
-        line 234: 14
-        line 235: 19
+        line 240: 0
+        line 241: 4
+        line 242: 9
+        line 243: 14
+        line 244: 19
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      20     0  this   Lorg/gradle/wrapper/Download$DefaultDownloadProgressListener;
             0      20     1 logger   Lorg/gradle/wrapper/Logger;
             0      20     2 delegate   Lorg/gradle/wrapper/DownloadProgressListener;
 
   public void downloadStatusChanged(java.net.URI, long, long);
@@ -175,21 +175,21 @@
         45: getfield      #3                  // Field delegate:Lorg/gradle/wrapper/DownloadProgressListener;
         48: aload_1
         49: lload_2
         50: lload         4
         52: invokeinterface #8,  6            // InterfaceMethod org/gradle/wrapper/DownloadProgressListener.downloadStatusChanged:(Ljava/net/URI;JJ)V
         57: return
       LineNumberTable:
-        line 240: 0
-        line 241: 13
-        line 244: 20
-        line 245: 27
-        line 248: 37
-        line 249: 44
-        line 251: 57
+        line 249: 0
+        line 250: 13
+        line 253: 20
+        line 254: 27
+        line 257: 37
+        line 258: 44
+        line 260: 57
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      58     0  this   Lorg/gradle/wrapper/Download$DefaultDownloadProgressListener;
             0      58     1 address   Ljava/net/URI;
             0      58     2 contentLength   J
             0      58     4 downloaded   J
       StackMapTable: number_of_entries = 3
@@ -236,22 +236,22 @@
         65: invokespecial #14                 // Method java/lang/RuntimeException."<init>":(Ljava/lang/Throwable;)V
         68: athrow
         69: return
       Exception table:
          from    to  target type
              0    54    57   Class java/io/IOException
       LineNumberTable:
-        line 255: 0
-        line 256: 14
-        line 257: 28
-        line 258: 48
-        line 262: 54
-        line 260: 57
-        line 261: 59
-        line 263: 69
+        line 264: 0
+        line 265: 14
+        line 266: 28
+        line 267: 48
+        line 271: 54
+        line 269: 57
+        line 270: 59
+        line 272: 69
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            14      40     5 currentDownloadPercent   I
            59      10     5     e   Ljava/io/IOException;
             0      70     0  this   Lorg/gradle/wrapper/Download$DefaultDownloadProgressListener;
             0      70     1 contentLength   J
             0      70     3 downloaded   J
@@ -276,15 +276,15 @@
          8: ldc2_w        #15                 // double 100.0d
         11: dmul
         12: d2i
         13: invokestatic  #17                 // Method java/lang/Math.max:(II)I
         16: invokestatic  #18                 // Method java/lang/Math.min:(II)I
         19: ireturn
       LineNumberTable:
-        line 266: 0
+        line 275: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      20     0  this   Lorg/gradle/wrapper/Download$DefaultDownloadProgressListener;
             0      20     1 totalLength   J
             0      20     3 downloadedLength   J
 }
 SourceFile: "Download.java"
```

#### org/gradle/wrapper/Download$ProxyAuthenticator.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 3b6be845e87c2d0672f437969bbf8c379f4c76533fb9efe637b46eead7e0ba59
+  SHA-256 checksum 58bd975d6fb7bcd634c0fe3bf9d2f941255f8da482cc811157a3c09b94b5f048
   Compiled from "Download.java"
 class org.gradle.wrapper.Download$ProxyAuthenticator extends java.net.Authenticator
   minor version: 0
   major version: 50
   flags: (0x0020) ACC_SUPER
   this_class: #22                         // org/gradle/wrapper/Download$ProxyAuthenticator
   super_class: #23                        // java/net/Authenticator
@@ -120,15 +120,15 @@
          0: aload_0
          1: aload_1
          2: putfield      #2                  // Field this$0:Lorg/gradle/wrapper/Download;
          5: aload_0
          6: invokespecial #3                  // Method java/net/Authenticator."<init>":()V
          9: return
       LineNumberTable:
-        line 206: 0
+        line 215: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lorg/gradle/wrapper/Download$ProxyAuthenticator;
 
   protected java.net.PasswordAuthentication getPasswordAuthentication();
     descriptor: ()Ljava/net/PasswordAuthentication;
     flags: (0x0004) ACC_PROTECTED
@@ -183,23 +183,23 @@
        105: invokevirtual #19                 // Method java/lang/String.toCharArray:()[C
        108: invokespecial #20                 // Method java/net/PasswordAuthentication."<init>":(Ljava/lang/String;[C)V
        111: areturn
        112: aload_0
        113: invokespecial #21                 // Method java/net/Authenticator.getPasswordAuthentication:()Ljava/net/PasswordAuthentication;
        116: areturn
       LineNumberTable:
-        line 209: 0
-        line 211: 10
-        line 212: 18
-        line 213: 53
-        line 214: 57
-        line 215: 92
-        line 216: 96
-        line 218: 99
-        line 222: 112
+        line 218: 0
+        line 220: 10
+        line 221: 18
+        line 222: 53
+        line 223: 57
+        line 224: 92
+        line 225: 96
+        line 227: 99
+        line 231: 112
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            92      20     3 proxyPassword   Ljava/lang/String;
            18      94     1 protocol   Ljava/lang/String;
            53      59     2 proxyUser   Ljava/lang/String;
             0     117     0  this   Lorg/gradle/wrapper/Download$ProxyAuthenticator;
       StackMapTable: number_of_entries = 2
@@ -215,15 +215,15 @@
     Code:
       stack=2, locals=3, args_size=3
          0: aload_0
          1: aload_1
          2: invokespecial #1                  // Method "<init>":(Lorg/gradle/wrapper/Download;)V
          5: return
       LineNumberTable:
-        line 206: 0
+        line 215: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lorg/gradle/wrapper/Download$ProxyAuthenticator;
             0       6     1    x0   Lorg/gradle/wrapper/Download;
             0       6     2    x1   Lorg/gradle/wrapper/Download$1;
 }
 SourceFile: "Download.java"
```

#### org/gradle/wrapper/Download.class

##### procyon -ec {}

```diff
@@ -18,42 +18,51 @@
 import java.util.HashMap;
 import java.util.Properties;
 import java.util.Map;
 
 public class Download implements IDownload
 {
     public static final String UNKNOWN_VERSION = "0";
+    public static final int DEFAULT_NETWORK_TIMEOUT_MILLISECONDS = 10000;
     private static final int BUFFER_SIZE = 10240;
     private static final int PROGRESS_CHUNK = 1048576;
-    private static final int CONNECTION_TIMEOUT_MILLISECONDS = 10000;
-    private static final int READ_TIMEOUT_MILLISECONDS = 10000;
     private final Logger logger;
     private final String appName;
     private final String appVersion;
     private final DownloadProgressListener progressListener;
     private final Map<String, String> systemProperties;
+    private final int networkTimeout;
     
     public Download(final Logger logger, final String appName, final String appVersion) {
         this(logger, null, appName, appVersion, convertSystemProperties(System.getProperties()));
     }
     
+    public Download(final Logger logger, final String appName, final String appVersion, final int networkTimeout) {
+        this(logger, null, appName, appVersion, convertSystemProperties(System.getProperties()), networkTimeout);
+    }
+    
     private static Map<String, String> convertSystemProperties(final Properties properties) {
         final Map<String, String> result = new HashMap<String, String>();
         for (final Map.Entry<Object, Object> entry : properties.entrySet()) {
             result.put(entry.getKey().toString(), (entry.getValue() == null) ? null : entry.getValue().toString());
         }
         return result;
     }
     
     public Download(final Logger logger, final DownloadProgressListener progressListener, final String appName, final String appVersion, final Map<String, String> systemProperties) {
+        this(logger, progressListener, appName, appVersion, systemProperties, 10000);
+    }
+    
+    public Download(final Logger logger, final DownloadProgressListener progressListener, final String appName, final String appVersion, final Map<String, String> systemProperties, final int networkTimeout) {
         this.logger = logger;
         this.appName = appName;
         this.appVersion = appVersion;
         this.systemProperties = systemProperties;
         this.progressListener = (DownloadProgressListener)new Download.DefaultDownloadProgressListener(logger, progressListener);
+        this.networkTimeout = networkTimeout;
         this.configureProxyAuthentication();
     }
     
     private void configureProxyAuthentication() {
         if (this.systemProperties.get("http.proxyUser") != null || this.systemProperties.get("https.proxyUser") != null) {
             Authenticator.setDefault((Authenticator)new Download.ProxyAuthenticator(this, (Download.Download$1)null));
         }
@@ -70,16 +79,16 @@
         final URL safeUrl = safeUri(address).toURL();
         try {
             out = new BufferedOutputStream(new FileOutputStream(destination));
             final URLConnection conn = safeUrl.openConnection();
             this.addBasicAuthentication(address, conn);
             final String userAgentValue = this.calculateUserAgent();
             conn.setRequestProperty("User-Agent", userAgentValue);
-            conn.setConnectTimeout(10000);
-            conn.setReadTimeout(10000);
+            conn.setConnectTimeout(this.networkTimeout);
+            conn.setReadTimeout(this.networkTimeout);
             in = conn.getInputStream();
             final byte[] buffer = new byte[10240];
             final int totalLength = conn.getContentLength();
             long downloadedLength = 0L;
             long progressCounter = 0L;
             int numRead;
             while ((numRead = in.read(buffer)) != -1) {
@@ -92,15 +101,15 @@
                     progressCounter -= 1048576L;
                     this.progressListener.downloadStatusChanged(address, (long)totalLength, downloadedLength);
                 }
                 out.write(buffer, 0, numRead);
             }
         }
         catch (final SocketTimeoutException e) {
-            throw new IOException("Downloading from " + safeUrl + " failed: timeout", e);
+            throw new IOException("Downloading from " + safeUrl + " failed: timeout (" + this.networkTimeout + "ms)", e);
         }
         finally {
             this.logger.log("");
             if (in != null) {
                 in.close();
             }
             if (out != null) {
```

#### org/gradle/wrapper/Install$1.class

##### procyon -ec {}

```diff
@@ -43,12 +43,13 @@
             Install.access$400(this.this$0).log("Reason: " + e.getMessage());
             throw e;
         }
         final Install.InstallCheck installCheck2 = Install.access$000(this.this$0, this.val$distDir, safeDistributionUrl.toString());
         if (Install.InstallCheck.access$100(installCheck2)) {
             Install.access$1000(this.this$0, Install.InstallCheck.access$200(installCheck2));
             markerFile.createNewFile();
+            this.val$localZipFile.delete();
             return Install.InstallCheck.access$200(installCheck2);
         }
         throw new RuntimeException(Install.InstallCheck.access$300(installCheck2));
     }
 }
```

#### org/gradle/wrapper/Install$InstallCheck.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 8a84f8295706c87c211756011c3c9a9de9f194ad7c3a71a959b829cb9bf594d0
+  SHA-256 checksum 4a8ae492423face8eb2a1a2ad3df38ca75664632f3b83b6af4e9cfed04155198
   Compiled from "Install.java"
 class org.gradle.wrapper.Install$InstallCheck
   minor version: 0
   major version: 50
   flags: (0x0020) ACC_SUPER
   this_class: #6                          // org/gradle/wrapper/Install$InstallCheck
   super_class: #9                         // java/lang/Object
@@ -78,15 +78,15 @@
          0: new           #6                  // class org/gradle/wrapper/Install$InstallCheck
          3: dup
          4: aconst_null
          5: aload_0
          6: invokespecial #7                  // Method "<init>":(Ljava/io/File;Ljava/lang/String;)V
          9: areturn
       LineNumberTable:
-        line 292: 0
+        line 293: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0 message   Ljava/lang/String;
 
   private static org.gradle.wrapper.Install$InstallCheck success(java.io.File);
     descriptor: (Ljava/io/File;)Lorg/gradle/wrapper/Install$InstallCheck;
     flags: (0x000a) ACC_PRIVATE, ACC_STATIC
@@ -95,15 +95,15 @@
          0: new           #6                  // class org/gradle/wrapper/Install$InstallCheck
          3: dup
          4: aload_0
          5: aconst_null
          6: invokespecial #7                  // Method "<init>":(Ljava/io/File;Ljava/lang/String;)V
          9: areturn
       LineNumberTable:
-        line 296: 0
+        line 297: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0 gradleHome   Ljava/io/File;
 
   private org.gradle.wrapper.Install$InstallCheck(java.io.File, java.lang.String);
     descriptor: (Ljava/io/File;Ljava/lang/String;)V
     flags: (0x0002) ACC_PRIVATE
@@ -115,18 +115,18 @@
          5: aload_1
          6: putfield      #4                  // Field gradleHome:Ljava/io/File;
          9: aload_0
         10: aload_2
         11: putfield      #3                  // Field failureMessage:Ljava/lang/String;
         14: return
       LineNumberTable:
-        line 299: 0
-        line 300: 4
-        line 301: 9
-        line 302: 14
+        line 300: 0
+        line 301: 4
+        line 302: 9
+        line 303: 14
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      15     0  this   Lorg/gradle/wrapper/Install$InstallCheck;
             0      15     1 gradleHome   Ljava/io/File;
             0      15     2 failureMessage   Ljava/lang/String;
 
   private boolean isVerified();
@@ -138,15 +138,15 @@
          1: getfield      #4                  // Field gradleHome:Ljava/io/File;
          4: ifnull        11
          7: iconst_1
          8: goto          12
         11: iconst_0
         12: ireturn
       LineNumberTable:
-        line 305: 0
+        line 306: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lorg/gradle/wrapper/Install$InstallCheck;
       StackMapTable: number_of_entries = 2
         frame_type = 11 /* same */
         frame_type = 64 /* same_locals_1_stack_item */
           stack = [ int ]
@@ -156,71 +156,71 @@
     flags: (0x1008) ACC_STATIC, ACC_SYNTHETIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #5                  // Method isVerified:()Z
          4: ireturn
       LineNumberTable:
-        line 287: 0
+        line 288: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0    x0   Lorg/gradle/wrapper/Install$InstallCheck;
 
   static java.io.File access$200(org.gradle.wrapper.Install$InstallCheck);
     descriptor: (Lorg/gradle/wrapper/Install$InstallCheck;)Ljava/io/File;
     flags: (0x1008) ACC_STATIC, ACC_SYNTHETIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #4                  // Field gradleHome:Ljava/io/File;
          4: areturn
       LineNumberTable:
-        line 287: 0
+        line 288: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0    x0   Lorg/gradle/wrapper/Install$InstallCheck;
 
   static java.lang.String access$300(org.gradle.wrapper.Install$InstallCheck);
     descriptor: (Lorg/gradle/wrapper/Install$InstallCheck;)Ljava/lang/String;
     flags: (0x1008) ACC_STATIC, ACC_SYNTHETIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #3                  // Field failureMessage:Ljava/lang/String;
          4: areturn
       LineNumberTable:
-        line 287: 0
+        line 288: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0    x0   Lorg/gradle/wrapper/Install$InstallCheck;
 
   static org.gradle.wrapper.Install$InstallCheck access$1100(java.lang.String);
     descriptor: (Ljava/lang/String;)Lorg/gradle/wrapper/Install$InstallCheck;
     flags: (0x1008) ACC_STATIC, ACC_SYNTHETIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokestatic  #2                  // Method failure:(Ljava/lang/String;)Lorg/gradle/wrapper/Install$InstallCheck;
          4: areturn
       LineNumberTable:
-        line 287: 0
+        line 288: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0    x0   Ljava/lang/String;
 
   static org.gradle.wrapper.Install$InstallCheck access$1200(java.io.File);
     descriptor: (Ljava/io/File;)Lorg/gradle/wrapper/Install$InstallCheck;
     flags: (0x1008) ACC_STATIC, ACC_SYNTHETIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokestatic  #1                  // Method success:(Ljava/io/File;)Lorg/gradle/wrapper/Install$InstallCheck;
          4: areturn
       LineNumberTable:
-        line 287: 0
+        line 288: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0    x0   Ljava/io/File;
 }
 SourceFile: "Install.java"
 InnerClasses:
   private static #15= #6 of #47;          // InstallCheck=class org/gradle/wrapper/Install$InstallCheck of class org/gradle/wrapper/Install
```

#### org/gradle/wrapper/Install.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 192dd3b30cdbc33a3500899d630fa65ba9a246cfdac65a66d0189273995ef849
+  SHA-256 checksum d821e204171825da49d0d9a6fe13c49997ed92a6ce2f9f261a50ef935beb22fa
   Compiled from "Install.java"
 public class org.gradle.wrapper.Install
   minor version: 0
   major version: 50
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #123                        // org/gradle/wrapper/Install
   super_class: #41                        // java/lang/Object
@@ -707,35 +707,35 @@
        145: invokevirtual #38                 // Method java/lang/StringBuffer.toString:()Ljava/lang/String;
        148: areturn
       Exception table:
          from    to  target type
             15    56    63   any
             63    65    63   any
       LineNumberTable:
-        line 117: 0
-        line 118: 6
-        line 120: 15
-        line 121: 18
-        line 122: 25
-        line 123: 31
-        line 124: 39
-        line 125: 44
-        line 129: 56
-        line 130: 60
-        line 129: 63
-        line 130: 69
-        line 132: 72
-        line 133: 78
-        line 134: 87
-        line 135: 98
-        line 136: 112
-        line 137: 121
-        line 139: 129
-        line 134: 137
-        line 142: 143
+        line 118: 0
+        line 119: 6
+        line 121: 15
+        line 122: 18
+        line 123: 25
+        line 124: 31
+        line 125: 39
+        line 126: 44
+        line 130: 56
+        line 131: 60
+        line 130: 63
+        line 131: 69
+        line 133: 72
+        line 134: 78
+        line 135: 87
+        line 136: 98
+        line 137: 112
+        line 138: 121
+        line 140: 129
+        line 135: 137
+        line 143: 143
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            18      38     4     n   I
            25      31     5 buffer   [B
           112      25     7   hex   Ljava/lang/String;
            90      53     6     i   I
             0     149     0  this   Lorg/gradle/wrapper/Install;
@@ -819,23 +819,23 @@
         89: invokestatic  #42                 // Method java/lang/String.format:(Ljava/lang/String;[Ljava/lang/Object;)Ljava/lang/String;
         92: invokestatic  #43                 // Method org/gradle/wrapper/Install$InstallCheck.access$1100:(Ljava/lang/String;)Lorg/gradle/wrapper/Install$InstallCheck;
         95: areturn
         96: aload         4
         98: invokestatic  #49                 // Method org/gradle/wrapper/Install$InstallCheck.access$1200:(Ljava/io/File;)Lorg/gradle/wrapper/Install$InstallCheck;
        101: areturn
       LineNumberTable:
-        line 146: 0
-        line 147: 6
-        line 148: 15
-        line 150: 32
-        line 151: 42
-        line 154: 59
-        line 155: 71
-        line 156: 79
-        line 158: 96
+        line 147: 0
+        line 148: 6
+        line 149: 15
+        line 151: 32
+        line 152: 42
+        line 155: 59
+        line 156: 71
+        line 157: 79
+        line 159: 96
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0     102     0  this   Lorg/gradle/wrapper/Install;
             0     102     1 distDir   Ljava/io/File;
             0     102     2 distributionDescription   Ljava/lang/String;
             6      96     3  dirs   Ljava/util/List;
            71      31     4 gradleHome   Ljava/io/File;
@@ -894,23 +894,23 @@
         56: new           #55                 // class java/lang/RuntimeException
         59: dup
         60: aload         5
         62: invokespecial #56                 // Method java/lang/RuntimeException."<init>":(Ljava/lang/String;)V
         65: athrow
         66: return
       LineNumberTable:
-        line 162: 0
-        line 164: 4
-        line 165: 11
-        line 166: 20
-        line 167: 25
-        line 176: 38
-        line 167: 51
-        line 178: 56
-        line 181: 66
+        line 163: 0
+        line 165: 4
+        line 166: 11
+        line 167: 20
+        line 168: 25
+        line 177: 38
+        line 168: 51
+        line 179: 56
+        line 182: 66
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            56      10     5 message   Ljava/lang/String;
            11      55     4 actualSum   Ljava/lang/String;
             0      67     0  this   Lorg/gradle/wrapper/Install;
             0      67     1 sourceUrl   Ljava/lang/String;
             0      67     2 localZipFile   Ljava/io/File;
@@ -960,23 +960,23 @@
         60: invokeinterface #62,  2           // InterfaceMethod java/util/List.add:(Ljava/lang/Object;)Z
         65: pop
         66: iinc          6, 1
         69: goto          35
         72: aload_2
         73: areturn
       LineNumberTable:
-        line 184: 0
-        line 185: 8
-        line 186: 15
-        line 187: 20
-        line 188: 24
-        line 189: 49
-        line 190: 57
-        line 188: 66
-        line 195: 72
+        line 185: 0
+        line 186: 8
+        line 187: 15
+        line 188: 20
+        line 189: 24
+        line 190: 49
+        line 191: 57
+        line 189: 66
+        line 196: 72
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            49      17     7  file   Ljava/io/File;
            20      52     3 files   [Ljava/io/File;
             0      74     0  this   Lorg/gradle/wrapper/Install;
             0      74     1 distDir   Ljava/io/File;
             8      66     2  dirs   Ljava/util/List;
@@ -1097,36 +1097,36 @@
        191: invokevirtual #96                 // Method org/gradle/wrapper/Logger.log:(Ljava/lang/String;)V
        194: return
       Exception table:
          from    to  target type
             21   133   136   Class java/io/IOException
             21   133   147   Class java/lang/InterruptedException
       LineNumberTable:
-        line 199: 0
-        line 200: 7
-        line 202: 8
-        line 203: 19
-        line 205: 21
-        line 206: 51
-        line 207: 58
-        line 208: 66
-        line 209: 87
-        line 211: 96
-        line 212: 107
-        line 214: 127
-        line 221: 133
-        line 216: 136
-        line 217: 138
-        line 221: 144
-        line 218: 147
-        line 219: 149
-        line 220: 155
-        line 222: 161
-        line 223: 165
-        line 225: 194
+        line 200: 0
+        line 201: 7
+        line 203: 8
+        line 204: 19
+        line 206: 21
+        line 207: 51
+        line 208: 58
+        line 209: 66
+        line 210: 87
+        line 212: 96
+        line 213: 107
+        line 215: 127
+        line 222: 133
+        line 217: 136
+        line 218: 138
+        line 222: 144
+        line 219: 147
+        line 220: 149
+        line 221: 155
+        line 223: 161
+        line 224: 165
+        line 226: 194
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            87      46     6    is   Ljava/io/BufferedReader;
            96      37     7 stdout   Ljava/util/Formatter;
           104      29     8  line   Ljava/lang/String;
            51      82     4    pb   Ljava/lang/ProcessBuilder;
            58      75     5     p   Ljava/lang/Process;
@@ -1167,16 +1167,16 @@
          8: invokevirtual #100                // Method java/lang/String.toLowerCase:(Ljava/util/Locale;)Ljava/lang/String;
         11: astore_1
         12: aload_1
         13: ldc           #101                // String windows
         15: invokevirtual #102                // Method java/lang/String.contains:(Ljava/lang/CharSequence;)Z
         18: ireturn
       LineNumberTable:
-        line 228: 0
-        line 229: 12
+        line 229: 0
+        line 230: 12
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      19     0  this   Lorg/gradle/wrapper/Install;
            12       7     1 osName   Ljava/lang/String;
 
   private boolean deleteDir(java.io.File);
     descriptor: (Ljava/io/File;)Z
@@ -1213,23 +1213,23 @@
         47: ireturn
         48: iinc          3, 1
         51: goto          18
         54: aload_1
         55: invokevirtual #52                 // Method java/io/File.delete:()Z
         58: ireturn
       LineNumberTable:
-        line 233: 0
-        line 234: 7
-        line 235: 12
-        line 236: 16
-        line 237: 24
-        line 238: 41
-        line 239: 46
-        line 236: 48
-        line 246: 54
+        line 234: 0
+        line 235: 7
+        line 236: 12
+        line 237: 16
+        line 238: 24
+        line 239: 41
+        line 240: 46
+        line 237: 48
+        line 247: 54
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            41       7     4 success   Z
            18      36     3     i   I
            12      42     2 children   [Ljava/lang/String;
             0      59     0  this   Lorg/gradle/wrapper/Install;
             0      59     1   dir   Ljava/io/File;
@@ -1311,34 +1311,34 @@
       Exception table:
          from    to  target type
             90   102   110   any
            110   112   110   any
              9   123   130   any
            130   132   130   any
       LineNumberTable:
-        line 250: 0
-        line 252: 9
-        line 254: 15
-        line 255: 25
-        line 257: 37
-        line 258: 55
-        line 259: 63
-        line 260: 69
-        line 263: 72
-        line 265: 90
-        line 267: 102
-        line 268: 107
-        line 267: 110
-        line 268: 117
-        line 269: 120
-        line 271: 123
-        line 272: 127
-        line 271: 130
-        line 272: 136
-        line 273: 139
+        line 251: 0
+        line 253: 9
+        line 255: 15
+        line 256: 25
+        line 258: 37
+        line 259: 55
+        line 260: 63
+        line 261: 69
+        line 264: 72
+        line 266: 90
+        line 268: 102
+        line 269: 107
+        line 268: 110
+        line 269: 117
+        line 270: 120
+        line 272: 123
+        line 273: 127
+        line 272: 130
+        line 273: 136
+        line 274: 139
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            37      83     5 entry   Ljava/util/zip/ZipEntry;
            55      65     6 destFile   Ljava/io/File;
            90      30     7 outputStream   Ljava/io/OutputStream;
            15     108     4 entries   Ljava/util/Enumeration;
             0     140     0  this   Lorg/gradle/wrapper/Install;
@@ -1391,20 +1391,20 @@
         25: goto          6
         28: aload_1
         29: invokevirtual #30                 // Method java/io/InputStream.close:()V
         32: aload_2
         33: invokevirtual #120                // Method java/io/OutputStream.close:()V
         36: return
       LineNumberTable:
-        line 276: 0
-        line 279: 6
-        line 280: 17
-        line 283: 28
-        line 284: 32
-        line 285: 36
+        line 277: 0
+        line 280: 6
+        line 281: 17
+        line 284: 28
+        line 285: 32
+        line 286: 36
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      37     0  this   Lorg/gradle/wrapper/Install;
             0      37     1    in   Ljava/io/InputStream;
             0      37     2   out   Ljava/io/OutputStream;
             6      31     3 buffer   [B
            14      23     4   len   I
```

#### org/gradle/wrapper/WrapperConfiguration.class

##### procyon -ec {}

```diff
@@ -7,20 +7,22 @@
 {
     private URI distribution;
     private String distributionBase;
     private String distributionPath;
     private String distributionSha256Sum;
     private String zipBase;
     private String zipPath;
+    private int networkTimeout;
     
     public WrapperConfiguration() {
         this.distributionBase = "GRADLE_USER_HOME";
         this.distributionPath = "wrapper/dists";
         this.zipBase = "GRADLE_USER_HOME";
         this.zipPath = "wrapper/dists";
+        this.networkTimeout = 10000;
     }
     
     public URI getDistribution() {
         return this.distribution;
     }
     
     public void setDistribution(final URI distribution) {
@@ -62,8 +64,16 @@
     public String getZipPath() {
         return this.zipPath;
     }
     
     public void setZipPath(final String zipPath) {
         this.zipPath = zipPath;
     }
+    
+    public int getNetworkTimeout() {
+        return this.networkTimeout;
+    }
+    
+    public void setNetworkTimeout(final int networkTimeout) {
+        this.networkTimeout = networkTimeout;
+    }
 }
```

#### org/gradle/wrapper/WrapperExecutor.class

##### procyon -ec {}

```diff
@@ -13,14 +13,15 @@
 {
     public static final String DISTRIBUTION_URL_PROPERTY = "distributionUrl";
     public static final String DISTRIBUTION_BASE_PROPERTY = "distributionBase";
     public static final String DISTRIBUTION_PATH_PROPERTY = "distributionPath";
     public static final String DISTRIBUTION_SHA_256_SUM = "distributionSha256Sum";
     public static final String ZIP_STORE_BASE_PROPERTY = "zipStoreBase";
     public static final String ZIP_STORE_PATH_PROPERTY = "zipStorePath";
+    public static final String NETWORK_TIMEOUT_PROPERTY = "networkTimeout";
     private final Properties properties;
     private final File propertiesFile;
     private final WrapperConfiguration config;
     
     public static WrapperExecutor forProjectDirectory(final File projectDir) {
         return new WrapperExecutor(new File(projectDir, "gradle/wrapper/gradle-wrapper.properties"), new Properties());
     }
@@ -41,14 +42,15 @@
                 loadProperties(propertiesFile, properties);
                 this.config.setDistribution(this.prepareDistributionUri());
                 this.config.setDistributionBase(this.getProperty("distributionBase", this.config.getDistributionBase()));
                 this.config.setDistributionPath(this.getProperty("distributionPath", this.config.getDistributionPath()));
                 this.config.setDistributionSha256Sum(this.getProperty("distributionSha256Sum", this.config.getDistributionSha256Sum(), false));
                 this.config.setZipBase(this.getProperty("zipStoreBase", this.config.getZipBase()));
                 this.config.setZipPath(this.getProperty("zipStorePath", this.config.getZipPath()));
+                this.config.setNetworkTimeout(this.getProperty("networkTimeout", this.config.getNetworkTimeout()));
             }
             catch (final Exception e) {
                 throw new RuntimeException(String.format("Could not load wrapper properties from '%s'.", propertiesFile), e);
             }
         }
     }
     
@@ -94,14 +96,18 @@
         return this.getProperty(propertyName, null, true);
     }
     
     private String getProperty(final String propertyName, final String defaultValue) {
         return this.getProperty(propertyName, defaultValue, true);
     }
     
+    private int getProperty(final String propertyName, final int defaultValue) {
+        return Integer.parseInt(this.getProperty(propertyName, String.valueOf(defaultValue)));
+    }
+    
     private String getProperty(final String propertyName, final String defaultValue, final boolean required) {
         final String value = this.properties.getProperty(propertyName);
         if (value != null) {
             return value;
         }
         if (defaultValue != null) {
             return defaultValue;
```

### Comparing `mtap-1.1.0/java/gradlew` & `mtap-1.2.0/java/gradlew`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 #       and GRADLE_OPTS) rely on word-splitting, this is performed explicitly;
 #       see the in-line comments for details.
 #
 #       There are tweaks for specific operating systems such as AIX, CygWin,
 #       Darwin, MinGW, and NonStop.
 #
 #   (3) This script is generated from the Groovy template
-#       https://github.com/gradle/gradle/blob/master/subprojects/plugins/src/main/resources/org/gradle/api/internal/plugins/unixStartScript.txt
+#       https://github.com/gradle/gradle/blob/HEAD/subprojects/plugins/src/main/resources/org/gradle/api/internal/plugins/unixStartScript.txt
 #       within the Gradle project.
 #
 #       You can find Gradle at https://github.com/gradle/gradle/.
 #
 ##############################################################################
 
 # Attempt to set APP_HOME
@@ -76,18 +76,18 @@
     link=${ls#*' -> '}
     case $link in             #(
       /*)   app_path=$link ;; #(
       *)    app_path=$APP_HOME$link ;;
     esac
 done
 
-APP_HOME=$( cd "${APP_HOME:-./}" && pwd -P ) || exit
-
-APP_NAME="Gradle"
+# This is normally unused
+# shellcheck disable=SC2034
 APP_BASE_NAME=${0##*/}
+APP_HOME=$( cd "${APP_HOME:-./}" && pwd -P ) || exit
 
 # Add default JVM options here. You can also use JAVA_OPTS and GRADLE_OPTS to pass JVM options to this script.
 DEFAULT_JVM_OPTS='"-Xmx64m" "-Xms64m"'
 
 # Use the maximum available, or set MAX_FD != -1 to use that value.
 MAX_FD=maximum
 
@@ -139,20 +139,24 @@
 location of your Java installation."
 fi
 
 # Increase the maximum file descriptors if we can.
 if ! "$cygwin" && ! "$darwin" && ! "$nonstop" ; then
     case $MAX_FD in #(
       max*)
+        # In POSIX sh, ulimit -H is undefined. That's why the result is checked to see if it worked.
+        # shellcheck disable=SC3045
         MAX_FD=$( ulimit -H -n ) ||
             warn "Could not query maximum file descriptor limit"
     esac
     case $MAX_FD in  #(
       '' | soft) :;; #(
       *)
+        # In POSIX sh, ulimit -n is undefined. That's why the result is checked to see if it worked.
+        # shellcheck disable=SC3045
         ulimit -n "$MAX_FD" ||
             warn "Could not set maximum file descriptor limit to $MAX_FD"
     esac
 fi
 
 # Collect all arguments for the java command, stacking in reverse order:
 #   * args from the command line
```

### Comparing `mtap-1.1.0/java/gradlew.bat` & `mtap-1.2.0/java/gradlew.bat`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 @rem ##########################################################################
 
 @rem Set local scope for the variables with windows NT shell
 if "%OS%"=="Windows_NT" setlocal
 
 set DIRNAME=%~dp0
 if "%DIRNAME%"=="" set DIRNAME=.
+@rem This is normally unused
 set APP_BASE_NAME=%~n0
 set APP_HOME=%DIRNAME%
 
 @rem Resolve any "." and ".." in APP_HOME to make it shorter.
 for %%i in ("%APP_HOME%") do set APP_HOME=%%~fi
 
 @rem Add default JVM options here. You can also use JAVA_OPTS and GRADLE_OPTS to pass JVM options to this script.
```

### Comparing `mtap-1.1.0/java/settings.gradle` & `mtap-1.2.0/java/settings.gradle`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/EventsServer.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/EventsServer.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/ExperimentalApi.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/ExperimentalApi.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/Internal.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/Internal.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/MTAP.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/MTAP.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/common/AbstractJsonObject.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/AbstractJsonObject.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/common/Config.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/Config.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/common/ConfigImpl.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/ConfigImpl.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObject.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObject.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObjectBuilder.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObjectBuilder.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObjectImpl.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/JsonObjectImpl.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/common/Server.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/common/Server.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/ConsulDiscoveryMechanism.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/ConsulDiscoveryMechanism.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/ConsulNameResolverProvider.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/ConsulNameResolverProvider.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/Discovery.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/Discovery.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/DiscoveryMechanism.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/DiscoveryMechanism.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/ServiceInfo.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/discovery/ServiceInfo.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/examples/HelloWorldExample.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/HelloWorldExample.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/examples/ReferenceLabelsExampleProcessor.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/ReferenceLabelsExampleProcessor.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/examples/WordOccurrencesExampleProcessor.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/WordOccurrencesExampleProcessor.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/examples/package-info.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/examples/package-info.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/exc/EventExistsException.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/exc/EventExistsException.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/exc/FailedToConnectToEventsException.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/exc/FailedToConnectToEventsException.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/exc/MtapException.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/exc/MtapException.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/AbstractLabelIndex.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/AbstractLabelIndex.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/Builder.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Builder.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/ChannelFactory.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/ChannelFactory.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/DistinctLabelIndex.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/DistinctLabelIndex.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/Document.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Document.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/Event.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Event.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/EventsClient.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/EventsClient.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/EventsClientPool.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/EventsClientPool.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/GenericLabel.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/GenericLabel.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/GenericLabelAdapter.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/GenericLabelAdapter.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/Label.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Label.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/LabelIndex.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/LabelIndex.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/LabelIndexInfo.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/LabelIndexInfo.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/Labeler.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Labeler.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/ProtoLabelAdapter.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/ProtoLabelAdapter.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/Span.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/Span.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/StandardLabelIndex.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/StandardLabelIndex.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/model/TextSpan.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/model/TextSpan.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/package-info.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/package-info.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/DefaultProcessorService.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/DefaultProcessorService.java`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 package edu.umn.nlpie.mtap.processing;
 
+import com.google.protobuf.Any;
 import com.google.protobuf.Struct;
 import com.google.protobuf.util.Durations;
+import com.google.rpc.Code;
 import com.google.rpc.DebugInfo;
+import com.google.rpc.ErrorInfo;
+import com.google.rpc.LocalizedMessage;
 import edu.umn.nlpie.mtap.Internal;
 import edu.umn.nlpie.mtap.MTAP;
 import edu.umn.nlpie.mtap.api.v1.Processing;
 import edu.umn.nlpie.mtap.api.v1.ProcessorGrpc;
 import edu.umn.nlpie.mtap.common.JsonObjectImpl;
 import edu.umn.nlpie.mtap.discovery.DiscoveryMechanism;
 import edu.umn.nlpie.mtap.discovery.ServiceInfo;
 import edu.umn.nlpie.mtap.exc.FailedToConnectToEventsException;
-import io.grpc.Metadata;
 import io.grpc.Status;
-import io.grpc.protobuf.ProtoUtils;
+import io.grpc.protobuf.StatusProto;
 import io.grpc.stub.StreamObserver;
 import org.jetbrains.annotations.NotNull;
 import org.jetbrains.annotations.Nullable;
 import org.slf4j.Logger;
 import org.slf4j.LoggerFactory;
 
 import java.time.Duration;
@@ -25,166 +28,185 @@
 import java.util.List;
 import java.util.Map;
 import java.util.UUID;
 import java.util.concurrent.ExecutionException;
 
 @Internal
 public class DefaultProcessorService extends ProcessorGrpc.ProcessorImplBase implements ProcessorService {
-  private static final Logger logger = LoggerFactory.getLogger(DefaultProcessorService.class);
+    private static final Logger logger = LoggerFactory.getLogger(DefaultProcessorService.class);
 
-  private final @NotNull ProcessorRunner runner;
-  private final @NotNull TimingService timingService;
-  private final @Nullable DiscoveryMechanism discoveryMechanism;
-  private final @NotNull HealthService healthService;
-
-  private final @NotNull String name;
-  private final @NotNull String sid;
-
-  private final @NotNull String host;
-
-  private int processed = 0;
-  private int failures = 0;
-  private int port;
-
-  public DefaultProcessorService(
-      @NotNull ProcessorRunner runner,
-      @NotNull TimingService timingService,
-      @Nullable DiscoveryMechanism discoveryMechanism,
-      @NotNull HealthService healthService,
-      @Nullable String name,
-      @Nullable String sid,
-      @NotNull String host
-  ) {
-    this.runner = runner;
-    this.timingService = timingService;
-    this.discoveryMechanism = discoveryMechanism;
-    this.healthService = healthService;
-    this.name = name != null ? name : runner.getProcessor().getProcessorName();
-    this.sid = sid != null ? sid : UUID.randomUUID().toString();
-    this.host = host;
-  }
-
-  @Override
-  public void started(int port) {
-    this.port = port;
-    healthService.startedServing(name);
-    if (discoveryMechanism != null) {
-      ServiceInfo serviceInfo = new ServiceInfo(
-          name,
-          sid,
-          host,
-          port,
-          Collections.singletonList(MTAP.PROCESSOR_SERVICE_TAG)
-      );
-      discoveryMechanism.register(serviceInfo);
-    }
-    logger.info("Server for processor_id: {} started on port: {}", name, port);
-  }
-
-  @Override
-  public void process(
-      Processing.ProcessRequest request,
-      StreamObserver<Processing.ProcessResponse> responseObserver
-  ) {
-    JsonObjectImpl params = JsonObjectImpl.newBuilder().copyStruct(request.getParams()).build();
-
-    String eventID = request.getEventId();
-    String eventServiceInstanceId = request.getEventServiceInstanceId();
-    logger.debug("{} received process request on event: ({}, {})", this.name, eventID, eventServiceInstanceId);
-    try {
-      ProcessingResult result = runner.process(eventID, eventServiceInstanceId, params);
-
-      Processing.ProcessResponse.Builder responseBuilder = Processing.ProcessResponse.newBuilder()
-          .setResult(result.getResult().copyToStruct(Struct.newBuilder()));
-      for (Map.Entry<String, List<String>> entry : result.getCreatedIndices().entrySet()) {
-        for (String indexName : entry.getValue()) {
-          responseBuilder.addCreatedIndices(Processing.CreatedIndex.newBuilder()
-              .setDocumentName(entry.getKey())
-              .setIndexName(indexName)
-              .build());
-        }
-      }
-      for (Map.Entry<String, Duration> entry : result.getTimes().entrySet()) {
-        long nanos = entry.getValue().toNanos();
-        timingService.addTime(entry.getKey(), nanos);
-        responseBuilder.putTimingInfo(entry.getKey(), Durations.fromNanos(nanos));
-      }
-      responseObserver.onNext(responseBuilder.build());
-      responseObserver.onCompleted();
-      processed++;
-    } catch (FailedToConnectToEventsException e) {
-      logger.error("Failed to connect to events service with address: {}", e.getAddress());
-      responseObserver.onError(Status.INTERNAL.withCause(e).asRuntimeException());
-    } catch (RuntimeException e) {
-      logger.error("Exception during processing of event '{}'", eventID, e);
-      Metadata trailers = new Metadata();
-      Metadata.Key<DebugInfo> key = ProtoUtils.keyForProto(DebugInfo.getDefaultInstance());
-      DebugInfo.Builder debugInfoBuilder = DebugInfo.newBuilder();
-      for (StackTraceElement stackTraceElement : e.getStackTrace()) {
-        debugInfoBuilder.addStackEntries(stackTraceElement.toString());
-      }
-      trailers.put(key, debugInfoBuilder.build());
-      responseObserver.onError(Status.INTERNAL.withDescription(e.toString())
-          .asRuntimeException(trailers));
-      failures++;
-    }
-  }
-
-  @Override
-  public void getInfo(
-      Processing.GetInfoRequest request,
-      StreamObserver<Processing.GetInfoResponse> responseObserver
-  ) {
-    Map<String, Object> processorMeta = runner.getProcessorMeta();
-    try {
-      JsonObjectImpl.Builder jsonObjectBuilder = JsonObjectImpl.newBuilder();
-      jsonObjectBuilder.putAll(processorMeta);
-      JsonObjectImpl jsonObject = jsonObjectBuilder.build();
-
-      Processing.GetInfoResponse.Builder builder = Processing.GetInfoResponse.newBuilder();
-      jsonObject.copyToStruct(builder.getMetadataBuilder());
-      responseObserver.onNext(builder.build());
-      responseObserver.onCompleted();
-    } catch (RuntimeException e) {
-      responseObserver.onError(Status.INTERNAL.withDescription(e.toString())
-          .withCause(e)
-          .asRuntimeException());
-    }
-  }
-
-  @Override
-  public void getStats(
-      Processing.GetStatsRequest request,
-      StreamObserver<Processing.GetStatsResponse> responseObserver
-  ) {
-    try {
-      Processing.GetStatsResponse.Builder builder = Processing.GetStatsResponse.newBuilder()
-          .setProcessed(processed)
-          .setFailures(failures);
-      Map<String, Processing.TimerStats> timerStatsMap = timingService.getTimerStats();
-      builder.putAllTimingStats(timerStatsMap);
-      responseObserver.onNext(builder.build());
-      responseObserver.onCompleted();
-    } catch (RuntimeException | InterruptedException | ExecutionException e) {
-      responseObserver.onError(Status.INTERNAL.withDescription(e.toString())
-          .withCause(e)
-          .asRuntimeException());
-    }
-  }
-
-  @Override
-  public void close() throws InterruptedException {
-    System.out.println("Shutting down processor server with name: \"" + name + "\" on address: \"" + host + ":" + port + "\"");
-    ServiceInfo serviceInfo = new ServiceInfo(
-        name,
-        sid,
-        null,
-        -1,
-        Collections.singletonList(MTAP.PROCESSOR_SERVICE_TAG)
-    );
-    healthService.stoppedServing(name);
-    if (discoveryMechanism != null) {
-      discoveryMechanism.deregister(serviceInfo);
+    private final @NotNull ProcessorRunner runner;
+    private final @NotNull TimingService timingService;
+    private final @Nullable DiscoveryMechanism discoveryMechanism;
+    private final @NotNull HealthService healthService;
+
+    private final @NotNull String name;
+    private final @NotNull String sid;
+
+    private final @NotNull String host;
+
+    private int processed = 0;
+    private int failures = 0;
+    private int port;
+
+    public DefaultProcessorService(
+            @NotNull ProcessorRunner runner,
+            @NotNull TimingService timingService,
+            @Nullable DiscoveryMechanism discoveryMechanism,
+            @NotNull HealthService healthService,
+            @Nullable String name,
+            @Nullable String sid,
+            @NotNull String host
+    ) {
+        this.runner = runner;
+        this.timingService = timingService;
+        this.discoveryMechanism = discoveryMechanism;
+        this.healthService = healthService;
+        this.name = name != null ? name : runner.getProcessor().getProcessorName();
+        this.sid = sid != null ? sid : UUID.randomUUID().toString();
+        this.host = host;
+    }
+
+    @Override
+    public void started(int port) {
+        this.port = port;
+        healthService.startedServing(name);
+        if (discoveryMechanism != null) {
+            ServiceInfo serviceInfo = new ServiceInfo(
+                    name,
+                    sid,
+                    host,
+                    port,
+                    Collections.singletonList(MTAP.PROCESSOR_SERVICE_TAG)
+            );
+            discoveryMechanism.register(serviceInfo);
+        }
+        logger.info("Server for processor_id: {} started on port: {}", name, port);
+    }
+
+    @Override
+    public void process(
+            Processing.ProcessRequest request,
+            StreamObserver<Processing.ProcessResponse> responseObserver
+    ) {
+        JsonObjectImpl params = JsonObjectImpl.newBuilder().copyStruct(request.getParams()).build();
+
+        String eventID = request.getEventId();
+        String eventServiceInstanceId = request.getEventServiceInstanceId();
+        logger.debug("{} received process request on event: ({}, {})", this.name, eventID, eventServiceInstanceId);
+        try {
+            ProcessingResult result = runner.process(eventID, eventServiceInstanceId, params);
+
+            Processing.ProcessResponse.Builder responseBuilder = Processing.ProcessResponse.newBuilder()
+                    .setResult(result.getResult().copyToStruct(Struct.newBuilder()));
+            for (Map.Entry<String, List<String>> entry : result.getCreatedIndices().entrySet()) {
+                for (String indexName : entry.getValue()) {
+                    responseBuilder.addCreatedIndices(Processing.CreatedIndex.newBuilder()
+                            .setDocumentName(entry.getKey())
+                            .setIndexName(indexName)
+                            .build());
+                }
+            }
+            for (Map.Entry<String, Duration> entry : result.getTimes().entrySet()) {
+                long nanos = entry.getValue().toNanos();
+                timingService.addTime(entry.getKey(), nanos);
+                responseBuilder.putTimingInfo(entry.getKey(), Durations.fromNanos(nanos));
+            }
+            responseObserver.onNext(responseBuilder.build());
+            responseObserver.onCompleted();
+            processed++;
+        } catch (FailedToConnectToEventsException e) {
+            logger.error("Failed to connect to events service with address: {}", e.getAddress());
+            String message = e.getMessage();
+            responseObserver.onError(StatusProto.toStatusRuntimeException(buildStatus(e, message)));
+        } catch (RuntimeException e) {
+            logger.error("Exception during processing of event '{}'", eventID, e);
+            String message = "An internal error occurred while attempting to process an Event. " +
+                    "This is potentially a bug, contact the developer of the component.";
+            responseObserver.onError(StatusProto.toStatusRuntimeException(buildStatus(e, message)));
+            failures++;
+        }
+    }
+
+    @NotNull
+    private static com.google.rpc.Status buildStatus(Exception e, String message) {
+        DebugInfo.Builder debugInfoBuilder = DebugInfo.newBuilder();
+        for (StackTraceElement stackTraceElement : e.getStackTrace()) {
+            debugInfoBuilder.addStackEntries(stackTraceElement.toString() + "\n");
+        }
+        return com.google.rpc.Status.newBuilder()
+                .setCode(Code.UNKNOWN.getNumber())
+                .setMessage("Internal error during processing.")
+                .addDetails(Any.pack(ErrorInfo.newBuilder()
+                        .setReason("PROCESSING_FAILURE")
+                        .setDomain("mtap.nlpie.umn.edu")
+                        .putMetadata("lang", "java")
+                        .putMetadata("errorType", e.getClass().getCanonicalName())
+                        .putMetadata("errorRepr", e.toString())
+                        .build()))
+                .addDetails(Any.pack(debugInfoBuilder.build()))
+                .addDetails(Any.pack(LocalizedMessage.newBuilder()
+                        .setLocale("en-US")
+                        .setMessage(message)
+                        .build()))
+                .build();
+    }
+
+    @Override
+    public void getInfo(
+            Processing.GetInfoRequest request,
+            StreamObserver<Processing.GetInfoResponse> responseObserver
+    ) {
+        Map<String, Object> processorMeta = runner.getProcessorMeta();
+        try {
+            JsonObjectImpl.Builder jsonObjectBuilder = JsonObjectImpl.newBuilder();
+            jsonObjectBuilder.putAll(processorMeta);
+            JsonObjectImpl jsonObject = jsonObjectBuilder.build();
+
+            Processing.GetInfoResponse.Builder builder = Processing.GetInfoResponse.newBuilder();
+            jsonObject.copyToStruct(builder.getMetadataBuilder());
+            responseObserver.onNext(builder.build());
+            responseObserver.onCompleted();
+        } catch (RuntimeException e) {
+            responseObserver.onError(Status.INTERNAL.withDescription(e.toString())
+                    .withCause(e)
+                    .asRuntimeException());
+        }
+    }
+
+    @Override
+    public void getStats(
+            Processing.GetStatsRequest request,
+            StreamObserver<Processing.GetStatsResponse> responseObserver
+    ) {
+        try {
+            Processing.GetStatsResponse.Builder builder = Processing.GetStatsResponse.newBuilder()
+                    .setProcessed(processed)
+                    .setFailures(failures);
+            Map<String, Processing.TimerStats> timerStatsMap = timingService.getTimerStats();
+            builder.putAllTimingStats(timerStatsMap);
+            responseObserver.onNext(builder.build());
+            responseObserver.onCompleted();
+        } catch (RuntimeException | InterruptedException | ExecutionException e) {
+            responseObserver.onError(Status.INTERNAL.withDescription(e.toString())
+                    .withCause(e)
+                    .asRuntimeException());
+        }
+    }
+
+    @Override
+    public void close() throws InterruptedException {
+        System.out.println("Shutting down processor server with name: \"" + name + "\" on address: \"" + host + ":" + port + "\"");
+        ServiceInfo serviceInfo = new ServiceInfo(
+                name,
+                sid,
+                null,
+                -1,
+                Collections.singletonList(MTAP.PROCESSOR_SERVICE_TAG)
+        );
+        healthService.stoppedServing(name);
+        if (discoveryMechanism != null) {
+            discoveryMechanism.deregister(serviceInfo);
+        }
+        runner.close();
     }
-    runner.close();
-  }
 }
```

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/DefaultTimingService.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/DefaultTimingService.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/DocumentProcessor.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/DocumentProcessor.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/EventProcessor.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/EventProcessor.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/HSMHealthService.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/HSMHealthService.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/LabelIndexDescription.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/LabelIndexDescription.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/LocalProcessorRunner.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/LocalProcessorRunner.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ParameterDescription.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ParameterDescription.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessingResult.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessingResult.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/Processor.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/Processor.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorBase.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorBase.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorContext.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorContext.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorRunner.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorRunner.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorServer.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorServer.java`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 package edu.umn.nlpie.mtap.processing;
 
 import edu.umn.nlpie.mtap.common.Config;
 import edu.umn.nlpie.mtap.common.ConfigImpl;
 import edu.umn.nlpie.mtap.discovery.Discovery;
 import edu.umn.nlpie.mtap.discovery.DiscoveryMechanism;
+import edu.umn.nlpie.mtap.examples.HelloWorldExample;
 import edu.umn.nlpie.mtap.model.ChannelFactory;
 import edu.umn.nlpie.mtap.model.EventsClientPool;
 import edu.umn.nlpie.mtap.utilities.Helpers;
 import io.grpc.Server;
 import io.grpc.netty.shaded.io.grpc.netty.NettyServerBuilder;
 import org.jetbrains.annotations.NotNull;
 import org.jetbrains.annotations.Nullable;
@@ -518,8 +519,25 @@
      * @param processor The processor to host.
      * @return A server object that can be used to control the lifecycle of the server.
      */
     public ProcessorServer createServer(EventProcessor processor) {
       return build(processor);
     }
   }
+
+  public static void hostProcessor(String[] args, EventProcessor processor) {
+    ProcessorServer.Builder options = new ProcessorServer.Builder();
+    CmdLineParser parser = new CmdLineParser(options);
+    try {
+      parser.parseArgument(args);
+      ProcessorServer server = options.build(processor);
+      server.start();
+      server.blockUntilShutdown();
+    } catch (IOException e) {
+      System.err.println("Failed to start server: " + e.getMessage());
+    } catch (InterruptedException e) {
+      System.err.println("Server interrupted.");
+    } catch (CmdLineException e) {
+      ProcessorServer.Builder.printHelp(parser, EventProcessor.class, e, null);
+    }
+  }
 }
```

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorService.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/ProcessorService.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/PropertyDescription.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/PropertyDescription.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/RunningVariance.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/RunningVariance.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/StandardChannelFactory.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/StandardChannelFactory.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/processing/Stopwatch.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/processing/Stopwatch.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/utilities/Helpers.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/utilities/Helpers.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/java/edu/umn/nlpie/mtap/utilities/PrintProcessorMetadata.java` & `mtap-1.2.0/java/src/main/java/edu/umn/nlpie/mtap/utilities/PrintProcessorMetadata.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/main/resources/edu/umn/nlpie/mtap/defaultConfig.yml` & `mtap-1.2.0/java/src/main/resources/edu/umn/nlpie/mtap/defaultConfig.yml`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/common/ConfigTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/common/ConfigTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexAscendingViewTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexAscendingViewTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexDescendingViewTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexDescendingViewTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/DistinctLabelIndexTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/DocumentTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/DocumentTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/EventTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/EventTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/EventsClientTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/EventsClientTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/GenericLabelAdapterTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/GenericLabelAdapterTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/GenericLabelTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/GenericLabelTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexAscendingViewTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexAscendingViewTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexDescendingViewTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexDescendingViewTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/model/StandardLabelIndexTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/processing/DefaultProcessorServiceTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/DefaultProcessorServiceTest.java`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         () -> stub.process(Processing.ProcessRequest.newBuilder()
             .setEventId("1")
             .setEventServiceInstanceId("1")
             .setParams(Struct.newBuilder()
                 .putFields("test", Value.newBuilder().setBoolValue(true).build()).build())
             .build()
         ));
-    assertEquals("INTERNAL: java.lang.IllegalStateException: foo", exception.getMessage());
+    assertEquals("UNKNOWN: Internal error during processing.", exception.getMessage());
   }
 
   @Test
   void getInfo() throws IOException {
     DefaultProcessorService processorService = createProcessorService(false);
     createServer(processorService).start();
     ProcessorGrpc.ProcessorBlockingStub stub = createStub();
```

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/processing/DefaultTimingServiceTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/DefaultTimingServiceTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/processing/EventProcessorTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/EventProcessorTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/processing/LocalProcessorRunnerTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/LocalProcessorRunnerTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/processing/ProcessorServerBuilderTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/ProcessorServerBuilderTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/processing/ProcessorServerTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/ProcessorServerTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/processing/RunningVarianceTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/processing/RunningVarianceTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/java/edu/umn/nlpie/mtap/utilities/PrintProcessorMetadataTest.java` & `mtap-1.2.0/java/src/test/java/edu/umn/nlpie/mtap/utilities/PrintProcessorMetadataTest.java`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/java/src/test/resources/edu/umn/nlpie/mtap/ExampleMeta.yaml` & `mtap-1.2.0/java/src/test/resources/edu/umn/nlpie/mtap/ExampleMeta.yaml`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/proto/mtap/api/v1/events.proto` & `mtap-1.2.0/proto/mtap/api/v1/events.proto`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import "google/protobuf/any.proto";
 import "google/protobuf/duration.proto";
 import "google/protobuf/struct.proto";
 
 package mtap.api.v1;
 
 option java_package = "edu.umn.nlpie.mtap.api.v1";
+option go_package = "mtap/api/v1";
 
 /* A request to retrieve the UUID for this events service instance.
  */
 message GetEventsInstanceIdRequest {
 }
 
 message GetEventsInstanceIdResponse {
```

### Comparing `mtap-1.1.0/proto/mtap/api/v1/processing.proto` & `mtap-1.2.0/proto/mtap/api/v1/processing.proto`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import "google/api/annotations.proto";
 import "google/protobuf/duration.proto";
 import "google/protobuf/struct.proto";
 
 package mtap.api.v1;
 
 option java_package = "edu.umn.nlpie.mtap.api.v1";
+option go_package = "mtap/api/v1";
 
 /* The name of a newly created label index during a process call.
  */
 message CreatedIndex {
   /* The document's name where the index was created.
    */
   string document_name = 1;
```

### Comparing `mtap-1.1.0/pyproject.toml` & `mtap-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "setuptools>=45",
     "setuptools-scm[toml]>=6.2",
     "wheel>=0.38.0",
     "importlib_resources>=1.3",
     "grpcio-tools>=1.48.2,<=1.51.1",
-    "googleapis-common-protos>=1.3.1,<=1.58.0",
+    "googleapis-common-protos>=1.3.1,<=1.59.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mtap"
 description = "A framework for distributed text analysis using gRPC and microservices-based architecture."
 readme = "README.md"
@@ -38,34 +38,35 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Java Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Text Processing :: General",
     "Topic :: Text Processing :: Linguistic",
 ]
 dependencies = [
-    "grpcio>=1.48.2,<=1.51.3",
-    "grpcio-health-checking>=1.48.2,<=1.51.3",
+    "grpcio>=1.48.2,<=1.53.0",
+    "grpcio-health-checking>=1.48.2,<=1.53.0",
+    "grpcio-status>=1.48.2,<=1.53.0",
     "pyyaml==6.0",
     "tqdm>=4.0.0,<=4.65.0",
-    "googleapis-common-protos>=1.3.1,<=1.58.0",
+    "googleapis-common-protos>=1.3.1,<=1.59.0",
 ]
 dynamic = ["version"]
 
 [tool.setuptools.packages.find]
 where = ["python"]
 include = ["mtap*"]
 
 [tool.setuptools_scm]
 write_to = "python/mtap/version.py"
 
 [project.optional-dependencies]
 test = [
-    "pytest==7.2.2",
+    "pytest==7.3.0",
     "pytest-mock==3.10.0",
-    "grpcio-testing>=1.48.2,<=1.51.3",
+    "grpcio-testing>=1.48.2,<=1.53.0",
     "requests==2.28.2",
     "importlib-resources==5.12.0",
 ]
 docs = [
     "sphinx==6.1.3",
 ]
 consul = ["python-consul"]
```

### Comparing `mtap-1.1.0/python/docs/Makefile` & `mtap-1.2.0/python/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/docs/conf.py` & `mtap-1.2.0/python/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,28 +61,33 @@
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.intersphinx',
     'sphinx.ext.coverage',
     'sphinx.ext.viewcode',
-    'sphinx.ext.githubpages',
-    'sphinx.ext.napoleon'
+    'sphinx.ext.napoleon',
+    'sphinx_rtd_theme',
 ]
 
-napoleon_google_docstring = True
-napoleon_numpy_docstring = False
-napoleon_include_special_with_doc = True
+html_theme = 'bizstyle'
 
+autosummary_generate = True
 autodoc_default_options = {
-    'members': None,
-    'member-order': 'bysource'
 }
+autoclass_content = 'class'
+autodoc_typehints_format = 'short'
+autodoc_member_order = 'bysource'
+autodoc_inherit_docstrings = False
+autodoc_preserve_defaults = True
+
+napoleon_google_docstring = True
+napoleon_numpy_docstring = False
+napoleon_attr_annotations = True
 
-autodoc_typehints = 'none'
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
@@ -108,15 +113,15 @@
 pygments_style = None
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'sphinxdoc'
+# html_theme = 'sphinxdoc'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 html_theme_options = {
 }
```

### Comparing `mtap-1.1.0/python/docs/make.bat` & `mtap-1.2.0/python/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/__init__.py` & `mtap-1.2.0/python/mtap/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,22 +23,22 @@
     label,
     label_index,
     Location,
 )
 from mtap.processing import (
     DocumentProcessor,
     EventProcessor,
-    LocalProcessor,
     Pipeline,
     ProcessorServer,
-    RemoteProcessor,
     descriptions,
     processor,
     processor_parser,
     run_processor,
+    RemoteProcessor,
+    LocalProcessor,
 )
 from mtap.version import (
     __version__,
     __version_tuple__,
     version,
     version_tuple
 )
```

### Comparing `mtap-1.1.0/python/mtap/__main__.py` & `mtap-1.2.0/python/mtap/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,17 +24,22 @@
         args: Command line arguments.
     """
     from mtap._config import Config
     from mtap._events_service import EventsServer
     with Config() as c:
         if args.mtap_config is not None:
             c.update_from_yaml(args.mtap_config)
-        server = EventsServer(args.host, sid=args.sid, port=args.port, register=args.register,
-                              workers=args.workers,
-                              write_address=args.write_address)
+        server = EventsServer(
+            args.host,
+            sid=args.sid,
+            port=args.port,
+            register=args.register,
+            workers=args.workers,
+            write_address=args.write_address
+        )
 
         e = threading.Event()
 
         def do_stop(*_):
             e.set()
 
         signal.signal(signal.SIGINT, do_stop)
@@ -44,34 +49,73 @@
         try:
             e.wait()
         except KeyboardInterrupt:
             pass
         server.stop()
 
 
-parser = argparse.ArgumentParser(allow_abbrev=False)
-subparsers = parser.add_subparsers(title='sub-commands', description='valid sub-commands')
+def main(args=None):
+    parser = argparse.ArgumentParser(allow_abbrev=False)
+    subparsers = parser.add_subparsers(title='sub-commands',
+                                       description='valid sub-commands')
+
+    # Documents service sub-command
+    events_parser = subparsers.add_parser('events',
+                                          help='starts a events service')
+    events_parser.add_argument(
+        '--host', '--address', '-a',
+        default="127.0.0.1",
+        metavar="HOST",
+        help='the address to serve the service on'
+    )
+    events_parser.add_argument(
+        '--port', '-p',
+        type=int,
+        default=0,
+        metavar="PORT",
+        help='the port to serve the service on'
+    )
+    events_parser.add_argument(
+        '--workers', '-w',
+        type=int,
+        default=10,
+        help='number of worker threads to handle requests'
+    )
+    events_parser.add_argument(
+        '--sid',
+        help='The unique service identifier for the events service.'
+    )
+    events_parser.add_argument(
+        '--register', '-r',
+        action='store_true',
+        help='whether to register the service with the configured '
+             'service discovery'
+    )
+    events_parser.add_argument(
+        "--mtap-config",
+        default=None,
+        help="path to MTAP config file"
+    )
+    events_parser.add_argument(
+        "--write-address",
+        action='store_true',
+        help="If set, will write the server's resolved address to a file "
+             "in the MTAP home directory (~/.mtap/addresses)"
+    )
+    events_parser.add_argument(
+        '--log-level',
+        default='INFO',
+        choices=['CRITICAL', 'ERROR', 'WARNING', 'INFO', 'DEBUG', 'NOTSET'],
+        help='The global python log level.'
+    )
+    events_parser.set_defaults(func=run_events_server)
+
+    # parse and execute
+    args = parser.parse_args(args)
+    try:
+        logging.basicConfig(level=args.log_level)
+    except AttributeError:
+        pass
+    args.func(args)
 
-# Documents service sub-command
-events_parser = subparsers.add_parser('events', help='starts a events service')
-events_parser.add_argument('--host', '--address', '-a', default="127.0.0.1", metavar="HOST",
-                           help='the address to serve the service on')
-events_parser.add_argument('--port', '-p', type=int, default=0, metavar="PORT",
-                           help='the port to serve the service on')
-events_parser.add_argument('--workers', '-w', type=int, default=10,
-                           help='number of worker threads to handle requests')
-events_parser.add_argument('--sid', help='The unique service identifier for the events service.')
-events_parser.add_argument('--register', '-r', action='store_true',
-                           help='whether to register the service with the configured '
-                                'service discovery')
-events_parser.add_argument("--mtap-config", default=None,
-                           help="path to MTAP config file")
-events_parser.add_argument("--write-address", action='store_true',
-                           help="If set, will write the server's resolved address to a file "
-                                "in the MTAP home directory (~/.mtap/addresses)")
-events_parser.add_argument('--log-level', default='INFO', help='The global python log level.')
-events_parser.set_defaults(func=run_events_server)
-
-# parse and execute
-args = parser.parse_args()
-logging.basicConfig(level=args.log_level)
-args.func(args)
+
+main()
```

### Comparing `mtap-1.1.0/python/mtap/_config.py` & `mtap-1.2.0/python/mtap/_config.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/_events_service.py` & `mtap-1.2.0/python/mtap/_events_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,18 @@
         port (int): The port to host the server on.
         register (bool): Whether to register the service with service discovery.
         workers (int): The number of workers that should handle requests.
         write_address (bool): Whether to write the events service address to a file.
         config (mtap.Config): An optional mtap config.
     """
 
-    def __init__(self, host: str, *, port: int = 0, register: bool = False, workers: int = 10,
-                 sid: Optional[str] = None, write_address: bool = False, config: 'Optional[mtap.Config]' = None):
+    def __init__(self, host: str, *, port: int = 0, register: bool = False,
+                 workers: int = 10,
+                 sid: Optional[str] = None, write_address: bool = False,
+                 config: 'Optional[mtap.Config]' = None):
         if host is None:
             host = '127.0.0.1'
         if port is None:
             port = 0
         self.sid = sid or str(uuid.uuid4())
         self.write_address = write_address
         thread_pool = ThreadPoolExecutor(max_workers=workers)
@@ -79,28 +81,31 @@
     def port(self) -> int:
         """int: The port the processor service is bound to."""
         return self._port
 
     def start(self):
         """Starts the service.
         """
-        logger.info(f'Starting events server (%s) on address: "%s:%d"', self.sid, self._address, self._port)
+        logger.info(f'Starting events server (%s) on address: "%s:%d"',
+                    self.sid, self._address, self._port)
         self._server.start()
         if self.write_address:
             self._address_file = utilities.write_address_file(
                 '{}:{}'.format(self._address, self.port),
                 self.sid
             )
         if self._register:
-            from mtap._discovery import Discovery
-            service_registration = Discovery(config=self._config)
-            self._deregister = service_registration.register_events_service(self.sid,
-                                                                            self._address,
-                                                                            self._port,
-                                                                            'v1')
+            from mtap.discovery import DiscoveryMechanism
+            service_registration = DiscoveryMechanism()
+            self._deregister = service_registration.register_events_service(
+                self.sid,
+                self._address,
+                self._port,
+                'v1'
+            )
 
     def stop(self, *, grace: Optional[float] = None):
         """De-registers (if registered with service discovery) the service and immediately stops
         accepting requests, completely stopping the service after a specified `grace` time.
 
         During the grace period the server will continue to process existing requests, but it will
         not accept any new requests. This function is idempotent, multiple calls will shutdown
@@ -111,15 +116,16 @@
             grace (~typing.Optional[float]):
                 The grace period in seconds that the server should continue processing requests
                 before shutdown.
 
         Returns:
             threading.Event: A shutdown event for the server.
         """
-        print("Shutting down events server on address: {}:{}".format(self._address, self._port))
+        print("Shutting down events server on address: {}:{}".format(
+            self._address, self._port))
         if self._address_file is not None:
             self._address_file.unlink()
         try:
             self._deregister()
         except AttributeError:
             pass
         return self._server.stop(grace=grace)
@@ -144,22 +150,24 @@
     def _get_document(self, request, context=None):
         event, event_id = self._get_event(request, context)
         document_name = request.document_name
         try:
             document = event.documents[document_name]
         except KeyError as e:
             _set_error_context(context, grpc.StatusCode.NOT_FOUND,
-                               "Event: '{}' does not have document: '{}'".format(event_id,
-                                                                                 document_name))
+                               "Event: '{}' does not have document: '{}'".format(
+                                   event_id,
+                                   document_name))
             raise e
         return document
 
     def GetEventsInstanceId(self, request, context):
         logger.debug("GetEventsInstanceId")
-        return events_pb2.GetEventsInstanceIdResponse(instance_id=self.instance_id)
+        return events_pb2.GetEventsInstanceIdResponse(
+            instance_id=self.instance_id)
 
     def OpenEvent(self, request, context=None):
         logger.debug("OpenEvent: %s", request.event_id)
         event_id = request.event_id
         if event_id == '':
             msg = "event_id was not set."
             _set_error_context(context, grpc.StatusCode.INVALID_ARGUMENT, msg)
@@ -216,15 +224,16 @@
 
     def GetAllBinaryDataNames(self, request, context):
         try:
             event, event_id = self._get_event(request, context)
         except KeyError:
             return empty_pb2.Empty()
         names = list(event.binaries.keys())
-        return events_pb2.GetAllBinaryDataNamesResponse(binary_data_names=names)
+        return events_pb2.GetAllBinaryDataNamesResponse(
+            binary_data_names=names)
 
     def AddBinaryData(self, request, context):
         try:
             event, event_id = self._get_event(request, context)
         except KeyError:
             return empty_pb2.Empty()
         name = request.binary_data_name
@@ -241,15 +250,16 @@
         except KeyError:
             return empty_pb2.Empty()
         name = request.binary_data_name
         if name == '':
             msg = 'binary_data_name cannot be null or empty'
             _set_error_context(context, grpc.StatusCode.INVALID_ARGUMENT, msg)
             return empty_pb2.Empty()
-        return events_pb2.GetBinaryDataResponse(binary_data=event.binaries[name])
+        return events_pb2.GetBinaryDataResponse(
+            binary_data=event.binaries[name])
 
     def AddDocument(self, request, context=None):
         logger.debug("AddDocument: %s", request.event_id)
         try:
             event, event_id = self._get_event(request, context)
         except KeyError:
             return empty_pb2.Empty()
@@ -258,15 +268,16 @@
             msg = 'document_name was not set.'
             _set_error_context(context, grpc.StatusCode.INVALID_ARGUMENT, msg)
             return empty_pb2.Empty()
 
         with event.d_lock:
             if document_name in event.documents:
                 msg = "Document '{}' already exists.".format(document_name)
-                _set_error_context(context, grpc.StatusCode.ALREADY_EXISTS, msg)
+                _set_error_context(context, grpc.StatusCode.ALREADY_EXISTS,
+                                   msg)
                 return empty_pb2.Empty()
             event.documents[document_name] = _Document(request.text)
 
         return events_pb2.AddDocumentResponse()
 
     def GetAllDocumentNames(self, request, context=None):
         logger.debug("GetAllDocumentNames: %s", request.event_id)
@@ -308,28 +319,35 @@
         labels_field = request.WhichOneof('labels')
         if labels_field is None:
             labels = ('generic_labels', events_pb2.GenericLabels())
         else:
             index_name = request.index_name
             if index_name == '':
                 msg = 'No index_name was set.'
-                _set_error_context(context, grpc.StatusCode.INVALID_ARGUMENT, msg)
+                _set_error_context(context, grpc.StatusCode.INVALID_ARGUMENT,
+                                   msg)
                 return empty_pb2.Empty()
             labels = (labels_field, getattr(request, labels_field))
         if labels_field == 'generic_labels' and not request.no_key_validation:
             for label in labels[1].labels:
                 for key in label.fields:
-                    if key in ["document", "location", "text", "id", "label_index_name"]:
-                        _set_error_context(context, grpc.StatusCode.INVALID_ARGUMENT,
-                                           "Label included a reserved key: {}".format(key))
+                    if key in ["document", "location", "text", "id",
+                               "label_index_name"]:
+                        _set_error_context(context,
+                                           grpc.StatusCode.INVALID_ARGUMENT,
+                                           "Label included a reserved key: {}".format(
+                                               key))
                         return empty_pb2.Empty()
                 for key in label.reference_ids:
-                    if key in ["document", "location", "text", "id", "id", "label_index_name"]:
-                        _set_error_context(context, grpc.StatusCode.INVALID_ARGUMENT,
-                                           "Label included a reserved key: {}".format(key))
+                    if key in ["document", "location", "text", "id", "id",
+                               "label_index_name"]:
+                        _set_error_context(context,
+                                           grpc.StatusCode.INVALID_ARGUMENT,
+                                           "Label included a reserved key: {}".format(
+                                               key))
                         return empty_pb2.Empty()
         document.labels[request.index_name] = labels
         return events_pb2.AddLabelsResponse()
 
     def GetLabels(self, request, context=None):
         try:
             document = self._get_document(request, context)
```

### Comparing `mtap-1.1.0/python/mtap/_structs.py` & `mtap-1.2.0/python/mtap/_structs.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/api/__init__.py` & `mtap-1.2.0/python/mtap/api/__init__.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/api/v1/__init__.py` & `mtap-1.2.0/python/mtap/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/api/v1/events_pb2.py` & `mtap-1.2.0/python/mtap/api/v1/events_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18mtap/api/v1/events.proto\x12\x0bmtap.api.v1\x1a\x1cgoogle/api/annotations.proto\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x1c\n\x1aGetEventsInstanceIdRequest\"2\n\x1bGetEventsInstanceIdResponse\x12\x13\n\x0binstance_id\x18\x01 \x01(\t\"p\n\x10OpenEventRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x17\n\x0fonly_create_new\x18\x02 \x01(\x08\x12\x31\n\x0elease_duration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\"6\n\x11OpenEventResponse\x12\x0f\n\x07\x63reated\x18\x01 \x01(\x08\x12\x10\n\x08lease_id\x18\x02 \x01(\x05\"7\n\x11\x43loseEventRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x10\n\x08lease_id\x18\x02 \x01(\x05\"%\n\x12\x43loseEventResponse\x12\x0f\n\x07\x64\x65leted\x18\x01 \x01(\x08\")\n\x15GetAllMetadataRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\"\x8e\x01\n\x16GetAllMetadataResponse\x12\x43\n\x08metadata\x18\x01 \x03(\x0b\x32\x31.mtap.api.v1.GetAllMetadataResponse.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"B\n\x12\x41\x64\x64MetadataRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\x15\n\x13\x41\x64\x64MetadataResponse\"0\n\x1cGetAllBinaryDataNamesRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\":\n\x1dGetAllBinaryDataNamesResponse\x12\x19\n\x11\x62inary_data_names\x18\x01 \x03(\t\"W\n\x14\x41\x64\x64\x42inaryDataRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x18\n\x10\x62inary_data_name\x18\x02 \x01(\t\x12\x13\n\x0b\x62inary_data\x18\x03 \x01(\x0c\"\x17\n\x15\x41\x64\x64\x42inaryDataResponse\"B\n\x14GetBinaryDataRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x18\n\x10\x62inary_data_name\x18\x02 \x01(\t\",\n\x15GetBinaryDataResponse\x12\x13\n\x0b\x62inary_data\x18\x01 \x01(\x0c\"K\n\x12\x41\x64\x64\x44ocumentRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x15\n\rdocument_name\x18\x02 \x01(\t\x12\x0c\n\x04text\x18\x03 \x01(\t\"\x15\n\x13\x41\x64\x64\x44ocumentResponse\".\n\x1aGetAllDocumentNamesRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\"5\n\x1bGetAllDocumentNamesResponse\x12\x16\n\x0e\x64ocument_names\x18\x01 \x03(\t\"A\n\x16GetDocumentTextRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x15\n\rdocument_name\x18\x02 \x01(\t\"\'\n\x17GetDocumentTextResponse\x12\x0c\n\x04text\x18\x01 \x01(\t\"E\n\x1aGetLabelIndicesInfoRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x15\n\rdocument_name\x18\x02 \x01(\t\"\xa6\x02\n\x1bGetLabelIndicesInfoResponse\x12R\n\x11label_index_infos\x18\x01 \x03(\x0b\x32\x37.mtap.api.v1.GetLabelIndicesInfoResponse.LabelIndexInfo\x1a\xb2\x01\n\x0eLabelIndexInfo\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12T\n\x04type\x18\x02 \x01(\x0e\x32\x46.mtap.api.v1.GetLabelIndicesInfoResponse.LabelIndexInfo.LabelIndexType\"6\n\x0eLabelIndexType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07GENERIC\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\"\xd9\x01\n\x10\x41\x64\x64LabelsRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x15\n\rdocument_name\x18\x02 \x01(\t\x12\x12\n\nindex_name\x18\x03 \x01(\t\x12\x34\n\x0egeneric_labels\x18\x04 \x01(\x0b\x32\x1a.mtap.api.v1.GenericLabelsH\x00\x12-\n\rcustom_labels\x18\x05 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x12\x19\n\x11no_key_validation\x18\x06 \x01(\x08\x42\x08\n\x06labels\"\x13\n\x11\x41\x64\x64LabelsResponse\"O\n\x10GetLabelsRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x15\n\rdocument_name\x18\x02 \x01(\t\x12\x12\n\nindex_name\x18\x03 \x01(\t\"O\n\rGenericLabels\x12\x13\n\x0bis_distinct\x18\x01 \x01(\x08\x12)\n\x06labels\x18\x02 \x03(\x0b\x32\x19.mtap.api.v1.GenericLabel\"\xa3\x01\n\x0cGenericLabel\x12\x12\n\nidentifier\x18\x01 \x01(\r\x12\x13\n\x0bstart_index\x18\x02 \x01(\r\x12\x11\n\tend_index\x18\x03 \x01(\r\x12\'\n\x06\x66ields\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12.\n\rreference_ids\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x82\x01\n\x11GetLabelsResponse\x12\x34\n\x0egeneric_labels\x18\x01 \x01(\x0b\x32\x1a.mtap.api.v1.GenericLabelsH\x00\x12-\n\rcustom_labels\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x42\x08\n\x06labels2\xd8\x0f\n\x06\x45vents\x12\x88\x01\n\x13GetEventsInstanceId\x12\'.mtap.api.v1.GetEventsInstanceIdRequest\x1a(.mtap.api.v1.GetEventsInstanceIdResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\x12\x16/v1/events/instance_id\x12l\n\tOpenEvent\x12\x1d.mtap.api.v1.OpenEventRequest\x1a\x1e.mtap.api.v1.OpenEventResponse\" \x82\xd3\xe4\x93\x02\x1a\"\x15/v1/events/{event_id}:\x01*\x12l\n\nCloseEvent\x12\x1e.mtap.api.v1.CloseEventRequest\x1a\x1f.mtap.api.v1.CloseEventResponse\"\x1d\x82\xd3\xe4\x93\x02\x17*\x15/v1/events/{event_id}\x12\x81\x01\n\x0eGetAllMetadata\x12\".mtap.api.v1.GetAllMetadataRequest\x1a#.mtap.api.v1.GetAllMetadataResponse\"&\x82\xd3\xe4\x93\x02 \x12\x1e/v1/events/{event_id}/metadata\x12\x81\x01\n\x0b\x41\x64\x64Metadata\x12\x1f.mtap.api.v1.AddMetadataRequest\x1a .mtap.api.v1.AddMetadataResponse\"/\x82\xd3\xe4\x93\x02)\"$/v1/events/{event_id}/metadata/{key}:\x01*\x12\x8c\x01\n\x0b\x41\x64\x64\x44ocument\x12\x1f.mtap.api.v1.AddDocumentRequest\x1a .mtap.api.v1.AddDocumentResponse\":\x82\xd3\xe4\x93\x02\x34\"//v1/events/{event_id}/documents/{document_name}:\x01*\x12\x91\x01\n\x13GetAllDocumentNames\x12\'.mtap.api.v1.GetAllDocumentNamesRequest\x1a(.mtap.api.v1.GetAllDocumentNamesResponse\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/v1/events/{event_id}/documents\x12\x95\x01\n\x0fGetDocumentText\x12#.mtap.api.v1.GetDocumentTextRequest\x1a$.mtap.api.v1.GetDocumentTextResponse\"7\x82\xd3\xe4\x93\x02\x31\x12//v1/events/{event_id}/documents/{document_name}\x12\xa8\x01\n\x13GetLabelIndicesInfo\x12\'.mtap.api.v1.GetLabelIndicesInfoRequest\x1a(.mtap.api.v1.GetLabelIndicesInfoResponse\">\x82\xd3\xe4\x93\x02\x38\x12\x36/v1/events/{event_id}/documents/{document_name}/labels\x12\x9a\x01\n\tAddLabels\x12\x1d.mtap.api.v1.AddLabelsRequest\x1a\x1e.mtap.api.v1.AddLabelsResponse\"N\x82\xd3\xe4\x93\x02H\"C/v1/events/{event_id}/documents/{document_name}/labels/{index_name}:\x01*\x12\x97\x01\n\tGetLabels\x12\x1d.mtap.api.v1.GetLabelsRequest\x1a\x1e.mtap.api.v1.GetLabelsResponse\"K\x82\xd3\xe4\x93\x02\x45\x12\x43/v1/events/{event_id}/documents/{document_name}/labels/{index_name}\x12\x96\x01\n\x15GetAllBinaryDataNames\x12).mtap.api.v1.GetAllBinaryDataNamesRequest\x1a*.mtap.api.v1.GetAllBinaryDataNamesResponse\"&\x82\xd3\xe4\x93\x02 \x12\x1e/v1/events/{event_id}/binaries\x12\x94\x01\n\rAddBinaryData\x12!.mtap.api.v1.AddBinaryDataRequest\x1a\".mtap.api.v1.AddBinaryDataResponse\"<\x82\xd3\xe4\x93\x02\x36\"1/v1/events/{event_id}/binaries/{binary_data_name}:\x01*\x12\x91\x01\n\rGetBinaryData\x12!.mtap.api.v1.GetBinaryDataRequest\x1a\".mtap.api.v1.GetBinaryDataResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/v1/events/{event_id}/binaries/{binary_data_name}B\x1b\n\x19\x65\x64u.umn.nlpie.mtap.api.v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18mtap/api/v1/events.proto\x12\x0bmtap.api.v1\x1a\x1cgoogle/api/annotations.proto\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x1c\n\x1aGetEventsInstanceIdRequest\"2\n\x1bGetEventsInstanceIdResponse\x12\x13\n\x0binstance_id\x18\x01 \x01(\t\"p\n\x10OpenEventRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x17\n\x0fonly_create_new\x18\x02 \x01(\x08\x12\x31\n\x0elease_duration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\"6\n\x11OpenEventResponse\x12\x0f\n\x07\x63reated\x18\x01 \x01(\x08\x12\x10\n\x08lease_id\x18\x02 \x01(\x05\"7\n\x11\x43loseEventRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x10\n\x08lease_id\x18\x02 \x01(\x05\"%\n\x12\x43loseEventResponse\x12\x0f\n\x07\x64\x65leted\x18\x01 \x01(\x08\")\n\x15GetAllMetadataRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\"\x8e\x01\n\x16GetAllMetadataResponse\x12\x43\n\x08metadata\x18\x01 \x03(\x0b\x32\x31.mtap.api.v1.GetAllMetadataResponse.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"B\n\x12\x41\x64\x64MetadataRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\x15\n\x13\x41\x64\x64MetadataResponse\"0\n\x1cGetAllBinaryDataNamesRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\":\n\x1dGetAllBinaryDataNamesResponse\x12\x19\n\x11\x62inary_data_names\x18\x01 \x03(\t\"W\n\x14\x41\x64\x64\x42inaryDataRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x18\n\x10\x62inary_data_name\x18\x02 \x01(\t\x12\x13\n\x0b\x62inary_data\x18\x03 \x01(\x0c\"\x17\n\x15\x41\x64\x64\x42inaryDataResponse\"B\n\x14GetBinaryDataRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x18\n\x10\x62inary_data_name\x18\x02 \x01(\t\",\n\x15GetBinaryDataResponse\x12\x13\n\x0b\x62inary_data\x18\x01 \x01(\x0c\"K\n\x12\x41\x64\x64\x44ocumentRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x15\n\rdocument_name\x18\x02 \x01(\t\x12\x0c\n\x04text\x18\x03 \x01(\t\"\x15\n\x13\x41\x64\x64\x44ocumentResponse\".\n\x1aGetAllDocumentNamesRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\"5\n\x1bGetAllDocumentNamesResponse\x12\x16\n\x0e\x64ocument_names\x18\x01 \x03(\t\"A\n\x16GetDocumentTextRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x15\n\rdocument_name\x18\x02 \x01(\t\"\'\n\x17GetDocumentTextResponse\x12\x0c\n\x04text\x18\x01 \x01(\t\"E\n\x1aGetLabelIndicesInfoRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x15\n\rdocument_name\x18\x02 \x01(\t\"\xa6\x02\n\x1bGetLabelIndicesInfoResponse\x12R\n\x11label_index_infos\x18\x01 \x03(\x0b\x32\x37.mtap.api.v1.GetLabelIndicesInfoResponse.LabelIndexInfo\x1a\xb2\x01\n\x0eLabelIndexInfo\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12T\n\x04type\x18\x02 \x01(\x0e\x32\x46.mtap.api.v1.GetLabelIndicesInfoResponse.LabelIndexInfo.LabelIndexType\"6\n\x0eLabelIndexType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07GENERIC\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\"\xd9\x01\n\x10\x41\x64\x64LabelsRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x15\n\rdocument_name\x18\x02 \x01(\t\x12\x12\n\nindex_name\x18\x03 \x01(\t\x12\x34\n\x0egeneric_labels\x18\x04 \x01(\x0b\x32\x1a.mtap.api.v1.GenericLabelsH\x00\x12-\n\rcustom_labels\x18\x05 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x12\x19\n\x11no_key_validation\x18\x06 \x01(\x08\x42\x08\n\x06labels\"\x13\n\x11\x41\x64\x64LabelsResponse\"O\n\x10GetLabelsRequest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\t\x12\x15\n\rdocument_name\x18\x02 \x01(\t\x12\x12\n\nindex_name\x18\x03 \x01(\t\"O\n\rGenericLabels\x12\x13\n\x0bis_distinct\x18\x01 \x01(\x08\x12)\n\x06labels\x18\x02 \x03(\x0b\x32\x19.mtap.api.v1.GenericLabel\"\xa3\x01\n\x0cGenericLabel\x12\x12\n\nidentifier\x18\x01 \x01(\r\x12\x13\n\x0bstart_index\x18\x02 \x01(\r\x12\x11\n\tend_index\x18\x03 \x01(\r\x12\'\n\x06\x66ields\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12.\n\rreference_ids\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x82\x01\n\x11GetLabelsResponse\x12\x34\n\x0egeneric_labels\x18\x01 \x01(\x0b\x32\x1a.mtap.api.v1.GenericLabelsH\x00\x12-\n\rcustom_labels\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x42\x08\n\x06labels2\xd8\x0f\n\x06\x45vents\x12\x88\x01\n\x13GetEventsInstanceId\x12\'.mtap.api.v1.GetEventsInstanceIdRequest\x1a(.mtap.api.v1.GetEventsInstanceIdResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\x12\x16/v1/events/instance_id\x12l\n\tOpenEvent\x12\x1d.mtap.api.v1.OpenEventRequest\x1a\x1e.mtap.api.v1.OpenEventResponse\" \x82\xd3\xe4\x93\x02\x1a\"\x15/v1/events/{event_id}:\x01*\x12l\n\nCloseEvent\x12\x1e.mtap.api.v1.CloseEventRequest\x1a\x1f.mtap.api.v1.CloseEventResponse\"\x1d\x82\xd3\xe4\x93\x02\x17*\x15/v1/events/{event_id}\x12\x81\x01\n\x0eGetAllMetadata\x12\".mtap.api.v1.GetAllMetadataRequest\x1a#.mtap.api.v1.GetAllMetadataResponse\"&\x82\xd3\xe4\x93\x02 \x12\x1e/v1/events/{event_id}/metadata\x12\x81\x01\n\x0b\x41\x64\x64Metadata\x12\x1f.mtap.api.v1.AddMetadataRequest\x1a .mtap.api.v1.AddMetadataResponse\"/\x82\xd3\xe4\x93\x02)\"$/v1/events/{event_id}/metadata/{key}:\x01*\x12\x8c\x01\n\x0b\x41\x64\x64\x44ocument\x12\x1f.mtap.api.v1.AddDocumentRequest\x1a .mtap.api.v1.AddDocumentResponse\":\x82\xd3\xe4\x93\x02\x34\"//v1/events/{event_id}/documents/{document_name}:\x01*\x12\x91\x01\n\x13GetAllDocumentNames\x12\'.mtap.api.v1.GetAllDocumentNamesRequest\x1a(.mtap.api.v1.GetAllDocumentNamesResponse\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/v1/events/{event_id}/documents\x12\x95\x01\n\x0fGetDocumentText\x12#.mtap.api.v1.GetDocumentTextRequest\x1a$.mtap.api.v1.GetDocumentTextResponse\"7\x82\xd3\xe4\x93\x02\x31\x12//v1/events/{event_id}/documents/{document_name}\x12\xa8\x01\n\x13GetLabelIndicesInfo\x12\'.mtap.api.v1.GetLabelIndicesInfoRequest\x1a(.mtap.api.v1.GetLabelIndicesInfoResponse\">\x82\xd3\xe4\x93\x02\x38\x12\x36/v1/events/{event_id}/documents/{document_name}/labels\x12\x9a\x01\n\tAddLabels\x12\x1d.mtap.api.v1.AddLabelsRequest\x1a\x1e.mtap.api.v1.AddLabelsResponse\"N\x82\xd3\xe4\x93\x02H\"C/v1/events/{event_id}/documents/{document_name}/labels/{index_name}:\x01*\x12\x97\x01\n\tGetLabels\x12\x1d.mtap.api.v1.GetLabelsRequest\x1a\x1e.mtap.api.v1.GetLabelsResponse\"K\x82\xd3\xe4\x93\x02\x45\x12\x43/v1/events/{event_id}/documents/{document_name}/labels/{index_name}\x12\x96\x01\n\x15GetAllBinaryDataNames\x12).mtap.api.v1.GetAllBinaryDataNamesRequest\x1a*.mtap.api.v1.GetAllBinaryDataNamesResponse\"&\x82\xd3\xe4\x93\x02 \x12\x1e/v1/events/{event_id}/binaries\x12\x94\x01\n\rAddBinaryData\x12!.mtap.api.v1.AddBinaryDataRequest\x1a\".mtap.api.v1.AddBinaryDataResponse\"<\x82\xd3\xe4\x93\x02\x36\"1/v1/events/{event_id}/binaries/{binary_data_name}:\x01*\x12\x91\x01\n\rGetBinaryData\x12!.mtap.api.v1.GetBinaryDataRequest\x1a\".mtap.api.v1.GetBinaryDataResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/v1/events/{event_id}/binaries/{binary_data_name}B(\n\x19\x65\x64u.umn.nlpie.mtap.api.v1Z\x0bmtap/api/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'mtap.api.v1.events_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\031edu.umn.nlpie.mtap.api.v1'
+  DESCRIPTOR._serialized_options = b'\n\031edu.umn.nlpie.mtap.api.v1Z\013mtap/api/v1'
   _GETALLMETADATARESPONSE_METADATAENTRY._options = None
   _GETALLMETADATARESPONSE_METADATAENTRY._serialized_options = b'8\001'
   _EVENTS.methods_by_name['GetEventsInstanceId']._options = None
   _EVENTS.methods_by_name['GetEventsInstanceId']._serialized_options = b'\202\323\344\223\002\030\022\026/v1/events/instance_id'
   _EVENTS.methods_by_name['OpenEvent']._options = None
   _EVENTS.methods_by_name['OpenEvent']._serialized_options = b'\202\323\344\223\002\032\"\025/v1/events/{event_id}:\001*'
   _EVENTS.methods_by_name['CloseEvent']._options = None
```

### Comparing `mtap-1.1.0/python/mtap/api/v1/events_pb2_grpc.py` & `mtap-1.2.0/python/mtap/api/v1/events_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/api/v1/processing_pb2.py` & `mtap-1.2.0/python/mtap/api/v1/processing_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cmtap/api/v1/processing.proto\x12\x0bmtap.api.v1\x1a\x1cgoogle/api/annotations.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\"9\n\x0c\x43reatedIndex\x12\x15\n\rdocument_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"\x84\x01\n\x0eProcessRequest\x12\x14\n\x0cprocessor_id\x18\x01 \x01(\t\x12\x10\n\x08\x65vent_id\x18\x02 \x01(\t\x12!\n\x19\x65vent_service_instance_id\x18\x04 \x01(\t\x12\'\n\x06params\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xff\x01\n\x0fProcessResponse\x12\x41\n\x0btiming_info\x18\x01 \x03(\x0b\x32,.mtap.api.v1.ProcessResponse.TimingInfoEntry\x12\'\n\x06result\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x32\n\x0f\x63reated_indices\x18\x03 \x03(\x0b\x32\x19.mtap.api.v1.CreatedIndex\x1aL\n\x0fTimingInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration:\x02\x38\x01\"&\n\x0eGetInfoRequest\x12\x14\n\x0cprocessor_id\x18\x01 \x01(\t\"<\n\x0fGetInfoResponse\x12)\n\x08metadata\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xd5\x01\n\nTimerStats\x12\'\n\x04mean\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12&\n\x03std\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12&\n\x03max\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12&\n\x03min\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\x12&\n\x03sum\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\"\'\n\x0fGetStatsRequest\x12\x14\n\x0cprocessor_id\x18\x01 \x01(\t\"\xca\x01\n\x10GetStatsResponse\x12\x11\n\tprocessed\x18\x01 \x01(\x05\x12\x10\n\x08\x66\x61ilures\x18\x02 \x01(\x05\x12\x44\n\x0ctiming_stats\x18\x03 \x03(\x0b\x32..mtap.api.v1.GetStatsResponse.TimingStatsEntry\x1aK\n\x10TimingStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.mtap.api.v1.TimerStats:\x02\x38\x01\x32\xf7\x02\n\tProcessor\x12\x81\x01\n\x07Process\x12\x1b.mtap.api.v1.ProcessRequest\x1a\x1c.mtap.api.v1.ProcessResponse\";\x82\xd3\xe4\x93\x02\x35\"0/v1/processors/{processor_id}/process/{event_id}:\x01*\x12p\n\x07GetInfo\x12\x1b.mtap.api.v1.GetInfoRequest\x1a\x1c.mtap.api.v1.GetInfoResponse\"*\x82\xd3\xe4\x93\x02$\x12\"/v1/processors/{processor_id}/info\x12t\n\x08GetStats\x12\x1c.mtap.api.v1.GetStatsRequest\x1a\x1d.mtap.api.v1.GetStatsResponse\"+\x82\xd3\xe4\x93\x02%\x12#/v1/processors/{processor_id}/statsB\x1b\n\x19\x65\x64u.umn.nlpie.mtap.api.v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cmtap/api/v1/processing.proto\x12\x0bmtap.api.v1\x1a\x1cgoogle/api/annotations.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\"9\n\x0c\x43reatedIndex\x12\x15\n\rdocument_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"\x84\x01\n\x0eProcessRequest\x12\x14\n\x0cprocessor_id\x18\x01 \x01(\t\x12\x10\n\x08\x65vent_id\x18\x02 \x01(\t\x12!\n\x19\x65vent_service_instance_id\x18\x04 \x01(\t\x12\'\n\x06params\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xff\x01\n\x0fProcessResponse\x12\x41\n\x0btiming_info\x18\x01 \x03(\x0b\x32,.mtap.api.v1.ProcessResponse.TimingInfoEntry\x12\'\n\x06result\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x32\n\x0f\x63reated_indices\x18\x03 \x03(\x0b\x32\x19.mtap.api.v1.CreatedIndex\x1aL\n\x0fTimingInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration:\x02\x38\x01\"&\n\x0eGetInfoRequest\x12\x14\n\x0cprocessor_id\x18\x01 \x01(\t\"<\n\x0fGetInfoResponse\x12)\n\x08metadata\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xd5\x01\n\nTimerStats\x12\'\n\x04mean\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12&\n\x03std\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12&\n\x03max\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12&\n\x03min\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\x12&\n\x03sum\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\"\'\n\x0fGetStatsRequest\x12\x14\n\x0cprocessor_id\x18\x01 \x01(\t\"\xca\x01\n\x10GetStatsResponse\x12\x11\n\tprocessed\x18\x01 \x01(\x05\x12\x10\n\x08\x66\x61ilures\x18\x02 \x01(\x05\x12\x44\n\x0ctiming_stats\x18\x03 \x03(\x0b\x32..mtap.api.v1.GetStatsResponse.TimingStatsEntry\x1aK\n\x10TimingStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.mtap.api.v1.TimerStats:\x02\x38\x01\x32\xf7\x02\n\tProcessor\x12\x81\x01\n\x07Process\x12\x1b.mtap.api.v1.ProcessRequest\x1a\x1c.mtap.api.v1.ProcessResponse\";\x82\xd3\xe4\x93\x02\x35\"0/v1/processors/{processor_id}/process/{event_id}:\x01*\x12p\n\x07GetInfo\x12\x1b.mtap.api.v1.GetInfoRequest\x1a\x1c.mtap.api.v1.GetInfoResponse\"*\x82\xd3\xe4\x93\x02$\x12\"/v1/processors/{processor_id}/info\x12t\n\x08GetStats\x12\x1c.mtap.api.v1.GetStatsRequest\x1a\x1d.mtap.api.v1.GetStatsResponse\"+\x82\xd3\xe4\x93\x02%\x12#/v1/processors/{processor_id}/statsB(\n\x19\x65\x64u.umn.nlpie.mtap.api.v1Z\x0bmtap/api/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'mtap.api.v1.processing_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\031edu.umn.nlpie.mtap.api.v1'
+  DESCRIPTOR._serialized_options = b'\n\031edu.umn.nlpie.mtap.api.v1Z\013mtap/api/v1'
   _PROCESSRESPONSE_TIMINGINFOENTRY._options = None
   _PROCESSRESPONSE_TIMINGINFOENTRY._serialized_options = b'8\001'
   _GETSTATSRESPONSE_TIMINGSTATSENTRY._options = None
   _GETSTATSRESPONSE_TIMINGSTATSENTRY._serialized_options = b'8\001'
   _PROCESSOR.methods_by_name['Process']._options = None
   _PROCESSOR.methods_by_name['Process']._serialized_options = b'\202\323\344\223\0025\"0/v1/processors/{processor_id}/process/{event_id}:\001*'
   _PROCESSOR.methods_by_name['GetInfo']._options = None
```

### Comparing `mtap-1.1.0/python/mtap/api/v1/processing_pb2_grpc.py` & `mtap-1.2.0/python/mtap/api/v1/processing_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/constants.py` & `mtap-1.2.0/python/mtap/constants.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/data/__init__.py` & `mtap-1.2.0/python/mtap/data/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,28 +8,25 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """Module for MTAP's Data Model
-
-Attributes:
-    GENERIC_ADAPTER (~mtap.data.ProtoLabelAdapter): label adapter used for standard
-        (non-distinct) :obj:`~mtap.GenericLabel`.
-    DISTINCT_GENERIC_ADAPTER (~mtap.data.ProtoLabelAdapter): label adapter used for distinct
-        (non-overlapping) :obj:`~mtap.GenericLabel`.
 """
 
 from mtap.data._base import LabelIndexType, LabelIndexInfo
 from mtap.data._events import (
     Document,
     Event,
+    EventsAddressLike,
     EventsClient,
     Labeler,
+    LabelAdapters,
+    FailedToConnectToEventsServiceException,
 )
 from mtap.data._label_adapters import (
     GENERIC_ADAPTER,
     DISTINCT_GENERIC_ADAPTER,
     ProtoLabelAdapter,
 )
 from mtap.data._label_indices import (
```

### Comparing `mtap-1.1.0/python/mtap/data/_base.py` & `mtap-1.2.0/python/mtap/data/_base.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/data/_events.py` & `mtap-1.2.0/python/mtap/data/_events.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,187 +8,238 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """Events service client API and wrapper classes.
-
 """
 
-import collections
 import threading
 import uuid
 from typing import (
+    Any,
     Iterator,
     List,
     Dict,
     MutableMapping,
     Generic,
     TypeVar,
-    NamedTuple,
     ContextManager,
     Iterable,
     Optional,
     Sequence,
     Union,
     Mapping,
     TYPE_CHECKING,
     Callable,
+    overload,
 )
 
 import grpc
-from grpc_health.v1 import health_pb2_grpc, health_pb2
 
-from mtap import _config, _discovery, constants
+from mtap import _config, constants
 from mtap.api.v1 import events_pb2, events_pb2_grpc
-from mtap.data import _base, _labels, _label_adapters
+from mtap.data import _base, _label_adapters
+from mtap.data._label_adapters import ProtoLabelAdapter
 
 if TYPE_CHECKING:
     import mtap
     import mtap.data as data
 
 L = TypeVar('L', bound='data.Label')
+EventsAddressLike = Union[str, Iterable[str], None]
 
 
 class Event:
-    """An object for interacting with a specific event locally or on the events service.
+    """An object for interacting with a specific event locally or on the
+    events service.
 
-    The Event object functions as a map from string document names to :obj:`Document` objects that
-    can be used to access document data from the events server.
+    The Event object functions as a map from string document names to
+    :obj:`Document` objects that can be used to access document data from the
+    events server.
+
+    To connect to the events service and load an existing event, all of
+    ``event_id``, ``event_service_instance_id``, and ``client`` must be
+    specified.
 
-    Keyword Args:
-        event_id (~typing.Optional[str]):
-            A globally-unique identifier for the event, or omit / none for a random UUID.
-        client (~typing.Optional[EventsClient]):
-            A client for an events service to push any changes to the event to.
-        only_create_new (bool): Fails if the event already exists on the events service.
+    Args:
+        event_id: A globally-unique identifier for the event, or omit / none
+            for a random UUID.
+        event_service_instance_id: A global-unique identifier for the events
+            service instance that the event lives on.
+        client: If specified, connects to the events service with id
+            ``event_service_instance_id`` and accesses either accesses the
+            existing event with the ``event_id`` or creates a new one.
+        only_create_new: Fails if the event already exists on the events
+            service.
+
+    Attributes:
+        label_adapters: A mapping of string label index names to
+            :class:`ProtoLabelAdapter` instances to perform custom
+            mapping of label types.
 
     Examples:
-        >>> with EventsClient() as c, Event(event_id='id', client=c) as event:
+        Creating a new event locally.
+
+        >>> event = Event()
+
+        Creating a new event remotely.
+
+        >>> with EventsClient(address='localohost:50000') as c, \
+        >>>     Event(event_id='id', client=c) as event:
         >>>     # use event
         >>>     ...
-    """
-    __slots__ = ('_event_id', '_client', '_lock', 'default_adapters', '_documents', '_metadata',
-                 '_binaries', '_event_service_instance_id')
 
-    def __init__(self, *, event_id: Optional[str] = None,
-                 event_service_instance_id: Optional[str] = None,
-                 client: Optional['mtap.EventsClient'] = None,
-                 only_create_new: bool = False,
-                 default_adapters: Optional[Mapping[str, 'data.ProtoLabelAdapter']] = None):
+        Connecting to an existing event.
+
+        >>> with EventsClient(address='localohost:50000') as c, \
+        >>>     Event(event_id='id',
+        >>>           event_service_instance_id='events_sid',
+        >>>           client=c) as event:
+        >>>
+        >>>
+    """
+    __slots__ = ('_event_id', '_client', '_lock', 'label_adapters',
+                 '_documents', '_metadata', '_binaries',
+                 '_event_service_instance_id')
+
+    label_adapters: 'Dict[str, ProtoLabelAdapter]'
+
+    def __init__(
+            self,
+            *, event_id: Optional[str] = None,
+            event_service_instance_id: Optional[str] = None,
+            client: 'Optional[mtap.EventsClient]' = None,
+            only_create_new: bool = False,
+            label_adapters: 'Optional[Mapping[str, ProtoLabelAdapter]]'
+            = None
+    ):
         self._event_id = event_id or str(uuid.uuid4())
         self._event_service_instance_id = event_service_instance_id
         self._lock = threading.RLock()
-        self.default_adapters = default_adapters or {}
+        if label_adapters is not None:
+            self.label_adapters = dict(label_adapters)
+        else:
+            self.label_adapters = {}
         self._client = client
         if self._client is not None:
-            self._client = client.get_local_instance(self._event_service_instance_id)
+            self._client = client.get_local_instance(
+                self._event_service_instance_id
+            )
             self._event_service_instance_id = self._client.instance_id
-            self._client.open_event(self._event_id, only_create_new=only_create_new)
+            self._client.open_event(self._event_id,
+                                    only_create_new=only_create_new)
 
     @property
-    def client(self) -> Optional['mtap.EventsClient']:
+    def client(self) -> 'Optional[mtap.EventsClient]':
         return self._client
 
     @property
     def event_id(self) -> str:
-        """str: The globally unique identifier for this event."""
+        """The globally unique identifier for this event."""
         return self._event_id
 
     @property
     def event_service_instance_id(self) -> str:
-        """str: The unique instance identifier for this event's paired event service."""
+        """The unique instance identifier for this event's paired event
+        service."""
         return self._event_service_instance_id
 
     @property
-    def documents(self) -> MutableMapping[str, 'mtap.Document']:
-        """~typing.MutableMapping[str, Document]: A mutable mapping of strings to :obj:`Document`
-        objects that can be used to query and add documents to the event."""
+    def documents(self) -> 'MutableMapping[str, mtap.Document]':
+        """A mutable mapping of strings to :obj:`Document` objects that can be
+        used to query and add documents to the event."""
         try:
             return self._documents
         except AttributeError:
             self._documents = _Documents(self, self.client)
             return self._documents
 
     @property
     def metadata(self) -> MutableMapping[str, str]:
-        """~typing.MutableMapping[str, str]: A mutable mapping of strings to strings that can be
-        used to query and add metadata to the event."""
+        """A mutable mapping of strings to strings that can be used to query
+        and add metadata to the event."""
         try:
             return self._metadata
         except AttributeError:
             self._metadata = _Metadata(self, self.client)
             return self._metadata
 
     @property
     def binaries(self) -> MutableMapping[str, bytes]:
-        """~typing.MutableMapping[str, str]: A mutable mapping of strings to bytes that can be used
-        to query and add binary data to the event."""
+        """A mutable mapping of strings to bytes that can be used to query and
+        add binary data to the event."""
         try:
             return self._binaries
         except AttributeError:
             self._binaries = _Binaries(self, self.client)
             return self._binaries
 
     @property
     def created_indices(self) -> Dict[str, List[str]]:
-        """~typing.Dict[str, ~typing.List[str]]: A mapping of document names to a list of the names
-        of all the label indices that have been added to that document"""
+        """A mapping of document names to a list of the names of all the label
+        indices that have been added to that document"""
         return {document_name: document.created_indices
                 for document_name, document in self.documents.items()}
 
     def close(self):
-        """Closes this event. Lets the event service know that we are done with the event,
-        allowing to clean up the event if no other clients have open leases to it."""
+        """Closes this event. Lets the event service know that we are done
+        with the event, allowing to clean up the event if no other clients
+        have open leases to it."""
         if self.client is not None:
             self.release_lease()
 
-    def create_document(self, document_name: str, text: str) -> 'mtap.Document':
+    def create_document(self,
+                        document_name: str,
+                        text: str) -> 'mtap.Document':
         """Adds a document to the event keyed by `document_name` and
         containing the specified `text`.
 
         Args:
-            document_name (str): The event-unique identifier for the document, example: 'plaintext'.
-            text (str):
-                The content of the document. This is a required field, document text is final and
-                immutable, as changing the text would very likely invalidate any labels on the
-                document.
+            document_name: The event-unique identifier for the document,
+                example: ``'plaintext'``.
+            text: The content of the document. This is a required field,
+                and the document text is final and immutable.
 
         Returns:
-            Document: The added document.
+            The added document.
 
         Examples:
 
             >>> event = Event()
-            >>> document = event.create_document('plaintext', text="The text of the document.")
+            >>> doc = event.create_document('plaintext',
+            >>>                             text="The text of the document.")
 
         """
         if not isinstance(text, str):
             raise ValueError('text is not string.')
-        document = Document(document_name, text=text, event=self)
+        document = Document(document_name, text=text, event=self,
+                            label_adapters=self.label_adapters)
         self.documents[document_name] = document
         return document
 
     def add_document(self, document: 'mtap.Document'):
-        """Adds the document to this event, first uploading to events service if this event has a
-        client connection to the events service.
+        """Adds the document to this event, first uploading to events service
+        if this event has a client connection to the events service.
 
         Args:
-            document (~mtap.Document): The document to add to this event.
+            document: The document to add to this event.
 
         Examples:
 
             >>> event = Event()
-            >>> document = Document('plaintext', text="The text of the document.")
-            >>> event.add_document(document)
+            >>> doc = Document('plaintext',
+            >>>                text="The text of the document.")
+            >>> event.add_document(doc)
 
         """
-        if document._event is not None:
-            raise ValueError('The document already exists on an event')
+        if document.event is not None:
+            raise ValueError('This document already has an event, it cannot '
+                             'be added to another.')
         document._event = self
         document._client = self.client
         document._event_id = self.event_id
         self.documents[document.document_name] = document
 
     def __enter__(self) -> 'Event':
         return self
@@ -209,258 +260,332 @@
             self.client.open_event(self.event_id, only_create_new=False)
 
     def release_lease(self):
         if self.client is not None:
             self.client.close_event(self.event_id)
 
 
-class _WaitingIndex(NamedTuple('_WaitingIndex',
-                               [('index_name', str),
-                                ('labels', List['mtap.GenericLabel']),
-                                ('waiting_on', List[int])])):
-    """A label index that is waiting on some labels to be staticized before uploading.
-    """
+LabelAdapters = Mapping[str, ProtoLabelAdapter]
 
 
 class Document:
-    """An object for interacting with text and labels stored on an :class:`Event`.
+    """An object for interacting with text and labels stored on an
+    :class:`Event`.
 
-    Documents are keyed by their name, and pipelines can store different pieces of
-    related text on a single processing event using multiple documents. An example would be storing
-    the text of one language on one document, and a translation on another, or storing the
-    rtf or html encoding on one document, and the parsed plaintext on another document.
-
-    Both the document text and any added label indices are immutable. This is to enable
-    parallelization and distribution of processing, and to prevent changes to the dependency graph
-    of label indices and text, which can make debugging difficult.
+    Documents are keyed by their name, and pipelines can store different
+    pieces of related text on a single processing event using multiple
+    documents. An example would be storing the text of one language on one
+    document, and a translation on another, or storing the rtf or html
+    encoding on one document (or as a binary in :method:`Event.binaries`, and
+    the parsed plaintext on another document.
+
+    Both the document text and any added label indices are immutable. This is
+    to enable parallelization and distribution of processing, and because other
+    label indices might be downstream dependents on the earlier created labels.
 
     Args:
-        document_name (str): The document name identifier.
-
-    Keyword Args:
-        text (~typing.Optional[str]):
-            The document text, can be omitted if this is an existing document and text needs to be
-            retrieved from the events service.
-        event (~typing.Optional[Event]):
-            The parent event of this document. If the event has a client, then that client will be
-            used to share changes to this document with all other clients of the Events service. In
-            that case, text should only be specified if it is the known existing text of the
+        document_name: The document name identifier.
+        text: The document text, can be omitted if this is an existing
+            document and text needs to be retrieved from the events service.
+        event: The parent event of this document. If the event has a client,
+            then that client will be used to share changes to this document
+            with all other clients of the Events service. In that case, text
+            should only be specified if it is the known existing text of the
             document.
 
     Examples:
         Local document:
 
         >>> document = Document('plaintext', text='Some document text.')
 
         Existing distributed object:
 
-        >>> with EventsClient(address='localhost:8080') as client, \\
-        >>>      Event(event_id='1', client=client) as event:
+        >>> with EventsClient(address='localhost:8080') as client, \
+        >>>      Event(event_id='1',
+        >>>            event_service_instance_id='events_sid',
+        >>>            client=client) as event:
         >>>     document = event.documents['plaintext']
         >>>     document.text
         'Some document text fetched from the server.'
 
         New distributed object:
 
-        >>> with EventsClient(address='localhost:8080') as client, \\
+        >>> with EventsClient(address='localhost:8080') as client, \
         >>>      Event(event_id='1', client=client) as event:
         >>>     document = Document('plaintext', text='Some document text.')
         >>>     event.add_document(document)
 
         or
 
-        >>> with EventsClient(address='localhost:8080') as client, \\
+        >>> with EventsClient(address='localhost:8080') as client, \
         >>>      Event(event_id='1', client=client) as event:
-        >>>     document = event.create_document('plaintext', text='Some document text.')
+        >>>     document = event.create_document('plaintext',
+        >>>                                      text='Some document text.')
 
     """
-    __slots__ = ('_document_name', '_event', '_client', '_event_id', '_text', '_labelers',
-                 '_created_indices', '_waiting_indices', 'default_adapters', '_labels')
-
-    def __init__(self,
-                 document_name: str,
-                 *,
-                 text: Optional[str] = None,
-                 event: Optional[Event] = None,
-                 default_adapters: Optional[Mapping[str, 'data.ProtoLabelAdapter']] = None):
+    __slots__ = (
+        '_document_name',
+        '_event',
+        '_client',
+        '_event_id',
+        '_text',
+        '_labelers',
+        '_created_indices',
+        '_waiting_indices',
+        'label_adapters',
+        '_labels',
+    )
+
+    @overload
+    def __init__(
+            self,
+            document_name: str,
+            *, text: str,
+            label_adapters: Optional[LabelAdapters] = None
+    ):
+        ...
+
+    @overload
+    def __init__(
+            self,
+            document_name: str,
+            *, event: Event,
+            label_adapters: Optional[LabelAdapters] = None
+    ):
+        pass
+
+    @overload
+    def __init__(
+            self,
+            document_name: str,
+            *, text: str,
+            event: Event,
+            label_adapters: Optional[LabelAdapters] = None
+    ):
+        pass
+
+    def __init__(
+            self,
+            document_name: str,
+            *, text: Optional[str] = None,
+            event: Optional[Event] = None,
+            label_adapters: Optional[LabelAdapters] = None
+    ):
         if not isinstance(document_name, str):
             raise TypeError('Document name is not string.')
         self._document_name = document_name
         self._event = event
         self._client = None
         self._event_id = None
         if event is not None:
             self._client = event.client
             self._event_id = event.event_id
         self._text = text
         self._labelers = []
         self._created_indices = []
         self._waiting_indices = []
-        self.default_adapters = default_adapters or {}
+        self.label_adapters = label_adapters or {}
         if self._client is None and text is None:
-            raise ValueError('Document without text or an event with a client to fetch the text '
-                             'from.')
+            raise ValueError(
+                'Document must either be an existing document (event.client '
+                'is not None) or must have the text parameter specified.'
+            )
 
     @property
     def event(self) -> Event:
-        """Event: The parent event of this document."""
+        """The parent event of this document."""
         return self._event
 
     @property
     def document_name(self) -> str:
-        """str: The unique identifier for this document on the event."""
+        """The unique identifier for this document on the event."""
         return self._document_name
 
     @property
     def text(self):
-        """str: The document text."""
+        """The document text."""
         if self._text is None and self._client is not None:
-            self._text = self._client.get_document_text(self._event_id, self._document_name)
+            self._text = self._client.get_document_text(self._event_id,
+                                                        self._document_name)
         return self._text
 
     @property
     def created_indices(self) -> List[str]:
-        """~typing.List[str]: A list of all of the label index names that have created on this
-                document using a labeler either locally or by remote pipeline components invoked on
-                this document."""
+        """A list of all the label index names that have been created on this
+        document using a labeler either locally or by remote pipeline
+        components invoked on this document."""
         return list(self._created_indices)
 
     @property
-    def labels(self) -> Mapping[str, 'data.LabelIndex']:
+    def labels(self) -> 'Mapping[str, data.LabelIndex]':
+        return self._label_indices
+
+    @property
+    def _label_indices(self) -> '_LabelIndices':
         try:
             return self._labels
         except AttributeError:
             self._labels = _LabelIndices(self)
             return self._labels
 
-    def get_label_index(self,
-                        label_index_name: str) -> 'data.LabelIndex[Union[mtap.GenericLabel, L]]':
+    def get_label_index(
+            self,
+            label_index_name: str
+    ) -> 'data.LabelIndex':
         """Gets the document's label index with the specified key.
 
-        Will fetch from the events service if it is not cached locally if the document has an event
-        with a client. Uses the `label_adapter` argument to perform unmarshalling from the proto
-        message if specified.
+        Will fetch from the events service if it is not cached locally if the
+        document has an event with a client. Uses the `label_adapter` argument
+        to perform unmarshalling from the proto message if specified.
 
         Args:
-            label_index_name (str): The name of the label index to get.
+            label_index_name: The name of the label index to get.
 
         Returns:
-            LabelIndex: The requested label index.
+            The requested label index.
         """
         return self.labels[label_index_name]
 
-    def get_labeler(self,
-                    label_index_name: str,
-                    *, distinct: Optional[bool] = None):
+    def get_labeler(
+            self,
+            label_index_name: str,
+            *, distinct: Optional[bool] = None
+    ) -> 'Callable[[Any, ...], mtap.GenericLabel]':
         """Creates a function that can be used to add labels to a label index.
 
         Args:
-            label_index_name (str): A document-unique identifier for the label index to be created.
-            distinct (~typing.Optional[bool]):
-                Optional, if using generic labels, whether to use distinct generic labels or
-                non-distinct generic labels, will default to False.
+            label_index_name: An identifying name for the label index.
+            distinct: Optional, if using generic labels, whether to use
+                distinct generic labels or non-distinct generic labels, will
+                default to False. Distinct labels are non-overlapping and
+                can use faster binary search indices.
 
         Returns:
-            Labeler: A callable when used in conjunction with the 'with' keyword will automatically
-            handle uploading any added labels to the server.
+            A callable when used in conjunction with the 'with' keyword will
+            automatically handle uploading any added labels to the server.
 
         Examples:
-            >>> with document.get_labeler('sentences', distinct=True) as labeler:
+            >>> with document.get_labeler('sentences',
+            >>>                           distinct=True) as labeler:
             >>>     labeler(0, 25, sentence_type='STANDARD')
             >>>     sentence = labeler(26, 34)
             >>>     sentence.sentence_type = 'FRAGMENT'
         """
         if label_index_name in self._labelers:
             raise KeyError("Labeler already in use: " + label_index_name)
         label_adapter = self.get_default_adapter(label_index_name, distinct)
 
         labeler = Labeler(self._client, self, label_index_name, label_adapter)
         self._labelers.append(label_index_name)
         return labeler
 
     def add_labels(self,
                    label_index_name: str,
-                   labels: Sequence[Union['data.Label', L]],
+                   labels: 'Sequence[L]',
                    *, distinct: Optional[bool] = None,
-                   label_adapter: Optional['data.ProtoLabelAdapter'] = None):
-        """Skips using a labeler and adds the sequence of labels as a new label index.
+                   label_adapter: 'Optional[ProtoLabelAdapter]' = None):
+        """Skips using a labeler and adds the sequence of labels as a new
+        label index.
 
         Args:
-            label_index_name (str): The name of the label index.
-            labels (~typing.Sequence[Label]): The labels to add.
-            distinct (~typing.Optional[bool]):
-                Whether the index is distinct or non-distinct.
-            label_adapter (mtap.label_adapters.ProtoLabelAdapter): A label adapter to use.
+            label_index_name: The name of the label index.
+            labels: The labels to add.
+            distinct: Whether the index is distinct or non-distinct.
+            label_adapter: A label adapter to use.
 
         Returns:
             LabelIndex: The new label index created from the labels.
         """
         if label_index_name in self.labels:
-            raise KeyError("Label index already exists with name: " + label_index_name)
+            raise KeyError(
+                "Label index already exists with name: " + label_index_name)
         if label_adapter is None:
             if distinct is None:
                 distinct = False
-            label_adapter = self.get_default_adapter(label_index_name, distinct)
-        labels, waiting_on = _labels._staticize(labels, self, label_index_name)
+            label_adapter = self.get_default_adapter(label_index_name,
+                                                     distinct)
+        labels = sorted(labels, key=lambda x: x.location)
+        waiting_on = set()
+        for i, lbl in enumerate(labels):
+            lbl.document = self
+            lbl.identifier = i
+            lbl.label_index_name = label_index_name
+        for lbl in labels:
+            lbl.collect_floating_references(waiting_on)
         if len(self._waiting_indices) > 0:
             label_ids = {id(label) for label in labels}
             self._check_waiting_indices(label_ids)
 
         if len(waiting_on) > 0:
-            self._waiting_indices.append((label_index_name, labels, label_adapter, waiting_on))
+            self._waiting_indices.append(
+                (label_index_name, labels, label_adapter, waiting_on))
         else:
             self._finalize_labels(label_adapter, label_index_name, labels)
 
     def _check_waiting_indices(self, updated_ids):
         waiting_indices = []
-        for label_index_name, labels, label_adapter, waiting_on in self._waiting_indices:
+        for (label_index_name,
+             labels,
+             label_adapter,
+             waiting_on) in self._waiting_indices:
             still_waiting = waiting_on.difference(updated_ids)
             if len(still_waiting) == 0:
                 self._finalize_labels(label_adapter, label_index_name, labels)
             else:
-                waiting_indices.append((label_index_name, labels, label_adapter, still_waiting))
+                waiting_indices.append(
+                    (label_index_name, labels, label_adapter, still_waiting))
         self._waiting_indices = waiting_indices
 
     def _finalize_labels(self, label_adapter, label_index_name, labels):
         label_adapter.store_references(labels)
         if self._client is not None:
             self._client.add_labels(event_id=self.event.event_id,
                                     document_name=self.document_name,
                                     index_name=label_index_name,
                                     labels=labels,
                                     adapter=label_adapter)
         self._created_indices.append(label_index_name)
         index = label_adapter.create_index(labels)
-        self.labels.add_to_cache(label_index_name, index)
+        self._label_indices.add_to_cache(label_index_name, index)
         return index
 
-    def get_default_adapter(self, label_index_name: str,
-                            distinct: Optional[bool] = None) -> Optional['data.ProtoLabelAdapter']:
+    def get_default_adapter(
+            self,
+            label_index_name: str,
+            distinct: Optional[bool] = None
+    ) -> 'Optional[data.ProtoLabelAdapter]':
         try:
-            return self.default_adapters[label_index_name]
+            return self.label_adapters[label_index_name]
         except KeyError:
             pass
         try:
-            return self.event.default_adapters[label_index_name]
+            return self.event.label_adapters[label_index_name]
         except (AttributeError, KeyError):
             return _label_adapters.DISTINCT_GENERIC_ADAPTER if distinct \
                 else _label_adapters.GENERIC_ADAPTER
 
     def add_created_indices(self, created_indices: Iterable[str]):
         # Internal, used by the pipeline to add any indices created remotely to the
         # "created_indices" on a local document.
         return self._created_indices.extend(created_indices)
 
 
 class Labeler(Generic[L], ContextManager['Labeler']):
-    """Object provided by :func:`~'mtap.Document'.get_labeler` which is responsible for adding labels
-    to a label index on a document.
+    """Object provided by :func:`~'mtap.Document'.get_labeler` which is
+    responsible for adding labels to a label index on a document.
     """
-    __slots__ = ('_client', '_document', '_label_index_name', '_label_adapter', 'is_done',
-                 '_current_labels', '_lock')
+    __slots__ = (
+        '_client',
+        '_document',
+        '_label_index_name',
+        '_label_adapter',
+        'is_done',
+        '_current_labels',
+        '_lock'
+    )
 
     def __init__(self,
                  client: 'mtap.EventsClient',
                  document: Document,
                  label_index_name: str,
                  label_adapter: 'data.ProtoLabelAdapter[L]'):
         self._client = client
@@ -468,73 +593,101 @@
         self._label_index_name = label_index_name
         self._label_adapter = label_adapter
         self.is_done = False
         self._current_labels = []
         self._lock = threading.Lock()
 
     def __call__(self, *args, **kwargs) -> L:
-        """Calls the constructor for the label type adding it to the list of labels to be uploaded.
+        """Calls the constructor for the label type adding it to the list of
+        labels to be uploaded.
 
         Args:
             args: Arguments passed to the label type's constructor.
             kwargs: Keyword arguments passed to the label type's constructor.
 
         Returns:
             Label: The object that was created by the label type's constructor.
 
         Examples:
             >>> labeler(0, 25, some_field='some_value', x=3)
-            GenericLabel(start_index=0, end_index=25, some_field='some_value', x=3)
+            GenericLabel(start_index=0, end_index=25, some_field='some_value',
+                         x=3)
         """
-        label = self._label_adapter.create_label(*args, document=self._document, **kwargs)
+        label = self._label_adapter.create_label(*args,
+                                                 document=self._document,
+                                                 **kwargs)
         self._current_labels.append(label)
         return label
 
     def __enter__(self) -> 'data.Labeler':
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if exc_type is not None:
             return False
         self.done()
 
     def done(self):
-        """Finalizes the label index, uploads the added labels to the events service.
+        """Finalizes the label index, uploads the added labels to the events
+        service.
 
-        Normally called automatically on exit from a context manager block, but can be manually
-        invoked if the labeler is not used in a context manager block."""
+        Normally called automatically on exit from a context manager block,
+        but can be manually invoked if the labeler is not used in a context
+        manager block."""
         with self._lock:
             if self.is_done:
                 return
             self.is_done = True
-            self._document.add_labels(self._label_index_name, self._current_labels,
+            self._document.add_labels(self._label_index_name,
+                                      self._current_labels,
                                       label_adapter=self._label_adapter)
 
 
 def create_channel(address):
     config = _config.Config()
     options = config.get('grpc.events_options', {})
-    channel = grpc.insecure_channel(address, options=list(options.items()))
+    try:
+        channel = grpc.insecure_channel(address, options=list(options.items()))
 
-    health = health_pb2_grpc.HealthStub(channel)
-    hcr = health.Check(health_pb2.HealthCheckRequest(service=constants.EVENTS_SERVICE_NAME),
-                       metadata=[('service-name', constants.EVENTS_SERVICE_NAME)])
+        from grpc_health.v1 import health_pb2_grpc, health_pb2
+        health = health_pb2_grpc.HealthStub(channel)
+        hcr = health.Check(health_pb2.HealthCheckRequest(
+            service=constants.EVENTS_SERVICE_NAME),
+            metadata=[('service-name',
+                       constants.EVENTS_SERVICE_NAME)])
+    except grpc.RpcError as e:
+        if e.code() == grpc.StatusCode.UNAVAILABLE:
+            raise FailedToConnectToEventsServiceException(address) from e
+        raise e
     if hcr.status != health_pb2.HealthCheckResponse.SERVING:
-        raise ValueError('Failed to connect to events service. Status:')
+        raise FailedToConnectToEventsServiceException(address)
     return channel
 
 
+class FailedToConnectToEventsServiceException(Exception):
+    def __init__(self, address):
+        self.address = address
+        self.msg = f"Failed to connect to the events service at: '{address}'"
+
+    def __repr__(self):
+        return f"FailedToConnectToEventsServiceException({self.address})"
+
+    def __str__(self):
+        return self.msg
+
+
 class _ClientPool:
     __slots__ = ('_ptr', 'clients', 'instance_id_to_delegate')
 
     def __init__(self, channel_factory, addresses):
         self._ptr = 0
-        self.clients = [EventsClient(address=addresses, channel_factory=channel_factory,
-                                     _pool=self, _channel=channel_factory(a))
-                        for a in addresses]
+        self.clients = [
+            EventsClient(address=addresses, channel_factory=channel_factory,
+                         _pool=self, _channel=channel_factory(a))
+            for a in addresses]
         self.instance_id_to_delegate = {d.instance_id: d for d in self.clients}
 
     def get_instance(self, instance_id):
         if instance_id is not None:
             try:
                 return self.instance_id_to_delegate[instance_id]
             except KeyError:
@@ -544,55 +697,79 @@
         self._ptr = (self._ptr + 1) % len(self.clients)
         return i
 
 
 class EventsClient:
     """A client object for interacting with the events service.
 
-    Normally, users shouldn't have to use any of the methods on this object, as they are invoked by
-    the globally distributed object classes of :obj:`Event`, :obj:`Document`, and :obj:`~data.Labeler`.
+    Normally, users shouldn't have to use any of the methods on this object,
+    as they are invoked by the globally distributed object classes of
+    :obj:`Event`, :obj:`Document`, and :obj:`~data.Labeler`.
 
-    Keyword Args:
-        address (~typing.Optional[str]): The events service target e.g. 'localhost:9090' or
-            omit/None to use service discovery.
-        stub (~typing.Optional[~mtap.api.v1.events_pb2_grpc.EventsStub]): An existing events service
-            client gRPC stub to use.
+    Args:
+        address: The events service target e.g. 'localhost:9090' or omit/None
+            to use service discovery.
+        channel_factory: Callable used to create a grpc channel from an
+            address.
 
     Examples:
         >>> with EventsClient(address='localhost:50000') as client, \\
         >>>      Event(event_id='1', client=client) as event:
-        >>>     document = event.create_document(document_name='plaintext',
-        >>>                                      text='The quick brown fox jumps over the lazy dog.')
+        >>>     document = event.create_document(
+        >>>         document_name='plaintext',
+        >>>         text='The quick brown fox jumps over the lazy dog.'
+        >>>     )
     """
-    __slots__ = ('addresses', 'channel_factory', '_pool', '_channel', 'stub', '_instance_id',
-                 '_is_open')
+    __slots__ = (
+        'addresses',
+        'channel_factory',
+        '_pool',
+        '_channel',
+        'stub',
+        '_instance_id',
+        '_is_open'
+    )
 
-    def __init__(self, address: Optional[Union[str, Iterable[str]]],
-                 channel_factory: Callable[[str], grpc.Channel] = None,
+    def __init__(self, address: EventsAddressLike,
+                 *, channel_factory: Callable[[str], grpc.Channel] = None,
                  _pool: Optional[_ClientPool] = None,
                  _channel: Optional[grpc.Channel] = None):
-        if address is None or (isinstance(address, Iterable) and len(address) == 0):
-            discovery = _discovery.Discovery(_config.Config())
-            address = discovery.discover_events_service('v1')
         if isinstance(address, str):
             self.addresses = [address]
-        elif isinstance(address, Iterable):
+        elif isinstance(address, list):
+            self.addresses = address
+        elif isinstance(address, Iterable) or hasattr(address, '__iter__'):
             self.addresses = list(address)
+        elif address is None:
+            self.addresses = []
         else:
-            raise ValueError("Unrecognized address type: " + str(type(address)))
+            raise ValueError(
+                "Unrecognized address type: " + str(type(address))
+            )
+
+        if len(self.addresses) == 0:
+            from mtap.discovery import DiscoveryMechanism
+            discovery = DiscoveryMechanism()
+            self.addresses = discovery.discover_events_service('v1')
+
+        if len(self.addresses) == 0:
+            raise ValueError("No addresses for the events service even after "
+                             "attempting discovery.")
+
         self.channel_factory = channel_factory
         if channel_factory is None:
             self.channel_factory = create_channel
         self._pool = _pool
         if self._pool is None:
             self._pool = _ClientPool(self.channel_factory, self.addresses)
         self._channel = _channel
         if self._channel is not None:
             self.stub = events_pb2_grpc.EventsStub(self._channel)
-            r = self.stub.GetEventsInstanceId(events_pb2.GetEventsInstanceIdRequest())
+            r = self.stub.GetEventsInstanceId(
+                events_pb2.GetEventsInstanceIdRequest())
             self._instance_id = r.instance_id
             self._is_open = True
 
     @property
     def instance_id(self) -> str:
         return self._instance_id
 
@@ -609,165 +786,205 @@
         return self._pool.get_instance(instance_id)
 
     def ensure_open(self):
         if not self._is_open:
             raise ValueError("Client to events service is not open")
 
     def open_event(self, event_id: str, only_create_new: bool):
-        request = events_pb2.OpenEventRequest(event_id=event_id, only_create_new=only_create_new)
+        request = events_pb2.OpenEventRequest(event_id=event_id,
+                                              only_create_new=only_create_new)
         try:
             response = self.stub.OpenEvent(request)
             assert response is not None
         except grpc.RpcError as e:
             if e.code() == grpc.StatusCode.UNAVAILABLE:
-                raise ConnectionError("Failed to connect to events service on addresses: {}".format(self.addresses))
+                raise ConnectionError(
+                    f"Failed to connect to events service on addresses: "
+                    f"{self.addresses}")
             if e.code() == grpc.StatusCode.ALREADY_EXISTS:
                 raise ValueError("Event already exists") from e
             raise e
 
     def close_event(self, event_id):
         request = events_pb2.CloseEventRequest(event_id=event_id)
         try:
             response = self.stub.CloseEvent(request)
         except grpc.RpcError as e:
             if e.code() == grpc.StatusCode.UNAVAILABLE:
-                raise ConnectionError("Failed to connect to events service on addresses: {}".format(self.addresses))
+                raise ConnectionError(
+                    f"Failed to connect to events service on addresses: "
+                    f"{self.addresses}")
             raise e
         return response is not None
 
     def get_all_metadata(self, event_id):
         request = events_pb2.GetAllMetadataRequest(event_id=event_id)
         try:
             response = self.stub.GetAllMetadata(request)
         except grpc.RpcError as e:
             if e.code() == grpc.StatusCode.UNAVAILABLE:
-                raise ConnectionError("Failed to connect to events service on addresses: {}".format(self.addresses))
+                raise ConnectionError(
+                    f"Failed to connect to events service on addresses: "
+                    f"{self.addresses}")
             raise e
         return response.metadata
 
     def add_metadata(self, event_id, key, value):
-        request = events_pb2.AddMetadataRequest(event_id=event_id, key=key, value=value)
+        request = events_pb2.AddMetadataRequest(event_id=event_id, key=key,
+                                                value=value)
         try:
             response = self.stub.AddMetadata(request)
         except grpc.RpcError as e:
             if e.code() == grpc.StatusCode.UNAVAILABLE:
-                raise ConnectionError("Failed to connect to events service on addresses: {}".format(self.addresses))
+                raise ConnectionError(
+                    f"Failed to connect to events service on addresses: "
+                    f"{self.addresses}")
             raise e
         return response is not None
 
     def get_all_binary_data_names(self, event_id: str) -> List[str]:
         request = events_pb2.GetAllBinaryDataNamesRequest(event_id=event_id)
         try:
             response = self.stub.GetAllBinaryDataNames(request)
         except grpc.RpcError as e:
             if e.code() == grpc.StatusCode.UNAVAILABLE:
-                raise ConnectionError("Failed to connect to events service on addresses: {}".format(self.addresses))
+                raise ConnectionError(
+                    f"Failed to connect to events service on addresses: "
+                    f"{self.addresses}")
             raise e
         return list(response.binary_data_names)
 
-    def add_binary_data(self, event_id: str, binary_data_name: str, binary_data: bytes):
-        request = events_pb2.AddBinaryDataRequest(event_id=event_id,
-                                                  binary_data_name=binary_data_name,
-                                                  binary_data=binary_data)
+    def add_binary_data(self, event_id: str, binary_data_name: str,
+                        binary_data: bytes):
+        request = events_pb2.AddBinaryDataRequest(
+            event_id=event_id,
+            binary_data_name=binary_data_name,
+            binary_data=binary_data
+        )
         try:
             response = self.stub.AddBinaryData(request)
         except grpc.RpcError as e:
             if e.code() == grpc.StatusCode.UNAVAILABLE:
-                raise ConnectionError("Failed to connect to events service on addresses: {}".format(self.addresses))
+                raise ConnectionError(
+                    f"Failed to connect to events service on addresses: "
+                    f"{self.addresses}")
             raise e
         return response is not None
 
     def get_binary_data(self, event_id: str, binary_data_name: str) -> bytes:
-        request = events_pb2.GetBinaryDataRequest(event_id=event_id,
-                                                  binary_data_name=binary_data_name)
+        request = events_pb2.GetBinaryDataRequest(
+            event_id=event_id,
+            binary_data_name=binary_data_name
+        )
         try:
             response = self.stub.GetBinaryData(request)
         except grpc.RpcError as e:
             if e.code() == grpc.StatusCode.UNAVAILABLE:
-                raise ConnectionError("Failed to connect to events service on addresses: {}".format(self.addresses))
+                raise ConnectionError(
+                    f"Failed to connect to events service on addresses: "
+                    f"{self.addresses}")
             raise e
         return response.binary_data
 
     def get_all_document_names(self, event_id):
         request = events_pb2.GetAllDocumentNamesRequest(event_id=event_id)
         try:
             response = self.stub.GetAllDocumentNames(request)
         except grpc.RpcError as e:
             if e.code() == grpc.StatusCode.UNAVAILABLE:
-                raise ConnectionError("Failed to connect to events service on addresses: {}".format(self.addresses))
+                raise ConnectionError(
+                    f"Failed to connect to events service on addresses: "
+                    f"{self.addresses}")
             raise e
         return list(response.document_names)
 
     def add_document(self, event_id, document_name, text):
         request = events_pb2.AddDocumentRequest(event_id=event_id,
                                                 document_name=document_name,
                                                 text=text)
         try:
             response = self.stub.AddDocument(request)
         except grpc.RpcError as e:
             if e.code() == grpc.StatusCode.UNAVAILABLE:
-                raise ConnectionError("Failed to connect to events service on addresses: {}".format(self.addresses))
+                raise ConnectionError(
+                    f"Failed to connect to events service on addresses: "
+                    f"{self.addresses}")
             raise e
         return response is not None
 
     def get_document_text(self, event_id, document_name):
-        request = events_pb2.GetDocumentTextRequest(event_id=event_id,
-                                                    document_name=document_name)
+        request = events_pb2.GetDocumentTextRequest(
+            event_id=event_id,
+            document_name=document_name
+        )
         try:
             response = self.stub.GetDocumentText(request)
         except grpc.RpcError as e:
             if e.code() == grpc.StatusCode.UNAVAILABLE:
-                raise ConnectionError("Failed to connect to events service on addresses: {}".format(self.addresses))
+                raise ConnectionError(
+                    f"Failed to connect to events service on addresses: "
+                    f"{self.addresses}")
             raise e
         return response.text
 
-    def get_label_index_info(self,
-                             event_id: str,
-                             document_name: str) -> List['data.LabelIndexInfo']:
-        request = events_pb2.GetLabelIndicesInfoRequest(event_id=event_id,
-                                                        document_name=document_name)
+    def get_label_index_info(
+            self,
+            event_id: str,
+            document_name: str
+    ) -> 'List[data.LabelIndexInfo]':
+        request = events_pb2.GetLabelIndicesInfoRequest(
+            event_id=event_id,
+            document_name=document_name
+        )
         try:
             response = self.stub.GetLabelIndicesInfo(request)
         except grpc.RpcError as e:
             if e.code() == grpc.StatusCode.UNAVAILABLE:
-                raise ConnectionError("Failed to connect to events service on addresses: {}".format(self.addresses))
+                raise ConnectionError(
+                    f"Failed to connect to events service on addresses: "
+                    f"{self.addresses}")
             raise e
         result = []
         for index in response.label_index_infos:
             if index.type == events_pb2.GetLabelIndicesInfoResponse.LabelIndexInfo.GENERIC:
                 index_type = _base.LabelIndexType.GENERIC
             elif index.type == events_pb2.GetLabelIndicesInfoResponse.LabelIndexInfo.CUSTOM:
                 index_type = _base.LabelIndexType.CUSTOM
             else:
                 index_type = _base.LabelIndexType.UNKNOWN
             result.append(_base.LabelIndexInfo(index.index_name, index_type))
         return result
 
     def add_labels(self, event_id, document_name, index_name, labels, adapter):
-        request = events_pb2.AddLabelsRequest(event_id=event_id, document_name=document_name,
+        request = events_pb2.AddLabelsRequest(event_id=event_id,
+                                              document_name=document_name,
                                               index_name=index_name,
                                               no_key_validation=True)
         adapter.add_to_message(labels, request)
         try:
             response = self.stub.AddLabels(request)
         except grpc.RpcError as e:
             if e.code() == grpc.StatusCode.UNAVAILABLE:
-                raise ConnectionError("Failed to connect to events service on addresses: {}".format(self.addresses))
+                raise ConnectionError(
+                    f"Failed to connect to events service on addresses: "
+                    f"{self.addresses}")
             raise e
         return response is not None
 
     def get_labels(self, event_id, document_name, index_name, adapter):
         request = events_pb2.GetLabelsRequest(event_id=event_id,
                                               document_name=document_name,
                                               index_name=index_name)
         try:
             response = self.stub.GetLabels(request)
         except grpc.RpcError as e:
             if e.code() == grpc.StatusCode.UNAVAILABLE:
-                raise ConnectionError("Failed to connect to events service on addresses: {}".format(self.addresses))
+                raise ConnectionError(
+                    f"Failed to connect to events service on addresses: "
+                    f"{self.addresses}")
             raise e
         return adapter.create_index_from_response(response)
 
     def close(self):
         self._is_open = False
         try:
             self._channel.close()
@@ -827,15 +1044,19 @@
         raise NotImplementedError()
 
     def _refresh_documents(self):
         if self.client is not None:
             document_names = self.client.get_all_document_names(self.event_id)
             for name in document_names:
                 if name not in self.documents:
-                    document = Document(name, event=self.event)
+                    document = Document(
+                        name,
+                        event=self.event,
+                        label_adapters=self.event.label_adapters
+                    )
                     self.documents[name] = document
 
 
 class _Metadata(MutableMapping[str, str]):
     __slots__ = ('_client', '_event', '_event_id', '_metadata')
 
     def __init__(self, event: Event, client: Optional[EventsClient] = None):
@@ -878,15 +1099,15 @@
 
     def _refresh_metadata(self):
         if self._client is not None:
             response = self._client.get_all_metadata(self._event_id)
             self._metadata.update(response)
 
 
-class _Binaries(collections.abc.MutableMapping):
+class _Binaries(MutableMapping[str, bytes]):
     __slots__ = ('_client', '_event', '_event_id', '_names', '_binaries')
 
     def __init__(self, event: Event, client: Optional[EventsClient] = None):
         self._client = client
         self._event = event
         self._event_id = event.event_id
         self._names = set()
@@ -909,15 +1130,16 @@
 
     def __getitem__(self, key):
         try:
             return self._binaries[key]
         except KeyError:
             pass
         if self._client is not None:
-            b = self._client.get_binary_data(event_id=self._event_id, binary_data_name=key)
+            b = self._client.get_binary_data(event_id=self._event_id,
+                                             binary_data_name=key)
             self._names.add(b)
             self._binaries[key] = b
         return self._binaries[key]
 
     def __delitem__(self, v) -> None:
         raise NotImplementedError
 
@@ -932,15 +1154,17 @@
     def _refresh_binaries(self):
         if self._client is not None:
             response = self._client.get_all_binary_data_names(self._event_id)
             self._names.update(response)
 
 
 class _LabelIndices(Mapping[str, 'data.LabelIndex']):
-    __slots__ = ('_document', '_document_name', '_event_id', '_client', '_cache', '_names_cache')
+    __slots__ = (
+        '_document', '_document_name', '_event_id', '_client', '_cache',
+        '_names_cache')
 
     def __init__(self, document: Document):
         self._document = document
         self._document_name = document.document_name
         try:
             self._event_id = document.event.event_id
             self._client = document.event.client
@@ -959,15 +1183,16 @@
         if k not in self:
             raise KeyError
 
         if self._client is not None:
             label_adapter = self._document.get_default_adapter(k)
             if label_adapter is None:
                 label_adapter = data.GENERIC_ADAPTER
-            index = self._client.get_labels(self._event_id, self._document_name, k,
+            index = self._client.get_labels(self._event_id,
+                                            self._document_name, k,
                                             adapter=label_adapter)
             for label in index:
                 label.label_index_name = k
                 label.document = self._document
             self._cache[k] = index
             self._names_cache.add(k)
             return index
@@ -984,14 +1209,15 @@
 
     def __iter__(self) -> Iterator[str]:
         self._refresh_names()
         return iter(self._names_cache)
 
     def _refresh_names(self):
         if self._client is not None:
-            infos = self._client.get_label_index_info(self._event_id, self._document_name)
+            infos = self._client.get_label_index_info(self._event_id,
+                                                      self._document_name)
             for info in infos:
                 self._names_cache.add(info.index_name)
 
     def add_to_cache(self, label_index_name, index):
         self._cache[label_index_name] = index
         self._names_cache.add(label_index_name)
```

### Comparing `mtap-1.1.0/python/mtap/data/_label_adapters.py` & `mtap-1.2.0/python/mtap/data/_label_adapters.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/data/_label_indices.py` & `mtap-1.2.0/python/mtap/data/_label_indices.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/data/_labels.py` & `mtap-1.2.0/python/mtap/data/_labels.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,206 +12,212 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """Labels functionality."""
 import threading
 from abc import ABC, abstractmethod, ABCMeta
 from queue import Queue
 from typing import (
-    List,
-    Tuple,
-    Set,
     TYPE_CHECKING,
     TypeVar,
     NamedTuple,
     Any,
     Mapping,
     Sequence,
     Union,
     Optional
 )
 
 if TYPE_CHECKING:
-    import mtap
-    from mtap import data
+    from mtap import (
+        Document
+    )
 
 
-class Location(NamedTuple('Location', [('start_index', float), ('end_index', float)])):
+LocationLike = 'Union[Location, Label, int]'
+
+
+class Location(NamedTuple):
     """A location in text, a tuple of (`start_index`, `end_index`).
 
     Used to perform comparison of labels based on their locations.
-
-    Args:
-        start_index (float):
-            The start index inclusive of the location in text.
-        end_index (float):
-            The end index exclusive of the location in text.
-
-    Attributes:
-        start_index (float):
-            The start index inclusive of the location in text.
-        end_index (float):
-            The end index exclusive of the location in text.
     """
-    __slots__ = ()
 
-    def covers(self, other: Union['data.Location', 'data.Label']):
-        """Whether the span of text covered by this label completely overlaps the span of text
-        covered by the ``other`` label or location.
+    start_index: float
+    """The start index inclusive of the location in text."""
+
+    end_index: float
+    """The end index exclusive of the location in text."""
+
+    def covers(self, other: 'Union[Location, Label]'):
+        """Whether the span of text covered by this label completely overlaps
+        the span of text covered by the ``other`` label or location.
 
         Args:
-            other (~typing.Union[Location, Label]): A location or label to compare against.
+            other: A location or label to compare against.
 
         Returns:
-            bool: ``True`` if `other` is completely overlapped/covered ``False`` otherwise.
+            ``True`` if `other` is completely overlapped/covered
+                ``False`` otherwise.
         """
-        return self.start_index <= other.start_index and self.end_index >= other.end_index
+        return self.start_index <= other.start_index \
+            and self.end_index >= other.end_index
 
-    def relative_to(self, location: Union['data.Location', 'data.Label', int]) -> 'data.Location':
-        """Creates a location relative to the the same origin as ``location`` and makes it relative
-        to ``location``.
+    def relative_to(self, location: LocationLike) -> 'Location':
+        """Creates a location relative to the same origin as ``location``
+        and makes it relative to ``location``.
 
         Args:
-            location (int or Location or Label): A location to relativize this location to.
+            location: A location to relativize this
+                location to.
 
         Returns:
-            ~data.Location: A copy with updated indices.
+            A copy with updated indices.
 
         Examples:
             >>> sentence = Location(10, 20)
             >>> token = Location(10, 15)
             >>> token.relative_to(sentence)
             Location(start_index=0, end_index=5)
 
         """
         try:
             start_index = location.start_index
         except AttributeError:
             start_index = location
         if not isinstance(start_index, int):
-            raise ValueError('location must be Label, Location, or an int value')
-        return Location(self.start_index - start_index, self.end_index - start_index)
-
-    def offset_by(self, location: Union['data.Location', 'data.Label', int]) -> 'data.Location':
-        """Creates a location by offsetting this location by an integer or the ``start_index`` of a
-        location / label. Derelativizes this location.
+            raise ValueError(
+                'location must be Label, Location, or an int value')
+        return Location(self.start_index - start_index,
+                        self.end_index - start_index)
+
+    def offset_by(self, location: LocationLike) -> 'Location':
+        """Creates a location by offsetting this location by an integer or the
+        ``start_index`` of a location / label. De-relativizes this location.
 
         Args:
-            location (int or Location or Label): A location to offset this location by.
+            location: A location to offset this location by.
 
         Returns:
-            ~data.Location: A copy with updated indices.
+            A copy with updated indices.
 
         Examples:
             >>> sentence = Location(10, 20)
             >>> token_in_sentence = Location(0, 5)
             >>> token_in_sentence.offset_by(sentence)
             Location(start_index=10, end_index=15)
 
         """
         try:
             start_index = location.start_index
         except AttributeError:
             start_index = location
         if not isinstance(start_index, int):
-            raise ValueError('location must be Label, Location, or an int value')
-        return Location(self.start_index + start_index, self.end_index + start_index)
+            raise ValueError(
+                'location must be Label, Location, or an int value'
+            )
+        return Location(self.start_index + start_index,
+                        self.end_index + start_index)
 
 
 class Label(ABC, metaclass=ABCMeta):
     """An abstract base class for a label of attributes on text.
     """
 
     @property
     @abstractmethod
-    def document(self) -> 'mtap.Document':
-        """Document: The parent document this label appears on."""
+    def document(self) -> 'Document':
+        """The parent document this label appears on."""
         ...
 
     @document.setter
     @abstractmethod
-    def document(self, value: 'mtap.Document'):
-        """Sets the label's document, this will automatically be done when the label is created
-        via a Document (i.e. get_label_index) or added to a document (i.e. via labeler or add_labels).
+    def document(self, value: 'Document'):
+        """Sets the label's document, this will automatically be done when the
+        label is created via a Document (i.e. get_label_index) or added to a
+        document (i.e. via labeler or add_labels).
         """
         ...
 
     @property
     @abstractmethod
     def label_index_name(self) -> str:
-        """str: The label index this label appears on."""
+        """The label index this label appears on."""
         ...
 
     @label_index_name.setter
     @abstractmethod
     def label_index_name(self, value: str):
-        """Sets the name for the label index this label appears on. Will automatically be called
-        when a label is added to a document via labeler or add_labels."""
+        """Sets the name for the label index this label appears on. Will
+        automatically be called when a label is added to a document via
+        labeler or add_labels."""
         ...
 
     @property
     @abstractmethod
     def identifier(self) -> int:
-        """int: The index of the label within its label index."""
+        """The index of the label within its label index."""
         ...
 
     @identifier.setter
     @abstractmethod
     def identifier(self, value: int):
-        """The index of the label within its label index. Labels will automatically be assigned
-        this when added to a document via labeler or add_labels."""
+        """The index of the label within its label index. Labels will
+        automatically be assigned this when added to a document via labeler or
+        add_labels."""
         ...
 
     @property
     @abstractmethod
     def start_index(self) -> int:
-        """int: The index of the first character of the text covered by this label.
+        """The index of the first character of the text covered by this label.
         """
         ...
 
     @start_index.setter
     @abstractmethod
     def start_index(self, value: int):
         ...
 
     @property
     @abstractmethod
     def end_index(self) -> int:
-        """int: The index after the last character of the text covered by this label.
+        """The index after the last character of the text covered by this label.
         """
         ...
 
     @end_index.setter
     @abstractmethod
     def end_index(self, value: int):
         ...
 
     @property
     def location(self) -> Location:
-        """Location: A tuple of (start_index, end_index) used to perform sorting and
-            comparison first based on start_index, then based on end_index.
+        """A tuple of (start_index, end_index) used to perform sorting and
+        comparison first based on start_index, then based on end_index.
         """
         return Location(self.start_index, self.end_index)
 
     @property
     def text(self):
-        """str: The slice of document text covered by this label. Will retrieve from events server
-        if it is not cached locally.
+        """The slice of document text covered by this label. Will
+        retrieve from events server if it is not cached locally.
         """
         return self.document.text[self.start_index:self.end_index]
 
     @abstractmethod
     def shallow_fields_equal(self, other) -> bool:
-        """Tests if the fields on this label and locations of references are the same as another
-        label.
+        """Tests if the fields on this label and locations of references are
+        the same as another label.
 
         Args:
             other: The other label to test.
 
         Returns:
-            True if all of the fields are equal and the references are at the same locations.
+            True if all the fields are equal and the references are at the
+            same locations.
 
         """
         pass
 
     @abstractmethod
     def collect_floating_references(self, s):
         pass
@@ -219,43 +225,44 @@
 
 L = TypeVar('L', bound=Label)
 
 _repr_local = threading.local()
 
 
 class GenericLabel(Label):
-    """Default implementation of the Label class which uses a dictionary to store attributes.
+    """Default implementation of the Label class which uses a dictionary to
+    store attributes.
 
     Will be suitable for the majority of use cases for labels.
 
     Args:
-        start_index (int): The index of the first character in text to be included in the label.
-        end_index (int): The index after the last character in text to be included in the label.
-
-    Keyword Args:
-        document (~typing.Optional[Document]): The parent document of the label. This will be
-            automatically set if a the label is created via labeler.
-        **kwargs : Arbitrary, any other fields that should be added to the label, values must be
-            json-serializable.
+        start_index: The index of the first character in text to be included
+            in the label.
+        end_index: The index after the last character in text to be included
+            in the label.
+        document: The parent document of the label. This will be automatically
+            set if the label is created via labeler.
+        **kwargs : Arbitrary, any other fields that should be added to the
+            label, values must be json-serializable.
 
     Examples:
         >>> pos_tag = pos_tag_labeler(0, 5)
         >>> pos_tag.tag = 'NNS'
         >>> pos_tag.tag
         'NNS'
 
         >>> pos_tag2 = pos_tag_labeler(6, 10, tag='VB')
         >>> pos_tag2.tag
         'VB'
     """
 
     def __init__(self, start_index: int, end_index: int, *,
                  identifier: Optional[int] = None,
-                 document: Optional['mtap.Document'] = None,
-                 label_index_name: Optional['str'] = None,
+                 document: 'Optional[Document]' = None,
+                 label_index_name: Optional[str] = None,
                  fields: Optional[dict] = None,
                  reference_field_ids: Optional[dict] = None,
                  **kwargs):
         self._document = document
         self._label_index_name = label_index_name
         self._identifier = identifier
         self._start_index = int(start_index)
@@ -269,19 +276,19 @@
         else:
             self.reference_field_ids = reference_field_ids
         self.reference_cache = {}
         for key, value in kwargs.items():
             setattr(self, key, value)
 
     @property
-    def document(self) -> 'mtap.Document':
+    def document(self) -> 'Document':
         return self._document
 
     @document.setter
-    def document(self, document: 'mtap.Document'):
+    def document(self, document: 'Document'):
         self._document = document
 
     @property
     def label_index_name(self) -> str:
         return self._label_index_name
 
     @label_index_name.setter
@@ -309,15 +316,16 @@
         return self._end_index
 
     @end_index.setter
     def end_index(self, end_index: int):
         self._end_index = end_index
 
     def _is_reserved(self, key):
-        return key in self.__dict__.keys() or key in vars(GenericLabel) or key in vars(Label)
+        return key in self.__dict__.keys() or key in vars(
+            GenericLabel) or key in vars(Label)
 
     def __getattr__(self, item):
         try:
             return self.fields[item]
         except KeyError:
             pass
         try:
@@ -325,20 +333,23 @@
         except KeyError:
             pass
         try:
             ref_value = self.reference_field_ids[item]
             self.reference_cache[item] = _dereference(ref_value, self.document)
             return self.reference_cache[item]
         except KeyError:
-            raise AttributeError('Key "{}" not in fields, reference cache, or reference ids.'
-                                 .format(item))
+            raise AttributeError(
+                'Key "{}" not in fields, reference cache, or reference ids.'
+                .format(item))
 
     def __setattr__(self, key, value):
-        if key in ('document', 'label_index_name', 'identifier', 'start_index', 'end_index',
-                   '_document', '_label_index_name', '_identifier', '_start_index', '_end_index',
+        if key in ('document', 'label_index_name', 'identifier', 'start_index',
+                   'end_index',
+                   '_document', '_label_index_name', '_identifier',
+                   '_start_index', '_end_index',
                    'fields', 'reference_field_ids', 'reference_cache'):
             object.__setattr__(self, key, value)
             return
         if self._is_reserved(key):
             raise ValueError('The key "{}" is a reserved key.'.format(key))
         is_ref = _is_referential(value, [id(self)])
         if is_ref:
@@ -354,16 +365,18 @@
         if not self.location == other.location:
             return False
         return self.shallow_fields_equal(other)
 
     def shallow_fields_equal(self, other):
         if not self.fields == other.fields:
             return False
-        refs = set(self.reference_field_ids.keys()).union(self.reference_cache.keys())
-        other_refs = set(other.reference_field_ids.keys()).union(other.reference_cache.keys())
+        refs = set(self.reference_field_ids.keys()).union(
+            self.reference_cache.keys())
+        other_refs = set(other.reference_field_ids.keys()).union(
+            other.reference_cache.keys())
         if not refs == other_refs:
             return False
         for k in refs:
             try:
                 if self.reference_field_ids[k] == other.reference_field_ids[k]:
                     continue
             except KeyError:
@@ -414,55 +427,32 @@
                 for v in o:
                     if v is not None:
                         queue.put(v)
 
 
 def label(start_index: int,
           end_index: int,
-          *, document: Optional['mtap.Document'] = None,
+          *, document: 'Optional[Document]' = None,
           **kwargs) -> GenericLabel:
     """An alias for :class:`GenericLabel`.
 
     Args:
-        start_index (int): The index of the first character in text to be included in the label.
-        end_index (int): The index after the last character in text to be included in the label.
-        document (~typing.Optional[Document]): The parent document of the label. This will be
-            automatically set if a the label is created via labeler.
-        **kwargs : Arbitrary, any other fields that should be added to the label, values must be
-            json-serializable.
+        start_index: The index of the first character in text to be included
+            in the label.
+        end_index: The index after the last character in text to be included
+            in the label.
+        document: The parent document of the label. This will be automatically
+            set if the label is created via labeler.
+        **kwargs : Arbitrary, any other fields that should be added to the
+            label, values must be json-serializable.
 
     """
     return GenericLabel(start_index, end_index, document=document, **kwargs)
 
 
-def _staticize(labels: Sequence['data.Label'],
-               document: 'mtap.Document',
-               label_index_name: str) -> Tuple[List['data.Label'], Set[int]]:
-    """Prepares a label index for serialization by finalizing sort order and setting label
-    identifiers.
-
-    Args:
-        labels (~typing.Sequence[GenericLabel]): The labels in a label index.
-
-    Returns:
-        List['GenericLabel']: The labels sorted by position.
-        Set[int]: A set of labels which a referenced by labels in this index.
-
-    """
-    labels = sorted(labels, key=lambda x: x.location)
-    waiting_on = set()
-    for i, lbl in enumerate(labels):
-        lbl.document = document
-        lbl.identifier = i
-        lbl.label_index_name = label_index_name
-    for lbl in labels:
-        lbl.collect_floating_references(waiting_on)
-    return labels, waiting_on
-
-
 def _is_referential(o: Any, parents=None) -> bool:
     if parents is None:
         parents = [id(o)]
     if isinstance(o, (str, float, bool, int)) or o is None:
         return False
     elif isinstance(o, Label):
         return True
@@ -471,34 +461,36 @@
         for v in o.values():
             if id(v) in parents:
                 raise ValueError('Recursive loop')
             x = _is_referential(v, parents + [id(v)])
             if map_is_ref is None:
                 map_is_ref = x
             elif x != map_is_ref:
-                raise TypeError('Label dictionaries cannot have mixes of references to labels'
-                                'and primitive types.')
+                raise TypeError(
+                    'Label dictionaries cannot have mixes of references to labels'
+                    'and primitive types.')
         return map_is_ref
     elif isinstance(o, Sequence):
         seq_is_ref = None
         for v in o:
             if id(v) in parents:
                 raise ValueError('Recursive loop')
             x = _is_referential(v, parents + [id(v)])
             if seq_is_ref is None:
                 seq_is_ref = x
             elif x != seq_is_ref:
-                raise TypeError('Label lists cannot have mixes of references to labels'
-                                'and primitive types.')
+                raise TypeError(
+                    'Label lists cannot have mixes of references to labels'
+                    'and primitive types.')
         return seq_is_ref
     else:
         raise TypeError('Unrecognized type')
 
 
-def _dereference(o: Any, document: 'mtap.Document') -> Any:
+def _dereference(o: Any, document: 'Document') -> Any:
     if o is None:
         return o
     if isinstance(o, str):
         label_index_name, label_id = o.split(':')
         label_index = document.labels[label_index_name]
         label_ = label_index[int(label_id)]
         return label_
```

### Comparing `mtap-1.1.0/python/mtap/defaultConfig.yml` & `mtap-1.2.0/python/mtap/defaultConfig.yml`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/examples/__init__.py` & `mtap-1.2.0/python/mtap/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/examples/exampleDeploymentConfiguration.yml` & `mtap-1.2.0/python/mtap/examples/exampleDeploymentConfiguration.yml`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/examples/examplePipelineConfiguration.yml` & `mtap-1.2.0/python/mtap/examples/examplePipelineConfiguration.yml`

 * *Files 16% similar despite different names*

```diff
@@ -2,24 +2,27 @@
 events_address: 127.0.0.1:10100  # The address for the events service
 # events_addresses:
 #   - 127.0.0.1:10100
 #   - 127.0.0.1:10101
 #   - 127.0.0.1:10102
 #   - 127.0.0.1:10103
 mp_config:
-  # The maximum number of document failures before stopping processing.
-  max_failures: 0
   # Whether to print a progress bar in the console
   show_progress: True
   # Concurrent workers / documents being processed at once (on the pipeline side).
   workers: 4
   # Number of documents to receive from the source and keep ready for processing.
   read_ahead: 2
   # Whether to close events that are handed off from the source to the pipeline.
   close_events: True
+error_handlers:
+  - name: simple
+  - name: termination
+    params:
+      max_failures: 0
 components:
   - name: mtap-example-processor-python # The processor's identifier
     address: localhost:10101 # The address of the processor, null to use service discovery
     component_id: null
     params:
       do_work: yes
   - name: mtap-example-processor-java
```

### Comparing `mtap-1.1.0/python/mtap/examples/example_pipeline.py` & `mtap-1.2.0/python/mtap/examples/example_pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,72 +13,109 @@
 #  limitations under the License.
 #
 import shutil
 from argparse import ArgumentParser
 from pathlib import Path
 
 import mtap
-from mtap import LocalProcessor
 from mtap.serialization import SerializationProcessor, JsonSerializer
-from mtap.processing import FilesInDirectoryProcessingSource, Pipeline
+from mtap.processing import (
+    FilesInDirectoryProcessingSource,
+    Pipeline,
+    LocalProcessor,
+)
 
 
 def print_example(_):
     print('Writing "examplePipelineConfiguration.yml" to ' + str(Path.cwd()))
-    shutil.copy2(str(Path(__file__).parent / 'examplePipelineConfiguration.yml'),
-                 'examplePipelineConfiguration.yml')
+    shutil.copy2(
+        str(Path(__file__).parent / 'examplePipelineConfiguration.yml'),
+        'examplePipelineConfiguration.yml')
 
 
 def run_pipeline(conf):
-    pipeline_conf = conf.pipeline_config or Path(__file__).parent / 'examplePipelineConfiguration.yml'
+    pipeline_conf = (
+            conf.pipeline_config
+            or Path(__file__).parent / 'examplePipelineConfiguration.yml'
+    )
     pipeline = Pipeline.from_yaml_file(pipeline_conf)
 
     with mtap.EventsClient(address=conf.events_address) as client:
         pipeline.events_client = client
         pipeline.append(
             LocalProcessor(
-                proc=SerializationProcessor(ser=JsonSerializer, output_dir=conf.output_directory),
+                processor=SerializationProcessor(
+                    serializer=JsonSerializer,
+                    output_dir=conf.output_directory
+                ),
                 component_id='serialization_processor'
             )
         )
-        source = FilesInDirectoryProcessingSource(directory=conf.input_directory, client=client)
+        source = FilesInDirectoryProcessingSource(directory=conf.directory,
+                                                  client=client)
         pipeline.run_multithread(source=source, workers=conf.threads,
-                                 max_failures=conf.max_failures, read_ahead=conf.read_ahead)
+                                 max_failures=conf.max_failures,
+                                 read_ahead=conf.read_ahead)
 
 
 def main(args=None):
     parser = ArgumentParser()
     subparsers = parser.add_subparsers()
 
     print_example_subparser = subparsers.add_parser('write_example')
     print_example_subparser.set_defaults(f=print_example)
 
     run_subparser = subparsers.add_parser('run')
 
-    run_subparser.add_argument('input_directory', metavar='IN_DIR',
-                               help='Directory of files to process.')
-
-    run_subparser.add_argument('output_directory', metavar='OUT_DIR',
-                               help='Where to write output files.')
-
-    run_subparser.add_argument('events_address', metavar='ADDRESS',
-                               help='Address of the events service.')
-
-    run_subparser.add_argument('--pipeline-config', metavar='PATH', default=None,
-                               help='Path to a pipeline configuration.')
-
-    run_subparser.add_argument('--threads', metavar='N', default=4,
-                               help='Number of threads to use for processing')
-
-    run_subparser.add_argument('--max-failures', metavar='N', default=0,
-                               help='The maximum number of failures to accept before stopping.')
-
-    run_subparser.add_argument('--read-ahead', metavar='N', default=1,
-                               help='The number of documents to read ahead of what is currently '
-                                    'being processed')
+    run_subparser.add_argument(
+        'input_directory',
+        metavar='IN_DIR',
+        help='Directory of files to process.'
+    )
+
+    run_subparser.add_argument(
+        'output_directory',
+        metavar='OUT_DIR',
+        help='Where to write output files.'
+    )
+
+    run_subparser.add_argument(
+        'events_address',
+        metavar='ADDRESS',
+        help='Address of the events service.'
+    )
+
+    run_subparser.add_argument(
+        '--pipeline-config',
+        metavar='PATH',
+        default=None,
+        help='Path to a pipeline configuration.'
+    )
+
+    run_subparser.add_argument(
+        '--threads',
+        metavar='N',
+        default=4,
+        help='Number of threads to use for processing'
+    )
+
+    run_subparser.add_argument(
+        '--max-failures',
+        metavar='N',
+        default=0,
+        help='The maximum number of failures to accept before stopping.'
+    )
+
+    run_subparser.add_argument(
+        '--read-ahead',
+        metavar='N',
+        default=1,
+        help='The number of documents to read ahead of what is currently '
+             'being processed'
+    )
 
     run_subparser.set_defaults(f=run_pipeline)
 
     conf = parser.parse_args(args)
     f = conf.f
     f(conf)
```

### Comparing `mtap-1.1.0/python/mtap/examples/example_processor.py` & `mtap-1.2.0/python/mtap/examples/example_processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,40 +15,51 @@
 
 from mtap import DocumentProcessor, processor, run_processor
 from mtap.processing.descriptions import parameter, labels, label_property
 
 
 @processor('mtap-example-processor-python',
            human_name="Python Example Processor",
-           description="counts the number of times the letters a and b occur in a document",
+           description="counts the number of times the letters a and b occur "
+                       "in a document",
            parameters=[
-               parameter('do_work', required=True, data_type='bool',
-                         description="Whether the processor should do anything.")
+               parameter(
+                   'do_work',
+                   required=True,
+                   data_type='bool',
+                   description="Whether the processor should do anything."
+               )
            ],
            outputs=[
                labels('mtap.examples.letter_counts',
                       properties=[label_property('letter', data_type='str'),
                                   label_property('count', data_type='int')])
            ])
 class ExampleProcessor(DocumentProcessor):
-    """Does some labeling of the counts of the letter 'a' and 'b' in a document.
+    """Does some labeling of the counts of the letter 'a' and 'b' in a
+    document.
     """
 
     def process_document(self, document, params):
         if params['do_work']:
             with self.started_stopwatch('fetch_time'):
                 text = document.text
 
             a_count = text.count('a')
             b_count = text.count('b')
 
-            with document.get_labeler('mtap.examples.letter_counts') as label_letter_count:
-                label_letter_count(start_index=0, end_index=len(document.text), letter='a',
+            with document.get_labeler('mtap.examples.letter_counts') as \
+                    label_letter_count:
+                label_letter_count(start_index=0,
+                                   end_index=len(document.text),
+                                   letter='a',
                                    count=a_count)
-                label_letter_count(start_index=0, end_index=len(document.text), letter='b',
+                label_letter_count(start_index=0,
+                                   end_index=len(document.text),
+                                   letter='b',
                                    count=b_count)
 
         return {'answer': 42}
 
 
 if __name__ == '__main__':
-    run_processor(ExampleProcessor(), mp=True)
+    run_processor(ExampleProcessor())
```

### Comparing `mtap-1.1.0/python/mtap/examples/example_references_processor.py` & `mtap-1.2.0/python/mtap/examples/example_references_processor.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/examples/print_processor_meta.py` & `mtap-1.2.0/python/mtap/examples/print_processor_meta.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/examples/serialization/__init__.py` & `mtap-1.2.0/python/mtap/examples/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/examples/serialization/brat_converter.py` & `mtap-1.2.0/python/mtap/examples/serialization/brat_converter.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/examples/tutorial/__init__.py` & `mtap-1.2.0/python/mtap/examples/tutorial/__init__.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/examples/tutorial/hello.py` & `mtap-1.2.0/python/mtap/examples/tutorial/hello.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/examples/tutorial/pipeline.py` & `mtap-1.2.0/python/mtap/examples/tutorial/pipeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Hello world tutorial pipeline."""
 import sys
 
 if __name__ == '__main__':
-    from mtap import Document, Event, Pipeline, RemoteProcessor
+    from mtap import Document, Event, Pipeline, EventsClient
+    from mtap.processing import RemoteProcessor
 
-    with Pipeline(
+    with EventsClient(sys.argv[1]) as client:
+        pipeline = Pipeline(
             RemoteProcessor(processor_name='hello', address=sys.argv[2]),
-            events_address=sys.argv[1]
-    ) as pipeline:
-        with Event(event_id='1', client=pipeline.events_client) as event:
+        )
+        with Event(event_id='1', client=client) as event:
             document = Document(document_name='name', text='YOUR NAME')
             event.add_document(document)
             pipeline.run(document)
             index = document.get_label_index('hello')
             for label in index:
                 print(label.response)
```

### Comparing `mtap-1.1.0/python/mtap/metrics.py` & `mtap-1.2.0/python/mtap/metrics.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/processing/__init__.py` & `mtap-1.2.0/python/mtap/processing/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,29 +9,59 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from mtap.processing._base import (
-    AggregateTimingInfo,
-    ComponentDescriptor,
     DocumentProcessor,
     EventProcessor,
-    PipelineResult,
     Processor,
     ProcessorContext,
     ProcessingComponent,
-    ProcessingError,
-    ProcessingResult,
     Stopwatch,
-    TimerStats,
 )
+from mtap.processing._exc import ProcessingError
+
+from mtap.processing._error_handling import (
+    StopProcessing,
+    SuppressError,
+    ErrorOrigin,
+    ErrorInfo,
+    ProcessingErrorHandler,
+    SimpleErrorHandler,
+    TerminationErrorHandler,
+    LoggingErrorHandler,
+    ErrorsDirectoryErrorHandler,
+    SuppressAllErrorsHandler,
+    ErrorHandlerFactory,
+    ErrorHandlerRegistry,
+)
+
 from mtap.processing.descriptions import processor
-from mtap.processing._pipeline import (
-    FilesInDirectoryProcessingSource,
+from mtap.processing._pipeline import Pipeline
+from mtap.processing._mp_config import MpConfig
+
+from mtap.processing._pipeline_components import (
+    RemoteProcessor,
     LocalProcessor,
-    Pipeline,
+    ComponentDescriptor,
+)
+
+from mtap.processing._pipeline_results import (
+    AggregateTimingInfo,
+    BatchPipelineResult,
+    PipelineResult,
+    ComponentResult,
+    TimerStats,
+)
+
+from mtap.processing._sources import (
+    FilesInDirectoryProcessingSource,
     ProcessingSource,
-    RemoteProcessor,
 )
-from mtap.processing._service import processor_parser, ProcessorServer, run_processor
+
+from mtap.processing._service import (
+    processor_parser,
+    ProcessorServer,
+    run_processor,
+)
```

### Comparing `mtap-1.1.0/python/mtap/processing/_runners.py` & `mtap-1.2.0/python/mtap/processing/_pipeline_components.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,144 +1,154 @@
-# Copyright 2019 Regents of the University of Minnesota.
+# Copyright 2023 Regents of the University of Minnesota.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import logging
-from typing import Optional, Dict, Any, TYPE_CHECKING
-
-import grpc
-
-from mtap import _discovery, _structs, Config
-from mtap import data
-from mtap.api.v1 import processing_pb2, processing_pb2_grpc
-from mtap.processing import _base
-
-if TYPE_CHECKING:
-    import mtap
-
-logger = logging.getLogger('mtap.processing')
-
-
-class ProcessorRunner(_base.ProcessingComponent):
-    __slots__ = ('processor', '_processor_name', '_component_id', 'params', 'metadata', 'client')
-
-    def __init__(self,
-                 proc: 'mtap.EventProcessor',
-                 client: 'Optional[mtap.EventsClient]',
-                 processor_name: str = None,
-                 component_id: str = None,
-                 params: Optional[Dict[str, Any]] = None):
-        self.processor = proc
-        self.params = params or {}
-        self.metadata = proc.metadata
-        self._processor_name = processor_name
-        self._component_id = component_id
-        self.client = client
-
-    @property
-    def processor_name(self) -> str:
-        return self._processor_name
+import copy
+import typing
+from abc import ABC, abstractmethod
+from typing import Optional, Dict, Any
+
+from mtap.data import EventsAddressLike
+from mtap.processing import _runners
+
+if typing.TYPE_CHECKING:
+    from mtap import EventProcessor, processing
+
+
+class ComponentDescriptor(ABC):
+    """A configuration which describes either a local or remote pipeline
+    component and what the pipeline needs to do to call the component.
+    """
+    __slots__ = ()
 
     @property
+    @abstractmethod
     def component_id(self) -> str:
-        return self._component_id
-
-    def call_process(self, event_id, event_instance_id, params):
-        p = dict(self.params)
-        if params is not None:
-            p.update(params)
-
-        with _base.Processor.enter_context() as c, \
-                data.Event(event_id=event_id,
-                           event_service_instance_id=event_instance_id,
-                           client=self.client) as event:
-            with _base.Processor.started_stopwatch('process_method'):
-                try:
-                    result = self.processor.process(event, p)
-                except Exception as e:
-                    logger.error(
-                        "Error while processing event_id %s through pipeline component  '%s'",
-                        event_id, self.component_id)
-                    raise e
-            return result, c.times, event.created_indices
+        ...
 
-    def close(self):
+    @abstractmethod
+    def create_pipeline_component(
+            self,
+            events_address: EventsAddressLike
+    ) -> 'processing.ProcessingComponent':
         pass
 
 
-class RemoteRunner(_base.ProcessingComponent):
-    __slots__ = ('_processor_name', '_component_id', '_address', 'params', '_channel', '_stub')
-
-    def __init__(self, processor_name, component_id, address=None, params=None,
-                 enable_proxy=None):
-        self._processor_name = processor_name
-        self._component_id = component_id
-        self._address = address
-        self.params = params
-        address = self._address
-        config = Config()
-        if enable_proxy is not None:
-            config['grpc.processor_options.gprc.enable_http_proxy'] = enable_proxy
-        if address is None:
-            discovery = _discovery.Discovery(config)
-            address = discovery.discover_processor_service(processor_name, 'v1')
-        channel_options = config.get('grpc.processor_options', {})
-        self._channel = grpc.insecure_channel(address, options=list(channel_options.items()))
-        self._stub = processing_pb2_grpc.ProcessorStub(self._channel)
+class LocalProcessor(ComponentDescriptor):
+    """A configuration of a locally-invoked processor.
 
-    @property
-    def processor_name(self) -> str:
-        return self._processor_name
+    Attributes:
+        processor: The processor instance to run with the pipeline.
+        component_id: How the processor's results will be identified locally.
+            Will be modified to be unique if it is not unique relative to other
+            components in the pipeline.
+        params: An optional parameter dictionary that will be passed to the
+            processor as parameters with every event or document processed.
+            Values should be json-serializable.
+    """
+    __slots__ = ('processor', 'component_id', 'params')
+
+    processor: 'EventProcessor'
+    component_id: str
+    params: Dict[str, Any]
 
-    @property
-    def component_id(self) -> str:
-        return self._component_id
+    def __init__(self,
+                 processor: 'EventProcessor',
+                 *, component_id: Optional[str] = None,
+                 params: Optional[Dict[str, Any]] = None):
+        self.processor = processor
+        self.component_id = component_id or self.processor.metadata['name']
+        self.params = params or {}
 
-    def call_process(self, event_id, event_instance_id, params):
-        logger.debug('calling process (%s, %s) on event: (%s, %s)',
-                     self.processor_name, self._address, event_id, event_instance_id)
-        p = dict(self.params or {})
-        if params is not None:
-            p.update(params)
-
-        with _base.Processor.enter_context() as context:
-            request = processing_pb2.ProcessRequest(processor_id=self.processor_name,
-                                                    event_id=event_id,
-                                                    event_service_instance_id=event_instance_id)
-            _structs.copy_dict_to_struct(p, request.params, [p])
-            with _base.Processor.started_stopwatch('remote_call'):
-                try:
-                    response = self._stub.Process(request,
-                                                  metadata=[('service-name', self.processor_name)])
-                except Exception as e:
-                    logger.error("Error while processing event_id %s through remote pipeline "
-                                 "component  '%s'", event_id, self.component_id)
-                    raise e
-            r = {}
-            _structs.copy_struct_to_dict(response.result, r)
-
-            timing_info = response.timing_info
-            for k, v in timing_info.items():
-                context.add_time(k, v.ToTimedelta())
-
-            created_indices = {}
-            for created_index in response.created_indices:
-                try:
-                    doc_created_indices = created_indices[created_index.document_name]
-                except KeyError:
-                    doc_created_indices = []
-                    created_indices[created_index.document_name] = doc_created_indices
-                doc_created_indices.append(created_index.index_name)
+    def __reduce__(self):
+        params = (
+            self.processor,
+            self.component_id,
+            self.params
+        )
+        return LocalProcessor, params
+
+    def create_pipeline_component(
+            self,
+            events_address: EventsAddressLike
+    ) -> 'processing.ProcessingComponent':
+        runner = _runners.LocalRunner(processor=self.processor,
+                                      events_address=events_address,
+                                      component_id=self.component_id,
+                                      params=copy.deepcopy(self.params))
+        return runner
+
+    def __repr__(self):
+        return (f"LocalProcessor(proc={self.processor}, "
+                f"component_id={self.component_id}, "
+                f"params={self.params}")
+
+
+class RemoteProcessor(ComponentDescriptor):
+    """A remote processor in a pipeline.
+
+    Attributes:
+        processor_name: The identifier used for health checking and
+            discovery.
+        address: Optionally an address to use, will use service discovery
+            configuration to locate the processor if this is ``None`` or
+            omitted.
+        component_id: How the processor's results will be identified locally.
+            Will be modified to be unique if it is not unique relative to other
+            components in a pipeline.
+        params: A parameter dictionary that will be passed to the
+            processor as parameters with every event or document processed.
+            Values should be json-serializable.
+        enable_proxy: Whether the grpc channel used to connect to the service
+            should respect the ``http_proxy`` environment variable.
+    """
+    __slots__ = (
+        'processor_name',
+        'address',
+        'component_id',
+        'params',
+        'enable_proxy'
+    )
+
+    processor_name: str
+    address: Optional[str]
+    component_id: str
+    params: Dict[str, Any]
+    enable_proxy: bool
 
-            return r, context.times, created_indices
+    def __init__(self,
+                 processor_name: str,
+                 *, address: Optional[str] = None,
+                 component_id: Optional[str] = None,
+                 params: Optional[Dict[str, Any]] = None,
+                 enable_proxy: bool = False):
+        self.processor_name = processor_name
+        self.address = address
+        self.component_id = component_id or self.processor_name
+        self.params = params or {}
+        self.enable_proxy = enable_proxy
 
-    def close(self):
-        self._channel.close()
+    def create_pipeline_component(
+            self,
+            events_address: EventsAddressLike
+    ) -> 'processing.ProcessingComponent':
+        runner = _runners.RemoteRunner(processor_name=self.processor_name,
+                                       component_id=self.component_id,
+                                       address=self.address,
+                                       params=copy.deepcopy(self.params),
+                                       enable_proxy=self.enable_proxy)
+        return runner
+
+    def __repr__(self):
+        return (f"RemoteProcessor(processor_name={self.processor_name}, "
+                f"address={self.address}, "
+                f"component_id={self.component_id}, "
+                f"params={self.params})")
```

### Comparing `mtap-1.1.0/python/mtap/processing/_service.py` & `mtap-1.2.0/python/mtap/processing/_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,79 +8,79 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import argparse
-import concurrent.futures.thread as thread
 import logging
 import signal
 import threading
 import traceback
 import typing
 import uuid
+from concurrent.futures import thread
 from logging.handlers import QueueListener
-from typing import Any, Dict, Tuple, Sequence, Optional, Union
+from typing import Any, Dict, Optional, Sequence, Tuple, Union
 
-import google.protobuf.empty_pb2 as empty_pb2
 import grpc
-import grpc_health.v1.health as health
-import grpc_health.v1.health_pb2_grpc as health_pb2_grpc
+from grpc_health.v1 import health, health_pb2_grpc
+from grpc_status import rpc_status
 
-from mtap import _config
-from mtap import _structs
-from mtap import data
-from mtap import utilities
+from mtap import _config, _structs, data, utilities
 from mtap.api.v1 import processing_pb2, processing_pb2_grpc
-from mtap.processing import _base, _runners, _timing
+from mtap.processing import _base, _runners, _pipeline_results
+from mtap.processing._error_handling import ProcessingException
 
 if typing.TYPE_CHECKING:
     import mtap
 
 logger = logging.getLogger('mtap.processing')
 
 
 def run_processor(proc: 'mtap.EventProcessor',
                   *,
                   mp: bool = False,
                   options: Optional[argparse.Namespace] = None,
                   args: Optional[Sequence[str]] = None,
                   mp_context=None):
-    """Runs the processor as a GRPC service, blocking until an interrupt signal is received.
+    """Runs the processor as a GRPC service, blocking until an interrupt signal 
+    is received.
 
     Args:
-        proc (EventProcessor): The processor to host.
-        mp (bool): If true, will create instances of ``proc`` on multiple forked processes to
-            process events. This is useful if the processor is computationally intensive and would
-            run into Python GIL issues on a single process.
-        options (~typing.Optional[~argparse.Namespace]): The parsed arguments from the parser
-            returned by :func:`processor_parser`.
-        args (~typing.Optional[~typing.Sequence[str]]): Arguments to parse server settings from if
-            ``namespace`` was not supplied.
-        mp_context: A multiprocessing context that gets passed to the process pool executor in the
-            case of mp = True.
+        proc: The processor to host.
+        mp: If true, will create instances of ``proc`` on multiple
+            forked processes to process events. This is useful if the processor 
+            is computationally intensive and would run into Python GIL issues 
+            on a single process.
+        options: The parsed arguments
+            from the parser returned by :func:`processor_parser`.
+        args: Arguments to parse
+            server settings from if ``namespace`` was not supplied.
+        mp_context: A multiprocessing context that gets passed to the process 
+            pool executor in the case of mp = True.
 
     Examples:
         Will automatically parse arguments:
 
         >>> run_processor(MyProcessor())
 
         Manual arguments:
 
         >>> run_processor(MyProcessor(), args=['-p', '8080'])
-
-
     """
     from mtap import EventProcessor
     if not isinstance(proc, EventProcessor):
-        raise ValueError("Processor must be instance of EventProcessor class.")
+        print("Processor must be instance of EventProcessor class.")
+        exit(1)
 
     if options is None:
-        processors_parser = argparse.ArgumentParser(parents=[processor_parser()])
+        processors_parser = argparse.ArgumentParser(
+            parents=[processor_parser()]
+        )
         processors_parser.add_help = True
         options = processors_parser.parse_args(args)
 
     if options.log_level:
         logging.basicConfig(level=getattr(logging, options.log_level))
 
     events_addresses = []
@@ -92,27 +92,26 @@
             c.update_from_yaml(options.mtap_config)
         # instantiate runner
         name = options.name or proc.metadata['name']
         sid = options.sid
 
         enable_http_proxy = options.grpc_enable_http_proxy
         if enable_http_proxy is not None:
-            c['grpc.events_channel_options.grpc.enable_http_proxy'] = enable_http_proxy
+            c['grpc.events_channel_options.grpc.enable_http_proxy'] \
+                = enable_http_proxy
         if mp:
             runner = MpProcessorRunner(proc=proc,
                                        workers=options.workers,
                                        events_address=events_addresses,
                                        processor_name=name,
                                        mp_context=mp_context,
                                        log_level=options.log_level)
         else:
-            client = data.EventsClient(address=events_addresses)
-            runner = _runners.ProcessorRunner(proc, client=client,
-                                              processor_name=name,
-                                              params=None)
+            runner = _runners.LocalRunner(proc,
+                                          events_address=events_addresses)
         server = ProcessorServer(runner=runner,
                                  sid=sid,
                                  host=options.host,
                                  port=options.port,
                                  register=options.register,
                                  workers=options.workers,
                                  write_address=options.write_address)
@@ -133,15 +132,18 @@
         server.stop()
 
 
 _mp_processor = ...  # EventProcessor
 _mp_client = ...  # EventClient
 
 
-def _mp_initialize(proc: 'mtap.EventProcessor', events_address, config, log_queue):
+def _mp_initialize(proc: 'mtap.EventProcessor',
+                   events_address,
+                   config,
+                   log_queue):
     global _mp_processor
     global _mp_client
 
     h = logging.handlers.QueueHandler(log_queue)
     root = logging.getLogger()
     root.addHandler(h)
     root.setLevel(logging.DEBUG)
@@ -151,23 +153,30 @@
     _mp_client = data.EventsClient(address=events_address)
 
 
 def _mp_call_process(event_id, event_service_instance_id, params):
     global _mp_processor
     global _mp_client
     with _base.Processor.enter_context() as c, \
-            data.Event(event_id=event_id, event_service_instance_id=event_service_instance_id,
+            data.Event(event_id=event_id,
+                       event_service_instance_id=event_service_instance_id,
                        client=_mp_client) as event:
         with _base.Processor.started_stopwatch('process_method'):
             result = _mp_processor.process(event, params)
         return result, c.times, event.created_indices
 
 
 class MpProcessorRunner:
-    __slots__ = ('pool', 'metadata', 'processor_name', 'component_id', 'log_listener')
+    __slots__ = (
+        'pool',
+        'metadata',
+        'processor_name',
+        'component_id',
+        'log_listener',
+    )
 
     def __init__(self,
                  proc: 'mtap.EventProcessor',
                  processor_name: str,
                  component_id: 'Optional[str]' = None,
                  workers: 'Optional[int]' = 8,
                  events_address: 'Optional[Union[str, Sequence[str]]]' = None,
@@ -180,84 +189,125 @@
         log_queue = mp_context.Queue(-1)
         handler = logging.StreamHandler()
         log_level = 'INFO' if log_level is None else log_level
         handler.setLevel(log_level)
         self.log_listener = QueueListener(log_queue, handler)
         self.log_listener.start()
 
-        self.pool = mp_context.Pool(workers,
-                                    initializer=_mp_initialize,
-                                    initargs=(proc, events_address, dict(config), log_queue))
+        self.pool = mp_context.Pool(
+            workers,
+            initializer=_mp_initialize,
+            initargs=(proc, events_address, dict(config), log_queue)
+        )
         self.metadata = proc.metadata
         self.processor_name = processor_name
         self.component_id = component_id or processor_name
 
-    def call_process(self,
-                     event_id: str,
-                     event_service_instance_id: str,
-                     params: Optional[Dict[str, Any]]) -> Tuple[Dict, Dict, Dict]:
+    def call_process(
+            self,
+            event_id: str,
+            event_service_instance_id: str,
+            params: Optional[Dict[str, Any]]
+    ) -> Tuple[Dict, Dict, Dict]:
         p = dict()
         if params is not None:
             p.update(params)
 
-        return self.pool.apply(_mp_call_process, args=(event_id, event_service_instance_id, p))
+        return self.pool.apply(_mp_call_process,
+                               args=(event_id, event_service_instance_id, p))
 
     def close(self):
         self.pool.terminate()
         self.pool.join()
         self.log_listener.stop()
 
 
 def processor_parser() -> argparse.ArgumentParser:
-    """An :class:`~argparse.ArgumentParser` that can be used to parse the settings for
-    :func:`run_processor`.
+    """An :class:`~argparse.ArgumentParser` that can be used to parse the 
+    settings for :func:`run_processor`.
 
     Returns:
-        ~argparse.ArgumentParser: A parser containing server settings.
+        A parser containing server settings.
 
     Examples:
         Using this as a parent parser:
 
         >>> parser = ArgumentParser(parents=[processor_parser()])
         >>> parser.add_argument('--my-arg-1')
         >>> parser.add_argument('--my-arg-2')
         >>> args = parser.parse_args()
         >>> processor = MyProcessor(args.my_arg_1, args.my_arg_2)
         >>> run_processor(processor, args)
 
     """
     processors_parser = argparse.ArgumentParser(add_help=False)
-    processors_parser.add_argument('--host', '--address', '-a', default="127.0.0.1", metavar="HOST",
-                                   help='the address to serve the service on')
-    processors_parser.add_argument('--port', '-p', type=int, default=0, metavar="PORT",
-                                   help='the port to serve the service on')
-    processors_parser.add_argument('--workers', '-w', type=int, default=10,
-                                   help='number of worker threads to handle requests')
-    processors_parser.add_argument('--register', '-r', action='store_true',
-                                   help='whether to register the service with the configured '
-                                        'service discovery')
-    processors_parser.add_argument("--mtap-config", default=None,
-                                   help="path to MTAP config file")
-    processors_parser.add_argument('--events-addresses', '--events-address', '--events', '-e',
-                                   default=None,
-                                   help='address of the events service to use, '
-                                        'omit to use discovery')
-    processors_parser.add_argument('--name', '-n',
-                                   help="Optional override service name, defaults to the processor annotation")
-    processors_parser.add_argument('--sid',
-                                   help="A unique identifier for this instance of the processor service.")
-    processors_parser.add_argument('--write-address', action='store_true',
-                                   help='If set, will write the server address ')
-    processors_parser.add_argument('--log-level', type=str, default='INFO',
-                                   help="Sets the python log level.")
-    processors_parser.add_argument('--grpc-enable-http-proxy', action='store_true',
-                                   help="If set, will enable usage of http_proxy by grpc.")
-    processors_parser.add_argument('--mp-spawn-method',
-                                   choices=['spawn', 'fork', 'forkserver', None],
-                                   help="A multiprocessing spawn method to use.")
+    processors_parser.add_argument(
+        '--host', '--address', '-a',
+        default="127.0.0.1",
+        metavar="HOST",
+        help='the address to serve the service on'
+    )
+    processors_parser.add_argument(
+        '--port', '-p',
+        type=int,
+        default=0,
+        metavar="PORT",
+        help='the port to serve the service on'
+    )
+    processors_parser.add_argument(
+        '--workers', '-w',
+        type=int,
+        default=10,
+        help='number of worker threads to handle requests'
+    )
+    processors_parser.add_argument(
+        '--register', '-r',
+        action='store_true',
+        help='whether to register the service with the configured service '
+             'discovery'
+    )
+    processors_parser.add_argument(
+        "--mtap-config",
+        default=None,
+        help="path to MTAP config file"
+    )
+    processors_parser.add_argument(
+        '--events-addresses', '--events-address', '--events', '-e',
+        default=None,
+        help='address of the events service to use, omit to use discovery'
+    )
+    processors_parser.add_argument(
+        '--name', '-n',
+        help="Optional override service name, defaults to the processor "
+             "annotation"
+    )
+    processors_parser.add_argument(
+        '--sid',
+        help="A unique identifier for this instance of the processor service."
+    )
+    processors_parser.add_argument(
+        '--write-address', action='store_true',
+        help='If set, will write the server address '
+    )
+    processors_parser.add_argument(
+        '--log-level',
+        type=str,
+        default='INFO',
+        help="Sets the python log level."
+    )
+    processors_parser.add_argument(
+        '--grpc-enable-http-proxy',
+        action='store_true',
+        help="If set, will enable usage of http_proxy by grpc."
+    )
+    processors_parser.add_argument(
+        '--mp-spawn-method',
+        choices=['spawn', 'fork', 'forkserver', 'None'],
+        help="A multiprocessing spawn method to use."
+    )
     return processors_parser
 
 
 def _label_index_meta_to_proto(d, message):
     message.name = d['name'] or ''
     message.name_from_parameter = d['name_from_parameter'] or ''
     message.optional = d.get('optional', False)
@@ -268,21 +318,20 @@
         p.description = property_meta['description'] or ''
         p.data_type = property_meta['data_type'] or ''
         p.nullable = property_meta['nullable']
 
 
 class _ProcessorServicer(processing_pb2_grpc.ProcessorServicer):
     def __init__(self,
-                 config: 'mtap.Config',
                  address: str,
                  sid: str,
                  runner: '_base.ProcessingComponent',
                  health_servicer: health.HealthServicer,
                  register: bool = False):
-        self.config = config
+        self.config = _config.Config()
         self.address = address
         self.sid = sid
         self._runner = runner
         self.register = register
         self.health_servicer = health_servicer
 
         self._times_map = {}
@@ -291,21 +340,23 @@
         self.failure_count = 0
 
     def start(self, port: int):
 
         self.health_servicer.set(self._runner, 'SERVING')
 
         if self.register:
-            from mtap._discovery import Discovery
-            service_registration = Discovery(config=self.config)
-            self._deregister = service_registration.register_processor_service(self._runner.processor_name,
-                                                                               self.sid,
-                                                                               self.address,
-                                                                               port,
-                                                                               'v1')
+            from mtap.discovery import DiscoveryMechanism
+            d = DiscoveryMechanism()
+            self._deregister = d.register_processor_service(
+                self._runner.processor_name,
+                self.sid,
+                self.address,
+                port,
+                'v1'
+            )
 
     def shutdown(self):
         self.health_servicer.set(self._runner.processor_name, 'NOT_SERVING')
         if self._deregister is not None:
             self._deregister()
         self._runner.close()
 
@@ -323,34 +374,34 @@
                 event_id,
                 event_service_instance_id,
                 params
             )
             if result is not None:
                 _structs.copy_dict_to_struct(result, response.result, [])
 
-            _timing.add_times(self._times_map, times)
+            _pipeline_results.add_times(self._times_map, times)
             for k, l in times.items():
                 response.timing_info[k].FromTimedelta(l)
             for document_name, l in added_indices.items():
                 for index_name in l:
                     created_index = response.created_indices.add()
                     created_index.document_name = document_name
                     created_index.index_name = index_name
             return response
-        except Exception as e:
+        except ProcessingException as e:
             logger.error(str(e))
             logger.error(traceback.format_exc())
-            context.set_code(grpc.StatusCode.INTERNAL)
-            context.set_details(str(e))
-            return empty_pb2.Empty()
+            context.abort_with_status(rpc_status.to_status(e.to_rpc_status()))
 
     def GetStats(self, request, context):
         r = processing_pb2.GetStatsResponse(processed=self.processed,
                                             failures=self.failure_count)
-        for k, v in _timing.create_timer_stats(self._times_map, self._runner.component_id).items():
+        tsd = _pipeline_results.create_timer_stats(self._times_map,
+                                                   self._runner.component_id)
+        for k, v in tsd.items():
             ts = r.timing_stats[k]
             ts.mean.FromTimedelta(v.mean)
             ts.std.FromTimedelta(v.std)
             ts.max.FromTimedelta(v.max)
             ts.min.FromTimedelta(v.min)
             ts.sum.FromTimedelta(v.sum)
         return r
@@ -360,108 +411,116 @@
         _structs.copy_dict_to_struct(self._runner.metadata, response.metadata)
         return response
 
 
 class ProcessorServer:
     """Host a MTAP processor as a service.
 
+    Normally should not need to use this class as :func:`run_processor` should
+    be sufficient for ordinary needs.
+
     Args:
-        proc (EventProcessor): The event processor to host.
-        host (str): The address / hostname / IP to host the server on.
-        port (int): The port to host the server on, or 0 to use a random port.
-
-    Keyword Args:
-        register (~typing.Optional[bool]): Whether to register the processor with service discovery.
-        events_address (~typing.Optional[str]):
-            The address of the events server, or omitted / None if the events service should be
-            discovered.
-        processor_name (~typing.Optional[str]):
-            The identifier to register the processor under, if omitted the processor name will be
-            used.
-        workers (~typing.Optional[int]):
-            The number of workers that should handle requests. Defaults to 10.
-        params (~typing.Optional[~typing.Mapping[str, ~typing.Any]):
-            A set of default parameters that will be passed to the processor every time it runs.
-        grpc_enable_http_proxy (bool):
-            Enables or disables the grpc channel to the event service using http_proxy or
-            https_proxy environment variables.
+        runner: A processing component runner to host.
+        port: The port to host the server on, or 0 to use a random port.
+        register: Whether to register the processor with service discovery.
+        workers: The number of workers that should handle requests. Defaults
+            to 10.
+
+    Attributes:
+        host: The address / hostname / IP to host the server on.
+        processor_name: The processor's service name.
+        sid: The service instance unique identifier for the processor.
+        write_address: Whether to store this processor's address in a file
+            named based on its pid in the biomedicus home directory. This is
+            useful for when the processor has a randomly assigned port.
+
+
     """
+    host: str
+    processor_name: str
+    sid: str
+    write_address: bool
 
     def __init__(self,
                  runner: 'mtap.processing.ProcessingComponent',
                  host: str,
                  port: int = 0,
                  *,
-                 sid: Optional[None] = None,
+                 sid: Optional[str] = None,
                  register: bool = False,
                  workers: Optional[int] = None,
-                 write_address: bool = False,
-                 config: 'Optional[mtap.Config]' = None):
+                 write_address: bool = False):
         self.host = host
         self.processor_name = runner.processor_name
         self.sid = sid or str(uuid.uuid4())
         self.write_address = write_address
 
-        if config is None:
-            config = _config.Config()
-
         self._health_servicer = health.HealthServicer()
         self._health_servicer.set('', 'SERVING')
         self._health_servicer.set(self.processor_name, 'SERVING')
         self._servicer = _ProcessorServicer(
-            config=config,
             address=host,
             sid=self.sid,
             runner=runner,
             health_servicer=self._health_servicer,
             register=register
         )
         workers = workers or 10
         thread_pool = thread.ThreadPoolExecutor(max_workers=workers)
+        config = _config.Config()
         options = config.get("grpc.processor_options", {})
         self._server = grpc.server(thread_pool, options=list(options.items()))
-        health_pb2_grpc.add_HealthServicer_to_server(self._health_servicer, self._server)
-        processing_pb2_grpc.add_ProcessorServicer_to_server(self._servicer, self._server)
-        self._port = self._server.add_insecure_port("{}:{}".format(self.host, port))
+        health_pb2_grpc.add_HealthServicer_to_server(self._health_servicer,
+                                                     self._server)
+        processing_pb2_grpc.add_ProcessorServicer_to_server(self._servicer,
+                                                            self._server)
+        self._port = self._server.add_insecure_port("{}:{}".format(self.host,
+                                                                   port))
         if port != 0 and self._port != port:
             raise ValueError(f"Unable to bind on port {port}, likely in use.")
         self._stopped_event = threading.Event()
         self._address_file = None
 
     @property
     def port(self) -> int:
-        """int: Port the hosted server is bound to.
+        """Port the hosted server is bound to.
         """
         return self._port
 
     def start(self):
         """Starts the service.
         """
         self._server.start()
         self._servicer.start(self.port)
         if self.write_address:
-            self._address_file = utilities.write_address_file('{}:{}'.format(self.host, self.port), self.sid)
-        logger.info('Started processor server with name: "%s"  on address: "%s:%d"',
-                    self.processor_name, self.host, self.port)
+            self._address_file = utilities.write_address_file(
+                '{}:{}'.format(self.host, self.port), self.sid)
+        logger.info(
+            'Started processor server with name: "%s"  on address: "%s:%d"',
+            self.processor_name, self.host, self.port)
 
     def stop(self, *, grace: Optional[float] = None) -> threading.Event:
-        """De-registers (if registered with service discovery) the service and immediately stops
-        accepting requests, completely stopping the service after a specified `grace` time.
-
-        During the grace period the server will continue to process existing requests, but it will
-        not accept any new requests. This function is idempotent, multiple calls will shutdown
-        the server after the soonest grace to expire, calling the shutdown event for all calls to
+        """De-registers (if registered with service discovery) the service and
+        immediately stops accepting requests, completely stopping the service
+        after a specified `grace` time.
+
+        During the grace period the server will continue to process existing
+        requests, but it will not accept any new requests. This function is
+        idempotent, multiple calls will shut down the server after the soonest
+        grace to expire, calling the shutdown event for all calls to
         this function.
 
-        Keyword Args:
-            grace (~typing.Optional[float]):
-                The grace period that the server should continue processing requests for shutdown.
+        Args:
+            grace: The grace period that the server should continue processing
+                requests or ``None`` if it should shut down immediately.
 
         Returns:
-            threading.Event: A shutdown event for the server.
+            A shutdown event for the server.
         """
-        print('Shutting down processor server with name: "{}"  on address: "{}:{}"'.format(
-            self.processor_name, self.host, self.port))
+        print(
+            f'Shutting down processor server with name: '
+            f'"{self.processor_name}" on address: "{self.host}:{self.port}"'
+        )
         if self._address_file is not None:
             self._address_file.unlink()
         self._servicer.shutdown()
         return self._server.stop(grace=grace)
```

### Comparing `mtap-1.1.0/python/mtap/processing/descriptions.py` & `mtap-1.2.0/python/mtap/processing/descriptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,191 +1,68 @@
-# Copyright 2019 Regents of the University of Minnesota.
+# Copyright 2023 Regents of the University of Minnesota.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Descriptors for processor functionality."""
 import typing
-from typing import NamedTuple, Optional, List, Type, Dict, Any
+from typing import NamedTuple, Optional, List, Dict, Any
 
 if typing.TYPE_CHECKING:
     from mtap import EventProcessor
 
 __all__ = [
     'label_property',
     'labels',
     'parameter',
     'processor',
 ]
 
 
-class label_property(NamedTuple('label_property',
-                                [('name', str),
-                                 ('description', Optional[str]),
-                                 ('data_type', Optional[str]),
-                                 ('nullable', bool)])):
-    """Creates a description for a property on a label.
-
-    Args:
-        name (str): The property's name.
-
-    Keyword Args:
-        description (~typing.Optional[str]): A short description of the property.
-        data_type (~typing.Optional[str]):
-            The data type of the property: str, float, or bool; List[T] or Mapping[T1, T2] of those.
-        nullable (bool): Whether the property can have a valid value of null.
-    """
-
-    def __new__(cls,
-                name: str,
-                *,
-                nullable: bool = False,
-                description: Optional[str] = None,
-                data_type: Optional[str] = None):
-        return super().__new__(cls, name, description, data_type, nullable)
-
-
-class labels(NamedTuple('LabelDescription',
-                        [('name', str),
-                         ('reference', Optional[str]),
-                         ('name_from_parameter', Optional[str]),
-                         ('optional', bool),
-                         ('description', Optional[str]),
-                         ('properties', List[label_property])])):
-    """A description for a label type.
-
-    Args:
-        name (str): The label index name.
-
-    Keyword Args:
-        reference (~typing.Optional[str]):
-            If this is an output of another processor, that processor's name followed by a slash
-            and the default output name of the index go here.
-            Example: "sentence-detector/sentences".
-        optional (bool): Whether this label index is an optional input or output.
-        name_from_parameter (~typing.Optional[str]):
-            If the label index gets its name from a processor parameter, the name of the parameter.
-        description (~typing.Optional[str]): A short description of the label index.
-        properties (~typing.Optional[~typing.List[label_property]]):
-            The properties of the labels in the label index.
-
-    Attributes:
-        name (str): The label index name.
-        reference (~typing.Optional[str]):
-            If this is an output of another processor, that processor's name followed by a slash
-            and the default output name of the index go here.
-            Example: "sentence-detector/sentences".
-        optional (bool): Whether this label index is an optional input or output.
-        name_from_parameter (~typing.Optional[str]):
-            If the label index gets its name from a processor parameter, the name of the parameter.
-        description (~typing.Optional[str]): A short description of the label index.
-        properties (~typing.Optional[~typing.List[label_property]]):
-            The properties of the labels in the label index.
-    """
-
-    def __new__(cls,
-                name: str,
-                *,
-                reference: Optional[str] = None,
-                optional: bool = False,
-                name_from_parameter: Optional[str] = None,
-                description: Optional[str] = None,
-                properties: Optional[List[label_property]] = None):
-        return super().__new__(cls, name, reference, name_from_parameter, optional, description,
-                               properties)
-
-
-class parameter(NamedTuple('parameter',
-                           [('name', str),
-                            ('description', Optional[str]),
-                            ('data_type', Optional[str]),
-                            ('required', bool)])):
-    def __new__(cls,
-                name: str,
-                *,
-                required: bool = False,
-                data_type: Optional[str] = None,
-                description: Optional[str] = None):
-        """A description of one of the processor's parameters.
-
-        Args:
-            name (str): The parameter name / key.
-
-        Keyword Args:
-            required (bool): Whether the processor parameter is required.
-            data_type (~typing.Optional[str]):
-                The data type of the parameter. str, float, or bool; List[T] or Mapping[T1, T2] of
-                those.
-            description (~typing.Optional[str]): A short description of the property and what it
-                does.
-
-        Attributes:
-            name (str): The parameter name / key.
-            required (bool): Whether the processor parameter is required.
-            data_type (~typing.Optional[str]):
-                The data type of the parameter. str, float, or bool; List[T] or Mapping[T1, T2] of
-                those.
-            description (~typing.Optional[str]): A short description of the property and what it
-                does.
-
-
-        Returns:
-            ParameterDescription: The parameter description object
-        """
-        return super().__new__(cls, name=name, description=description, data_type=data_type,
-                               required=required)
-
-
 def processor(name: str,
               *,
               human_name: Optional[str] = None,
               description: Optional[str] = None,
-              parameters: Optional[List[parameter]] = None,
-              inputs: Optional[List[labels]] = None,
-              outputs: Optional[List[labels]] = None,
-              **additional_metadata: str):
-    """Decorator which attaches a service name and metadata to a processor. Which then can be used
-    for runtime reflection of how the processor works.
+              parameters: 'Optional[List[parameter]]' = None,
+              inputs: 'Optional[List[labels]]' = None,
+              outputs: 'Optional[List[labels]]' = None,
+              **additional_metadata: Any):
+    """Decorator which attaches a service name and metadata to a processor.
+    Which then can be used for runtime reflection of how the processor works.
 
     Args:
-        name (str):
-            Identifying service name both for launching via command line and for service
-            registration.
-
-            Should be a mix of alphanumeric characters and dashes so that it plays nice with the
-            DNS name requirements of service discovery tools like Consul. Can be overridden at
-            runtime via the `identifier` option on :func:`processor_parser`.
-
-    Keyword Args:
-        human_name (~typing.Optional[str]): An option human name for the processor.
-        description (~typing.Optional[str]): A short description of the processor and what it does.
-        parameters (~typing.Optional[~typing.List[ParameterDescription]]):
-            The processor's parameters.
-        inputs (~typing.Optional[~typing.List[str]]):
-            String identifiers for the output from a processor that this processor uses as an input.
-
-            Takes the format "[processor-name]/[output]". Examples would be "tagger:pos_tags" or
-            "sentence-detector:sentences".
-        outputs (~typing.Optional[~typing.List[LabelDescription]]):
-            The label indices this processor outputs.
-        **additional_metadata (~typing.Any):
-            Any other data that should be added to the processor's metadata, should be serializable
-            to yaml and json.
+        name: Identifying service name both for launching via command line and
+            for service registration.
+            Should be a mix of alphanumeric characters and dashes so that it
+            plays nice with the DNS name requirements of service discovery
+            tools like Consul.
+        human_name: An optional human name for the processor.
+        description: A short description of the processor and what it does.
+        parameters: The processor's parameters.
+        inputs: String identifiers for the label output from a previously-run
+            processor that this processor requires as an input.
+
+            Takes the format ``"[processor-name]/[output]"``. Examples would be
+            ``"tagger/pos_tags"`` or ``"sentence-detector/sentences"``.
+        outputs: The label indices this processor outputs.
+        **additional_metadata: Any other data that should be added to the
+            processor's metadata, should be serializable to yaml and json.
 
     Returns:
-        A decorator to be applied to instances of EventProcessor or DocumentProcessor. This
-        decorator attaches the metadata so it can be reflected at runtime.
+        A decorator to be applied to instances of EventProcessor or
+        DocumentProcessor. This decorator attaches the metadata, so it can be
+        reflected at runtime.
 
     Examples:
         >>> from mtap.processing import EventProcessor
         >>> @processor('example-text-converter')
         >>> class TextConverter(EventProcessor):
         >>>     ...
 
@@ -197,51 +74,122 @@
         >>>     ...
 
         From our own example processor:
 
         >>> from mtap.processing import DocumentProcessor
         >>> @processor('mtap-example-processor-python',
         >>>            human_name="Python Example Processor",
-        >>>            description="counts the number of times the letters a and b occur in a document",
+        >>>            description="counts the number of times the letters a"
+        >>>                        "and b occur in a document",
         >>>            parameters=[
-        >>>                parameter('do_work', required=True, data_type='bool',
-        >>>                          description="Whether the processor should do anything.")
+        >>>                parameter(
+        >>>                     'do_work',
+        >>>                     required=True,
+        >>>                     data_type='bool',
+        >>>                     description="Whether the processor should do"
+        >>>                                 "anything."
+        >>>                )
         >>>            ],
         >>>            outputs=[
         >>>                labels('mtap.examples.letter_counts',
-        >>>                            properties=[label_property('letter', data_type='str'),
-        >>>                                        label_property('count', data_type='int')])
+        >>>                       properties=[label_property('letter',
+        >>>                                                  data_type='str'),
+        >>>                                   label_property('count',
+        >>>                                                  data_type='int')])
         >>>            ])
         >>> class ExampleProcessor(DocumentProcessor):
         >>>     ...
 
 
     """
 
-    def decorator(f: Type['EventProcessor']) -> Type['EventProcessor']:
-        f.metadata = {
+    def decorator(cls):
+        cls.metadata = {
             'name': name,
             'human_name': human_name,
             'description': description
         }
         if parameters is not None:
-            f.metadata['parameters'] = [_parameter_to_map(p) for p in parameters]
+            cls.metadata['parameters'] = [_parameter_to_map(p)
+                                          for p in parameters]
         if inputs is not None:
-            f.metadata['inputs'] = [_desc_to_dict(desc) for desc in inputs]
+            cls.metadata['inputs'] = [_desc_to_dict(desc) for desc in inputs]
         if outputs is not None:
-            f.metadata['outputs'] = [_desc_to_dict(desc) for desc in outputs]
+            cls.metadata['outputs'] = [_desc_to_dict(desc) for desc in outputs]
         if additional_metadata is not None:
-            f.metadata.update(additional_metadata)
-        if 'implementation_lang' not in f.metadata:
-            f.metadata['implementation_lang'] = 'Python'
-        return f
+            cls.metadata.update(additional_metadata)
+        if 'implementation_lang' not in cls.metadata:
+            cls.metadata['implementation_lang'] = 'Python'
+
+        return cls
 
     return decorator
 
 
+class parameter(NamedTuple):
+    """A description of one of the processor's parameters.
+    """
+    name: str
+    """The parameter name / key."""
+
+    description: Optional[str] = None
+    """A short description of the property and what it does."""
+
+    data_type: Optional[str] = None
+    """The data type of the parameter. str, float, or bool; List[T] 
+    or Mapping[T1, T2] of those."""
+
+    required: bool = False
+    """Whether the processor parameter is required."""
+
+
+class labels(NamedTuple):
+    """A description for a label type.
+    """
+    name: str
+    """The label index name."""
+
+    reference: Optional[str] = None
+    """If this is an output of another processor, that processor's
+    name followed by a slash and the default output name of the index
+    go here.
+    Example: "sentence-detector/sentences"."""
+
+    name_from_parameter: Optional[str] = None
+    """If the label index gets its name from a parameter of the processor, 
+    specify that name here."""
+
+    optional: bool = False
+    """Whether this label index is an optional input or  output."""
+
+    description: Optional[str] = None
+    """A short description of the label index."""
+
+    properties: 'Optional[List[label_property]]' = None
+    """The properties of the labels in the label index."""
+
+
+class label_property(NamedTuple):
+    """Creates a description for a property on a label.
+    """
+    name: str
+    """The property's name."""
+
+    description: Optional[str] = None
+    """A short description of the property."""
+
+    data_type: Optional[str] = None
+    """The data type of the property. Options are ``"str"``, ``"float"``, or 
+    ``"bool"``; ``"List[T]"`` or ``"Mapping[str, T]"`` where ``T`` is 
+    one of those types."""
+
+    nullable: bool = False
+    """Whether the property can have a valid value of null."""
+
+
 def _desc_to_dict(description: labels) -> dict:
     m = {
         'name': description.name
     }
     if description.name_from_parameter is not None:
         m['name_from_parameter'] = description.name_from_parameter
     if description.reference is not None:
```

### Comparing `mtap-1.1.0/python/mtap/processors/__init__.py` & `mtap-1.2.0/python/mtap/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/processors/copy_document.py` & `mtap-1.2.0/python/mtap/processors/copy_document.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/serialization/__init__.py` & `mtap-1.2.0/python/mtap/serialization/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,9 +20,11 @@
     dict_to_document,
     Serializer,
     SerializationProcessor,
     JsonSerializer,
     YamlSerializer,
     PickleSerializer,
     standard_serializers,
-    get_serializer
+    get_serializer,
+    SerializerRegistry,
+    SerializerFactory,
 )
```

### Comparing `mtap-1.1.0/python/mtap/serialization/_serialization.py` & `mtap-1.2.0/python/mtap/serialization/_serialization.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,87 +1,76 @@
-#  Copyright 2022 Regents of the University of Minnesota.
+#  Copyright 2023 Regents of the University of Minnesota.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-"""Serialization, serializers, and helper methods for going to and from flattened python dictionary
-representations of events.
-
-Attributes:
-    JsonSerializer (Serializer): For serializing to and from json.
-
+"""Serialization, serializers, and helper methods for going to and from
+flattened python dictionary representations of events.
 """
 import io
 import logging
 from abc import ABC, abstractmethod
+from os import PathLike
 from pathlib import Path
-from typing import Union, Dict, Any, Optional, TextIO
+from typing import Union, Dict, Any, Optional, TextIO, Callable
 
 import mtap
 from mtap import data, processing
-from mtap import descriptions as d
+from mtap.processing.descriptions import *
 
 logger = logging.getLogger('mtap.serialization')
 
 
-def event_to_dict(event: mtap.Event, *, include_label_text: bool = False) -> Dict:
+def event_to_dict(event: mtap.Event, *,
+                  include_label_text: bool = False) -> Dict:
     """A helper method that turns an event into a python dictionary.
 
     Args:
-        event (Event): The event object.
-
-    Keyword Args:
-        include_label_text (bool): Whether to include the text labels cover with the labels.
+        event: The event object.
+        include_label_text: Whether to include the text labels cover with the
+            labels.
 
     Returns:
         dict: A dictionary object suitable for serialization.
 
     """
     d = {
         'event_id': event.event_id,
         'metadata': {},
         'documents': {}
     }
     for k, v in event.metadata.items():
         d['metadata'][k] = v
     for doc in event.documents.values():
-        d['documents'][doc.document_name] = document_to_dict(doc,
-                                                             include_label_text=include_label_text)
+        d['documents'][doc.document_name] = document_to_dict(
+            doc,
+            include_label_text=include_label_text
+        )
     return d
 
 
-def document_to_dict(document: mtap.Document, *, include_label_text: bool = False) -> Dict:
+def document_to_dict(document: mtap.Document, *,
+                     include_label_text: bool = False) -> Dict:
     """A helper method that turns a document into a python dictionary.
 
     Args:
-        document (Document): The document object.
-        include_label_text (bool): Whether to include the text labels cover with the labels.
+        document: The document object.
+        include_label_text: Whether to include the text labels cover with the
+            labels.
 
     Returns:
-        dict: A dictionary object suitable for serialization.
+        A dictionary object suitable for serialization.
     """
     d = {
         'text': document.text,
         'label_indices': {}
     }
 
     for index_name, index in document.labels.items():
@@ -91,23 +80,26 @@
         d['label_indices'][index_name] = adapter.pack(
             index,
             include_label_text=include_label_text
         )
     return d
 
 
-def dict_to_event(d: Dict, *, client: Optional[mtap.EventsClient] = None) -> mtap.Event:
+def dict_to_event(d: Dict, *,
+                  client: Optional[mtap.EventsClient] = None) -> mtap.Event:
     """Turns a serialized dictionary into an Event.
 
     Args:
-        d (dict): The dictionary representation of the event.
-        client (~typing.Optional[EventsClient]): An events service to create the event on.
+        d: A json-like (only ``str`` keys) dictionary representation of the
+            event.
+        client: If specified, will upload the event to this events service.
+            Otherwise, creates a local event.
 
     Returns:
-        Event: The deserialized event object.
+        The deserialized event object.
     """
     event = mtap.Event(event_id=d['event_id'], client=client)
     for k, v in d['metadata'].items():
         event.metadata[k] = v
     for k, v in d['documents'].items():
         dict_to_document(k, v, event=event)
     return event
@@ -115,20 +107,22 @@
 
 def dict_to_document(document_name: str,
                      d: Dict,
                      *, event: Optional[mtap.Event] = None) -> mtap.Document:
     """Turns a serialized dictionary into a Document.
 
     Args:
-        document_name (str): The name identifier of the document on the event.
-        d (dict): The dictionary representation of the document.
-        event (~typing.Optional[Event]): An event that the document should be added to.
+        document_name: The name identifier of the document.
+        d: A json-like (only ``str`` keys) dictionary representation of the
+            document.
+        event: If specified, the function will add the document to this
+            event. Otherwise, it will create a stand-alone document.
 
     Returns:
-        Document: The deserialized Document object.
+        The deserialized Document object.
 
     """
     document = mtap.Document(document_name=document_name, text=d['text'])
     if event is not None:
         event.add_document(document)
     for k, v in d['label_indices'].items():
         adapter = document.get_default_adapter(k)
@@ -145,106 +139,167 @@
     @property
     @abstractmethod
     def extension(self) -> str:
         """str: Filename extension, including period. Ex: ``'.json'``."""
         ...
 
     @abstractmethod
-    def event_to_file(self, event: mtap.Event, f: Union[Path, str, TextIO],
-                      *, include_label_text: bool = False):
+    def event_to_file(
+            self,
+            event: mtap.Event,
+            f: Union[str, bytes, PathLike, TextIO],
+            *, include_label_text: bool = False
+    ):
         """Writes the event to a file.
 
         Args:
             event (Event): The event object to serialize.
             f (~typing.Union[~pathlib.Path, str, ~io.IOBase]):
                 A file or a path to a file to write the event to.
             include_label_text (bool):
-                Whether, when serializing, to include the text that each label covers with the rest
-                of the label.
+                Whether, when serializing, to include the text that each label
+                covers with the rest of the label.
         """
         ...
 
     @abstractmethod
-    def file_to_event(self, f: Union[Path, str, TextIO], *,
-                      client: Optional[mtap.EventsClient] = None) -> mtap.Event:
+    def file_to_event(
+            self,
+            f: Union[str, bytes, PathLike, TextIO], *,
+            client: Optional[mtap.EventsClient] = None
+    ) -> mtap.Event:
         """Loads an event from a serialized file.
 
         Args:
-            f (~typing.Union[~pathlib.Path, str, ~io.IOBase]): The file to load from.
-            client (~typing.Optional[EventsClient]): The events service to load the event into.
+            f (~typing.Union[~pathlib.Path, str, ~io.IOBase]):
+                The file to load from.
+            client (~typing.Optional[EventsClient]):
+                The events service to load the event into.
 
         Returns:
             Event: The loaded event object.
         """
         ...
 
 
-@mtap.processor('mtap-serializer',
-                description='Serializes events to a specific directory',
-                parameters=[d.parameter('filename', data_type='str',
-                                        description='Optional override for the filename to write the '
-                                                    'document to.')])
+SerializerFactory = Callable[[Dict[str, Any]], Serializer]
+
+registry: Dict[str, SerializerFactory] = {}
+
+
+class SerializerRegistry:
+    @staticmethod
+    def register(
+            name: str
+    ) -> Callable[[SerializerFactory], SerializerFactory]:
+        def decorate(f: SerializerFactory) -> SerializerFactory:
+            registry[name] = f
+            return f
+
+        return decorate
+
+    @staticmethod
+    def create(name: str,
+               params: Optional[Dict[str, Any]] = None) -> Serializer:
+        return registry[name](**params)
+
+    @staticmethod
+    def from_dict(conf: Dict[str, Any]):
+        name = conf['name']
+        params = conf.get('params', {})
+        return SerializerRegistry.create(name, params)
+
+
+@mtap.processing.processor(
+    'mtap-serializer',
+    description='Serializes events to a specific directory',
+    parameters=[
+        parameter(
+            'filename',
+            data_type='str',
+            description='Optional override for the filename '
+                        'to write the document to.'
+        )
+    ]
+)
 class SerializationProcessor(mtap.EventProcessor):
-    """An MTAP :obj:`EventProcessor` that serializes events to a specific directory.
+    """An MTAP :obj:`EventProcessor` that serializes events to a specific
+    directory.
 
-    Args:
-        ser (Serializer): The serializer to use.
-        output_dir (str): The output_directory.
-    """
+    Attributes:
+        serializer: The serializer to use.
+        output_dir: The output directory.
+        include_label_text: Whether to attach the covered text to labels.
 
-    def __init__(self, ser: Serializer, output_dir: str, include_label_text: bool = False):
-        self.serializer = ser
+    """
+    serializer: Serializer
+    output_dir: Union[str, bytes, PathLike]
+    include_label_text: bool
+
+    def __init__(
+            self,
+            serializer: Serializer,
+            output_dir: Union[str, bytes, PathLike],
+            include_label_text: bool = False
+    ):
+        self.serializer = serializer
         self.output_dir = output_dir
         self.include_label_text = include_label_text
         Path(self.output_dir).mkdir(parents=True, exist_ok=True)
 
     def process(self, event: mtap.Event, params: Dict[str, Any]):
-        name = params.get('filename', event.event_id + self.serializer.extension)
+        name = params.get('filename',
+                          event.event_id + self.serializer.extension)
         path = Path(self.output_dir, name)
-        self.serializer.event_to_file(event, path, include_label_text=self.include_label_text)
+        self.serializer.event_to_file(
+            event, path, include_label_text=self.include_label_text)
 
 
+@SerializerRegistry.register('json')
 class _JsonSerializer(Serializer):
     """Serializer implementation that performs serialization to JSON.
     """
-
     @property
     def extension(self) -> str:
         return '.json'
 
-    def event_to_file(self, event: mtap.Event, f: Union[Path, str, TextIO], *, include_label_text: bool = False):
+    def event_to_file(self, event: mtap.Event, f: Union[Path, str, TextIO], *,
+                      include_label_text: bool = False):
         import json
         with processing.Processor.started_stopwatch('transform'):
             d = event_to_dict(event, include_label_text=include_label_text)
         with processing.Processor.started_stopwatch('io'):
             try:
                 json.dump(d, f)
             except AttributeError:
                 f = Path(f)
                 f.parent.mkdir(parents=True, exist_ok=True)
                 with f.open('w') as f:
                     json.dump(d, f)
 
     def file_to_event(self, f: Union[Path, str, TextIO],
-                      client: Optional[mtap.EventsClient] = None) -> mtap.Event:
+                      client: Optional[
+                          mtap.EventsClient] = None) -> mtap.Event:
         import json
         with processing.Processor.started_stopwatch('io'):
             try:
                 d = json.load(f)
             except AttributeError:
                 if isinstance(f, str):
                     f = Path(f)
                 with f.open('r') as f:
                     d = json.load(f)
         with processing.Processor.started_stopwatch('transform'):
             return dict_to_event(d, client=client)
 
 
+@SerializerRegistry.register('yaml')
 class _YamlSerializer(Serializer):
-
+    """Serializer implementation that performs serialization to YAML.
+    """
     @property
     def extension(self) -> str:
         return '.yml'
 
     def event_to_file(self, event: mtap.Event, f: Union[Path, str, TextIO], *,
                       include_label_text: bool = False):
         import yaml
@@ -259,15 +314,16 @@
                 yaml.dump(d, f, Dumper=Dumper)
             else:
                 f = Path(f)
                 with f.open('w') as f:
                     yaml.dump(d, f, Dumper=Dumper)
 
     def file_to_event(self, f: Union[Path, str, TextIO], *,
-                      client: Optional[mtap.EventsClient] = None) -> mtap.Event:
+                      client: Optional[
+                          mtap.EventsClient] = None) -> mtap.Event:
         import yaml
         try:
             from yaml import CLoader as Loader
         except ImportError:
             from yaml import Loader
         with processing.Processor.started_stopwatch('io'):
             if isinstance(f, io.IOBase):
@@ -275,16 +331,18 @@
             else:
                 with Path(f).open() as f:
                     d = yaml.load(f, Loader=Loader)
         with processing.Processor.started_stopwatch('transform'):
             return dict_to_event(d, client=client)
 
 
+@SerializerRegistry.register('pickle')
 class _PickleSerializer(Serializer):
-
+    """Serializer implementation that performs serialization to .pickle.
+    """
     @property
     def extension(self) -> str:
         return '.pickle'
 
     def event_to_file(self, event: mtap.Event, f: Union[Path, str, TextIO], *,
                       include_label_text: bool = False):
         import pickle
@@ -294,32 +352,45 @@
             try:
                 pickle.dump(d, f)
             except TypeError:
                 with Path(f).open('wb') as f:
                     pickle.dump(d, f)
 
     def file_to_event(self, f: Union[Path, str, TextIO], *,
-                      client: Optional[mtap.EventsClient] = None) -> mtap.Event:
+                      client: Optional[
+                          mtap.EventsClient] = None) -> mtap.Event:
         import pickle
         with processing.Processor.started_stopwatch('io'):
             try:
                 d = pickle.load(f)
             except TypeError:
                 with Path(f).open('rb') as f:
                     d = pickle.load(f)
         with processing.Processor.started_stopwatch('transform'):
             return dict_to_event(d, client=client)
 
 
-JsonSerializer = _JsonSerializer()
-YamlSerializer = _YamlSerializer()
-PickleSerializer = _PickleSerializer()
+JsonSerializer: Serializer = _JsonSerializer()
+
+YamlSerializer: Serializer = _YamlSerializer()
+
+PickleSerializer: Serializer = _PickleSerializer()
 
 standard_serializers = {
     'json': JsonSerializer,
     'yml': YamlSerializer,
     'pickle': PickleSerializer
 }
 
 
-def get_serializer(identifier):
+def get_serializer(identifier: str) -> Serializer:
+    """Returns a serializer by its identifier.
+
+    Options are: ``json``, ``yml``, and ``pickle``.
+
+    Parameters:
+        identifier: The serializer identifier.
+
+    Returns:
+        The specified serializer.
+    """
     return standard_serializers[identifier]
```

### Comparing `mtap-1.1.0/python/mtap/serialization/brat.py` & `mtap-1.2.0/python/mtap/serialization/brat.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/serialization/event.schema.json` & `mtap-1.2.0/python/mtap/serialization/event.schema.json`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/utilities/__init__.py` & `mtap-1.2.0/python/mtap/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap/utilities/tokenization.py` & `mtap-1.2.0/python/mtap/utilities/tokenization.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/mtap.egg-info/PKG-INFO` & `mtap-1.2.0/python/mtap.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtap
-Version: 1.1.0
+Version: 1.2.0
 Summary: A framework for distributed text analysis using gRPC and microservices-based architecture.
 Author-email: University of Minnesota NLP/IE Group <nlp-ie@umn.edu>, Ben Knoll <benknoll@umn.edu>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -235,15 +235,15 @@
 Provides-Extra: docs
 Provides-Extra: consul
 License-File: LICENSE.txt
 
 <p align="center">
   <a href="https://pypi.org/project/mtap/">
     <img src="https://img.shields.io/pypi/v/mtap" /></a>
-  <a href="https://central.sonatype.com/artifact/edu.umn.nlpie/mtap/1.1.0">
+  <a href="https://mvnrepository.com/artifact/edu.umn.nlpie/mtap">
     <img src="https://img.shields.io/maven-central/v/edu.umn.nlpie/mtap" /></a>
 </p>
 
 # MTAP
 
 [nlpie.github.io/mtap](https://nlpie.github.io/mtap)
 
@@ -270,48 +270,21 @@
 
 By using the microservice pattern, text analysis components can be deployed once and then mixed and matched in different pipelines. Components written in different languages can interoperate without hassle. We also provide a RESTful API gateway that lets you call components using HTTP.
 
 ### Scalability
 
 MTAP is designed to bridge the gap between prototyping new ideas and deploying them into a production environment. It supports calling components locally without using any network infastructure all the way up to deploying services and using service discovery via Consul to build pipelines.
 
-## Getting started
-
-### Installation
-
-#### Python
-```bash
-pip install mtap
-```
-
-#### Java
-
-Gradle:
-
-```groovy
-implementation 'edu.umn.nlpie:mtap:1.1.0'
-```
-
-Maven:
-
-```xml
-<dependency>
-  <groupId>edu.umn.nlpie</groupId>
-  <artifactId>mtap</artifactId>
-  <version>1.1.0</version>
-</dependency>
-```
-
-### Instructions
+## Instructions
 
 We make getting started tutorials available on our project website for both [Python](https://nlpie.github.io/mtap/docs/tutorials/python.html) and [Java](https://nlpie.github.io/mtap/docs/tutorials/java.html).
 
-### About Us
+## About Us
 
 MTAP is developed at the University of Minnesota by the [NLP/IE Group in the Institute for Health Informatics](https://healthinformatics.umn.edu/research/nlpie-group).
 
-### Acknowledgements
+## Acknowledgements
 Funding for this work was provided by:
 
 - 1 R01 LM011364-01 NIH-NLM
 - 1 R01 GM102282-01A1 NIH-NIGMS
 - U54 RR026066-01A2 NIH-NCRR
```

### Comparing `mtap-1.1.0/python/mtap.egg-info/SOURCES.txt` & `mtap-1.2.0/python/mtap.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .dockerignore
 .flake8
 .gitignore
+.readthedocs.yaml
 Dockerfile-dev
 LICENSE.txt
 README.md
 pyproject.toml
 setup.py
 .github/dependabot.yml
 .github/workflows/ci.yml
@@ -12,19 +13,18 @@
 go/doc.go
 go/go.mod
 go/go.sum
 go/tools.go
 go/mtap-gateway/mtap-gateway.go
 go/mtap/api/v1/events.pb.go
 go/mtap/api/v1/events.pb.gw.go
-go/mtap/api/v1/events.swagger.json
+go/mtap/api/v1/events_grpc.pb.go
 go/mtap/api/v1/processing.pb.go
 go/mtap/api/v1/processing.pb.gw.go
-go/mtap/api/v1/processing.swagger.json
-go/mtap/api/v1/swaggers.go
+go/mtap/api/v1/processing_grpc.pb.go
 go/mtap/consul/resolver.go
 go/mtap/processors/processors.go
 go/store-swaggers/main.go
 go/third_party/googleapis/google/api/annotations.proto
 go/third_party/googleapis/google/api/field_behavior.proto
 go/third_party/googleapis/google/api/http.proto
 go/third_party/googleapis/google/api/httpbody.proto
@@ -48,14 +48,15 @@
 java/src/main/java/edu/umn/nlpie/mtap/common/JsonObjectImpl.java
 java/src/main/java/edu/umn/nlpie/mtap/common/Server.java
 java/src/main/java/edu/umn/nlpie/mtap/discovery/ConsulDiscoveryMechanism.java
 java/src/main/java/edu/umn/nlpie/mtap/discovery/ConsulNameResolverProvider.java
 java/src/main/java/edu/umn/nlpie/mtap/discovery/Discovery.java
 java/src/main/java/edu/umn/nlpie/mtap/discovery/DiscoveryMechanism.java
 java/src/main/java/edu/umn/nlpie/mtap/discovery/ServiceInfo.java
+java/src/main/java/edu/umn/nlpie/mtap/examples/ErrorThrower.java
 java/src/main/java/edu/umn/nlpie/mtap/examples/HelloWorldExample.java
 java/src/main/java/edu/umn/nlpie/mtap/examples/ReferenceLabelsExampleProcessor.java
 java/src/main/java/edu/umn/nlpie/mtap/examples/WordOccurrencesExampleProcessor.java
 java/src/main/java/edu/umn/nlpie/mtap/examples/package-info.java
 java/src/main/java/edu/umn/nlpie/mtap/exc/EventExistsException.java
 java/src/main/java/edu/umn/nlpie/mtap/exc/FailedToConnectToEventsException.java
 java/src/main/java/edu/umn/nlpie/mtap/exc/MtapException.java
@@ -131,20 +132,20 @@
 python/docs/index.rst
 python/docs/make.bat
 python/docs/mtap.rst
 python/docs/serialization.rst
 python/mtap/__init__.py
 python/mtap/__main__.py
 python/mtap/_config.py
-python/mtap/_discovery.py
 python/mtap/_events_service.py
 python/mtap/_structs.py
 python/mtap/constants.py
 python/mtap/defaultConfig.yml
 python/mtap/deployment.py
+python/mtap/discovery.py
 python/mtap/metrics.py
 python/mtap/version.py
 python/mtap.egg-info/PKG-INFO
 python/mtap.egg-info/SOURCES.txt
 python/mtap.egg-info/dependency_links.txt
 python/mtap.egg-info/requires.txt
 python/mtap.egg-info/top_level.txt
@@ -170,18 +171,24 @@
 python/mtap/examples/serialization/__init__.py
 python/mtap/examples/serialization/brat_converter.py
 python/mtap/examples/tutorial/__init__.py
 python/mtap/examples/tutorial/hello.py
 python/mtap/examples/tutorial/pipeline.py
 python/mtap/processing/__init__.py
 python/mtap/processing/_base.py
+python/mtap/processing/_error_handling.py
+python/mtap/processing/_exc.py
+python/mtap/processing/_mp_config.py
+python/mtap/processing/_mp_pipeline.py
 python/mtap/processing/_pipeline.py
+python/mtap/processing/_pipeline_components.py
+python/mtap/processing/_pipeline_results.py
 python/mtap/processing/_runners.py
 python/mtap/processing/_service.py
-python/mtap/processing/_timing.py
+python/mtap/processing/_sources.py
 python/mtap/processing/descriptions.py
 python/mtap/processors/__init__.py
 python/mtap/processors/copy_document.py
 python/mtap/serialization/__init__.py
 python/mtap/serialization/_serialization.py
 python/mtap/serialization/brat.py
 python/mtap/serialization/event.schema.json
```

### Comparing `mtap-1.1.0/python/tests/config/test_config.py` & `mtap-1.2.0/python/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/conftest.py` & `mtap-1.2.0/python/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 def _listen(process: subprocess.Popen):
     for line in process.stdout:
         print(line.decode(), end='')
     return process.wait()
 
 
-@pytest.fixture(name='processor_watcher')
+@pytest.fixture(name='processor_watcher', scope="session")
 def fixture_processor_watcher():
     def func(address, process, timeout=20.0):
         listener = Thread(target=_listen, args=(process,))
         listener.start()
         try:
             if process.returncode is not None:
                 raise ValueError('subprocess terminated')
@@ -93,15 +93,15 @@
                     listener.join()
                 print("processor exited with code: ", process.returncode)
             except Exception:
                 pass
     return func
 
 
-@pytest.fixture(name='java_exe')
+@pytest.fixture(name='java_exe', scope="session")
 def fixture_java_exe():
     import pathlib
     try:
         mtap_jar = os.environ['MTAP_JAR']
     except KeyError:
         mtap_jar = None
     if not mtap_jar:
```

### Comparing `mtap-1.1.0/python/tests/consul/integrationConfig.yaml` & `mtap-1.2.0/python/tests/consul/integrationConfig.yaml`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/consul/test_discovery.py` & `mtap-1.2.0/python/tests/consul/test_discovery.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,70 +8,80 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import signal
 import sys
 import time
 from pathlib import Path
 from subprocess import Popen, TimeoutExpired, PIPE, STDOUT
 
 import pytest
 import requests
 from requests import RequestException
 
 import mtap
-from mtap import RemoteProcessor, EventsClient, Event
+from mtap import EventsClient, Event, RemoteProcessor, utilities
 from mtap.utilities import subprocess_events_server
 
 
-@pytest.fixture(name='disc_python_events')
+@pytest.fixture(name='disc_python_events', scope='module')
 def fixture_disc_python_events():
-    with subprocess_events_server(cwd=Path(__file__).parents[2], register=True) as address:
+    with subprocess_events_server(cwd=Path(__file__).parents[2],
+                                  register=True) as address:
         yield address
 
 
-@pytest.fixture(name='disc_python_processor')
+@pytest.fixture(name='disc_python_processor', scope='module')
 def fixture_disc_python_processor(disc_python_events, processor_watcher):
     p = Popen([sys.executable, '-m', 'mtap.examples.example_processor',
                '-p', '50501', '--register'],
               start_new_session=True, stdin=PIPE, stdout=PIPE, stderr=STDOUT)
     yield from processor_watcher(address="127.0.0.1:50501", process=p)
 
 
-@pytest.fixture(name="disc_java_processor")
-def fixture_disc_java_processor(java_exe, disc_python_events, processor_watcher):
-    p = Popen(java_exe + ['edu.umn.nlpie.mtap.examples.WordOccurrencesExampleProcessor', '-p', '50502', '--register'],
+@pytest.fixture(name="disc_java_processor", scope='module')
+def fixture_disc_java_processor(java_exe, disc_python_events,
+                                processor_watcher):
+    p = Popen(java_exe + [
+        'edu.umn.nlpie.mtap.examples.WordOccurrencesExampleProcessor', '-p',
+        '50502', '--register'],
               stdin=PIPE, stdout=PIPE, stderr=STDOUT)
     yield from processor_watcher(address="127.0.0.1:50502", process=p)
 
 
-@pytest.fixture(name="disc_api_gateway")
-def fixture_disc_api_gateway(disc_python_events, disc_python_processor, disc_java_processor):
-    p = Popen(['mtap-gateway', '-mtap-config',  str(Path(__file__).parent / 'integrationConfig.yaml'),
+@pytest.fixture(name="disc_api_gateway", scope='module')
+def fixture_disc_api_gateway(disc_python_events, disc_python_processor,
+                             disc_java_processor):
+    port = utilities.find_free_port()
+    address = f"127.0.0.1:{port}"
+    p = Popen(['mtap-gateway', '-mtap-config',
+               str(Path(__file__).parent / 'integrationConfig.yaml'),
+               '-port', str(port),
                '-logtostderr', '-v=3'], stdin=PIPE, stdout=PIPE, stderr=STDOUT)
     session = requests.Session()
     session.trust_env = False
     try:
         if p.returncode is not None:
             raise ValueError("Failed to launch go gateway")
         for i in range(6):
             if i == 5:
                 raise ValueError("Failed to connect to go gateway")
             try:
                 time.sleep(3)
-                resp = session.get("http://127.0.0.1:50503/v1/processors", timeout=10)
-                if resp.status_code == 200 and len(resp.json()['Processors']) == 2:
+                resp = session.get(f"http://{address}/v1/processors",
+                                   timeout=10)
+                if resp.status_code == 200 and len(
+                        resp.json()['Processors']) == 2:
                     break
             except RequestException:
                 pass
-        yield
+        yield address
     finally:
         session.close()
         p.terminate()
         try:
             stdout, _ = p.communicate(timeout=1)
             print("api gateway exited with code: ", p.returncode)
             print(stdout.decode('utf-8'))
@@ -88,41 +98,46 @@
 be far less bloody. The Enterprise computer system is controlled by three primary main processor 
 cores, cross-linked with a redundant melacortz ramistat, fourteen kiloquad interface modules. Our 
 neural pathways have become accustomed to your sensory input patterns. Mr. Worf, you do remember 
 how to fire phasers?"""
 
 
 @pytest.mark.consul
-def test_disc_pipeline(disc_python_events, disc_python_processor, disc_java_processor):
-    with EventsClient(address=disc_python_events) as client, mtap.Pipeline(
-            RemoteProcessor('mtap-example-processor-python', address='localhost:50501',
-                            params={'do_work': True}),
-            RemoteProcessor('mtap-example-processor-java', address='localhost:50502',
-                            params={'do_work': True})
-    ) as pipeline:
+def test_disc_pipeline(disc_python_events, disc_python_processor,
+                       disc_java_processor):
+    pipeline = mtap.Pipeline(
+        RemoteProcessor('mtap-example-processor-python',
+                        address='localhost:50501',
+                        params={'do_work': True}),
+        RemoteProcessor('mtap-example-processor-java',
+                        address='localhost:50502',
+                        params={'do_work': True})
+    )
+    with EventsClient(address=disc_python_events) as client:
         with Event(event_id='1', client=client) as event:
             event.metadata['a'] = 'b'
             document = event.create_document('plaintext', PHASERS)
-            pipeline.run(document)
-            letter_counts = document.get_label_index('mtap.examples.letter_counts')
+            result = pipeline.run_multithread([document])
+            letter_counts = document.get_label_index(
+                'mtap.examples.letter_counts')
             a_counts = letter_counts[0]
             assert a_counts.count == 23
             b_counts = letter_counts[1]
             assert b_counts.count == 6
-            pipeline.print_times()
+            result.print_times()
             thes = document.get_label_index("mtap.examples.word_occurrences")
             assert thes[0].start_index == 121
             assert thes[0].end_index == 124
 
 
 @pytest.mark.consul
 def test_disc_api_gateway(disc_api_gateway):
     session = requests.Session()
     session.trust_env = False
-    resp = session.get("http://localhost:50503/v1/processors", timeout=10)
+    resp = session.get(f"http://{disc_api_gateway}/v1/processors", timeout=10)
     assert resp.status_code == 200
     processors = resp.json()
     all_ids = []
     for processor in processors['Processors']:
         all_ids.append(processor['Identifier'])
     assert 'mtap-example-processor-python' in all_ids
     assert 'mtap-example-processor-java' in all_ids
```

### Comparing `mtap-1.1.0/python/tests/data/test_document.py` & `mtap-1.2.0/python/tests/data/test_document.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/data/test_event.py` & `mtap-1.2.0/python/tests/data/test_event.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/data/test_events_client.py` & `mtap-1.2.0/python/tests/data/test_events_client.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/data/test_generic_label.py` & `mtap-1.2.0/python/tests/data/test_generic_label.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/data/test_labels.py` & `mtap-1.2.0/python/tests/data/test_labels.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/data/test_standard_ascending_label_index.py` & `mtap-1.2.0/python/tests/data/test_standard_ascending_label_index.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/data/test_standard_descending_label_index.py` & `mtap-1.2.0/python/tests/data/test_standard_descending_label_index.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/deployment/test_deployment.py` & `mtap-1.2.0/python/tests/deployment/test_deployment.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+import pytest
 
 import mtap
-from mtap import RemoteProcessor
+from mtap import RemoteProcessor, EventsClient
 from mtap.deployment import Deployment, ProcessorDeployment
 
 text = """
 Why, friends, you go to do you know not what:
 Wherein hath Caesar thus deserved your loves?
 Alas, you know not: I must tell you then:
 You have forgot the will I told you of.
@@ -31,14 +32,15 @@
 On this side Tiber; he hath left them you,
 And to your heirs for ever, common pleasures,
 To walk abroad, and recreate yourselves.
 Here was a Caesar! when comes such another?
 """
 
 
+@pytest.mark.integration
 def test_deployment(java_exe):
     from importlib_resources import files, as_file
     deployment_config = files('mtap.examples').joinpath('exampleDeploymentConfiguration.yml')
     run_config = files('mtap.examples').joinpath('examplePipelineConfiguration.yml')
     with as_file(deployment_config) as deployment_f, as_file(run_config) as run_f:
         deployment = Deployment.from_yaml_file(deployment_f)
         deployment.global_settings.log_level = 'DEBUG'
@@ -53,20 +55,22 @@
             pipeline = mtap.Pipeline.from_yaml_file(run_f)
             pipeline.append(
                 RemoteProcessor(
                     processor_name='hello',
                     address='127.0.0.1:10103'
                 )
             )
-            with mtap.Event(client=pipeline.events_client) as e:
-                d = e.create_document('plaintext', text)
-                results = pipeline.run(d)
-                assert results is not None
-            with mtap.Event(client=pipeline.events_client) as e:
-                d = e.create_document('plaintext', text)
-
-                def source():
-                    yield d
-
-                pipeline.run_multithread(source(), total=1, log_level='DEBUG')
-                assert len(d.labels['mtap.examples.letter_counts']) > 0
-                assert len(d.labels['mtap.examples.word_occurrences']) > 0
+            pipeline.mp_config.close_events = False
+            with EventsClient(deployment.events_deployment.address) as c:
+                with mtap.Event(client=c) as e:
+                    d = e.create_document('plaintext', text)
+                    results = pipeline.run(d)
+                    assert results is not None
+                with mtap.Event(client=c) as e:
+                    d = e.create_document('plaintext', text)
+
+                    def source():
+                        yield d
+
+                    pipeline.run_multithread(source(), total=1, log_level='DEBUG')
+                    assert len(d.labels['mtap.examples.letter_counts']) > 0
+                    assert len(d.labels['mtap.examples.word_occurrences']) > 0
```

### Comparing `mtap-1.1.0/python/tests/integration/test_hello_world_tutorial.py` & `mtap-1.2.0/python/tests/integration/test_hello_world_tutorial.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,19 +44,19 @@
               stdin=PIPE, stdout=PIPE, stderr=STDOUT)
     address = "127.0.0.1:" + port
     yield from processor_watcher(address=address, process=p)
 
 
 @pytest.mark.integration
 def test_hello_world(python_events, hello_processor):
-    p = run(['python', '-m', 'mtap.examples.tutorial.pipeline', python_events, hello_processor],
+    p = run([sys.executable, '-m', 'mtap.examples.tutorial.pipeline', python_events, hello_processor],
             stdout=PIPE)
     p.check_returncode()
     assert p.stdout.decode('utf-8') == 'Hello YOUR NAME!\n'
 
 
 @pytest.mark.integration
 def test_java_hello_world(python_events, java_hello_processor):
-    p = run(['python', '-m', 'mtap.examples.tutorial.pipeline', python_events,
+    p = run([sys.executable, '-m', 'mtap.examples.tutorial.pipeline', python_events,
              java_hello_processor], stdout=PIPE)
     p.check_returncode()
     assert p.stdout.decode('utf-8') == 'Hello YOUR NAME!\n'
```

### Comparing `mtap-1.1.0/python/tests/integration/test_integration.py` & `mtap-1.2.0/python/tests/integration/test_integration.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
-import signal
 import sys
 import tempfile
 import time
 from pathlib import Path
 from subprocess import Popen, PIPE, STDOUT, TimeoutExpired
 
 import pytest
@@ -26,39 +25,42 @@
 try:
     from yaml import CDumper as Dumper
 except ImportError:
     from yaml import Dumper
 from requests import RequestException
 
 import mtap
-from mtap import RemoteProcessor, EventsClient, Event
+from mtap import EventsClient, Event, RemoteProcessor
 from mtap.utilities import subprocess_events_server, find_free_port
 
 os.environ['no_proxy'] = '127.0.0.1,localhost'
 
 
 @pytest.fixture(name='python_events')
 def fixture_python_events():
     with subprocess_events_server(cwd=Path(__file__).parents[2]) as address:
         yield address
 
 
 @pytest.fixture(name='python_processor')
 def fixture_python_processor(python_events, processor_watcher):
     port = str(find_free_port())
-    p = Popen([sys.executable, '-m', 'mtap.examples.example_processor', '-p', port,
-               '--events', python_events], stdin=PIPE, stdout=PIPE, stderr=STDOUT)
+    p = Popen(
+        [sys.executable, '-m', 'mtap.examples.example_processor', '-p', port,
+         '--events', python_events], stdin=PIPE, stdout=PIPE, stderr=STDOUT)
     yield from processor_watcher(address="127.0.0.1:" + port, process=p)
 
 
 @pytest.fixture(name="java_processor")
 def fixture_java_processor(java_exe, python_events, processor_watcher):
     port = str(find_free_port())
-    p = Popen(java_exe + ['edu.umn.nlpie.mtap.examples.WordOccurrencesExampleProcessor',
-                          '-p', port, '-e', python_events], stdin=PIPE, stdout=PIPE, stderr=STDOUT)
+    p = Popen(java_exe + [
+        'edu.umn.nlpie.mtap.examples.WordOccurrencesExampleProcessor',
+        '-p', port, '-e', python_events], stdin=PIPE, stdout=PIPE,
+              stderr=STDOUT)
     yield from processor_watcher(address="127.0.0.1:" + port, process=p)
 
 
 @pytest.fixture(name="api_gateway")
 def fixture_api_gateway(python_events, python_processor, java_processor):
     port = find_free_port()
     config = {
@@ -92,29 +94,32 @@
             ]
         }
     }
 
     with tempfile.NamedTemporaryFile('w', suffix='.yml') as conf_file:
         yaml.dump(config, conf_file, Dumper=Dumper)
         conf_file.flush()
-        p = Popen(['mtap-gateway', '-logtostderr', '-v=3', '-mtap-config=' + conf_file.name],
+        p = Popen(['mtap-gateway', '-logtostderr', '-v=3',
+                   '-mtap-config=' + conf_file.name],
                   stdin=PIPE, stdout=PIPE, stderr=STDOUT)
         session = requests.Session()
         session.trust_env = False
         gateway = '127.0.0.1:{}'.format(port)
         try:
             if p.returncode is not None:
                 raise ValueError("Failed to launch go gateway")
             for i in range(6):
                 if i == 5:
                     raise ValueError("Failed to connect to go gateway")
                 try:
                     time.sleep(3)
-                    resp = session.get("http://{}/v1/processors".format(gateway), timeout=1)
-                    if resp.status_code == 200 and len(resp.json()['Processors']) == 2:
+                    resp = session.get(
+                        "http://{}/v1/processors".format(gateway), timeout=1)
+                    if resp.status_code == 200 and len(
+                            resp.json()['Processors']) == 2:
                         break
                 except RequestException:
                     pass
             yield gateway
         finally:
             session.close()
             p.terminate()
@@ -136,38 +141,43 @@
 cores, cross-linked with a redundant melacortz ramistat, fourteen kiloquad interface modules. Our 
 neural pathways have become accustomed to your sensory input patterns. Mr. Worf, you do remember 
 how to fire phasers?"""
 
 
 @pytest.mark.integration
 def test_pipeline(python_events, python_processor, java_processor):
-    with EventsClient(address=python_events) as client, mtap.Pipeline(
-            RemoteProcessor('mtap-example-processor-python', address=python_processor,
-                            params={'do_work': True}),
-            RemoteProcessor('mtap-example-processor-java', address=java_processor,
-                            params={'do_work': True})
-    ) as pipeline:
+    pipeline = mtap.Pipeline(
+        RemoteProcessor('mtap-example-processor-python',
+                        address=python_processor,
+                        params={'do_work': True}),
+        RemoteProcessor('mtap-example-processor-java',
+                        address=java_processor,
+                        params={'do_work': True})
+    )
+    with EventsClient(address=python_events) as client:
         with Event(event_id='1', client=client) as event:
             event.metadata['a'] = 'b'
             document = event.create_document('plaintext', PHASERS)
-            pipeline.run(document)
-            letter_counts = document.get_label_index('mtap.examples.letter_counts')
+            result = pipeline.run_multithread([document])
+            letter_counts = document.get_label_index(
+                'mtap.examples.letter_counts')
             a_counts = letter_counts[0]
             assert a_counts.count == 23
             b_counts = letter_counts[1]
             assert b_counts.count == 6
-            pipeline.print_times()
+            result.print_times()
             thes = document.get_label_index("mtap.examples.word_occurrences")
             assert thes[0].start_index == 121
             assert thes[0].end_index == 124
 
 
 @pytest.mark.integration
 @pytest.mark.gateway
-def test_api_gateway(python_events, python_processor, java_processor, api_gateway):
+def test_api_gateway(python_events, python_processor, java_processor,
+                     api_gateway):
     session = requests.Session()
     session.trust_env = False
     base_url = "http://" + api_gateway
     resp = session.get(base_url + "/v1/processors", timeout=10)
     assert resp.status_code == 200
     processors = resp.json()
     all_ids = []
@@ -185,34 +195,37 @@
     assert resp.status_code == 200
     create_event = resp.json()
     assert create_event['created'] is True
 
     body = {
         'value': 'bar'
     }
-    resp = session.post(base_url + "/v1/events/1/metadata/foo", json=body, timeout=1)
+    resp = session.post(base_url + "/v1/events/1/metadata/foo", json=body,
+                        timeout=1)
     assert resp.status_code == 200
 
     resp = session.get(base_url + "/v1/events/1/metadata", timeout=1)
     assert resp.status_code == 200
     metadata = resp.json()['metadata']
     assert metadata['foo'] == 'bar'
 
     body = {
         'text': PHASERS
     }
-    resp = session.post(base_url + "/v1/events/1/documents/plaintext", json=body, timeout=1)
+    resp = session.post(base_url + "/v1/events/1/documents/plaintext",
+                        json=body, timeout=1)
     assert resp.status_code == 200
 
     resp = session.get(base_url + "/v1/events/1/documents", timeout=1)
     assert resp.status_code == 200
     documents = resp.json()["document_names"]
     assert documents == ['plaintext']
 
-    resp = session.get(base_url + "/v1/events/1/documents/plaintext", timeout=1)
+    resp = session.get(base_url + "/v1/events/1/documents/plaintext",
+                       timeout=1)
     assert resp.status_code == 200
     text = resp.json()['text']
     assert text == PHASERS
 
     body = {
         'generic_labels': {
             'is_distinct': True,
@@ -235,18 +248,21 @@
                         'foo': 'baz'
                     }
                 }
             ]
         }
     }
     resp = session.post(
-        base_url + "/v1/events/1/documents/plaintext/labels/test-labels", json=body, timeout=1)
+        base_url + "/v1/events/1/documents/plaintext/labels/test-labels",
+        json=body, timeout=1)
     assert resp.status_code == 200
 
-    resp = session.get(base_url + "/v1/events/1/documents/plaintext/labels/test-labels", timeout=1)
+    resp = session.get(
+        base_url + "/v1/events/1/documents/plaintext/labels/test-labels",
+        timeout=1)
     assert resp.status_code == 200
     labels = resp.json()
     generic_labels = labels['generic_labels']
     assert generic_labels['is_distinct']
     assert generic_labels['labels'] == body['generic_labels']['labels']
 
     body = {
@@ -263,15 +279,16 @@
         timeout=1
     )
     assert resp.status_code == 200
     python_process = resp.json()
     assert python_process['result']['answer'] == 42
 
     resp = session.get(
-        base_url + "/v1/events/1/documents/plaintext/labels/mtap.examples.letter_counts", timeout=1
+        base_url + "/v1/events/1/documents/plaintext/labels/mtap.examples.letter_counts",
+        timeout=1
     )
     assert resp.status_code == 200
     labels = resp.json()
     generic_labels = labels['generic_labels']
     assert generic_labels['labels'] == [
         {
             'identifier': 0,
```

### Comparing `mtap-1.1.0/python/tests/processing/test_event_processor.py` & `mtap-1.2.0/python/tests/processing/test_event_processor.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/processing/test_pipeline.py` & `mtap-1.2.0/python/tests/processing/test_pipeline.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,17 +14,25 @@
 
 import pickle
 import time
 from datetime import timedelta
 from pathlib import Path
 from typing import Dict, Any
 
-from mtap import Pipeline, LocalProcessor, Event, EventsClient, processor
-from mtap.processing import EventProcessor
-from mtap.processing._pipeline import MpConfig, RemoteProcessor
+from mtap import (
+    Pipeline,
+    EventProcessor,
+    Event,
+    EventsClient,
+    processor,
+    RemoteProcessor,
+    LocalProcessor
+)
+from mtap.processing import MpConfig, SimpleErrorHandler, \
+    TerminationErrorHandler
 
 
 @processor('test-processor')
 class Processor(EventProcessor):
     def __init__(self, identifier='1'):
         self.identifier = identifier
         self.seen = 0
@@ -42,28 +50,33 @@
 
 def test_time_result(mocker):
     client = mocker.Mock(EventsClient)
     client.get_local_instance.return_value = client
     client.get_all_document_names.return_value = ['plaintext']
     client.get_all_metadata.return_value = {}
     client.instance_id = 0
-    with Pipeline(
-            LocalProcessor(Processor(), component_id='test_processor'),
-            events_client=client
-    ) as pipeline:
+    pipeline = Pipeline(
+        LocalProcessor(Processor(),
+                       component_id='test_processor')
+    )
+    with pipeline.activate() as active:
+        active.components[0]._client = client
         event = Event()
-        result = pipeline.run(event)
-        assert result.component_results[0].timing_info['process_method'] >= timedelta(seconds=0.001)
+        result = active.run(event)
+        assert result.component_results[0].timing_info['process_method'] \
+               >= timedelta(seconds=0.001)
 
 
 def test_load_from_config():
     pipeline = Pipeline.from_yaml_file(Path(__file__).parent / 'pipeline.yml')
     assert pipeline.name == 'mtap-test-pipeline'
-    assert pipeline.events_address == 'localhost:123'
-    assert pipeline.mp_config.max_failures == 3
+    assert len(pipeline.error_handlers) == 2
+    assert type(pipeline.error_handlers[0]) == SimpleErrorHandler
+    assert type(pipeline.error_handlers[1]) == TerminationErrorHandler
+    assert pipeline.error_handlers[1].max_failures == 3
     assert not pipeline.mp_config.show_progress
     assert pipeline.mp_config.workers == 12
     assert pipeline.mp_config.read_ahead == 4
     assert not pipeline.mp_config.close_events
     assert len(pipeline) == 2
     assert pipeline[0].processor_name == 'processor-1'
     assert pipeline[0].address == 'localhost:1234'
@@ -78,28 +91,24 @@
             address='localhost:1234'
         ),
         RemoteProcessor(
             processor_name='processor-2',
             address='localhost:5678'
         ),
         name='mtap-test-pipeline',
-        events_address='localhost:123',
         mp_config=MpConfig(
-            max_failures=3,
             show_progress=False,
             workers=12,
             read_ahead=4,
             close_events=False
         ),
     )
     s = pickle.dumps(p)
     r = pickle.loads(s)
     assert r.name == 'mtap-test-pipeline'
-    assert r.events_address == 'localhost:123'
-    assert r.mp_config.max_failures == 3
     assert not r.mp_config.show_progress
     assert r.mp_config.workers == 12
     assert r.mp_config.read_ahead == 4
     assert not r.mp_config.close_events
     assert len(r) == 2
     assert r[0].processor_name == 'processor-1'
     assert r[0].address == 'localhost:1234'
```

### Comparing `mtap-1.1.0/python/tests/processing/test_pipeline_result.py` & `mtap-1.2.0/python/tests/processing/test_pipeline_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 from datetime import timedelta
 
 import pytest
 
-from mtap.processing import PipelineResult, ProcessingResult
+from mtap.processing import PipelineResult, ComponentResult
 
 
 def test_component_result():
     result = PipelineResult(
         component_results=[
-            ProcessingResult(
+            ComponentResult(
                 identifier='a',
                 result_dict={'b': 'c'},
                 timing_info={},
                 created_indices={}
             )
         ],
         elapsed_time=timedelta(seconds=4)
```

### Comparing `mtap-1.1.0/python/tests/processing/test_processor.py` & `mtap-1.2.0/python/tests/processing/test_processor.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/processing/test_processor_service.py` & `mtap-1.2.0/python/tests/processing/test_processor_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,59 +13,65 @@
 # limitations under the License.
 from typing import Dict, Any
 
 import grpc
 import grpc_testing
 import pytest
 
-from mtap import processor, Document
+from mtap import processor, Document, DocumentProcessor
 from mtap.api.v1 import processing_pb2
-from mtap.processing import DocumentProcessor, _runners
+from mtap.processing import _runners
 from mtap.processing.descriptions import parameter, labels, label_property
 from mtap.processing._service import _ProcessorServicer
 
 
 @processor('mtap-test-processor',
            description='Processor desc.',
            parameters=[
                parameter('a_param', required=True, data_type='bool',
                          description="desc.")
            ],
            inputs=[
-               labels('input_index', properties=[label_property('bar', data_type='bool')])
+               labels('input_index',
+                      properties=[label_property('bar', data_type='bool')])
            ],
            outputs=[
                labels('output_index',
                       description='desc.',
-                      properties=[label_property('foo', data_type='str', nullable=True,
-                                                      description='A label property.')])
+                      properties=[
+                          label_property('foo', data_type='str', nullable=True,
+                                         description='A label property.')])
            ])
 class ExampleTestProcessor(DocumentProcessor):
     def process_document(self, document: Document, params: Dict[str, Any]):
         pass
 
 
 @pytest.fixture(name='processor_servicer')
 def fixture_processor_servicer():
-    runner = _runners.ProcessorRunner(ExampleTestProcessor(), client=None)
-    processor_service = _ProcessorServicer(config={}, runner=runner, address='',
+    runner = _runners.LocalRunner(ExampleTestProcessor(), events_address=None)
+    processor_service = _ProcessorServicer(runner=runner,
+                                           address='',
                                            sid='1',
                                            health_servicer=None)
     yield grpc_testing.server_from_dictionary(
         {
-            processing_pb2.DESCRIPTOR.services_by_name['Processor']: processor_service
+            processing_pb2.DESCRIPTOR.services_by_name[
+                'Processor']: processor_service
         },
         grpc_testing.strict_real_time()
     )
 
 
 def test_GetInfo(processor_servicer):
-    request = processing_pb2.GetInfoRequest(processor_id='mtap-example-processor-python')
+    request = processing_pb2.GetInfoRequest(
+        processor_id='mtap-example-processor-python')
     resp, _, status_code, _ = processor_servicer.invoke_unary_unary(
-        processing_pb2.DESCRIPTOR.services_by_name['Processor'].methods_by_name['GetInfo'],
+        processing_pb2.DESCRIPTOR.services_by_name[
+            'Processor'].methods_by_name['GetInfo'],
         {},
         request,
         None
     ).termination()
 
     assert status_code == grpc.StatusCode.OK
     assert resp.metadata['name'] == 'mtap-test-processor'
@@ -82,8 +88,9 @@
     assert len(resp.metadata['outputs']) == 1
     assert resp.metadata['outputs'][0]['name'] == 'output_index'
     assert resp.metadata['outputs'][0]['description'] == 'desc.'
     assert len(resp.metadata['outputs'][0]['properties']) == 1
     assert resp.metadata['outputs'][0]['properties'][0]['name'] == 'foo'
     assert resp.metadata['outputs'][0]['properties'][0]['data_type'] == 'str'
     assert resp.metadata['outputs'][0]['properties'][0]['nullable']
-    assert resp.metadata['outputs'][0]['properties'][0]['description'] == 'A label property.'
+    assert resp.metadata['outputs'][0]['properties'][0][
+               'description'] == 'A label property.'
```

### Comparing `mtap-1.1.0/python/tests/processors/test_copy_document.py` & `mtap-1.2.0/python/tests/processors/test_copy_document.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/references/test_references.py` & `mtap-1.2.0/python/tests/references/test_references.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,88 +14,101 @@
 import os
 import sys
 from pathlib import Path
 from subprocess import Popen, PIPE, STDOUT
 
 import pytest
 
-from mtap import EventsClient, RemoteProcessor, Pipeline, Event, GenericLabel
+from mtap import EventsClient, Pipeline, Event, GenericLabel, RemoteProcessor
 from mtap.utilities import subprocess_events_server, find_free_port
 
 
 @pytest.fixture(name='python_events')
 def fixture_python_events():
     with subprocess_events_server(cwd=Path(__file__).parents[2]) as address:
         yield address
 
 
 @pytest.fixture(name='python_references_processor')
 def fixture_python_references_processor(python_events, processor_watcher):
     env = dict(os.environ)
     port = str(find_free_port())
-    p = Popen([sys.executable, '-m', 'mtap.examples.example_references_processor', '-p', port,
-               '--events', python_events, '--log-level', 'DEBUG'], stdin=PIPE, stdout=PIPE, stderr=STDOUT, env=env)
+    p = Popen(
+        [sys.executable, '-m', 'mtap.examples.example_references_processor',
+         '-p', port,
+         '--events', python_events, '--log-level', 'DEBUG'], stdin=PIPE,
+        stdout=PIPE, stderr=STDOUT, env=env)
     yield from processor_watcher(address="127.0.0.1:" + port, process=p)
 
 
 @pytest.fixture(name="java_references_processor")
-def fixture_java_references_processor(java_exe, python_events, processor_watcher):
+def fixture_java_references_processor(java_exe, python_events,
+                                      processor_watcher):
     env = dict(os.environ)
     port = str(find_free_port())
-    p = Popen(java_exe + ['edu.umn.nlpie.mtap.examples.ReferenceLabelsExampleProcessor',
-                          '-p', port, '-e', python_events], stdin=PIPE, stdout=PIPE, stderr=STDOUT, env=env)
+    p = Popen(java_exe + [
+        'edu.umn.nlpie.mtap.examples.ReferenceLabelsExampleProcessor',
+        '-p', port, '-e', python_events], stdin=PIPE, stdout=PIPE,
+              stderr=STDOUT, env=env)
     yield from processor_watcher(address="127.0.0.1:" + port, process=p)
 
 
 @pytest.mark.integration
 def test_java_references(python_events, java_references_processor):
-    with EventsClient(address=python_events) as client, Pipeline(
-            RemoteProcessor('mtap-java-reference-labels-example-processor',
-                            address=java_references_processor)
-    ) as pipeline:
-        with Event(event_id='1', client=client) as event:
-            document = event.create_document('plaintext', 'abcd')
-            pipeline.run(document)
-            references = document.labels['references']
-            assert references[0].a == GenericLabel(0, 1)
-            assert references[0].b == GenericLabel(1, 2)
-            assert references[1].a == GenericLabel(2, 3)
-            assert references[1].b == GenericLabel(3, 4)
-
-            map_references = document.labels['map_references']
-            assert map_references[0].ref == {
-                'a': GenericLabel(0, 1),
-                'b': GenericLabel(1, 2),
-                'c': GenericLabel(2, 3),
-                'd': GenericLabel(3, 4)
-            }
-
-            list_references = document.labels['list_references']
-            assert list_references[0].ref == [GenericLabel(0, 1), GenericLabel(1, 2)]
-            assert list_references[1].ref == [GenericLabel(2, 3), GenericLabel(3, 4)]
+    pipeline = Pipeline(
+        RemoteProcessor('mtap-java-reference-labels-example-processor',
+                        address=java_references_processor)
+    )
+    with EventsClient(python_events) as c, \
+            Event(event_id='1', client=c) as event:
+        document = event.create_document('plaintext', 'abcd')
+        pipeline.run(document)
+        references = document.labels['references']
+        assert references[0].a == GenericLabel(0, 1)
+        assert references[0].b == GenericLabel(1, 2)
+        assert references[1].a == GenericLabel(2, 3)
+        assert references[1].b == GenericLabel(3, 4)
+
+        map_references = document.labels['map_references']
+        assert map_references[0].ref == {
+            'a': GenericLabel(0, 1),
+            'b': GenericLabel(1, 2),
+            'c': GenericLabel(2, 3),
+            'd': GenericLabel(3, 4)
+        }
+
+        list_references = document.labels['list_references']
+        assert list_references[0].ref == [GenericLabel(0, 1),
+                                          GenericLabel(1, 2)]
+        assert list_references[1].ref == [GenericLabel(2, 3),
+                                          GenericLabel(3, 4)]
 
 
 @pytest.mark.integration
 def test_python_references(python_events, python_references_processor):
-    with EventsClient(address=python_events) as client, Pipeline(
-            RemoteProcessor('mtap-python-references-example', address=python_references_processor)
-    ) as pipeline:
-        with Event(event_id='1', client=client) as event:
-            document = event.create_document('plaintext', 'abcd')
-            pipeline.run(document)
-            references = document.labels['references']
-            assert references[0].a == GenericLabel(0, 1)
-            assert references[0].b == GenericLabel(1, 2)
-            assert references[1].a == GenericLabel(2, 3)
-            assert references[1].b == GenericLabel(3, 4)
-
-            map_references = document.labels['map_references']
-            assert map_references[0].ref == {
-                'a': GenericLabel(0, 1),
-                'b': GenericLabel(1, 2),
-                'c': GenericLabel(2, 3),
-                'd': GenericLabel(3, 4)
-            }
-
-            list_references = document.labels['list_references']
-            assert list_references[0].ref == [GenericLabel(0, 1), GenericLabel(1, 2)]
-            assert list_references[1].ref == [GenericLabel(2, 3), GenericLabel(3, 4)]
+    pipeline = Pipeline(
+        RemoteProcessor('mtap-python-references-example',
+                        address=python_references_processor)
+    )
+    with EventsClient(python_events) as client, \
+            Event(event_id='1', client=client) as event:
+        document = event.create_document('plaintext', 'abcd')
+        pipeline.run(document)
+        references = document.labels['references']
+        assert references[0].a == GenericLabel(0, 1)
+        assert references[0].b == GenericLabel(1, 2)
+        assert references[1].a == GenericLabel(2, 3)
+        assert references[1].b == GenericLabel(3, 4)
+
+        map_references = document.labels['map_references']
+        assert map_references[0].ref == {
+            'a': GenericLabel(0, 1),
+            'b': GenericLabel(1, 2),
+            'c': GenericLabel(2, 3),
+            'd': GenericLabel(3, 4)
+        }
+
+        list_references = document.labels['list_references']
+        assert list_references[0].ref == [GenericLabel(0, 1),
+                                          GenericLabel(1, 2)]
+        assert list_references[1].ref == [GenericLabel(2, 3),
+                                          GenericLabel(3, 4)]
```

### Comparing `mtap-1.1.0/python/tests/serialization/brat/100_1442.txt` & `mtap-1.2.0/python/tests/serialization/brat/100_1442.txt`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/serialization/test_brat.py` & `mtap-1.2.0/python/tests/serialization/test_brat.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/serialization/test_json.py` & `mtap-1.2.0/python/tests/serialization/test_json.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/serialization/test_pickle.py` & `mtap-1.2.0/python/tests/serialization/test_pickle.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/serialization/test_serialization.py` & `mtap-1.2.0/python/tests/serialization/test_serialization.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/serialization/test_yml.py` & `mtap-1.2.0/python/tests/serialization/test_yml.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/slf4j-simple-2.0.3.jar` & `mtap-1.2.0/python/tests/slf4j-simple-2.0.3.jar`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/test_events_service.py` & `mtap-1.2.0/python/tests/test_events_service.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/test_metrics.py` & `mtap-1.2.0/python/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/python/tests/test_structs.py` & `mtap-1.2.0/python/tests/test_structs.py`

 * *Files identical despite different names*

### Comparing `mtap-1.1.0/setup.py` & `mtap-1.2.0/setup.py`

 * *Files identical despite different names*

