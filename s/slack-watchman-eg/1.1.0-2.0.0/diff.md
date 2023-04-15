# Comparing `tmp/slack-watchman-eg-1.1.0.tar.gz` & `tmp/slack-watchman-eg-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack-watchman-eg-1.1.0.tar", last modified: Sun Apr  3 20:26:23 2022, max compression
+gzip compressed data, was "slack-watchman-eg-2.0.0.tar", last modified: Sat Apr 15 19:50:51 2023, max compression
```

## Comparing `slack-watchman-eg-1.1.0.tar` & `slack-watchman-eg-2.0.0.tar`

### file list

```diff
@@ -1,93 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 20:26:23.247131 slack-watchman-eg-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8373 2022-04-03 20:26:23.247131 slack-watchman-eg-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7060 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-04-03 20:26:23.247131 slack-watchman-eg-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 20:26:23.239131 slack-watchman-eg-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 20:26:23.239131 slack-watchman-eg-1.1.0/src/signatures/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 20:26:23.239131 slack-watchman-eg-1.1.0/src/signatures/competitive/
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/competitive/archive_files.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/competitive/budget_files.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/competitive/excel_files.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/competitive/powerpoint_files.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/competitive/word_files.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 20:26:23.239131 slack-watchman-eg-1.1.0/src/signatures/compliance/
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/compliance/bank_cards.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/compliance/cusip_numbers.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/compliance/cv_files.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/compliance/date_of_birth.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/compliance/drivers_licence_uk.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/compliance/iban_numbers.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/compliance/itin_numbers.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/compliance/mastercard_datacash.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/compliance/ni_numbers.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/compliance/passport_numbers.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/compliance/ssn_us.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 20:26:23.239131 slack-watchman-eg-1.1.0/src/signatures/sandbox/
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/sandbox/placeholder.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 20:26:23.243131 slack-watchman-eg-1.1.0/src/signatures/security/
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/access_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/aws_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/azure_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/azure_service_account_files.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/bearer_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/certificate_files.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/client_secrets.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/cloudflare_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/config_files.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/executable_files.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/facebook_access_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/facebook_secret_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/ftp_credentials.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/gcp_service_account_files.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/gcp_service_accounts_text.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      620 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/github_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/google_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/grafana_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/heroku_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/interesting_files.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/mailchimp_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/mailgun_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/new_relic_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/new_relic_prefixed_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/pagerduty_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/passwords.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/paypal_braintree.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/private_keys.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/private_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/s3_config_files.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/shodan_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/slack_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/slack_webhooks.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/snyk_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/stripe_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/twilio_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/twitter_api_tokens.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/x_api_key.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/signatures/security/x_auth_key.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 20:26:23.243131 slack-watchman-eg-1.1.0/src/slack_watchman_eg/
--rw-r--r--   0 runner    (1001) docker     (121)    11967 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/slack_watchman_eg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/slack_watchman_eg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/slack_watchman_eg/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2084 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/slack_watchman_eg/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     2879 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/slack_watchman_eg/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 20:26:23.247131 slack-watchman-eg-1.1.0/src/slack_watchman_eg/slack_objects/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/slack_watchman_eg/slack_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4510 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/slack_watchman_eg/slack_objects/conversation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/slack_watchman_eg/slack_objects/enterprise.py
--rw-r--r--   0 runner    (1001) docker     (121)     4474 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/slack_watchman_eg/slack_objects/post.py
--rw-r--r--   0 runner    (1001) docker     (121)     4009 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/slack_watchman_eg/slack_objects/user.py
--rw-r--r--   0 runner    (1001) docker     (121)     2579 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/slack_watchman_eg/slack_objects/workspace.py
--rw-r--r--   0 runner    (1001) docker     (121)    55414 2022-04-03 20:26:01.000000 slack-watchman-eg-1.1.0/src/slack_watchman_eg/slack_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 20:26:23.247131 slack-watchman-eg-1.1.0/src/slack_watchman_eg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8373 2022-04-03 20:26:22.000000 slack-watchman-eg-1.1.0/src/slack_watchman_eg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3502 2022-04-03 20:26:23.000000 slack-watchman-eg-1.1.0/src/slack_watchman_eg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-03 20:26:22.000000 slack-watchman-eg-1.1.0/src/slack_watchman_eg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-04-03 20:26:22.000000 slack-watchman-eg-1.1.0/src/slack_watchman_eg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-03 20:26:21.000000 slack-watchman-eg-1.1.0/src/slack_watchman_eg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-04-03 20:26:23.000000 slack-watchman-eg-1.1.0/src/slack_watchman_eg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-04-03 20:26:23.000000 slack-watchman-eg-1.1.0/src/slack_watchman_eg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:50:51.703666 slack-watchman-eg-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-15 19:50:35.000000 slack-watchman-eg-2.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-15 19:50:35.000000 slack-watchman-eg-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-04-15 19:50:51.707666 slack-watchman-eg-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-04-15 19:50:35.000000 slack-watchman-eg-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-15 19:50:35.000000 slack-watchman-eg-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-15 19:50:51.707666 slack-watchman-eg-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:50:51.703666 slack-watchman-eg-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:50:51.703666 slack-watchman-eg-2.0.0/src/slack_watchman_eg/
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-04-15 19:50:35.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-15 19:50:35.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-15 19:50:35.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:50:51.703666 slack-watchman-eg-2.0.0/src/slack_watchman_eg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:50:35.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-04-15 19:50:35.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg/models/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-15 19:50:35.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg/models/enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-04-15 19:50:35.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg/models/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-15 19:50:35.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg/models/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-15 19:50:35.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-15 19:50:35.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-15 19:50:35.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg/signature_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55433 2023-04-15 19:50:35.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg/slack_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-04-15 19:50:35.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg/sw_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:50:51.703666 slack-watchman-eg-2.0.0/src/slack_watchman_eg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-04-15 19:50:51.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-15 19:50:51.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 19:50:51.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-15 19:50:51.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 19:50:51.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-15 19:50:51.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-15 19:50:51.000000 slack-watchman-eg-2.0.0/src/slack_watchman_eg.egg-info/top_level.txt
```

### Comparing `slack-watchman-eg-1.1.0/LICENSE` & `slack-watchman-eg-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slack-watchman-eg-1.1.0/PKG-INFO` & `slack-watchman-eg-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 Metadata-Version: 2.1
 Name: slack-watchman-eg
-Version: 1.1.0
-Summary: Monitoring your Slack Enterprise Grid for sensitive information
+Version: 2.0.0
+Summary: Monitoring Slack Enterprise Grid for exposed secrets
 Home-page: https://github.com/PaperMtn/slack-watchman-enterprise-grid
 Author: PaperMtn
 Author-email: papermtn@protonmail.com
 License: GPL-3.0
 Keywords: audit,slack,slack-watchman,watchman,blue-team,red-team,threat-hunting,slack-watchman-enterprise-grid
