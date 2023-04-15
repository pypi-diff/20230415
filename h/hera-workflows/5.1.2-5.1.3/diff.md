# Comparing `tmp/hera_workflows-5.1.2.tar.gz` & `tmp/hera_workflows-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hera_workflows-5.1.2.tar", max compression
+gzip compressed data, was "hera_workflows-5.1.3.tar", max compression
```

## Comparing `hera_workflows-5.1.2.tar` & `hera_workflows-5.1.3.tar`

### file list

```diff
@@ -1,131 +1,132 @@
--rw-r--r--   0        0        0     1066 2023-04-08 15:37:35.795590 hera_workflows-5.1.2/LICENSE
--rw-r--r--   0        0        0    11197 2023-04-08 15:37:35.795590 hera_workflows-5.1.2/README.md
--rw-r--r--   0        0        0     3540 2023-04-08 15:37:55.911484 hera_workflows-5.1.2/pyproject.toml
--rw-r--r--   0        0        0      522 2023-04-08 15:37:35.807590 hera_workflows-5.1.2/src/hera/__init__.py
--rw-r--r--   0        0        0      310 2023-04-08 15:37:55.915484 hera_workflows-5.1.2/src/hera/_version.py
--rw-r--r--   0        0        0        0 2023-04-08 15:37:35.807590 hera_workflows-5.1.2/src/hera/events/__init__.py
--rw-r--r--   0        0        0     3267 2023-04-08 15:37:35.807590 hera_workflows-5.1.2/src/hera/events/models/__init__.py
--rw-r--r--   0        0        0     1418 2023-04-08 15:37:35.807590 hera_workflows-5.1.2/src/hera/events/models/eventsource.py
--rw-r--r--   0        0        0      861 2023-04-08 15:37:35.807590 hera_workflows-5.1.2/src/hera/events/models/eventsource.pyi
--rw-r--r--   0        0        0      144 2023-04-08 15:37:35.807590 hera_workflows-5.1.2/src/hera/events/models/google/__init__.py
--rw-r--r--   0        0        0      347 2023-04-08 15:37:35.807590 hera_workflows-5.1.2/src/hera/events/models/google/protobuf.py
--rw-r--r--   0        0        0      164 2023-04-08 15:37:35.807590 hera_workflows-5.1.2/src/hera/events/models/google/protobuf.pyi
--rw-r--r--   0        0        0        0 2023-04-08 15:37:35.807590 hera_workflows-5.1.2/src/hera/events/models/grpc/__init__.py
--rw-r--r--   0        0        0      144 2023-04-08 15:37:35.807590 hera_workflows-5.1.2/src/hera/events/models/grpc/gateway/__init__.py
--rw-r--r--   0        0        0      691 2023-04-08 15:37:35.807590 hera_workflows-5.1.2/src/hera/events/models/grpc/gateway/runtime.py
--rw-r--r--   0        0        0      470 2023-04-08 15:37:35.807590 hera_workflows-5.1.2/src/hera/events/models/grpc/gateway/runtime.pyi
--rw-r--r--   0        0        0        0 2023-04-08 15:37:35.807590 hera_workflows-5.1.2/src/hera/events/models/io/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 15:37:35.807590 hera_workflows-5.1.2/src/hera/events/models/io/argoproj/__init__.py
--rw-r--r--   0        0        0      144 2023-04-08 15:37:35.807590 hera_workflows-5.1.2/src/hera/events/models/io/argoproj/events/__init__.py
--rw-r--r--   0        0        0   102993 2023-04-08 15:37:35.807590 hera_workflows-5.1.2/src/hera/events/models/io/argoproj/events/v1alpha1.py
--rw-r--r--   0        0        0    25271 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/argoproj/events/v1alpha1.pyi
--rw-r--r--   0        0        0      144 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/argoproj/workflow/__init__.py
--rw-r--r--   0        0        0   144549 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/argoproj/workflow/v1alpha1.py
--rw-r--r--   0        0        0    31958 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi
--rw-r--r--   0        0        0        0 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/api/__init__.py
--rw-r--r--   0        0        0      144 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/api/core/__init__.py
--rw-r--r--   0        0        0   127883 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/api/core/v1.py
--rw-r--r--   0        0        0    18004 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/api/core/v1.pyi
--rw-r--r--   0        0        0      144 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/api/policy/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/api/policy/v1beta1.py
--rw-r--r--   0        0        0      376 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/api/policy/v1beta1.pyi
--rw-r--r--   0        0        0        0 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/apimachinery/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/apimachinery/pkg/__init__.py
--rw-r--r--   0        0        0      144 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0        0        0     3161 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py
--rw-r--r--   0        0        0      105 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.pyi
--rw-r--r--   0        0        0        0 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0        0        0      144 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0        0        0    22218 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
--rw-r--r--   0        0        0     2064 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
--rw-r--r--   0        0        0      144 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0        0        0      277 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.py
--rw-r--r--   0        0        0      108 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.pyi
--rw-r--r--   0        0        0     1453 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/sensor.py
--rw-r--r--   0        0        0      887 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/models/sensor.pyi
--rw-r--r--   0        0        0    26908 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/events/service.py
--rw-r--r--   0        0        0      282 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/expr/__init__.py
--rw-r--r--   0        0        0    12021 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/expr/_node.py
--rw-r--r--   0        0        0      647 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/expr/_sprig.py
--rw-r--r--   0        0        0        0 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/py.typed
--rw-r--r--   0        0        0      188 2023-04-08 15:37:35.811590 hera_workflows-5.1.2/src/hera/shared/__init__.py
--rw-r--r--   0        0        0      269 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/shared/_base_model.py
--rw-r--r--   0        0        0     4927 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/shared/_global_config.py
--rw-r--r--   0        0        0      513 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/shared/serialization.py
--rw-r--r--   0        0        0     4413 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/__init__.py
--rw-r--r--   0        0        0     2298 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/_context.py
--rw-r--r--   0        0        0    23829 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/_mixins.py
--rw-r--r--   0        0        0       25 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/action.py
--rw-r--r--   0        0        0     1115 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/archive.py
--rw-r--r--   0        0        0     7697 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/artifact.py
--rw-r--r--   0        0        0     3446 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/container.py
--rw-r--r--   0        0        0     3988 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/container_set.py
--rw-r--r--   0        0        0     3763 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/cron_workflow.py
--rw-r--r--   0        0        0     2771 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/dag.py
--rw-r--r--   0        0        0     2186 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/data.py
--rw-r--r--   0        0        0     4855 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/env.py
--rw-r--r--   0        0        0     1329 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/env_from.py
--rw-r--r--   0        0        0      208 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/exceptions.py
--rw-r--r--   0        0        0     2291 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/http_template.py
--rw-r--r--   0        0        0       30 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/memoize.py
--rw-r--r--   0        0        0     6913 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/__init__.py
--rw-r--r--   0        0        0     1418 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/eventsource.py
--rw-r--r--   0        0        0      861 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/eventsource.pyi
--rw-r--r--   0        0        0      144 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/google/__init__.py
--rw-r--r--   0        0        0      347 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/google/protobuf.py
--rw-r--r--   0        0        0      164 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/google/protobuf.pyi
--rw-r--r--   0        0        0        0 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/grpc/__init__.py
--rw-r--r--   0        0        0      144 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/grpc/gateway/__init__.py
--rw-r--r--   0        0        0      691 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/grpc/gateway/runtime.py
--rw-r--r--   0        0        0      470 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/grpc/gateway/runtime.pyi
--rw-r--r--   0        0        0        0 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/argoproj/__init__.py
--rw-r--r--   0        0        0      144 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/argoproj/events/__init__.py
--rw-r--r--   0        0        0   102993 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/argoproj/events/v1alpha1.py
--rw-r--r--   0        0        0    25271 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi
--rw-r--r--   0        0        0      144 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/argoproj/workflow/__init__.py
--rw-r--r--   0        0        0   144549 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py
--rw-r--r--   0        0        0    31958 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi
--rw-r--r--   0        0        0        0 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/api/__init__.py
--rw-r--r--   0        0        0      144 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/api/core/__init__.py
--rw-r--r--   0        0        0   127883 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/api/core/v1.py
--rw-r--r--   0        0        0    18004 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/api/core/v1.pyi
--rw-r--r--   0        0        0      144 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/api/policy/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py
--rw-r--r--   0        0        0      376 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/api/policy/v1beta1.pyi
--rw-r--r--   0        0        0        0 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/apimachinery/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/__init__.py
--rw-r--r--   0        0        0      144 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0        0        0     3161 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py
--rw-r--r--   0        0        0      105 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.pyi
--rw-r--r--   0        0        0        0 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0        0        0      144 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0        0        0    22218 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
--rw-r--r--   0        0        0     2064 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
--rw-r--r--   0        0        0      144 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0        0        0      277 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.py
--rw-r--r--   0        0        0      108 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.pyi
--rw-r--r--   0        0        0     1453 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/sensor.py
--rw-r--r--   0        0        0      887 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/models/sensor.pyi
--rw-r--r--   0        0        0      722 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/operator.py
--rw-r--r--   0        0        0     4084 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/parameter.py
--rw-r--r--   0        0        0     1018 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/protocol.py
--rw-r--r--   0        0        0     2554 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/resource.py
--rw-r--r--   0        0        0     5262 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/resources.py
--rw-r--r--   0        0        0     1856 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/retry_strategy.py
--rw-r--r--   0        0        0     3707 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/runner.py
--rw-r--r--   0        0        0    14855 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/script.py
--rw-r--r--   0        0        0    49478 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/service.py
--rw-r--r--   0        0        0     9297 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/steps.py
--rw-r--r--   0        0        0     3266 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/suspend.py
--rw-r--r--   0        0        0    10495 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/task.py
--rw-r--r--   0        0        0       27 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/toleration.py
--rw-r--r--   0        0        0     2007 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/user_container.py
--rw-r--r--   0        0        0     2610 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/validators.py
--rw-r--r--   0        0        0    18656 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/volume.py
--rw-r--r--   0        0        0    15590 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/workflow.py
--rw-r--r--   0        0        0      911 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/workflow_status.py
--rw-r--r--   0        0        0     5925 2023-04-08 15:37:35.815590 hera_workflows-5.1.2/src/hera/workflows/workflow_template.py
--rw-r--r--   0        0        0    12781 1970-01-01 00:00:00.000000 hera_workflows-5.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-15 21:34:41.499745 hera_workflows-5.1.3/LICENSE
+-rw-r--r--   0        0        0    11696 2023-04-15 21:34:41.499745 hera_workflows-5.1.3/README.md
+-rw-r--r--   0        0        0     3540 2023-04-15 21:35:04.008046 hera_workflows-5.1.3/pyproject.toml
+-rw-r--r--   0        0        0      522 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/__init__.py
+-rw-r--r--   0        0        0      310 2023-04-15 21:35:04.008046 hera_workflows-5.1.3/src/hera/_version.py
+-rw-r--r--   0        0        0        0 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/__init__.py
+-rw-r--r--   0        0        0     3267 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/__init__.py
+-rw-r--r--   0        0        0     1418 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/eventsource.py
+-rw-r--r--   0        0        0      861 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/eventsource.pyi
+-rw-r--r--   0        0        0      144 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/google/__init__.py
+-rw-r--r--   0        0        0      347 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/google/protobuf.py
+-rw-r--r--   0        0        0      164 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/google/protobuf.pyi
+-rw-r--r--   0        0        0        0 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/grpc/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/grpc/gateway/__init__.py
+-rw-r--r--   0        0        0      691 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/grpc/gateway/runtime.py
+-rw-r--r--   0        0        0      470 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/grpc/gateway/runtime.pyi
+-rw-r--r--   0        0        0        0 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/argoproj/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/argoproj/events/__init__.py
+-rw-r--r--   0        0        0   102993 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/argoproj/events/v1alpha1.py
+-rw-r--r--   0        0        0    25271 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/argoproj/events/v1alpha1.pyi
+-rw-r--r--   0        0        0      144 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/argoproj/workflow/__init__.py
+-rw-r--r--   0        0        0   144549 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/argoproj/workflow/v1alpha1.py
+-rw-r--r--   0        0        0    31958 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi
+-rw-r--r--   0        0        0        0 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-15 21:34:41.511745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/core/__init__.py
+-rw-r--r--   0        0        0   127883 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/core/v1.py
+-rw-r--r--   0        0        0    18004 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/core/v1.pyi
+-rw-r--r--   0        0        0      144 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/policy/__init__.py
+-rw-r--r--   0        0        0     1751 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/policy/v1beta1.py
+-rw-r--r--   0        0        0      376 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/policy/v1beta1.pyi
+-rw-r--r--   0        0        0        0 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0        0        0     3161 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py
+-rw-r--r--   0        0        0      105 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.pyi
+-rw-r--r--   0        0        0        0 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0        0        0    22218 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
+-rw-r--r--   0        0        0     2064 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
+-rw-r--r--   0        0        0      144 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0        0        0      277 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.py
+-rw-r--r--   0        0        0      108 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.pyi
+-rw-r--r--   0        0        0     1453 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/sensor.py
+-rw-r--r--   0        0        0      887 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/models/sensor.pyi
+-rw-r--r--   0        0        0    26908 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/events/service.py
+-rw-r--r--   0        0        0      282 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/expr/__init__.py
+-rw-r--r--   0        0        0    12021 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/expr/_node.py
+-rw-r--r--   0        0        0      647 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/expr/_sprig.py
+-rw-r--r--   0        0        0        0 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/py.typed
+-rw-r--r--   0        0        0      188 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/shared/__init__.py
+-rw-r--r--   0        0        0      269 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/shared/_base_model.py
+-rw-r--r--   0        0        0     4927 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/shared/_global_config.py
+-rw-r--r--   0        0        0      513 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/shared/serialization.py
+-rw-r--r--   0        0        0     4413 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/__init__.py
+-rw-r--r--   0        0        0     2298 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/_context.py
+-rw-r--r--   0        0        0    23829 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/_mixins.py
+-rw-r--r--   0        0        0    32815 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/_unparse.py
+-rw-r--r--   0        0        0       25 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/action.py
+-rw-r--r--   0        0        0     1115 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/archive.py
+-rw-r--r--   0        0        0     7697 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/artifact.py
+-rw-r--r--   0        0        0     3446 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/container.py
+-rw-r--r--   0        0        0     3988 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/container_set.py
+-rw-r--r--   0        0        0     3763 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/cron_workflow.py
+-rw-r--r--   0        0        0     2771 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/dag.py
+-rw-r--r--   0        0        0     2186 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/data.py
+-rw-r--r--   0        0        0     4855 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/env.py
+-rw-r--r--   0        0        0     1329 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/env_from.py
+-rw-r--r--   0        0        0      208 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/exceptions.py
+-rw-r--r--   0        0        0     2291 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/http_template.py
+-rw-r--r--   0        0        0       30 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/memoize.py
+-rw-r--r--   0        0        0     6913 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/__init__.py
+-rw-r--r--   0        0        0     1418 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/eventsource.py
+-rw-r--r--   0        0        0      861 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/eventsource.pyi
+-rw-r--r--   0        0        0      144 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/google/__init__.py
+-rw-r--r--   0        0        0      347 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/google/protobuf.py
+-rw-r--r--   0        0        0      164 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/google/protobuf.pyi
+-rw-r--r--   0        0        0        0 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/grpc/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/grpc/gateway/__init__.py
+-rw-r--r--   0        0        0      691 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/grpc/gateway/runtime.py
+-rw-r--r--   0        0        0      470 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/grpc/gateway/runtime.pyi
+-rw-r--r--   0        0        0        0 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/events/__init__.py
+-rw-r--r--   0        0        0   102993 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/events/v1alpha1.py
+-rw-r--r--   0        0        0    25271 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi
+-rw-r--r--   0        0        0      144 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/workflow/__init__.py
+-rw-r--r--   0        0        0   144549 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py
+-rw-r--r--   0        0        0    31958 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi
+-rw-r--r--   0        0        0        0 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/core/__init__.py
+-rw-r--r--   0        0        0   127883 2023-04-15 21:34:41.515745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/core/v1.py
+-rw-r--r--   0        0        0    18004 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/core/v1.pyi
+-rw-r--r--   0        0        0      144 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/policy/__init__.py
+-rw-r--r--   0        0        0     1751 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py
+-rw-r--r--   0        0        0      376 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/policy/v1beta1.pyi
+-rw-r--r--   0        0        0        0 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0        0        0     3161 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py
+-rw-r--r--   0        0        0      105 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.pyi
+-rw-r--r--   0        0        0        0 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0        0        0    22218 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
+-rw-r--r--   0        0        0     2064 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
+-rw-r--r--   0        0        0      144 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0        0        0      277 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.py
+-rw-r--r--   0        0        0      108 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.pyi
+-rw-r--r--   0        0        0     1453 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/sensor.py
+-rw-r--r--   0        0        0      887 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/models/sensor.pyi
+-rw-r--r--   0        0        0      722 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/operator.py
+-rw-r--r--   0        0        0     4084 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/parameter.py
+-rw-r--r--   0        0        0     1018 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/protocol.py
+-rw-r--r--   0        0        0     2554 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/resource.py
+-rw-r--r--   0        0        0     5262 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/resources.py
+-rw-r--r--   0        0        0     1856 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/retry_strategy.py
+-rw-r--r--   0        0        0     3707 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/runner.py
+-rw-r--r--   0        0        0    14748 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/script.py
+-rw-r--r--   0        0        0    49478 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/service.py
+-rw-r--r--   0        0        0     9297 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/steps.py
+-rw-r--r--   0        0        0     3266 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/suspend.py
+-rw-r--r--   0        0        0    10495 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/task.py
+-rw-r--r--   0        0        0       27 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/toleration.py
+-rw-r--r--   0        0        0     2007 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/user_container.py
+-rw-r--r--   0        0        0     2610 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/validators.py
+-rw-r--r--   0        0        0    18656 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/volume.py
+-rw-r--r--   0        0        0    15590 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/workflow.py
+-rw-r--r--   0        0        0      911 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/workflow_status.py
+-rw-r--r--   0        0        0     5925 2023-04-15 21:34:41.519745 hera_workflows-5.1.3/src/hera/workflows/workflow_template.py
+-rw-r--r--   0        0        0    13280 1970-01-01 00:00:00.000000 hera_workflows-5.1.3/PKG-INFO
```

### Comparing `hera_workflows-5.1.2/LICENSE` & `hera_workflows-5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/README.md` & `hera_workflows-5.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -12,18 +12,24 @@
 [![codecov](https://codecov.io/gh/argoproj-labs/hera/branch/main/graph/badge.svg?token=x4tvsQRKXP)](https://codecov.io/gh/argoproj-labs/hera)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 [![Pypi](https://img.shields.io/pypi/v/hera.svg)](https://pypi.python.org/pypi/hera)
 [![CondaForge](https://anaconda.org/conda-forge/hera-workflows/badges/version.svg)](https://anaconda.org/conda-forge/hera-workflows)
 [![Versions](https://img.shields.io/pypi/pyversions/hera.svg)](https://github.com/argoproj-labs/hera)
 
+### Stats after the [rename to Hera](https://github.com/argoproj-labs/hera/discussions/532)
 [![Downloads](https://pepy.tech/badge/hera)](https://pepy.tech/project/hera)
 [![Downloads/month](https://pepy.tech/badge/hera/month)](https://pepy.tech/project/hera)
 [![Downloads/week](https://pepy.tech/badge/hera/week)](https://pepy.tech/project/hera)
 
+### Stats before the [rename to Hera](https://github.com/argoproj-labs/hera/discussions/532)
+[![Downloads](https://pepy.tech/badge/hera-workflows)](https://pepy.tech/project/hera-workflows)
+[![Downloads/month](https://pepy.tech/badge/hera-workflows/month)](https://pepy.tech/project/hera-workflows)
+[![Downloads/week](https://pepy.tech/badge/hera-workflows/week)](https://pepy.tech/project/hera-workflows)
+
 Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make the Argo
 ecosystem accessible by simplifying workflow construction and submission.
 
 You can watch the introductory Hera presentation at the "Argo Workflows and Events Community Meeting 20 Oct
 2021" [here](https://www.youtube.com/watch?v=QETfzfVV-GY&t=181s)!
 
 # Table of content
```

### Comparing `hera_workflows-5.1.2/pyproject.toml` & `hera_workflows-5.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "hera-workflows"  # project-name
 # The version is automatically substituted by the CI
-version = "5.1.2"
+version = "5.1.3"
 description = "Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make Argo Workflows more accessible by abstracting away some setup that is typically necessary for constructing Argo workflows."
 authors = ["Flaviu Vadan <flaviu.vadan@dynotx.com>", "Sambhav Kothari <sambhavs.email@gmail.com>", "Elliot Gunton <elliotgunton@gmail.com>"]
 maintainers = ["Flaviu Vadan <flaviu.vadan@dynotx.com>", "Sambhav Kothari <sambhavs.email@gmail.com>", "Elliot Gunton <elliotgunton@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/argoproj-labs/hera"
 repository = "https://github.com/argoproj-labs/hera"
```

### Comparing `hera_workflows-5.1.2/src/hera/__init__.py` & `hera_workflows-5.1.3/src/hera/__init__.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/events/models/__init__.py` & `hera_workflows-5.1.3/src/hera/events/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/events/models/eventsource.py` & `hera_workflows-5.1.3/src/hera/events/models/eventsource.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/events/models/eventsource.pyi` & `hera_workflows-5.1.3/src/hera/events/models/eventsource.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/events/models/grpc/gateway/runtime.py` & `hera_workflows-5.1.3/src/hera/events/models/grpc/gateway/runtime.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/events/models/io/argoproj/events/v1alpha1.py` & `hera_workflows-5.1.3/src/hera/events/models/io/argoproj/events/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/events/models/io/argoproj/events/v1alpha1.pyi` & `hera_workflows-5.1.3/src/hera/events/models/io/argoproj/events/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/events/models/io/argoproj/workflow/v1alpha1.py` & `hera_workflows-5.1.3/src/hera/events/models/io/argoproj/workflow/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi` & `hera_workflows-5.1.3/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/events/models/io/k8s/api/core/v1.py` & `hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/core/v1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/events/models/io/k8s/api/core/v1.pyi` & `hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/core/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/events/models/io/k8s/api/policy/v1beta1.py` & `hera_workflows-5.1.3/src/hera/events/models/io/k8s/api/policy/v1beta1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py` & `hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py` & `hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi` & `hera_workflows-5.1.3/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/events/models/sensor.py` & `hera_workflows-5.1.3/src/hera/events/models/sensor.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/events/models/sensor.pyi` & `hera_workflows-5.1.3/src/hera/events/models/sensor.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/events/service.py` & `hera_workflows-5.1.3/src/hera/events/service.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/expr/_node.py` & `hera_workflows-5.1.3/src/hera/expr/_node.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/expr/_sprig.py` & `hera_workflows-5.1.3/src/hera/expr/_sprig.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/shared/_global_config.py` & `hera_workflows-5.1.3/src/hera/shared/_global_config.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/shared/serialization.py` & `hera_workflows-5.1.3/src/hera/shared/serialization.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/__init__.py` & `hera_workflows-5.1.3/src/hera/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/_context.py` & `hera_workflows-5.1.3/src/hera/workflows/_context.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/_mixins.py` & `hera_workflows-5.1.3/src/hera/workflows/_mixins.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/archive.py` & `hera_workflows-5.1.3/src/hera/workflows/archive.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/artifact.py` & `hera_workflows-5.1.3/src/hera/workflows/artifact.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/container.py` & `hera_workflows-5.1.3/src/hera/workflows/container.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/container_set.py` & `hera_workflows-5.1.3/src/hera/workflows/container_set.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/cron_workflow.py` & `hera_workflows-5.1.3/src/hera/workflows/cron_workflow.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/dag.py` & `hera_workflows-5.1.3/src/hera/workflows/dag.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/data.py` & `hera_workflows-5.1.3/src/hera/workflows/data.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/env.py` & `hera_workflows-5.1.3/src/hera/workflows/env.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/env_from.py` & `hera_workflows-5.1.3/src/hera/workflows/env_from.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/http_template.py` & `hera_workflows-5.1.3/src/hera/workflows/http_template.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/models/__init__.py` & `hera_workflows-5.1.3/src/hera/workflows/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/models/eventsource.py` & `hera_workflows-5.1.3/src/hera/workflows/models/eventsource.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/models/eventsource.pyi` & `hera_workflows-5.1.3/src/hera/workflows/models/eventsource.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/models/grpc/gateway/runtime.py` & `hera_workflows-5.1.3/src/hera/workflows/models/grpc/gateway/runtime.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/models/io/argoproj/events/v1alpha1.py` & `hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/events/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi` & `hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py` & `hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi` & `hera_workflows-5.1.3/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/api/core/v1.py` & `hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/core/v1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/api/core/v1.pyi` & `hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/core/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py` & `hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py` & `hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py` & `hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi` & `hera_workflows-5.1.3/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/models/sensor.py` & `hera_workflows-5.1.3/src/hera/workflows/models/sensor.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/models/sensor.pyi` & `hera_workflows-5.1.3/src/hera/workflows/models/sensor.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/operator.py` & `hera_workflows-5.1.3/src/hera/workflows/operator.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/parameter.py` & `hera_workflows-5.1.3/src/hera/workflows/parameter.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/protocol.py` & `hera_workflows-5.1.3/src/hera/workflows/protocol.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/resource.py` & `hera_workflows-5.1.3/src/hera/workflows/resource.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/resources.py` & `hera_workflows-5.1.3/src/hera/workflows/resources.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/retry_strategy.py` & `hera_workflows-5.1.3/src/hera/workflows/retry_strategy.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/runner.py` & `hera_workflows-5.1.3/src/hera/workflows/runner.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/script.py` & `hera_workflows-5.1.3/src/hera/workflows/script.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     ContainerMixin,
     EnvIOMixin,
     ExperimentalMixin,
     ResourceMixin,
     TemplateMixin,
     VolumeMountMixin,
 )
+from hera.workflows._unparse import roundtrip
 from hera.workflows.models import (
     Inputs as ModelInputs,
     Lifecycle,
     ScriptTemplate as _ModelScriptTemplate,
     SecurityContext,
     Template as _ModelTemplate,
 )
@@ -324,26 +325,24 @@
             script = "import os\nimport sys\nsys.path.append(os.getcwd())\n"
 
         script_extra = self._get_param_script_portion(instance) if args else None
         if script_extra:
             script += copy.deepcopy(script_extra)
             script += "\n"
 
-        # content represents the function components, separated by new lines
-        # therefore, the actual code block occurs after the end parenthesis, which is a literal `):\n`
-        content = inspect.getsourcelines(instance.source)[0]
-        token_index, start_token = 1, ":\n"
-        for curr_index, curr_token in enumerate(content):
-            if start_token in curr_token:
-                # when we find the curr token we find the end of the function header. The next index is the
-                # starting point of the function body
-                token_index = curr_index + 1
+        # We use ast parse/unparse to get the source code of the function
+        # in order to have consistent looking functions and getting rid of any comments
+        # parsing issues.
+        # See https://github.com/argoproj-labs/hera/issues/572
+        content = roundtrip(inspect.getsource(instance.source)).splitlines()
+        for i, line in enumerate(content):
+            if line.startswith("def") or line.startswith("async def"):
                 break
 
-        s = "".join(content[token_index:])
+        s = "\n".join(content[i + 1 :])
         script += textwrap.dedent(s)
         return textwrap.dedent(script)
 
 
 class RunnerScriptConstructor(ScriptConstructor, ExperimentalMixin):
     _flag: str = "script_runner"
```

### Comparing `hera_workflows-5.1.2/src/hera/workflows/service.py` & `hera_workflows-5.1.3/src/hera/workflows/service.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/steps.py` & `hera_workflows-5.1.3/src/hera/workflows/steps.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/suspend.py` & `hera_workflows-5.1.3/src/hera/workflows/suspend.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/task.py` & `hera_workflows-5.1.3/src/hera/workflows/task.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/user_container.py` & `hera_workflows-5.1.3/src/hera/workflows/user_container.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/validators.py` & `hera_workflows-5.1.3/src/hera/workflows/validators.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/volume.py` & `hera_workflows-5.1.3/src/hera/workflows/volume.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/workflow.py` & `hera_workflows-5.1.3/src/hera/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/workflow_status.py` & `hera_workflows-5.1.3/src/hera/workflows/workflow_status.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/src/hera/workflows/workflow_template.py` & `hera_workflows-5.1.3/src/hera/workflows/workflow_template.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.2/PKG-INFO` & `hera_workflows-5.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hera-workflows
-Version: 5.1.2
+Version: 5.1.3
 Summary: Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make Argo Workflows more accessible by abstracting away some setup that is typically necessary for constructing Argo workflows.
 Home-page: https://github.com/argoproj-labs/hera
 License: MIT
 Author: Flaviu Vadan
 Author-email: flaviu.vadan@dynotx.com
 Maintainer: Flaviu Vadan
 Maintainer-email: flaviu.vadan@dynotx.com
@@ -46,18 +46,24 @@
 [![codecov](https://codecov.io/gh/argoproj-labs/hera/branch/main/graph/badge.svg?token=x4tvsQRKXP)](https://codecov.io/gh/argoproj-labs/hera)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 [![Pypi](https://img.shields.io/pypi/v/hera.svg)](https://pypi.python.org/pypi/hera)
 [![CondaForge](https://anaconda.org/conda-forge/hera-workflows/badges/version.svg)](https://anaconda.org/conda-forge/hera-workflows)
 [![Versions](https://img.shields.io/pypi/pyversions/hera.svg)](https://github.com/argoproj-labs/hera)
 
+### Stats after the [rename to Hera](https://github.com/argoproj-labs/hera/discussions/532)
 [![Downloads](https://pepy.tech/badge/hera)](https://pepy.tech/project/hera)
 [![Downloads/month](https://pepy.tech/badge/hera/month)](https://pepy.tech/project/hera)
 [![Downloads/week](https://pepy.tech/badge/hera/week)](https://pepy.tech/project/hera)
 
+### Stats before the [rename to Hera](https://github.com/argoproj-labs/hera/discussions/532)
+[![Downloads](https://pepy.tech/badge/hera-workflows)](https://pepy.tech/project/hera-workflows)
+[![Downloads/month](https://pepy.tech/badge/hera-workflows/month)](https://pepy.tech/project/hera-workflows)
+[![Downloads/week](https://pepy.tech/badge/hera-workflows/week)](https://pepy.tech/project/hera-workflows)
+
 Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make the Argo
 ecosystem accessible by simplifying workflow construction and submission.
 
 You can watch the introductory Hera presentation at the "Argo Workflows and Events Community Meeting 20 Oct
 2021" [here](https://www.youtube.com/watch?v=QETfzfVV-GY&t=181s)!
 
 # Table of content
```