-Platform: UNKNOWN
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://i.imgur.com/VPgx6ra.png" width="550">
 
 # Slack Watchman for Enterprise Grid
 ![Python 2.7 and 3 compatible](https://img.shields.io/pypi/pyversions/slack-watchman-eg)
 ![PyPI version](https://img.shields.io/pypi/v/slack-watchman-eg.svg)
 ![License: MIT](https://img.shields.io/pypi/l/slack-watchman-eg.svg)
 
 
 ## About Slack Watchman for Enterprise Grid
 
-Slack Watchman for Enterprise Grid uses the Slack Enterprise Grid DLP API to look for potentially sensitive data exposed in your Slack Enterprise.
+Slack Watchman for Enterprise Grid uses the Slack Enterprise Grid DLP API to look for potentially exposed secrets and sensitive data in Slack Enterprise Grid.
 
 **Note**: Slack Watchman for Enterprise Grid is designed for Enterprise Grid subscribers of Slack only. If you use Slack without an Enterprise subscription, you can use the standard version of [Slack Watchman](https://github.com/PaperMtn/slack-watchman)
 
 ### Features
 Slack Watchman for Enterprise Grid looks for:
 
 - API Keys, Tokens & Service Accounts
@@ -70,50 +66,15 @@
 #### Multiprocessing
 Multiprocessing is used to search the potentially huge amount of data retrieved when getting all messages sent in an Enterprise. You can specify how many cores to use at runtime, and the more cores you use, the faster processing is generally done. That being said, you are still constrained by the API.
 
 I have found the most efficient approach is to use between 8-12 cores.
 
 You can specify cores using the optional flag `--cores` at runtime. If this flag is not set, Slack Watchman will automatically use all available cores up to a maximum of 8.
 ### Signatures
-Slack Watchman uses custom YAML signatures to detect matches in Slack.
-
-They follow this format:
-
-```yaml
----
-filename:
-enabled: [true|false]
-meta:
-  name:
-  author:
-  date:
-  description: # what the search should find
-  severity: # rating out of 100
-tombstone: [true|false]
-scope:
-  - [files|messages]
-file_types: # optional list for use with file searching*
-locations: # what conversations to search in. Any combination of:
-  - public
-  - private
-  - connect
-  - im
-  - mpim
-test_cases:
-  match_cases:
-  - # test case that should match the regex*
-  fail_cases:
-  - # test case that should not match the regex*
-search_strings:
-- # search query(s) to use in Slack
-pattern: # Regex pattern to filter out false positives
-```
-There are Python tests to ensure signatures are formatted properly and that the Regex patterns work in the `tests` dir
-
-More information about signatures, and how you can add your own, is in the file `docs/signatures.md`.
+Slack Watchman uses custom YAML signatures to detect matches in Slack. These signatures are pulled from the central [Watchman Signatures repository](https://github.com/PaperMtn/watchman-signatures). Slack Watchman for Enterprise Grid automatically updates its signature base at runtime to ensure its using the latest signatures to detect secrets. 
 
 ## Requirements
 ### Slack API token
 To run Slack Watchman for Enterprise Grid, you will need a Slack API access token that is authorised to use the Enterprise DLP API.
 
 To do this, you need to create a [Slack App](https://api.slack.com/apps) and install it at the organisation level.
 
@@ -130,15 +91,15 @@
 Provide the token in the environment variable `SLACK_WATCHMAN_EG_TOKEN`
 
 ## Installation
 You can install the latest stable version via pip:
 
 `python3 -m pip install slack-watchman-eg`
 
-Or build from source yourself, which is useful for if you intend to add your own signatures:
+Or build from source yourself:
 
 Download the release source files, then from the top level repository run:
 ```shell
 python3 -m pip build
 python3 -m pip install --force-reinstall dist/*.whl
 ```
 
@@ -157,55 +118,74 @@
 // scan all
 docker run --rm -e SLACK_WATCHMAN_EG_TOKENN=xoxp... papermountain/slack-watchman-eg --hours 1 --cores 8
 docker run --rm --env-file .env papermountain/slack-watchman-eg --hours 1 --cores 8
 ```
 
 ## Usage
 ```
-usage: slack-watchman-eg [-h] [--hours HOURS] [--minutes MINUTES] [--cores CORES] [--version] [--users] [--workspaces] [--sandbox] [--tombstone] [--tombstone-text-file TOMBSTONE_FILEPATH]
+usage: slack-watchman-eg [-h] [--hours HOURS] [--minutes MINUTES] [--output {json,terminal}] [--cores CORES] [--version] [--users] [--workspaces] [--debug] [--verbose]
 
 Monitoring your Slack Enterprise Grid for sensitive information
 
 options:
   -h, --help            show this help message and exit
-  --hours HOURS         How far back to search in whole hours between 1-24. Defaults to 1 if no acceptable value given
-  --minutes MINUTES     How far back to search in whole minutes between 1-60
-  --cores CORES         Number of cores to use between 1-12
-  --version             show program's version number and exit
-  --users               Find all users
-  --workspaces          Find all workspaces
-  --sandbox             Search using only sandbox signatures
-  --tombstone           Tombstone (REMOVE) all matching messages
-  --tombstone-text-file TOMBSTONE_FILEPATH
-                        Path to file containing custom tombstone notification text (Optional)
+  --hours HOURS, -hr HOURS
+                        How far back to search in whole hours between 1-24. Defaults to 1 if no acceptable value given
+  --minutes MINUTES, -m MINUTES
+                        How far back to search in whole minutes between 1-60
+  --output {json,terminal}, -o {json,terminal}
+                        What logging output to use - JSON formatted output, or textual outputfor reading via terminal. Default is terminal
+  --cores CORES, -c CORES
+                        Number of cores to use between 1-12
+  --version, -v         show program's version number and exit
+  --users, -u           Return all users
+  --workspaces, -w      Return all workspaces
+  --debug, -d           Turn on debug level logging
+  --verbose, -V         Turn on more verbose output for JSON logging. This includes more fields, but is larger
 ```
 
 ## Other Watchman apps
 You may be interested in the other apps in the Watchman family:
+- [Slack Watchman](https://github.com/PaperMtn/slack-watchman)
 - [GitLab Watchman](https://github.com/PaperMtn/gitlab-watchman)
 - [GitHub Watchman](https://github.com/PaperMtn/github-watchman)
-- [Slack Watchman](https://github.com/PaperMtn/slack-watchman)
-- [Trello Watchman](https://github.com/PaperMtn/trello-watchman)
 
 ## License
-The source code for this project is released under the [GNU General Public Licence](https://www.gnu.org/licenses/licenses.html#GPL). This project is not associated with Slack.
-## 1.1.0 - 2022-04-02
+The source code for this project is released under the [GNU General Public Licence](https://www.gnu.org/licenses/licenses.html#GPL). This project is not associated with Slack Technologies or Salesforce.
+## [2.0.0] - 2023-04-14
+This major version release brings multiple updates to Slack Watchman for Enterprise Grid, both in usability, functionality and behind the scenes improvements.
+### Added
+- Support for centralised signatures from the Watchman Signatures repository. This makes it much easier to keep the signature base for all Watchman applications up to date, and to add functionality to Slack Watchman with new signatures. New signatures are downloaded, and updates to existing signatures are applied, at runtime, meaning Slack Watchman for Enterprise Grid will always be using the most up to date signatures. 
+- Option for terminal optimised logging instead of JSON formatting. This is now the default when running with no output option selected, and is a lot easier for humans to read. Also, colours! 
+- Option choose between verbose or succinct logging when using JSON output. Default is succinct.
+- Debug logging option
+### Removed
+- Support for tombstoning posts that match signatures removed
+- Local signatures - Centralised signatures mean that user-created custom signatures can't be used with Slack Watchman for Enterprise Grid anymore. If you have made a signature you think would be good for sharing with the community, feel free to add it to the Watchman Signatures repository, so it can be used in all Watchman applications 
+- For the reason above, the functionality to have sandbox signatures has been removed as well
+### Fixed
+- Draft searches were giving an error due to not being able to populate some workspace information. This has now been fixed
+
+## [1.1.1] - 2022-05-16
+### Added
+- Signature to find Atlassian tokens
+
+## [1.1.0] - 2022-04-02
 ### Added
 - Docker image now available from the Docker hub, or by building from source.
 - Support for Python 3.7
 - New logo to play nicely with dark mode
 ### Fixed
 - More errors when importing packages
 
-## 1.0.2 - 2021-12-30
+## [1.0.2] - 2021-12-30
 ### Fixed
 - Error when importing packages
 - Signatures not being included in the distribution package
 
-## 1.0.1 - 2021-12-30
+## [1.0.1] - 2021-12-30
+### Added
 - Refactor and update distribution files
 
-## 1.0.0 - 2021-12-30
+## [1.0.0] - 2021-12-30
 - Initial release
 
-
-
```

### Comparing `slack-watchman-eg-1.1.0/README.md` & `slack-watchman-eg-2.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ![Python 2.7 and 3 compatible](https://img.shields.io/pypi/pyversions/slack-watchman-eg)
 ![PyPI version](https://img.shields.io/pypi/v/slack-watchman-eg.svg)
 ![License: MIT](https://img.shields.io/pypi/l/slack-watchman-eg.svg)
 
 
 ## About Slack Watchman for Enterprise Grid
 
-Slack Watchman for Enterprise Grid uses the Slack Enterprise Grid DLP API to look for potentially sensitive data exposed in your Slack Enterprise.
+Slack Watchman for Enterprise Grid uses the Slack Enterprise Grid DLP API to look for potentially exposed secrets and sensitive data in Slack Enterprise Grid.
 
 **Note**: Slack Watchman for Enterprise Grid is designed for Enterprise Grid subscribers of Slack only. If you use Slack without an Enterprise subscription, you can use the standard version of [Slack Watchman](https://github.com/PaperMtn/slack-watchman)
 
 ### Features
 Slack Watchman for Enterprise Grid looks for:
 
 - API Keys, Tokens & Service Accounts
@@ -49,50 +49,15 @@
 #### Multiprocessing
 Multiprocessing is used to search the potentially huge amount of data retrieved when getting all messages sent in an Enterprise. You can specify how many cores to use at runtime, and the more cores you use, the faster processing is generally done. That being said, you are still constrained by the API.
 
 I have found the most efficient approach is to use between 8-12 cores.
 
 You can specify cores using the optional flag `--cores` at runtime. If this flag is not set, Slack Watchman will automatically use all available cores up to a maximum of 8.
 ### Signatures
-Slack Watchman uses custom YAML signatures to detect matches in Slack.
-
-They follow this format:
-
-```yaml
----
-filename:
-enabled: [true|false]
-meta:
-  name:
-  author:
-  date:
-  description: # what the search should find
-  severity: # rating out of 100
-tombstone: [true|false]
-scope:
-  - [files|messages]
-file_types: # optional list for use with file searching*
-locations: # what conversations to search in. Any combination of:
-  - public
-  - private
-  - connect
-  - im
-  - mpim
-test_cases:
-  match_cases:
-  - # test case that should match the regex*
-  fail_cases:
-  - # test case that should not match the regex*
-search_strings:
-- # search query(s) to use in Slack
-pattern: # Regex pattern to filter out false positives
-```
-There are Python tests to ensure signatures are formatted properly and that the Regex patterns work in the `tests` dir
-
-More information about signatures, and how you can add your own, is in the file `docs/signatures.md`.
+Slack Watchman uses custom YAML signatures to detect matches in Slack. These signatures are pulled from the central [Watchman Signatures repository](https://github.com/PaperMtn/watchman-signatures). Slack Watchman for Enterprise Grid automatically updates its signature base at runtime to ensure its using the latest signatures to detect secrets. 
 
 ## Requirements
 ### Slack API token
 To run Slack Watchman for Enterprise Grid, you will need a Slack API access token that is authorised to use the Enterprise DLP API.
 
 To do this, you need to create a [Slack App](https://api.slack.com/apps) and install it at the organisation level.
 
@@ -109,15 +74,15 @@
 Provide the token in the environment variable `SLACK_WATCHMAN_EG_TOKEN`
 
 ## Installation
 You can install the latest stable version via pip:
 
 `python3 -m pip install slack-watchman-eg`
 
-Or build from source yourself, which is useful for if you intend to add your own signatures:
+Or build from source yourself:
 
 Download the release source files, then from the top level repository run:
 ```shell
 python3 -m pip build
 python3 -m pip install --force-reinstall dist/*.whl
 ```
 
@@ -136,34 +101,36 @@
 // scan all
 docker run --rm -e SLACK_WATCHMAN_EG_TOKENN=xoxp... papermountain/slack-watchman-eg --hours 1 --cores 8
 docker run --rm --env-file .env papermountain/slack-watchman-eg --hours 1 --cores 8
 ```
 
 ## Usage
 ```
-usage: slack-watchman-eg [-h] [--hours HOURS] [--minutes MINUTES] [--cores CORES] [--version] [--users] [--workspaces] [--sandbox] [--tombstone] [--tombstone-text-file TOMBSTONE_FILEPATH]
+usage: slack-watchman-eg [-h] [--hours HOURS] [--minutes MINUTES] [--output {json,terminal}] [--cores CORES] [--version] [--users] [--workspaces] [--debug] [--verbose]
 
 Monitoring your Slack Enterprise Grid for sensitive information
 
 options:
   -h, --help            show this help message and exit
-  --hours HOURS         How far back to search in whole hours between 1-24. Defaults to 1 if no acceptable value given
-  --minutes MINUTES     How far back to search in whole minutes between 1-60
-  --cores CORES         Number of cores to use between 1-12
-  --version             show program's version number and exit
-  --users               Find all users
-  --workspaces          Find all workspaces
-  --sandbox             Search using only sandbox signatures
-  --tombstone           Tombstone (REMOVE) all matching messages
-  --tombstone-text-file TOMBSTONE_FILEPATH
-                        Path to file containing custom tombstone notification text (Optional)
+  --hours HOURS, -hr HOURS
+                        How far back to search in whole hours between 1-24. Defaults to 1 if no acceptable value given
+  --minutes MINUTES, -m MINUTES
+                        How far back to search in whole minutes between 1-60
+  --output {json,terminal}, -o {json,terminal}
+                        What logging output to use - JSON formatted output, or textual outputfor reading via terminal. Default is terminal
+  --cores CORES, -c CORES
+                        Number of cores to use between 1-12
+  --version, -v         show program's version number and exit
+  --users, -u           Return all users
+  --workspaces, -w      Return all workspaces
+  --debug, -d           Turn on debug level logging
+  --verbose, -V         Turn on more verbose output for JSON logging. This includes more fields, but is larger
 ```
 
 ## Other Watchman apps
 You may be interested in the other apps in the Watchman family:
+- [Slack Watchman](https://github.com/PaperMtn/slack-watchman)
 - [GitLab Watchman](https://github.com/PaperMtn/gitlab-watchman)
 - [GitHub Watchman](https://github.com/PaperMtn/github-watchman)
-- [Slack Watchman](https://github.com/PaperMtn/slack-watchman)
-- [Trello Watchman](https://github.com/PaperMtn/trello-watchman)
 
 ## License
-The source code for this project is released under the [GNU General Public Licence](https://www.gnu.org/licenses/licenses.html#GPL). This project is not associated with Slack.
+The source code for this project is released under the [GNU General Public Licence](https://www.gnu.org/licenses/licenses.html#GPL). This project is not associated with Slack Technologies or Salesforce.
```

### Comparing `slack-watchman-eg-1.1.0/setup.cfg` & `slack-watchman-eg-2.0.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 [metadata]
 name = slack-watchman-eg
 version = attr: slack_watchman_eg.__version__.__version__
-description = Monitoring your Slack Enterprise Grid for sensitive information
+description = Monitoring Slack Enterprise Grid for exposed secrets
 long_description = file: README.md, CHANGELOG.md
 long_description_content_type = text/markdown
 license = GPL-3.0
 url = https://github.com/PaperMtn/slack-watchman-enterprise-grid
 author = PaperMtn
 author_email = papermtn@protonmail.com
 keywords = audit, slack, slack-watchman, watchman, blue-team, red-team, threat-hunting, slack-watchman-enterprise-grid
 classifiers = 
 	Intended Audience :: Information Technology
 	Topic :: Security
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 
 [options]
 zip_safe = False
 package_dir = 
 	= src
 include_package_data = True
 packages = find_namespace:
-python_requires = >=3.7
+python_requires = >=3.10
 install_requires = 
 	requests
 	PyYAML
 	numpy
+	colorama
 
 [options.package_data]
 * = *.yml, *.yaml
 
 [options.data_files]
 . = signatures/*.yml, signatures/*.yaml
```

### Comparing `slack-watchman-eg-1.1.0/src/slack_watchman_eg/__init__.py` & `slack-watchman-eg-2.0.0/src/slack_watchman_eg/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,211 +1,185 @@
 import argparse
 import multiprocessing
 import os
 import time
 import calendar
 from pathlib import Path
+from typing import List
 
 from . import __version__
-from . import logger as logger
+from . import sw_logger
 from . import slack_wrapper
-from . import signature
+from . import signature_updater
+from .models import (
+    signature,
+    user,
+    workspace,
+    post,
+    conversation
+)
 
-SIGNATURES_PATH = (Path(__file__).parents[1] / 'signatures').resolve()
-OUTPUT_LOGGER: logger.StdoutLogger
-TOMBSTONE_CONTENT = None
+SIGNATURES_PATH = (Path(__file__).parents[2] / 'watchman-signatures').resolve()
+OUTPUT_LOGGER: sw_logger.JSONLogger
 
 
-def load_signatures(sandbox: bool) -> [signature.Signature]:
-    """
-    Load signatures from YAML files
-
-    Args:
-        sandbox: Whether to load sandbox signatures
+def load_signatures() -> List[signature.Signature]:
+    """ Load signatures from YAML files
     Returns:
-        List containing loaded definitions as signatures objects
-
+        List containing loaded definitions as Signatures objects
     """
 
     loaded_signatures = []
-    if sandbox:
-        signature_path = (SIGNATURES_PATH / 'sandbox').resolve()
-        OUTPUT_LOGGER.log_info('Importing sandbox signatures')
-    else:
-        signature_path = SIGNATURES_PATH
-
     try:
-        for root, dirs, files in os.walk(signature_path):
+        for root, dirs, files in os.walk(SIGNATURES_PATH):
             for sig_file in files:
                 sig_path = (Path(root) / sig_file).resolve()
                 if sig_path.name.endswith('.yaml'):
-                    loaded_sig = signature.load_from_yaml(sig_path)
-                    if loaded_sig.enabled:
-                        loaded_signatures.append(loaded_sig)
+                    loaded_def = signature.load_from_yaml(sig_path)
+                    for sig in loaded_def:
+                        if sig.status == 'enabled' and 'slack_eg' in sig.watchman_apps:
+                            loaded_signatures.append(sig)
         return loaded_signatures
     except Exception as e:
         raise e
 
 
-def search(sig: signature,
+def search(loaded_signature: signature,
            slack_connection: slack_wrapper.SlackAPI,
-           user_list: list,
-           message_list: list,
-           workspace_list: list,
-           files_list: list,
+           user_list: List[user.User],
+           message_list: List[post.Message],
+           workspace_list: List[workspace.Workspace],
+           files_list: List[post.File],
            scope: str,
            cores: int,
-           tombstone: bool):
+           verbose: bool) -> None:
     """ Uses the signature to call the relevant search functions to find data in messages
     files and drafts. Results are output to stdout logging.
-
     Args:
         slack_connection: Slack API object
-        sig: Signature object
+        loaded_signature: Signature object
         user_list: List of User objects from the Enterprise
         message_list: List of Message objects to search through
         workspace_list: List of Workspace objects from the Enterprise
         files_list: List of File objects to search through
-        scope: Scope of any results found for logging: e.g Draft
+        scope: Scope of any results found for logging: e.g. Draft
         cores: Number of CPU cores to use
-        tombstone: Whether to tombstone the file or not
+        verbose: Whether to use verbose logging or not
     """
 
     if scope == 'messages':
-        OUTPUT_LOGGER.log_info(f'Searching for posts containing {sig.meta.name}')
+        OUTPUT_LOGGER.log('INFO', f'Searching for posts containing {loaded_signature.name}')
         messages = slack_wrapper.search_message_matches(
-            sig,
+            loaded_signature,
             slack_connection,
             user_list,
             message_list,
             workspace_list,
             cores,
-            OUTPUT_LOGGER
+            OUTPUT_LOGGER,
+            verbose
         )
         if messages:
             for message in messages:
-                OUTPUT_LOGGER.log_notification(
+                OUTPUT_LOGGER.log(
+                    'NOTIFY',
                     message,
                     scope=scope,
-                    severity=sig.meta.severity,
-                    detect_type=sig.meta.name
+                    severity=loaded_signature.severity,
+                    detect_type=loaded_signature.name,
+                    notify_type='result'
                 )
-            if tombstone:
-                OUTPUT_LOGGER.log_info(f'Tombstoning messages containing {sig.meta.name}')
-                for message in messages:
-                    slack_wrapper.tombstone_message(slack_connection, message.get('message'), content=TOMBSTONE_CONTENT)
-                OUTPUT_LOGGER.log_info(f'{len(messages)} messages tombstoned')
 
     if scope == 'files':
-        OUTPUT_LOGGER.log_info(f'Searching for {sig.meta.name}')
+        OUTPUT_LOGGER.log('INFO', f'Searching for {loaded_signature.name}')
         files = slack_wrapper.search_file_matches(
-            sig,
+            loaded_signature,
             user_list,
             files_list,
             cores,
             OUTPUT_LOGGER
         )
         if files:
             for file in files:
-                OUTPUT_LOGGER.log_notification(
+                OUTPUT_LOGGER.log(
+                    'NOTIFY',
                     file,
                     scope=scope,
-                    severity=sig.meta.severity,
-                    detect_type=sig.meta.name
+                    severity=loaded_signature.severity,
+                    detect_type=loaded_signature.name,
+                    notify_type='result'
                 )
-            if tombstone:
-                OUTPUT_LOGGER.log_info(f'Tombstoning {sig.meta.name}')
-                for file in files:
-                    slack_wrapper.tombstone_file(slack_connection, file.get('file'), content=TOMBSTONE_CONTENT)
-                OUTPUT_LOGGER.log_info(f'{len(files)} files tombstoned')
 
 
 def core_validation(cores: int) -> int:
     """ Validate the number of cores entered
-
     Args:
         cores: Number of cores passed to CLI
     Returns:
         Number of cores to use
-
     """
 
     if not cores or cores > multiprocessing.cpu_count() or cores > 12:
         if multiprocessing.cpu_count() >= 8:
             return 8
         else:
             return multiprocessing.cpu_count()
     else:
         return cores
 
 
-def init_logger() -> logger.StdoutLogger:
+def init_logger(logging_type: str, debug: bool) -> sw_logger.JSONLogger or sw_logger.StdoutLogger:
     """ Create a logger object
-
     Returns:
         Logging object for outputting results
     """
 
-    return logger.StdoutLogger()
-
-
-def parse_tombstone_text(filepath: str) -> str or None:
-    """ Use a custom tombstone notification from a txt file
-
-    Args:
-        filepath: Path to txt file containing custom tombstone text
-    Returns:
-        String containing contents of the txt file, or None to use the default
-    """
-
-    try:
-        with open(filepath, encoding='utf8') as f:
-            contents = f.read()
-            return contents
-    except:
-        return None
+    if not logging_type or logging_type == 'terminal':
+        return sw_logger.StdoutLogger(debug=debug)
+    else:
+        return sw_logger.JSONLogger(debug=debug)
 
 
 def main():
-    global OUTPUT_LOGGER, TOMBSTONE_CONTENT
+    global OUTPUT_LOGGER
     try:
-        OUTPUT_LOGGER = init_logger()
+        OUTPUT_LOGGER = ''
         parser = argparse.ArgumentParser(description=__version__.__summary__)
 
-        parser.add_argument('--hours', dest='hours', type=int,
+        parser.add_argument('--hours', '-hr', dest='hours', type=int,
                             help='How far back to search in whole hours between 1-24. Defaults to 1 if no acceptable '
                                  'value given', required=False)
-        parser.add_argument('--minutes', dest='minutes', type=int,
+        parser.add_argument('--minutes', '-m', dest='minutes', type=int,
                             help='How far back to search in whole minutes between 1-60', required=False)
-        parser.add_argument('--cores', dest='cores', type=int,
+        parser.add_argument('--output', '-o', choices=['json', 'terminal'], dest='logging_type',
+                            help='What logging output to use - JSON formatted output, or textual output'
+                                 'for reading via terminal. Default is terminal')
+        parser.add_argument('--cores', '-c', dest='cores', type=int,
                             help='Number of cores to use between 1-12', required=False)
-        parser.add_argument('--version', action='version',
+        parser.add_argument('--version', '-v', action='version',
                             version=f'Slack Watchman for Enterprise Grid: {__version__.__version__}')
-        parser.add_argument('--users', dest='users', action='store_true', help='Find all users')
-        parser.add_argument('--workspaces', dest='workspaces', action='store_true', help='Find all workspaces')
-        parser.add_argument('--sandbox', dest='sandbox', action='store_true', help='Search using only sandbox '
-                                                                                   'signatures')
-        parser.add_argument('--tombstone', dest='tombstone', action='store_true', help='Tombstone (REMOVE) all '
-                                                                                       'matching messages')
-        parser.add_argument('--tombstone-text-file', dest='tombstone_filepath', type=str,
-                            help='Path to file containing custom tombstone notification text (Optional)',
-                            required=False)
+        parser.add_argument('--users', '-u', dest='users', action='store_true', help='Return all users')
+        parser.add_argument('--workspaces', '-w', dest='workspaces', action='store_true', help='Return all workspaces')
+        parser.add_argument('--debug', '-d', dest='debug', action='store_true', help='Turn on debug level logging')
+        parser.add_argument('--verbose', '-V', dest='verbose', action='store_true',
+                            help='Turn on more verbose output for JSON logging. '
+                                 'This includes more fields, but is larger')
 
         args = parser.parse_args()
         hours = args.hours
         minutes = args.minutes
-        tombstone = args.tombstone
-        tombstone_filepath = args.tombstone_filepath
         cores = args.cores
         users = args.users
         workspaces = args.workspaces
-        sandbox = args.sandbox
+        logging_type = args.logging_type
+        debug = args.debug
+        verbose = args.verbose
 
         span = 0
-
+        OUTPUT_LOGGER = init_logger(logging_type, debug)
         if minutes:
             if isinstance(minutes, int) and 1 <= int(minutes) <= 60:
                 span = (int(minutes) * 60)
             else:
                 minutes = None
 
         if hours:
@@ -224,100 +198,100 @@
         if not minutes:
             minutes = 0
         if not hours:
             hours = 0
 
         cores = core_validation(cores)
 
-        slack_con = slack_wrapper.initiate_slack_connection()
-        OUTPUT_LOGGER.log_info('Slack Watchman Enterprise Grid started execution')
-        OUTPUT_LOGGER.log_info(f'Version: {__version__.__version__}')
-        OUTPUT_LOGGER.log_info(f'Created by: {__version__.__author__} - {__version__.__email__}')
-        OUTPUT_LOGGER.log_info(f'{cores} cores in use')
-        OUTPUT_LOGGER.log_info('Importing signatures...')
-        signature_list = load_signatures(sandbox)
-        OUTPUT_LOGGER.log_info(f'{len(signature_list)} signatures loaded')
-
-        if tombstone:
-            OUTPUT_LOGGER.log_info('Tombstone option selected. All files and messages that match signatures will be '
-                                   'removed and replaced with a notification')
-            if tombstone_filepath:
-                TOMBSTONE_CONTENT = parse_tombstone_text(tombstone_filepath)
-
-        OUTPUT_LOGGER.log_info(f'Searching previous {hours} hour(s), {minutes} minutes')
-        OUTPUT_LOGGER.log_info('Enumerating Enterprise information')
-        OUTPUT_LOGGER.log_notification(slack_wrapper.get_enterprise(slack_con), detect_type='Enterprise')
-        OUTPUT_LOGGER.log_info('Enumerating Enterprise workspaces')
-        workspace_list = slack_wrapper.get_workspaces(slack_con)
-        OUTPUT_LOGGER.log_info(f'{len(workspace_list)} workspaces discovered')
-        OUTPUT_LOGGER.log_info('Enumerating Enterprise users')
-        user_list = slack_wrapper.get_users(slack_con, workspace_list)
-        OUTPUT_LOGGER.log_info(f'{len(user_list)} users discovered')
+        slack_con = slack_wrapper.initiate_slack_connection(os.environ.get('SLACK_WATCHMAN_EG_TOKEN'))
+        OUTPUT_LOGGER.log('SUCCESS', 'Slack Watchman Enterprise Grid started execution')
+        OUTPUT_LOGGER.log('INFO', f'Version: {__version__.__version__}')
+        OUTPUT_LOGGER.log('INFO', f'Created by: {__version__.__author__} - {__version__.__email__}')
+        OUTPUT_LOGGER.log('INFO', f'{cores} cores in use')
+        OUTPUT_LOGGER.log('INFO', 'Downloading signature file updates')
+        signature_updater.SignatureUpdater(OUTPUT_LOGGER).update_signatures()
+        OUTPUT_LOGGER.log('INFO', 'Importing signatures...')
+        signature_list = load_signatures()
+        OUTPUT_LOGGER.log('SUCCESS', f'{len(signature_list)} signatures loaded')
+        OUTPUT_LOGGER.log('INFO', f'Searching previous {hours} hour(s), {minutes} minutes')
+        OUTPUT_LOGGER.log('INFO', 'Enumerating Enterprise information')
+        OUTPUT_LOGGER.log('NOTIFY', slack_wrapper.get_enterprise(slack_con), scope='Enterprise',
+                          notify_type='enterprise')
+        OUTPUT_LOGGER.log('INFO', 'Enumerating Enterprise workspaces')
+        workspace_list = slack_wrapper.get_workspaces(slack_con, verbose)
+        OUTPUT_LOGGER.log('INFO', f'{len(workspace_list)} workspaces discovered')
+        OUTPUT_LOGGER.log('INFO', 'Enumerating Enterprise users')
+        user_list = slack_wrapper.get_users(slack_con, workspace_list, verbose)
+        OUTPUT_LOGGER.log('INFO', f'{len(user_list)} users discovered')
 
         if users:
-            OUTPUT_LOGGER.log_info('Outputting Enterprise users')
+            OUTPUT_LOGGER.log('INFO', 'Outputting Enterprise users')
             for user in user_list:
-                OUTPUT_LOGGER.log_notification(user, detect_type='User')
+                OUTPUT_LOGGER.log('NOTIFY', user, detect_type='User', notify_type='user')
 
         if workspaces:
-            OUTPUT_LOGGER.log_info('Outputting Enterprise workspaces')
+            OUTPUT_LOGGER.log('INFO', 'Outputting Enterprise workspaces')
             for workspace in workspace_list:
-                OUTPUT_LOGGER.log_notification(workspace, detect_type='Workspace')
+                OUTPUT_LOGGER.log('NOTIFY', workspace, detect_type='Workspace', notify_type='workspace')
 
-        OUTPUT_LOGGER.log_info('Enumerating files')
-        file_list = slack_wrapper.get_all_files(slack_con, cores=cores, timeframe=tf)
-        OUTPUT_LOGGER.log_info(f'{len(file_list)} files discovered')
+        OUTPUT_LOGGER.log('INFO', 'Enumerating files')
+        file_list = slack_wrapper.get_all_files(slack_con, cores=cores, verbose=verbose, timeframe=tf)
+        OUTPUT_LOGGER.log('INFO', f'{len(file_list)} files discovered')
 
-        OUTPUT_LOGGER.log_info('Enumerating messages')
+        OUTPUT_LOGGER.log('INFO', 'Enumerating messages')
         message_list = slack_wrapper.get_all_messages(slack_con, cores=cores, timeframe=tf)
-        OUTPUT_LOGGER.log_info(f'{len(message_list)} messages discovered')
+        OUTPUT_LOGGER.log('INFO', f'{len(message_list)} messages discovered')
 
         for sig in signature_list:
             for scope in sig.scope:
                 search(
                     sig,
                     slack_con,
                     user_list,
                     message_list,
                     workspace_list,
                     file_list,
                     scope,
                     cores,
-                    tombstone
+                    verbose
                 )
 
-        OUTPUT_LOGGER.log_info('Enumerating draft messages')
+        OUTPUT_LOGGER.log('INFO', 'Enumerating draft messages')
         draft_list = slack_wrapper.get_all_drafts(
             slack_con,
             workspace_list,
             cores=cores,
+            verbose=verbose,
             timeframe=tf
         )
-        OUTPUT_LOGGER.log_info(f'{len(draft_list)} drafts discovered')
+        OUTPUT_LOGGER.log('INFO', f'{len(draft_list)} drafts discovered')
         for sig in signature_list:
             if 'drafts' in sig.scope:
-                OUTPUT_LOGGER.log_info(f'Searching for drafts containing {sig.meta.name}')
+                OUTPUT_LOGGER.log('INFO', f'Searching for drafts containing {sig.name}')
                 drafts = slack_wrapper.search_draft_matches(
                     slack_con,
                     sig,
                     draft_list,
                     user_list,
                     OUTPUT_LOGGER,
+                    verbose,
                     tf
                 )
                 if drafts:
                     for draft in drafts:
-                        OUTPUT_LOGGER.log_notification(
+                        OUTPUT_LOGGER.log(
+                            'NOTIFY',
                             draft,
                             scope='Draft',
-                            severity=sig.meta.severity,
-                            detect_type=sig.meta.name
+                            severity=sig.severity,
+                            detect_type=sig.name,
+                            notify_type='result'
                         )
 
-        OUTPUT_LOGGER.log_info('Slack Watchman Enterprise Grid finished execution')
+        OUTPUT_LOGGER.log('SUCCESS', 'Slack Watchman Enterprise Grid finished execution')
 
     except Exception as e:
-        OUTPUT_LOGGER.log_critical(e)
+        OUTPUT_LOGGER.log('CRITICAL', e)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `slack-watchman-eg-1.1.0/src/slack_watchman_eg/slack_objects/enterprise.py` & `slack-watchman-eg-2.0.0/src/slack_watchman_eg/models/enterprise.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,28 @@
 from dataclasses import dataclass
+from typing import Dict
 
 
-@dataclass
+@dataclass(slots=True)
 class Enterprise(object):
     """ Class that defines Enterprise objects. A Slack Enterprise
     is the top level organisation that contains workspaces"""
 
-    __slots__ = [
-        'id',
-        'name',
-        'domain',
-        'email_domain',
-        'is_verified',
-        'discoverable',
-        'pay_prod_cur',
-        'locale',
-        'url'
-    ]
-
     id: str
     name: str
     domain: str
     email_domain: str
     is_verified: bool
     discoverable: bool
     pay_prod_cur: str
     locale: str
     url: str
 
 
-def create_from_dict(enterprise_dict: dict) -> Enterprise:
+def create_from_dict(enterprise_dict: Dict) -> Enterprise:
     """ Create an Enterprise object from a dict response from the Slack API
 
     Args:
         enterprise_dict: dict/JSON format data from Slack API
     Returns:
         A new Enterprise object
     """
```

### Comparing `slack-watchman-eg-1.1.0/src/slack_watchman_eg/slack_objects/post.py` & `slack-watchman-eg-2.0.0/src/slack_watchman_eg/models/post.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import time
 from dataclasses import dataclass
+from typing import List, Dict
+
+from . import conversation
 
 
 def _convert_timestamp(timestamp: str or int) -> str or None:
-    """ Converts epoch timestamp into human readable time
+    """ Converts epoch timestamp into human-readable time
 
     Args:
         timestamp: epoch timestamp in seconds
     Returns:
         String time in the format YYYY-mm-dd hh:mm:ss
     """
 
@@ -16,15 +19,15 @@
             timestamp = timestamp.split('.', 1)[0]
 
         return time.strftime('%Y-%m-%d %H:%M:%S', time.localtime(int(timestamp)))
     else:
         return None
 
 
-@dataclass
+@dataclass(slots=True)
 class Post(object):
     """ Parent that defines Post objects. A Slack
     post can be a:
         - Message
         - Draft
         - File
     """
@@ -32,84 +35,108 @@
     id: str
     team: str
     created: int or float or str
     client_msg_id: str
     user: str
 
 
-@dataclass
+@dataclass(slots=True)
 class File(Post):
     name: str
     title: str
     mimetype: str
     filetype: str
     pretty_type: str
     editable: bool
     size: int or float
     mode: str
     is_public: bool
     public_url_shared: bool
     url_private: str
     url_private_download: str
-    shares: list
+    shares: List
 
 
-@dataclass
+@dataclass(slots=True)
 class Message(Post):
     text: str
     type: str
-    blocks: list
-    timestamp: float
-    conversation: dataclass
+    blocks: List[Dict]
+    timestamp: int or float or str
+    conversation: conversation.Conversation or conversation.ConversationSuccinct
 
 
-@dataclass
+@dataclass(slots=True)
 class Draft(Post):
     last_updated_ts: str
     last_updated_client: str
-    blocks: list
-    file_ids: list
+    blocks: List[Dict]
+    file_ids: List[str]
     is_from_composer: bool
     is_deleted: bool
     is_sent: bool
-    destinations: list
-    attachments: list
+    destinations: List[Dict]
+    attachments: List[Dict]
     date_scheduled: int or float
 
 
-def create_draft_from_dict(draft_dict: dict) -> Draft:
+@dataclass(slots=True)
+class DraftSuccinct(Post):
+    last_updated_ts: str
+    last_updated_client: str
+    blocks: List[Dict]
+    destinations: List[Dict]
+    attachments: List[Dict]
+
+
+def create_draft_from_dict(draft_dict: Dict, verbose: bool) -> Draft or DraftSuccinct:
     """ Create a Draft post object from a dict containing JSON data from
     the Slack API
 
     Args:
         draft_dict: dict containing post information from the Slack API
+        verbose: Whether to use verbose logging or not
     Returns:
         Draft object for the post
     """
 
-    return Draft(
-        id=draft_dict.get('id'),
-        team=draft_dict.get('team_id'),
-        created=draft_dict.get('date_created'),
-        client_msg_id=draft_dict.get('client_msg_id'),
-        user=draft_dict.get('user_id'),
-        last_updated_ts=_convert_timestamp(draft_dict.get('last_updated_ts')),
-        last_updated_client=draft_dict.get('last_updated_client'),
-        blocks=draft_dict.get('blocks'),
-        file_ids=draft_dict.get('file_ids'),
-        is_from_composer=draft_dict.get('is_from_composer'),
-        is_deleted=draft_dict.get('is_deleted'),
-        is_sent=draft_dict.get('is_sent'),
-        destinations=[i.get('channel_id') for i in draft_dict.get('destinations')],
-        attachments=draft_dict.get('attachments'),
-        date_scheduled=_convert_timestamp(draft_dict.get('date_scheduled'))
-    )
+    if verbose:
+        return Draft(
+            id=draft_dict.get('id'),
+            team=draft_dict.get('team_id'),
+            created=draft_dict.get('date_created'),
+            client_msg_id=draft_dict.get('client_msg_id'),
+            user=draft_dict.get('user_id'),
+            last_updated_ts=_convert_timestamp(draft_dict.get('last_updated_ts')),
+            last_updated_client=draft_dict.get('last_updated_client'),
+            blocks=draft_dict.get('blocks'),
+            file_ids=draft_dict.get('file_ids'),
+            is_from_composer=draft_dict.get('is_from_composer'),
+            is_deleted=draft_dict.get('is_deleted'),
+            is_sent=draft_dict.get('is_sent'),
+            destinations=[i.get('channel_id') for i in draft_dict.get('destinations')],
+            attachments=draft_dict.get('attachments'),
+            date_scheduled=_convert_timestamp(draft_dict.get('date_scheduled'))
+        )
+    else:
+        return DraftSuccinct(
+            id=draft_dict.get('id'),
+            team=draft_dict.get('team_id'),
+            created=draft_dict.get('date_created'),
+            client_msg_id=draft_dict.get('client_msg_id'),
+            user=draft_dict.get('user_id'),
+            last_updated_ts=_convert_timestamp(draft_dict.get('last_updated_ts')),
+            last_updated_client=draft_dict.get('last_updated_client'),
+            blocks=draft_dict.get('blocks'),
+            destinations=[i.get('channel_id') for i in draft_dict.get('destinations')],
+            attachments=draft_dict.get('attachments'),
+        )
 
 
-def create_message_from_dict(message_dict: dict) -> Message:
+def create_message_from_dict(message_dict: Dict) -> Message:
     """ Create a Message post object from a dict containing JSON data from
     the Slack API
 
     Args:
         message_dict: dict containing post information from the Slack API
     Returns:
         Message object for the post
@@ -125,15 +152,15 @@
         user=message_dict.get('user'),
         text=message_dict.get('text'),
         type=message_dict.get('type'),
         blocks=message_dict.get('blocks'),
     )
 
 
-def create_file_from_dict(file_dict: dict) -> File:
+def create_file_from_dict(file_dict: Dict) -> File:
     """ Create a File post object from a dict containing JSON data from
     the Slack API
 
     Args:
         file_dict: dict containing post information from the Slack API
     Returns:
         File object for the post
```

### Comparing `slack-watchman-eg-1.1.0/src/slack_watchman_eg/slack_objects/user.py` & `slack-watchman-eg-2.0.0/src/slack_watchman_eg/models/user.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import time
 from dataclasses import dataclass
+from typing import Dict, List
 
 from . import workspace
 
 
 def _convert_timestamp(timestamp: str or int) -> str or None:
-    """ Converts epoch timestamp into human readable time
+    """ Converts epoch timestamp into human-readable time
 
     Args:
         timestamp: epoch timestamp in seconds
     Returns:
         String time in the format YYYY-mm-dd hh:mm:ss
     """
 
@@ -18,66 +19,31 @@
             timestamp = timestamp.split('.', 1)[0]
 
         return time.strftime('%Y-%m-%d %H:%M:%S', time.localtime(int(timestamp)))
     else:
         return None
 
 
-@dataclass
+@dataclass(slots=True)
 class User(object):
     """ Class that defines User objects for Slack users"""
 
-    __slots__ = [
-        'id',
-        'name',
-        'deleted',
-        'color',
-        'real_name',
-        'first_name',
-        'last_name',
-        'title',
-        'phone',
-        'skype',
-        'display_name',
-        'fields',
-        'email',
-        'api_app_id',
-        'always_active',
-        'bot_id',
-        'enterprise',
-        'tz',
-        'tz_label',
-        'tz_offset',
-        'is_admin',
-        'is_owner',
-        'is_primary_owner',
-        'is_restricted',
-        'is_ultra_restricted',
-        'is_bot',
-        'is_app_user',
-        'updated',
-        'is_email_confirmed',
-        'who_can_share_contact_card',
-        'is_workflow_bot',
-        'workspaces'
-    ]
-
     id: str
     name: str
     email: str
     title: str
     deleted: bool
     color: str
     real_name: str
     first_name: str
     last_name: str
     phone: str
     skype: str
     display_name: str
-    fields: dict
+    fields: Dict
     api_app_id: str
     always_active: bool
     bot_id: str
     enterprise: str
     tz: str
     tz_label: str
     tz_offset: str
@@ -88,54 +54,94 @@
     is_ultra_restricted: bool
     is_bot: bool
     is_app_user: bool
     updated: int or float or str
     is_email_confirmed: bool
     who_can_share_contact_card: str
     is_workflow_bot: bool
-    workspaces: [workspace.Workspace]
+    workspaces: List[workspace.Workspace]
+
 
+@dataclass(slots=True)
+class UserSuccinct(object):
+    """ Class that defines User objects for Slack users"""
 
-def create_from_dict(user_dict: dict, workspaces: list) -> User:
+    id: str
+    name: str
+    email: str
+    title: str
+    deleted: bool
+    real_name: str
+    first_name: str
+    last_name: str
+    is_admin: bool
+    is_owner: bool
+    is_bot: bool
+    is_app_user: bool
+    is_workflow_bot: bool
+
+
+def create_from_dict(user_dict: Dict,
+                     workspaces: List[workspace.Workspace],
+                     verbose: bool) -> User or UserSuccinct:
     """ Create a User object from a dict response from the Slack API
 
     Args:
+        verbose: Whether to output a full User object, or use
+            less verbose succinct class
         user_dict: dict/JSON format data from Slack API
         workspaces: list of Workspace objects
     Returns:
         A new User object
     """
 
-    return User(
-        id=user_dict.get('id'),
-        name=user_dict.get('name'),
-        deleted=user_dict.get('deleted'),
-        color=user_dict.get('colour'),
-        real_name=user_dict.get('real_name'),
-        tz=user_dict.get('tz'),
-        tz_label=user_dict.get('tz_label'),
-        tz_offset=user_dict.get('tz_offset'),
-        title=user_dict.get('profile').get('title'),
-        phone=user_dict.get('profile').get('phone'),
-        skype=user_dict.get('profile').get('skype'),
-        display_name=user_dict.get('profile').get('display_name'),
-        fields=user_dict.get('profile').get('fields'),
-        email=user_dict.get('profile').get('email'),
-        api_app_id=user_dict.get('profile').get('api_app_id'),
-        always_active=user_dict.get('profile').get('always_active'),
-        bot_id=user_dict.get('profile').get('bot_id'),
-        first_name=user_dict.get('profile').get('first_name'),
-        last_name=user_dict.get('profile').get('last_name'),
-        enterprise=user_dict.get('profile').get('enterprise'),
-        is_admin=user_dict.get('is_admin'),
-        is_owner=user_dict.get('is_owner'),
-        is_primary_owner=user_dict.get('is_primary_owner'),
-        is_restricted=user_dict.get('is_restricted'),
-        is_ultra_restricted=user_dict.get('is_ultra_restricted'),
-        is_bot=user_dict.get('is_bot'),
-        is_app_user=user_dict.get('is_app_user'),
-        updated=_convert_timestamp(user_dict.get('updated')),
-        is_email_confirmed=user_dict.get('is_email_confirmed'),
-        who_can_share_contact_card=user_dict.get('who_can_share_contact_card'),
-        is_workflow_bot=user_dict.get('is_workflow_bot'),
-        workspaces=workspaces
-    )
+    if verbose:
+        return User(
+            id=user_dict.get('id'),
+            name=user_dict.get('name'),
+            deleted=user_dict.get('deleted'),
+            color=user_dict.get('colour'),
+            real_name=user_dict.get('real_name'),
+            tz=user_dict.get('tz'),
+            tz_label=user_dict.get('tz_label'),
+            tz_offset=user_dict.get('tz_offset'),
+            title=user_dict.get('profile').get('title'),
+            phone=user_dict.get('profile').get('phone'),
+            skype=user_dict.get('profile').get('skype'),
+            display_name=user_dict.get('profile').get('display_name'),
+            fields=user_dict.get('profile').get('fields'),
+            email=user_dict.get('profile').get('email'),
+            api_app_id=user_dict.get('profile').get('api_app_id'),
+            always_active=user_dict.get('profile').get('always_active'),
+            bot_id=user_dict.get('profile').get('bot_id'),
+            first_name=user_dict.get('profile').get('first_name'),
+            last_name=user_dict.get('profile').get('last_name'),
+            enterprise=user_dict.get('profile').get('enterprise'),
+            is_admin=user_dict.get('is_admin'),
+            is_owner=user_dict.get('is_owner'),
+            is_primary_owner=user_dict.get('is_primary_owner'),
+            is_restricted=user_dict.get('is_restricted'),
+            is_ultra_restricted=user_dict.get('is_ultra_restricted'),
+            is_bot=user_dict.get('is_bot'),
+            is_app_user=user_dict.get('is_app_user'),
+            updated=_convert_timestamp(user_dict.get('updated')),
+            is_email_confirmed=user_dict.get('is_email_confirmed'),
+            who_can_share_contact_card=user_dict.get('who_can_share_contact_card'),
+            is_workflow_bot=user_dict.get('is_workflow_bot'),
+            workspaces=workspaces
+        )
+    else:
+        return UserSuccinct(
+            id=user_dict.get('id'),
+            name=user_dict.get('name'),
+            deleted=user_dict.get('deleted'),
+            real_name=user_dict.get('real_name'),
+            title=user_dict.get('profile').get('title'),
+            email=user_dict.get('profile').get('email'),
+            first_name=user_dict.get('profile').get('first_name'),
+            last_name=user_dict.get('profile').get('last_name'),
+            is_admin=user_dict.get('is_admin'),
+            is_owner=user_dict.get('is_owner'),
+            is_bot=user_dict.get('is_bot'),
+            is_app_user=user_dict.get('is_app_user'),
+            is_workflow_bot=user_dict.get('is_workflow_bot'),
+        )
```

### Comparing `slack-watchman-eg-1.1.0/src/slack_watchman_eg/slack_wrapper.py` & `slack-watchman-eg-2.0.0/src/slack_watchman_eg/slack_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,126 +1,135 @@
 import dataclasses
 import json
 import multiprocessing
 import numpy
-import os
 import re
 import requests
 import time
 import calendar
-from requests.packages.urllib3.util import Retry
+from urllib3.util import Retry
 from requests.adapters import HTTPAdapter
+from typing import List, Dict
 
-from . import signature
-from . import logger
-from .slack_objects import workspace
-from .slack_objects import user
-from .slack_objects import enterprise
-from .slack_objects import conversation
-from .slack_objects import post
+from . import sw_logger
+from .models import (
+    signature,
+    user,
+    workspace,
+    post,
+    conversation,
+    enterprise
+)
 
 # Default timeframe of 1 hour
 DEFAULT_TIMEFRAME = calendar.timegm(time.gmtime()) - 3600
+DEFAULT_TIMEOUT = 5
 
 
 class ScopeError(Exception):
     pass
 
 
 class SlackAPIError(Exception):
     pass
 
 
 class SlackAPI(object):
 
-    def __init__(self, token):
+    def __init__(self, token: str):
         self.token = token
         self.base_url = 'https://slack.com/api'
         self.limit = '1000'
         self.session = session = requests.session()
-        session.mount(self.base_url, HTTPAdapter(max_retries=Retry(connect=3, backoff_factor=1)))
+        session.mount(
+            self.base_url,
+            HTTPAdapter(max_retries=Retry(total=5, backoff_factor=0.2)))
         session.headers.update({
             'Connection': 'keep-alive, close',
             'Authorization': f'Bearer {self.token}',
             'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_5) AppleWebKit/537.36 (KHTML, like Gecko) '
                           'Cafari/537.36 '
         })
         session.params['limit'] = self.limit
 
     def _pagination_loop(self,
                          response: requests.Response,
                          pagination: str,
                          method: str,
                          relative_url: str,
-                         params: dict,
-                         data: dict,
-                         verify_ssl: bool) -> list:
+                         params: Dict,
+                         data: Dict,
+                         verify_ssl: bool) -> List:
 
         results = []
 
         if pagination == 'offset' and response.json().get('offset'):
             while response.json().get('offset'):
                 response = self.session.request(
                     method,
                     relative_url,
                     params=params,
                     data=data,
-                    verify=verify_ssl
+                    verify=verify_ssl,
+                    timeout=5
                 )
 
                 params.update({
                     'offset': response.json().get('offset')
                 })
                 results.append(response.json())
         elif pagination == 'latest' and response.json().get('offset'):
             while response.json().get('offset'):
                 response = self.session.request(
                     method,
                     relative_url,
                     params=params,
                     data=data,
-                    verify=verify_ssl
+                    verify=verify_ssl,
+                    timeout=5
                 )
 
                 params.update({
                     'latest': response.json().get('offset')
                 })
                 results.append(response.json())
         else:
             results.append(response.json())
 
         return results
 
     def _make_request(self,
-                      url,
-                      params=None,
-                      data=None,
-                      method='GET',
-                      verify_ssl=True,
-                      pagination=None):
+                      url: str,
+                      params: Dict = None,
+                      data: Dict = None,
+                      method: str = 'GET',
+                      verify_ssl: bool = True,
+                      pagination: str = None) -> List:
         try:
             relative_url = '/'.join((self.base_url, url))
             response = self.session.request(
                 method,
                 relative_url,
                 params=params,
                 data=data,
-                verify=verify_ssl
+                verify=verify_ssl,
+                timeout=5
             )
 
             if not response.json().get('ok') and response.json().get('error') == 'missing_scope':
                 raise ScopeError()
             elif not response.json().get('ok') and response.json().get('error') == 'channel_not_found':
                 params['team'] = ''
                 response = self.session.request(
                     method='GET',
                     url=relative_url,
                     params=params,
                     data=data,
-                    verify=verify_ssl
+                    verify=verify_ssl,
+                    timeout=5
                 )
                 return self._pagination_loop(
                     response,
                     pagination,
                     method,
                     relative_url,
                     params,
@@ -156,39 +165,39 @@
         except ScopeError:
             raise ScopeError(f"Missing required scope: {response.json().get('needed')}")
         except SlackAPIError:
             raise SlackAPIError(f"Slack API Error: {response.json().get('error')}")
         except Exception as e:
             raise Exception(e)
 
-    def get_enterprise_info(self) -> dict:
+    def get_enterprise_info(self) -> Dict:
         """ Return all information for the Enterprise Grid
 
         Returns:
             JSON object containing information on the Slack Enterprise Grid
         """
 
         return self._make_request('discovery.enterprise.info')[0].get('enterprise')
 
-    def get_all_users(self, offset: str = None) -> [dict]:
+    def get_all_users(self, offset: str = None) -> List[Dict]:
         """ Get all users in a Grid
 
         Returns:
             All users in a Grid, plus Workspaces they are assigned to
         """
 
         params = {
             'offset': offset
         }
 
         users = self._make_request('discovery.users.list', params=params, pagination='offset')
 
         return _format_results(users, 'users')
 
-    def get_user_info(self, user_id: str) -> dict:
+    def get_user_info(self, user_id: str) -> Dict:
         """ Get information from one user in the Grid
 
         Returns:
             User information for a single user
         """
 
         params = {
@@ -199,15 +208,15 @@
 
     def get_user_conversations(self,
                                user_id: str,
                                public: bool = None,
                                private: bool = None,
                                im: bool = None,
                                mpim: bool = None,
-                               historical: bool = None) -> [dict]:
+                               historical: bool = None) -> List[Dict]:
         """ return all conversations a user is involved in
 
         Args:
             historical: Whether to search for
                 channels that the user is not currently a member of, but has been in the past
             mpim: Whether to look at multi-person instant messages
             im: Whether to look at instant messages
@@ -233,15 +242,15 @@
 
     def get_all_conversations(self,
                               public: bool = None,
                               private: bool = None,
                               im: bool = None,
                               mpim: bool = None,
                               ext_shared: bool = None,
-                              historical: bool = None) -> [dict]:
+                              historical: bool = None) -> List[Dict]:
         """ return all conversations in a Grid
 
         Args:
             ext_shared: Whether to look for only external shared channels
             historical: Whether to search for
                 channels that the user is not currently a member of, but has been in the past
             mpim: Whether to look at multi-person instant messages
@@ -261,15 +270,15 @@
             'include_historical': historical
         }
 
         conversations = self._make_request('discovery.conversations.list', params=params, pagination='offset')
 
         return _format_results(conversations, 'channels')
 
-    def get_recent_conversations(self, latest: float = None) -> [dict]:
+    def get_recent_conversations(self, latest: float = None) -> List[Dict]:
         """
         Args:
             latest: Timestamp within the last 24 hours to shorten or lengthen the requested timespan.
                 This method can return up to 7 days worth of data (prior to the current timestamp).
                 If this parameter is not included, this endpoint will return data from the last 24 hours.
         Returns:
             JSON containing recent conversations created
@@ -283,15 +292,15 @@
 
         return _format_results(conversations, 'channels')
 
     def get_conversation_history(self,
                                  channel_id: str,
                                  team_id: str = None,
                                  latest: float = None,
-                                 oldest: float = None) -> [dict]:
+                                 oldest: float = None) -> List[Dict]:
         """ Retrieves the history of the channel-object. This can be thought of as
          the state of the conversation in the client: it’s what the users are seeing.
 
         Args:
             team_id: ID for the team the channel is in
             channel_id: ID for the channel to return
             latest: The newest date to retrieve messages from
@@ -311,15 +320,15 @@
 
         return _format_results(conversations, 'messages')
 
     def get_conversation_edits(self,
                                channel_id: str,
                                team_id: str,
                                latest: float = None,
-                               oldest: float = None) -> [dict]:
+                               oldest: float = None) -> List[Dict]:
         """ Returns edit and delete records of messages
 
         Args:
             team_id: ID for the team to search in
             channel_id: ID for the channel to return
             latest: The newest date to retrieve messages from
             oldest: The oldest date to retrieve messages from
@@ -337,15 +346,15 @@
 
         conversations = self._make_request('discovery.conversations.edits', params=params, pagination='latest')
 
         return _format_results(conversations, 'edits')
 
     def get_conversation_info(self,
                               channel_id: str,
-                              team_id: str = None) -> [dict]:
+                              team_id: str = None) -> List[Dict]:
         """ Provides a comprehensive overview of a single channel outside of its message history
 
         Args:
             team_id: ID of the team the channel is in
             channel_id: ID of the channel to return
         Returns:
             JSON object with channel information
@@ -357,15 +366,15 @@
         }
 
         return self._make_request('discovery.conversations.info', params=params)[0].get('info')
 
     def get_conversation_members(self,
                                  channel_id: str,
                                  team_id: str = None,
-                                 include_member_left: bool = None) -> [dict]:
+                                 include_member_left: bool = None) -> List[Dict]:
         """ Provides a list of everyone in a given channel, private channel, MDPM or DM
 
         Args:
             team_id: ID of the team the channel is in
             include_member_left: Whether to include members who have left the channel
             channel_id: ID of the channel to get members for
         Returns:
@@ -381,15 +390,15 @@
         conversations = self._make_request('discovery.conversations.members', params=params, pagination='offset')
 
         return _format_results(conversations, 'members')
 
     def get_conversation_renames(self,
                                  latest: float = None,
                                  oldest: float = None,
-                                 private: bool = None) -> [dict]:
+                                 private: bool = None) -> List[Dict]:
         """ Get all channel renames that have occurred in an organisation
 
         Args:
             latest: Newest date (timestamp) of renames to include
             oldest: Oldest date (timestamp) of renames to include
             private: Setting this value to true will return only private channels.
              The default (or a false value) will include only public channels.
@@ -407,15 +416,15 @@
 
         return _format_results(conversations, 'renames')
 
     def search_conversations(self,
                              query: str,
                              include_messages: bool = None,
                              latest: float = None,
-                             oldest: float = None) -> [dict]:
+                             oldest: float = None) -> List[Dict]:
         """ Find channels and messages within an instance that contain the provided search term.
 
         Args:
             query: Term or keyword to search conversation messages for.
             include_messages: By default, messages are not included in the response.
                 To include both messages and channel information, pass include_messages with a true value.
             latest: Newest date (timestamp) of messages to include.
@@ -558,15 +567,15 @@
         }
 
         return self._make_request('discovery.chat.restore', method='POST', params=params)[0]
 
     def list_drafts(self,
                     team_id: str,
                     oldest: int = None,
-                    latest: int = None) -> [dict]:
+                    latest: int = None) -> List[Dict]:
         """
 
         Args:
             team_id: Team ID of the workspace the draft was created within.
             oldest: Start of time range of messages to include in results.
             latest: End of time range of messages to include in results.
         Returns:
@@ -609,15 +618,15 @@
             'oldest': oldest
         }
 
         return self._make_request('discovery.draft.info', params=params)[0].get('draft')
 
     def list_files(self,
                    oldest: int or str = None,
-                   latest: int or str = None) -> [dict]:
+                   latest: int or str = None) -> List[Dict]:
         """ Returns files uploaded within a specified timeframe.
 
         Args:
             oldest: Start of time range of messages to include in results.
             latest: End of time range of messages to include in results.
         Returns:
             JSON object containing file data
@@ -713,15 +722,15 @@
         params = {
             'team': team_id
         }
 
         return self._make_request('team.info', params=params)[0].get('team')
 
 
-def _format_results(results_list: list, identifier: str) -> [dict]:
+def _format_results(results_list: list, identifier: str) -> List[Dict]:
     """ Format a JSON result from the Slack API. Results come in the format below:
     {
         "ok": true,
         "offset": "T2B5NCQZO",
         "info": [{
             "id": "...",
             "name": "...",
@@ -787,15 +796,15 @@
 
     if isinstance(timestamp, str):
         timestamp = timestamp.split('.', 1)[0]
 
     return time.strftime('%Y-%m-%d %H:%M:%S', time.localtime(int(timestamp)))
 
 
-def _deduplicate(input_list: list) -> [dict]:
+def _deduplicate(input_list: list) -> List[Dict]:
     """ Removes duplicates where results are returned by multiple queries
     Nested class handles JSON encoding for dataclass objects
 
     Args:
         input_list: List of dataclass objects
     Returns:
         List of JSON objects with duplicates removed
@@ -808,108 +817,111 @@
             return super().default(o)
 
     json_set = {json.dumps(dictionary, sort_keys=True, cls=EnhancedJSONEncoder) for dictionary in input_list}
 
     return [json.loads(t) for t in json_set]
 
 
-def initiate_slack_connection():
+def initiate_slack_connection(token: str) -> SlackAPI:
     """ Create a Slack API object to use for interacting with the Slack API
     First tries to get the API token from the environment variable:
         SLACK_WATCHMAN_EG_TOKEN
     Failing this, looks for it in the config file:
         watchman.conf
 
     Returns:
         Slack API object
     """
 
     try:
-        token = os.environ['SLACK_WATCHMAN_EG_TOKEN']
+        return SlackAPI(token)
     except Exception as e:
         raise e
 
-    return SlackAPI(token)
-
 
 def get_enterprise(slack_connection: SlackAPI) -> enterprise.Enterprise:
     """ Get information on the Slack Enterprise
 
     Args:
         slack_connection: Slack API connection object
     Returns:
         Enterprise object containing details about the Slack Enterprise
     """
     enterprise_info = slack_connection.get_enterprise_info()
 
     return enterprise.create_from_dict(slack_connection.get_team_info(enterprise_info.get('id')))
 
 
-def get_workspaces(slack_connection: SlackAPI) -> [workspace.Workspace]:
+def get_workspaces(slack_connection: SlackAPI, verbose: bool) -> List[workspace.Workspace]:
     """ Get all workspaces in the Slack environment
 
     Args:
         slack_connection: Slack API connection object
+        verbose: Whether to use verbose logging or not
     Returns:
         List containing Workspace objects for all Slack Workspaces
     """
 
     enterprise_info = slack_connection.get_enterprise_info()
 
-    return [workspace.create_from_dict(wrk) for wrk in enterprise_info.get('teams')]
+    return [workspace.create_from_dict(wrk, verbose) for wrk in enterprise_info.get('teams')]
 
 
 def get_users(slack_connection: SlackAPI,
-              workspaces_list: [workspace.Workspace]) -> [user.User]:
+              workspaces_list: List[workspace.Workspace],
+              verbose: bool) -> List[user.User]:
     """ Find all users in the Enterprise
 
     Args:
         workspaces_list: List of Slack Workspaces
         slack_connection: Slack API object
+        verbose: Whether to use verbose logging or not
     Returns:
         List of Slack User objects for all users in the enterprise
     """
 
     all_users = slack_connection.get_all_users()
     results = []
 
     for user_info in all_users:
         wk = []
         for w in workspaces_list:
             workspace = next((item for item in workspaces_list if item.id == w.id))
             wk.append(workspace)
 
-        results.append(user.create_from_dict(user_info, workspaces_list))
+        results.append(user.create_from_dict(user_info, workspaces_list, verbose))
 
     return results
 
 
 def get_conversations(slack_connection: SlackAPI,
-                      timeframe: int = DEFAULT_TIMEFRAME) -> [conversation.Conversation]:
+                      verbose: bool,
+                      timeframe: int = DEFAULT_TIMEFRAME) -> List[conversation.Conversation]:
     """ Gets all conversations created in a given timeframe, returns a list of
     Conversation objects
 
     Args:
         timeframe: timeframe to search in
         slack_connection: Slack API object
+        verbose: Whether to use verbose logging or not
     Returns:
         List of Conversation objects that have been created in the given timeframe
     """
 
     all_conversations = slack_connection.get_all_conversations()
     results = []
     for conv in all_conversations:
         if conv.get('created') >= timeframe:
             shared = []
             conv_info = slack_connection.get_conversation_info(conv.get('id'))[0]
             if conv_info.get('shared'):
                 for wrk in conv.get('shared').get('shared_team_ids'):
-                    shared.append(workspace.create_from_dict(slack_connection.get_team_info(wrk)))
+                    shared.append(workspace.create_from_dict(slack_connection.get_team_info(wrk), verbose))
             conv_info['shared'] = shared
-            results.append(conversation.create_from_dict(conv_info))
+            results.append(conversation.create_from_dict(conv_info, verbose))
 
     return results
 
 
 def tombstone_file(slack_connection: SlackAPI,
                    file: dict,
                    content: str = None):
@@ -947,31 +959,33 @@
         )
     except Exception as e:
         raise e
 
 
 def search_message_matches(sig: signature.Signature,
                            slack_connection: SlackAPI,
-                           users_list: [user.User],
-                           message_list: [post.Message],
-                           workspaces_list: [workspace.Workspace],
+                           users_list: List[user.User],
+                           message_list: List[post.Message],
+                           workspaces_list: List[workspace.Workspace],
                            cores: int,
-                           log: logger.StdoutLogger) -> [dict]:
+                           logger: sw_logger.JSONLogger,
+                           verbose: bool) -> List[Dict]:
     """ Use the search API to find messages posted in a certain timeframe
     matching search terms in the signature file. These are then compared against a regex
     to assess whether they contain sensitive data matching the signature.
 
     Args:
         slack_connection: Slack API object
         message_list: List of Message objects to search through
         sig: Signature object defining what to search for
         users_list: List of User objects
         workspaces_list: List of Workspace objects
         cores: number of cores to use
-        log: Logging object for output
+        logger: Logging object
+        verbose: Whether to use verbose logging or not
     Returns:
         List of Message objects containing post data
     """
 
     try:
         results = multiprocessing.Manager().list()
         list_of_chunks = numpy.array_split(numpy.array(message_list), cores)
@@ -983,47 +997,47 @@
                 target=_mp_find_messages_worker,
                 args=(
                     sig,
                     slack_connection,
                     users_list,
                     message_list,
                     workspaces_list,
-                    results
+                    results,
+                    verbose
                 )
             )
             processes.append(p)
             p.start()
 
         for process in processes:
             process.join()
 
         if results:
             results = _deduplicate(results)
-            log.log_info(f'{len(results)} total matches found after filtering')
+            logger.log('INFO', f'{len(results)} total matches found after filtering')
             return results
         else:
-            log.log_info('No matches found after filtering')
+            logger.log('INFO', 'No matches found after filtering')
     except Exception as e:
-        log.log_critical(e)
+        logger.log('CRITICAL', e)
 
 
 def search_file_matches(sig: signature.Signature,
-                        users_list: [user.User],
-                        files_list: [post.File],
+                        users_list: List[user.User],
+                        files_list: List[post.File],
                         cores: int,
-                        log: logger.StdoutLogger) -> [dict]:
+                        logger: sw_logger.JSONLogger) -> List[Dict]:
     """ Use the search API to find files posted in a certain timeframe
     matching search terms in the signature file.
 
     Args:
         files_list:
         sig: Signature object defining what to search for
         users_list: List of User objects
         cores: Number of cores to use
-        log: Logging object for output
     Returns:
         List of Message objects containing post data
     """
 
     try:
         results = multiprocessing.Manager().list()
         list_of_chunks = numpy.array_split(numpy.array(files_list), cores)
@@ -1044,39 +1058,41 @@
             p.start()
 
         for process in processes:
             process.join()
 
         if results:
             results = _deduplicate(results)
-            log.log_info(f'{len(results)} total matches found after filtering')
+            logger.log('INFO', f'{len(results)} total matches found after filtering')
             return results
         else:
-            log.log_info('No matches found after filtering')
+            logger.log('INFO', 'No matches found after filtering')
     except Exception as e:
-        log.log_critical(e)
+        logger.log('CRITICAL', e)
 
 
 def search_draft_matches(slack_connection: SlackAPI,
                          sig: signature.Signature,
-                         drafts_list: [post.Draft],
-                         users_list: [user.User],
-                         log: logger.StdoutLogger,
-                         timeframe: int = DEFAULT_TIMEFRAME) -> [dict]:
+                         drafts_list: List[post.Draft],
+                         users_list: List[user.User],
+                         logger: sw_logger.JSONLogger,
+                         verbose: bool,
+                         timeframe: int = DEFAULT_TIMEFRAME) -> List[Dict]:
     """ Find drafts posted in a certain timeframe
     matching search terms in the signature file. These are then compared against a regex
     to assess whether they contain sensitive data matching the signature.
 
     Args:
+        logger: Logging object
         slack_connection: Slack API object
         sig: Signature object defining what to search for
         users_list: List of User objects
         drafts_list: List of Draft objects
-        log: Logging object for output
         timeframe: How far back to search for drafts
+        verbose: Whether to use verbose logging or not
     Returns:
         List of Drafts objects containing post data
     """
 
     results = []
     try:
         for draft in drafts_list:
@@ -1088,77 +1104,61 @@
             if draft.blocks and draft.created >= timeframe:
                 for block_list in draft.blocks:
                     if block_list.get('type') == 'rich_text':
                         for element in block_list.get('elements'):
                             element_sub_list = element.get('elements')
                             for esl in element_sub_list:
                                 if esl.get('type') == 'text':
-                                    r = re.compile(sig.pattern)
-                                    if sig.search_strings:
-                                        for search_string in sig.search_strings:
-                                            if str(search_string.lower()) in esl.get('text').lower():
-                                                if r.search(esl.get('text')):
-                                                    draft_user = next((item for item in users_list if
-                                                                       item.id == draft.user), None)
-                                                    team_id = draft.team
-                                                    team = slack_connection.get_team_info(team_id)
-                                                    channel_id = draft.destinations[0]
-                                                    if channel_id.startswith('D'):
-                                                        team_id = get_enterprise(slack_connection).id
-
-                                                    conv_info = slack_connection.get_conversation_info(
-                                                        channel_id, team_id)[0]
-                                                    shared = []
-                                                    if conv_info.get('shared').get('shared_team_ids'):
-                                                        for wksp in conv_info.get('shared').get('shared_team_ids'):
-                                                            shared.append(workspace.create_from_dict(
-                                                                slack_connection.get_team_info(wksp)))
-                                                        conv_info['shared'] = shared
-                                                    channel = conversation.create_from_dict(conv_info)
-
-                                                    if _location_verification(channel, sig):
+                                    for pattern in sig.patterns:
+                                        r = re.compile(pattern)
+                                        if sig.search_strings:
+                                            for search_string in sig.search_strings:
+                                                if str(search_string.lower()) in esl.get('text').lower():
+                                                    if r.search(esl.get('text')):
+                                                        draft_user = next((item for item in users_list if
+                                                                           item.id == draft.user), None)
+                                                        team_id = draft.team
+                                                        team = slack_connection.get_team_info(team_id)
                                                         if draft_user:
-                                                            draft_user.workspaces = []
                                                             user_dict = draft_user
                                                         else:
                                                             user_dict = None
 
                                                         if team:
-                                                            team_dict = workspace.create_from_dict(team)
+                                                            team_dict = workspace.create_from_dict(team, verbose)
                                                         else:
                                                             team_dict = None
 
                                                         result_drafts.append({
                                                             'timestamp': _convert_timestamp(draft.created),
                                                             'match_string': r.search(esl.get('text')).group(0),
                                                             'draft': draft,
                                                             'user': user_dict,
                                                             'workspace': team_dict,
-                                                            'conversation': channel
                                                         })
             if result_drafts:
-                log.info(f'{len(result_drafts)} found containing {sig.meta.name} after filtering')
                 for result in result_drafts:
                     results.append(result)
         if results:
             results = _deduplicate(results)
-            log.log_info(f'{len(results)} total matches found after filtering')
+            logger.log('INFO', f'{len(results)} total matches found after filtering')
             return results
         else:
-            log.log_info('No matches found after filtering')
+            logger.log('INFO', 'No matches found after filtering')
     except Exception as e:
-        log.log_critical(e)
+        logger.log('CRITICAL', e)
 
 
-def find_shared_channels(slack_connection: SlackAPI) -> [conversation.Conversation]:
+def find_shared_channels(slack_connection: SlackAPI, verbose: bool) -> List[conversation.Conversation]:
     """ Find all shared channels. These could be either shared between
     Workspaces in an Enterprise Grid, or Slack Connect external channels.
 
     Args:
         slack_connection: Slack API object
+        verbose: Whether to use verbose logging or not
     Returns:
         List containing information on all external shared channels
     """
 
     channels = slack_connection.get_all_conversations(ext_shared=True)
 
     results = []
@@ -1167,24 +1167,24 @@
         conversation_info = slack_connection.get_conversation_info(channel_id=channel.get('id'))[0]
         connected_teams = []
         for team in conversation_info.get('shared').get('connected_team_ids'):
             team_info = slack_connection.get_team_info(team)
             if team_info.get('id').startswith('E'):
                 connected_teams.append(enterprise.create_from_dict(team_info))
             else:
-                connected_teams.append(workspace.create_from_dict(team_info))
+                connected_teams.append(workspace.create_from_dict(team_info, verbose))
 
-        results.append(conversation.create_from_dict(conversation_info))
+        results.append(conversation.create_from_dict(conversation_info, verbose))
 
     return results
 
 
 def get_all_messages(slack_connection: SlackAPI,
                      cores: int,
-                     timeframe: int = DEFAULT_TIMEFRAME) -> [post.Message]:
+                     timeframe: int = DEFAULT_TIMEFRAME) -> List[post.Message]:
     """ Get all messages in the Enterprise for a given timeframe
 
     Args:
         timeframe: timeframe to search in
         slack_connection: Slack API object
         cores: number of cores to use
     Returns:
@@ -1213,21 +1213,23 @@
         process.join()
 
     return results
 
 
 def get_all_files(slack_connection: SlackAPI,
                   cores: int,
-                  timeframe: int = DEFAULT_TIMEFRAME) -> [post.File]:
+                  verbose: bool,
+                  timeframe: int = DEFAULT_TIMEFRAME) -> List[post.File]:
     """ Get all files in the Enterprise for a given timeframe
 
     Args:
         timeframe: timeframe to search in
         slack_connection: Slack API object
         cores: Number of cores to use
+        verbose: Whether to use verbose logging or not
     Returns:
         list of File objects containing all drafts
     """
 
     results = multiprocessing.Manager().list()
     updated_files = slack_connection.list_files(oldest=timeframe)
     list_of_chunks = numpy.array_split(numpy.array(updated_files), cores)
@@ -1235,37 +1237,40 @@
 
     for file_list in list_of_chunks:
         p = multiprocessing.Process(
             target=_mp_file_search_worker,
             args=(
                 file_list,
                 slack_connection,
-                results
+                results,
+                verbose
             )
         )
         processes.append(p)
         p.start()
 
     for process in processes:
         process.join()
 
     return results
 
 
 def get_all_drafts(slack_connection: SlackAPI,
-                   workspaces_list: [workspace.Workspace],
+                   workspaces_list: List[workspace.Workspace],
                    cores: int,
-                   timeframe: int = DEFAULT_TIMEFRAME) -> [post.Draft]:
+                   verbose: bool,
+                   timeframe: int = DEFAULT_TIMEFRAME) -> List[post.Draft]:
     """ Get all drafts in the Enterprise for a given timeframe
 
     Args:
         timeframe: timeframe to search in
         slack_connection: Slack API object
         workspaces_list: List of all workspaces in the Enterprise
         cores: Number of cores to use
+        verbose: Whether to use verbose logging or not
     Returns:
         list of Draft objects containing all drafts
     """
 
     results = multiprocessing.Manager().list()
     list_of_chunks = numpy.array_split(numpy.array(workspaces_list), cores)
     processes = []
@@ -1273,15 +1278,16 @@
     for workspace in list_of_chunks:
         p = multiprocessing.Process(
             target=_mp_draft_search_worker,
             args=(
                 workspace,
                 slack_connection,
                 timeframe,
-                results
+                results,
+                verbose
             )
         )
         processes.append(p)
         p.start()
 
     for process in processes:
         process.join()
@@ -1336,35 +1342,37 @@
                     if regex.search(str(block.get('text').get('text'))):
                         return regex.search(str(block.get('text').get('text'))).group(0)
     elif regex.search(str(message.get('text'))):
         return regex.search(str(message.get('text'))).group(0)
 
 
 # Multiprocessing Worker Functions
-def _mp_draft_search_worker(workspaces_list: [workspace.Workspace],
+def _mp_draft_search_worker(workspaces_list: List[workspace.Workspace],
                             slack_connection: SlackAPI,
                             timeframe: int,
-                            results: list):
+                            results: list,
+                            verbose: bool):
     """ MULTIPROCESSING WORKER - Iterates through a workspace and returns all draft
     messages.
 
     Args:
         workspaces_list: List of workspace Objects
         slack_connection: Slack API connection
         timeframe: Furthest back time to get messages from
         results: MP results list to pass back to calling function
+        verbose: Whether to use verbose logging or not
     Returns:
         List of draft objects
     """
 
     for workspace in workspaces_list:
         workspace_drafts = slack_connection.list_drafts(workspace.id, oldest=timeframe)
         for draft_info in workspace_drafts:
             if draft_info.get('date_created') >= timeframe:
-                results.append(post.create_draft_from_dict(draft_info))
+                results.append(post.create_draft_from_dict(draft_info, verbose))
 
     return results
 
 
 def _mp_message_search_worker(conv_list: list,
                               slack_connection: SlackAPI,
                               timeframe: int,
@@ -1389,105 +1397,109 @@
                 message['conv_team'] = conv.get('team')
                 results.append(message)
     return results
 
 
 def _mp_file_search_worker(file_list: list,
                            slack_connection: SlackAPI,
-                           results: list) -> list:
+                           results: list,
+                           verbose: bool) -> list:
     """ MULTIPROCESSING WORKER - Iterates through a list of conversation IDs
     and gets recent messages for each
 
     Args:
         file_list: List of file information in dict format from the discovery.files.list endpoint
         slack_connection: Slack API object
         results: MP results list to pass back to calling function
+        verbose: Whether to use verbose logging or not
     Returns:
         List of File objects
     """
 
     for f in file_list:
         file_info = slack_connection.get_file_info(f.get('id'))
         shares = []
         if file_info.get('shares'):
             for share in file_info.get('shares'):
                 if share.get('channel').startswith('D'):
                     team_id = get_enterprise(slack_connection).id
                 else:
                     team_id = share.get('team')
                 conv = slack_connection.get_conversation_info(share.get('channel'), team_id)[0]
-                shares.append(conversation.create_from_dict(conv))
+                shares.append(conversation.create_from_dict(conv, verbose))
             file_info['shares'] = shares
             results.append(post.create_file_from_dict(file_info))
 
     return results
 
 
 def _mp_find_messages_worker(sig: signature.Signature,
                              slack_connection: SlackAPI,
-                             users_list: [user.User],
-                             message_list: [dict],
-                             workspaces_list: [workspace.Workspace],
-                             results):
+                             users_list: List[user.User],
+                             message_list: List[Dict],
+                             workspaces_list: List[workspace.Workspace],
+                             results,
+                             verbose: bool):
     """ MULTIPROCESSING WORKER - Iterates through lists of messages to find matches against a signature
 
     Args:
         sig: Signature objects
         users_list: List of User objects from the Enterprise
         message_list: List of Message objects
         workspaces_list: List of Workspaces objects from the Enterprise
         results: MP results list to pass back to calling function
+        verbose: Whether to use verbose logging or not
     Returns:
         List of Message objects that match the signature
     """
 
     for query in sig.search_strings:
         message_list = [message for message in message_list if _message_block_search(message, query)]
         for message in message_list:
-            r = re.compile(sig.pattern)
-            workspace = next(
-                (item for item in workspaces_list if item.id == message.get('team')), None)
-
-            match_string = _regex_search_message(message, r)
-            if match_string:
-                conv_info = slack_connection.get_conversation_info(message.get('conv_id'),
-                                                                   message.get('conv_team'))[0]
-
-                shared = []
-                if conv_info.get('shared').get('shared_team_ids'):
-                    for wrk_id in conv_info.get('shared').get('shared_team_ids'):
-                        shared.append(slack_connection.get_team_info(wrk_id))
-                conv_info['shared'] = shared
-                conv_info = conversation.create_from_dict(conv_info)
-                message['conversation'] = conv_info
-                message = post.create_message_from_dict(message)
-                post_user = next(
-                    (item for item in users_list if item.id == message.user), None)
-                post_user.workspaces = []
-
-                if workspace:
-                    url = f'https://{workspace.domain}.slack.com/archives/{message.conversation.id}' \
-                          f'/p{message.timestamp}'
-                else:
-                    url = None
-                if _location_verification(message.conversation, sig):
-                    results.append({
-                        'match_string': match_string,
-                        'message': message,
-                        'url': url,
-                        'user': post_user,
-                        'workspace': workspace
-                    })
+            for pattern in sig.patterns:
+                r = re.compile(pattern)
+                workspace = next(
+                    (item for item in workspaces_list if item.id == message.get('team')), None)
+
+                match_string = _regex_search_message(message, r)
+                if match_string:
+                    conv_info = slack_connection.get_conversation_info(message.get('conv_id'),
+                                                                       message.get('conv_team'))[0]
+
+                    shared = []
+                    if conv_info.get('shared').get('shared_team_ids'):
+                        for wrk_id in conv_info.get('shared').get('shared_team_ids'):
+                            shared.append(slack_connection.get_team_info(wrk_id))
+                    conv_info['shared'] = shared
+                    conv_info = conversation.create_from_dict(conv_info, verbose)
+                    message['conversation'] = conv_info
+                    message = post.create_message_from_dict(message)
+                    post_user = next(
+                        (item for item in users_list if item.id == message.user), None)
+
+                    if workspace:
+                        url = f'https://{workspace.domain}.slack.com/archives/{message.conversation.id}' \
+                              f'/p{message.timestamp}'
+                    else:
+                        url = None
+                    if _location_verification(message.conversation, sig):
+                        results.append({
+                            'match_string': match_string,
+                            'message': message,
+                            'url': url,
+                            'user': post_user,
+                            'workspace': workspace
+                        })
 
     return results
 
 
 def _mp_find_files_worker(sig: signature.Signature,
-                          users_list: [user.User],
-                          file_list: [post.File],
+                          users_list: List[user.User],
+                          file_list: List[post.File],
                           results):
     """ MULTIPROCESSING WORKER - Iterates through lists of files to find matches against a signature
 
     Args:
         sig: Signature objects
         users_list: List of User objects from the Enterprise
         file_list: List of File objects
@@ -1503,29 +1515,27 @@
                 for file_type in sig.file_types:
                     if file_type.lower() in target_file.filetype.lower() \
                             and str(query.lower()) in target_file.title.lower():
                         for conv in target_file.shares:
                             if _location_verification(conv, sig):
                                 file_user = next((item for item in users_list if item.id == target_file.user),
                                                  None)
-                                file_user.workspaces = []
                                 results_dict = {
                                     'file': target_file,
                                     'conversation': conv,
                                     'user': file_user
                                 }
 
                                 results.append(results_dict)
             else:
                 if str(query.lower()) in target_file.title.lower():
                     for conv in target_file.shares:
                         if _location_verification(conv, sig):
                             file_user = next((item for item in users_list if item.id == target_file.user),
                                              None)
-                            file_user.workspaces = []
                             results_dict = {
                                 'file': target_file,
                                 'conversation': conv,
                                 'user': file_user
                             }
 
                             results.append(results_dict)
```

### Comparing `slack-watchman-eg-1.1.0/src/slack_watchman_eg.egg-info/PKG-INFO` & `slack-watchman-eg-2.0.0/src/slack_watchman_eg.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 Metadata-Version: 2.1
 Name: slack-watchman-eg
-Version: 1.1.0
-Summary: Monitoring your Slack Enterprise Grid for sensitive information
+Version: 2.0.0
+Summary: Monitoring Slack Enterprise Grid for exposed secrets
 Home-page: https://github.com/PaperMtn/slack-watchman-enterprise-grid
 Author: PaperMtn
 Author-email: papermtn@protonmail.com
 License: GPL-3.0
 Keywords: audit,slack,slack-watchman,watchman,blue-team,red-team,threat-hunting,slack-watchman-enterprise-grid
-Platform: UNKNOWN
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://i.imgur.com/VPgx6ra.png" width="550">
 
 # Slack Watchman for Enterprise Grid
 ![Python 2.7 and 3 compatible](https://img.shields.io/pypi/pyversions/slack-watchman-eg)
 ![PyPI version](https://img.shields.io/pypi/v/slack-watchman-eg.svg)
 ![License: MIT](https://img.shields.io/pypi/l/slack-watchman-eg.svg)
 
 
 ## About Slack Watchman for Enterprise Grid
 
-Slack Watchman for Enterprise Grid uses the Slack Enterprise Grid DLP API to look for potentially sensitive data exposed in your Slack Enterprise.
+Slack Watchman for Enterprise Grid uses the Slack Enterprise Grid DLP API to look for potentially exposed secrets and sensitive data in Slack Enterprise Grid.
 
 **Note**: Slack Watchman for Enterprise Grid is designed for Enterprise Grid subscribers of Slack only. If you use Slack without an Enterprise subscription, you can use the standard version of [Slack Watchman](https://github.com/PaperMtn/slack-watchman)
 
 ### Features
 Slack Watchman for Enterprise Grid looks for:
 
 - API Keys, Tokens & Service Accounts
@@ -70,50 +66,15 @@
 #### Multiprocessing
 Multiprocessing is used to search the potentially huge amount of data retrieved when getting all messages sent in an Enterprise. You can specify how many cores to use at runtime, and the more cores you use, the faster processing is generally done. That being said, you are still constrained by the API.
 
 I have found the most efficient approach is to use between 8-12 cores.
 
 You can specify cores using the optional flag `--cores` at runtime. If this flag is not set, Slack Watchman will automatically use all available cores up to a maximum of 8.
 ### Signatures
-Slack Watchman uses custom YAML signatures to detect matches in Slack.
-
-They follow this format:
-
-```yaml
----
-filename:
-enabled: [true|false]
-meta:
-  name:
-  author:
-  date:
-  description: # what the search should find
-  severity: # rating out of 100
-tombstone: [true|false]
-scope:
-  - [files|messages]
-file_types: # optional list for use with file searching*
-locations: # what conversations to search in. Any combination of:
-  - public
-  - private
-  - connect
-  - im
-  - mpim
-test_cases:
-  match_cases:
-  - # test case that should match the regex*
-  fail_cases:
-  - # test case that should not match the regex*
-search_strings:
-- # search query(s) to use in Slack
-pattern: # Regex pattern to filter out false positives
-```
-There are Python tests to ensure signatures are formatted properly and that the Regex patterns work in the `tests` dir
-
-More information about signatures, and how you can add your own, is in the file `docs/signatures.md`.
+Slack Watchman uses custom YAML signatures to detect matches in Slack. These signatures are pulled from the central [Watchman Signatures repository](https://github.com/PaperMtn/watchman-signatures). Slack Watchman for Enterprise Grid automatically updates its signature base at runtime to ensure its using the latest signatures to detect secrets. 
 
 ## Requirements
 ### Slack API token
 To run Slack Watchman for Enterprise Grid, you will need a Slack API access token that is authorised to use the Enterprise DLP API.
 
 To do this, you need to create a [Slack App](https://api.slack.com/apps) and install it at the organisation level.
 
@@ -130,15 +91,15 @@
 Provide the token in the environment variable `SLACK_WATCHMAN_EG_TOKEN`
 
 ## Installation
 You can install the latest stable version via pip:
 
 `python3 -m pip install slack-watchman-eg`
 
-Or build from source yourself, which is useful for if you intend to add your own signatures:
+Or build from source yourself:
 
 Download the release source files, then from the top level repository run:
 ```shell
 python3 -m pip build
 python3 -m pip install --force-reinstall dist/*.whl
 ```
 
@@ -157,55 +118,74 @@
 // scan all
 docker run --rm -e SLACK_WATCHMAN_EG_TOKENN=xoxp... papermountain/slack-watchman-eg --hours 1 --cores 8
 docker run --rm --env-file .env papermountain/slack-watchman-eg --hours 1 --cores 8
 ```
 
 ## Usage
 ```
-usage: slack-watchman-eg [-h] [--hours HOURS] [--minutes MINUTES] [--cores CORES] [--version] [--users] [--workspaces] [--sandbox] [--tombstone] [--tombstone-text-file TOMBSTONE_FILEPATH]
+usage: slack-watchman-eg [-h] [--hours HOURS] [--minutes MINUTES] [--output {json,terminal}] [--cores CORES] [--version] [--users] [--workspaces] [--debug] [--verbose]
 
 Monitoring your Slack Enterprise Grid for sensitive information
 
 options:
   -h, --help            show this help message and exit
-  --hours HOURS         How far back to search in whole hours between 1-24. Defaults to 1 if no acceptable value given
-  --minutes MINUTES     How far back to search in whole minutes between 1-60
-  --cores CORES         Number of cores to use between 1-12
-  --version             show program's version number and exit
-  --users               Find all users
-  --workspaces          Find all workspaces
-  --sandbox             Search using only sandbox signatures
-  --tombstone           Tombstone (REMOVE) all matching messages
-  --tombstone-text-file TOMBSTONE_FILEPATH
-                        Path to file containing custom tombstone notification text (Optional)
+  --hours HOURS, -hr HOURS
+                        How far back to search in whole hours between 1-24. Defaults to 1 if no acceptable value given
+  --minutes MINUTES, -m MINUTES
+                        How far back to search in whole minutes between 1-60
+  --output {json,terminal}, -o {json,terminal}
+                        What logging output to use - JSON formatted output, or textual outputfor reading via terminal. Default is terminal
+  --cores CORES, -c CORES
+                        Number of cores to use between 1-12
+  --version, -v         show program's version number and exit
+  --users, -u           Return all users
+  --workspaces, -w      Return all workspaces
+  --debug, -d           Turn on debug level logging
+  --verbose, -V         Turn on more verbose output for JSON logging. This includes more fields, but is larger
 ```
 
 ## Other Watchman apps
 You may be interested in the other apps in the Watchman family:
+- [Slack Watchman](https://github.com/PaperMtn/slack-watchman)
 - [GitLab Watchman](https://github.com/PaperMtn/gitlab-watchman)
 - [GitHub Watchman](https://github.com/PaperMtn/github-watchman)
-- [Slack Watchman](https://github.com/PaperMtn/slack-watchman)
-- [Trello Watchman](https://github.com/PaperMtn/trello-watchman)
 
 ## License
-The source code for this project is released under the [GNU General Public Licence](https://www.gnu.org/licenses/licenses.html#GPL). This project is not associated with Slack.
-## 1.1.0 - 2022-04-02
+The source code for this project is released under the [GNU General Public Licence](https://www.gnu.org/licenses/licenses.html#GPL). This project is not associated with Slack Technologies or Salesforce.
+## [2.0.0] - 2023-04-14
+This major version release brings multiple updates to Slack Watchman for Enterprise Grid, both in usability, functionality and behind the scenes improvements.
+### Added
+- Support for centralised signatures from the Watchman Signatures repository. This makes it much easier to keep the signature base for all Watchman applications up to date, and to add functionality to Slack Watchman with new signatures. New signatures are downloaded, and updates to existing signatures are applied, at runtime, meaning Slack Watchman for Enterprise Grid will always be using the most up to date signatures. 
+- Option for terminal optimised logging instead of JSON formatting. This is now the default when running with no output option selected, and is a lot easier for humans to read. Also, colours! 
+- Option choose between verbose or succinct logging when using JSON output. Default is succinct.
+- Debug logging option
+### Removed
+- Support for tombstoning posts that match signatures removed
+- Local signatures - Centralised signatures mean that user-created custom signatures can't be used with Slack Watchman for Enterprise Grid anymore. If you have made a signature you think would be good for sharing with the community, feel free to add it to the Watchman Signatures repository, so it can be used in all Watchman applications 
+- For the reason above, the functionality to have sandbox signatures has been removed as well
+### Fixed
+- Draft searches were giving an error due to not being able to populate some workspace information. This has now been fixed
+
+## [1.1.1] - 2022-05-16
+### Added
+- Signature to find Atlassian tokens
+
+## [1.1.0] - 2022-04-02
 ### Added
 - Docker image now available from the Docker hub, or by building from source.
 - Support for Python 3.7
 - New logo to play nicely with dark mode
 ### Fixed
 - More errors when importing packages
 
-## 1.0.2 - 2021-12-30
+## [1.0.2] - 2021-12-30
 ### Fixed
 - Error when importing packages
 - Signatures not being included in the distribution package
 
-## 1.0.1 - 2021-12-30
+## [1.0.1] - 2021-12-30
+### Added
 - Refactor and update distribution files
 
-## 1.0.0 - 2021-12-30
+## [1.0.0] - 2021-12-30
 - Initial release
 
-
-
```

