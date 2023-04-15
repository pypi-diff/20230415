# Comparing `tmp/krakenci_server-1.0.tar.gz` & `tmp/krakenci_server-1.1.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krakenci_server-1.0.tar", max compression
+gzip compressed data, was "krakenci_server-1.1.44.tar", max compression
```

## Comparing `krakenci_server-1.0.tar` & `krakenci_server-1.1.44.tar`

### file list

```diff
@@ -1,123 +1,126 @@
--rw-r--r--   0        0        0     2900 2023-03-04 17:57:05.541088 krakenci_server-1.0/README.md
--rw-r--r--   0        0        0        0 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/__init__.py
--rw-r--r--   0        0        0       38 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/README
--rw-r--r--   0        0        0        0 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/__init__.py
--rw-r--r--   0        0        0     2032 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/alembic.ini
--rw-r--r--   0        0        0     2012 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/apply.py
--rw-r--r--   0        0        0     2703 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/env.py
--rw-r--r--   0        0        0      494 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/script.py.mako
--rw-r--r--   0        0        0      560 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/050fbc3d126c_added_deployment_to_agents_group.py
--rw-r--r--   0        0        0      707 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/0615faca43b1_added_url_tag_and_tool_file_to_tool.py
--rw-r--r--   0        0        0      433 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/0731897c862e_add_enabled_to_stage.py
--rw-r--r--   0        0        0      448 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/0ad7507aa6d0_added_age_to_issue.py
--rw-r--r--   0        0        0      562 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/19396769e240_added_extra_atrs_to_agents_group.py
--rw-r--r--   0        0        0      461 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/1982be95e79f_added_system_to_job.py
--rw-r--r--   0        0        0     1173 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/1cf31ab18f84_create_secret_table.py
--rw-r--r--   0        0        0     1485 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/1f5039135dd8_removed_enabled_from_projects.py
--rw-r--r--   0        0        0     1122 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/26c6d691e7ce_added_last_flows_to_branch.py
--rw-r--r--   0        0        0      587 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/2996b1b6e227_user_is_session_nullable.py
--rw-r--r--   0        0        0      681 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/29b96da53f09_added_reason_to_run.py
--rw-r--r--   0        0        0      533 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/2b5751b83fec_added_artifacts_to_flow.py
--rw-r--r--   0        0        0     1035 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/2dd5cf2d12dc_added_new_repo_fields_to_stage.py
--rw-r--r--   0        0        0      482 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/38088514157a_removed_cancel_from_agent.py
--rw-r--r--   0        0        0      656 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/3c1af14e0370_added_timeouts_to_stage_and_job.py
--rw-r--r--   0        0        0      527 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/411094f6b709_added_details_to_user.py
--rw-r--r--   0        0        0    21962 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/42ea01a6cf31_convert_timestamps_to_with_timezones.py
--rw-r--r--   0        0        0      458 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/466de256799e_added_label_to_run.py
--rw-r--r--   0        0        0     1867 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/4a7ac9143bb1_added_branch_sequences.py
--rw-r--r--   0        0        0      492 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/54efe873f88f_added_git_clone_params_to_stage.py
--rw-r--r--   0        0        0     3897 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/5b13b262b132_added_repo_changes.py
--rw-r--r--   0        0        0      545 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/5c16623f4d55_added_fields_masked_to_step.py
--rw-r--r--   0        0        0      527 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/5e38f55beb11_added_summary_to_flow.py
--rw-r--r--   0        0        0      434 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/66808ea51a72_delete_setting_records_with_no_group.py
--rw-r--r--   0        0        0     1028 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/6745adaf40e5_added_schema_repo_to_stage.py
--rw-r--r--   0        0        0      478 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/67d4f5a5ee98_added_authorized_to_executor.py
--rw-r--r--   0        0        0      638 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/735e81eedae4_change_project_id_in_executorgroup_to_.py
--rw-r--r--   0        0        0      457 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/73db0f22e1e6_added_cancel_to_agent.py
--rw-r--r--   0        0        0      500 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/770cfcc80cfb_added_relevancy_to_test_case_result.py
--rw-r--r--   0        0        0      706 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/818e190ca142_move_webhook_to_project.py
--rw-r--r--   0        0        0     1732 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/8200318b9e18_added_several_stats_fields_to_run.py
--rw-r--r--   0        0        0     1317 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/87358b464400_added_casbin_rules_table.py
--rw-r--r--   0        0        0     1795 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/899dadc28f9c_added_missing_indexes.py
--rw-r--r--   0        0        0     5629 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/89ffd52f1f00_rename_executor_to_agent.py
--rw-r--r--   0        0        0      490 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/8b4adeca953d_added_group_to_setting.py
--rw-r--r--   0        0        0      551 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/9666bf8c1bb0_added_details_to_user_session.py
--rw-r--r--   0        0        0      826 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/98af95844f27_added_results_change_stats_to_run.py
--rw-r--r--   0        0        0      536 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/9d8d8713c1ad_added_unique_index_for_address_of_non_.py
--rw-r--r--   0        0        0        0 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/__init__.py
--rw-r--r--   0        0        0      700 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/a0741baf2dbc_added_indexes_to_test_case_results.py
--rw-r--r--   0        0        0      542 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/a26a02d0ac01_added_extra_atrs_to_agents.py
--rw-r--r--   0        0        0      698 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/a35aec7afa0a_added_processed_at_in_run_and_index_to_.py
--rw-r--r--   0        0        0      469 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/a7de4bdee425_added_section_to_artifact.py
--rw-r--r--   0        0        0     1439 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/ab9326d5fc02_added_index_to_flows.py
--rw-r--r--   0        0        0      690 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/af348b43d9d5_extended_tool.py
--rw-r--r--   0        0        0      626 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/b2c9024746f5_added_unique_constraint_for_system_name_.py
--rw-r--r--   0        0        0      522 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/b5cc62f79980_add_extra_to_issue.py
--rw-r--r--   0        0        0      604 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/b84bdc5d3c67_uniqued_agent_address.py
--rw-r--r--   0        0        0      698 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/b908e219f07f_longer_message_in_issue.py
--rw-r--r--   0        0        0      411 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/ba436d491bf8_update_stage_enabled_to_true.py
--rw-r--r--   0        0        0     1478 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/bb0d4908ba49_added_artifact_and_file.py
--rw-r--r--   0        0        0      907 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/befa07ac5d1c_changed_tool_version_to_string.py
--rw-r--r--   0        0        0     3622 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/cb7654d57bca_added_systems_table_and_host_info_user_.py
--rw-r--r--   0        0        0    11177 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/ce05198f524a_convert_char_n_to_text.py
--rw-r--r--   0        0        0      562 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/cea0e48abb5a_added_retention_policy_to_branch.py
--rw-r--r--   0        0        0      461 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/d2b23f410d02_added_label_to_flow.py
--rw-r--r--   0        0        0      714 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/d45087b62027_move_trigger_data_to_flow.py
--rw-r--r--   0        0        0     1542 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/d524cbcbf19c_added_users_and_users_session.py
--rw-r--r--   0        0        0      530 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/dae910bd9587_added_repo_data_to_run.py
--rw-r--r--   0        0        0      719 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/e0d8421619c2_removed_unique_constraint_agent_non_.py
--rw-r--r--   0        0        0      814 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/e404f52562c2_added_unique_constraints_on_branch_name_.py
--rw-r--r--   0        0        0     1638 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/f566580fd139_added_test_case_comment_table.py
--rw-r--r--   0        0        0      476 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/migrations/versions/ff4a425a6070_added_last_seen_to_executor.py
--rw-r--r--   0        0        0      582 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/__init__.py
--rw-r--r--   0        0        0    12197 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/access.py
--rw-r--r--   0        0        0     2919 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/agentblob.py
--rw-r--r--   0        0        0    10192 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/authn.py
--rw-r--r--   0        0        0    21894 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/backend.py
--rw-r--r--   0        0        0     4378 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/badge.py
--rw-r--r--   0        0        0        0 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/bg/__init__.py
--rw-r--r--   0        0        0    44750 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/bg/jobs.py
--rw-r--r--   0        0        0      954 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/chops.py
--rw-r--r--   0        0        0        0 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/cloud/__init__.py
--rw-r--r--   0        0        0     2003 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/cloud/aws.py
--rw-r--r--   0        0        0     9147 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/cloud/aws_ec2.py
--rw-r--r--   0        0        0     7191 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/cloud/aws_ecs.py
--rw-r--r--   0        0        0    17629 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/cloud/azure.py
--rw-r--r--   0        0        0     3244 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/cloud/cloud.py
--rw-r--r--   0        0        0     1892 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/cloud/common.py
--rw-r--r--   0        0        0     9421 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/cloud/k8s.py
--rw-r--r--   0        0        0        0 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/config.py
--rw-r--r--   0        0        0     5055 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/consts.py
--rw-r--r--   0        0        0     1687 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/dbutils.py
--rw-r--r--   0        0        0    16911 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/exec_utils.py
--rw-r--r--   0        0        0    23385 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/execution.py
--rw-r--r--   0        0        0     9981 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/gitops.py
--rw-r--r--   0        0        0    24636 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/initdb.py
--rw-r--r--   0        0        0     3839 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/job_log.py
--rw-r--r--   0        0        0     4523 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/kkrq.py
--rw-r--r--   0        0        0    14059 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/logs.py
--rw-r--r--   0        0        0    45095 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/management.py
--rw-r--r--   0        0        0     4435 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/minioops.py
--rw-r--r--   0        0        0    45774 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/models.py
--rw-r--r--   0        0        0     9980 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/notify.py
--rwxr-xr-x   0        0        0     6478 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/planner.py
--rw-r--r--   0        0        0     1248 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/pljobs.py
--rw-r--r--   0        0        0     4440 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/qneck.py
--rw-r--r--   0        0        0    11619 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/results.py
--rwxr-xr-x   0        0        0     5714 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/scheduler.py
--rw-r--r--   0        0        0    13052 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/schema.py
--rw-r--r--   0        0        0    30836 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/schemaval.py
--rwxr-xr-x   0        0        0     7289 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/server.py
--rw-r--r--   0        0        0     2010 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/srvcheck.py
--rw-r--r--   0        0        0     3908 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/storage.py
--rw-r--r--   0        0        0    81318 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/swagger.yml
--rw-r--r--   0        0        0     2222 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/toolops.py
--rw-r--r--   0        0        0     3197 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/toolutils.py
--rw-r--r--   0        0        0    10872 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/users.py
--rw-r--r--   0        0        0     1032 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/utils.py
--rw-r--r--   0        0        0    19687 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/watchdog.py
--rw-r--r--   0        0        0    12005 2023-03-04 17:55:02.000000 krakenci_server-1.0/kraken/server/webhooks.py
--rw-r--r--   0        0        0       16 2023-03-04 17:57:05.537088 krakenci_server-1.0/kraken/version.py
--rw-r--r--   0        0        0     2429 2023-03-04 17:57:06.517089 krakenci_server-1.0/pyproject.tml
--rw-r--r--   0        0        0     5243 1970-01-01 00:00:00.000000 krakenci_server-1.0/setup.py
--rw-r--r--   0        0        0     5554 1970-01-01 00:00:00.000000 krakenci_server-1.0/PKG-INFO
+-rw-r--r--   0        0        0     2900 2023-04-14 16:38:17.608205 krakenci_server-1.1.44/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/__init__.py
+-rw-r--r--   0        0        0       38 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/README
+-rw-r--r--   0        0        0        0 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/__init__.py
+-rw-r--r--   0        0        0     2032 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/alembic.ini
+-rw-r--r--   0        0        0     2041 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/apply.py
+-rw-r--r--   0        0        0     2703 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/env.py
+-rw-r--r--   0        0        0      494 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/script.py.mako
+-rw-r--r--   0        0        0      560 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/050fbc3d126c_added_deployment_to_agents_group.py
+-rw-r--r--   0        0        0      707 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/0615faca43b1_added_url_tag_and_tool_file_to_tool.py
+-rw-r--r--   0        0        0      433 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/0731897c862e_add_enabled_to_stage.py
+-rw-r--r--   0        0        0      448 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/0ad7507aa6d0_added_age_to_issue.py
+-rw-r--r--   0        0        0      562 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/19396769e240_added_extra_atrs_to_agents_group.py
+-rw-r--r--   0        0        0      461 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/1982be95e79f_added_system_to_job.py
+-rw-r--r--   0        0        0     1173 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/1cf31ab18f84_create_secret_table.py
+-rw-r--r--   0        0        0     1485 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/1f5039135dd8_removed_enabled_from_projects.py
+-rw-r--r--   0        0        0     1122 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/26c6d691e7ce_added_last_flows_to_branch.py
+-rw-r--r--   0        0        0      587 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/2996b1b6e227_user_is_session_nullable.py
+-rw-r--r--   0        0        0      654 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/29b96da53f09_added_reason_to_run.py
+-rw-r--r--   0        0        0      533 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/2b5751b83fec_added_artifacts_to_flow.py
+-rw-r--r--   0        0        0     1035 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/2dd5cf2d12dc_added_new_repo_fields_to_stage.py
+-rw-r--r--   0        0        0      482 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/38088514157a_removed_cancel_from_agent.py
+-rw-r--r--   0        0        0      656 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/3c1af14e0370_added_timeouts_to_stage_and_job.py
+-rw-r--r--   0        0        0      527 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/411094f6b709_added_details_to_user.py
+-rw-r--r--   0        0        0    21962 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/42ea01a6cf31_convert_timestamps_to_with_timezones.py
+-rw-r--r--   0        0        0      458 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/466de256799e_added_label_to_run.py
+-rw-r--r--   0        0        0     1867 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/4a7ac9143bb1_added_branch_sequences.py
+-rw-r--r--   0        0        0      492 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/54efe873f88f_added_git_clone_params_to_stage.py
+-rw-r--r--   0        0        0     3897 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/5b13b262b132_added_repo_changes.py
+-rw-r--r--   0        0        0      545 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/5c16623f4d55_added_fields_masked_to_step.py
+-rw-r--r--   0        0        0      527 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/5e38f55beb11_added_summary_to_flow.py
+-rw-r--r--   0        0        0      407 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/66808ea51a72_delete_setting_records_with_no_group.py
+-rw-r--r--   0        0        0     1028 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/6745adaf40e5_added_schema_repo_to_stage.py
+-rw-r--r--   0        0        0      478 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/67d4f5a5ee98_added_authorized_to_executor.py
+-rw-r--r--   0        0        0      638 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/735e81eedae4_change_project_id_in_executorgroup_to_.py
+-rw-r--r--   0        0        0      457 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/73db0f22e1e6_added_cancel_to_agent.py
+-rw-r--r--   0        0        0      500 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/770cfcc80cfb_added_relevancy_to_test_case_result.py
+-rw-r--r--   0        0        0      706 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/818e190ca142_move_webhook_to_project.py
+-rw-r--r--   0        0        0     1732 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/8200318b9e18_added_several_stats_fields_to_run.py
+-rw-r--r--   0        0        0     1317 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/87358b464400_added_casbin_rules_table.py
+-rw-r--r--   0        0        0     1737 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/899dadc28f9c_added_missing_indexes.py
+-rw-r--r--   0        0        0     5629 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/89ffd52f1f00_rename_executor_to_agent.py
+-rw-r--r--   0        0        0      490 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/8b4adeca953d_added_group_to_setting.py
+-rw-r--r--   0        0        0      551 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/9666bf8c1bb0_added_details_to_user_session.py
+-rw-r--r--   0        0        0      826 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/98af95844f27_added_results_change_stats_to_run.py
+-rw-r--r--   0        0        0      509 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/9d8d8713c1ad_added_unique_index_for_address_of_non_.py
+-rw-r--r--   0        0        0        0 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/__init__.py
+-rw-r--r--   0        0        0      700 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/a0741baf2dbc_added_indexes_to_test_case_results.py
+-rw-r--r--   0        0        0      542 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/a26a02d0ac01_added_extra_atrs_to_agents.py
+-rw-r--r--   0        0        0      698 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/a35aec7afa0a_added_processed_at_in_run_and_index_to_.py
+-rw-r--r--   0        0        0      469 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/a7de4bdee425_added_section_to_artifact.py
+-rw-r--r--   0        0        0     1385 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/ab9326d5fc02_added_index_to_flows.py
+-rw-r--r--   0        0        0      690 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/af348b43d9d5_extended_tool.py
+-rw-r--r--   0        0        0      626 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/b2c9024746f5_added_unique_constraint_for_system_name_.py
+-rw-r--r--   0        0        0      859 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/b510fae321ba_added_seq_to_flow_and_run.py
+-rw-r--r--   0        0        0      522 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/b5cc62f79980_add_extra_to_issue.py
+-rw-r--r--   0        0        0      604 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/b84bdc5d3c67_uniqued_agent_address.py
+-rw-r--r--   0        0        0      698 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/b908e219f07f_longer_message_in_issue.py
+-rw-r--r--   0        0        0      384 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/ba436d491bf8_update_stage_enabled_to_true.py
+-rw-r--r--   0        0        0     1478 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/bb0d4908ba49_added_artifact_and_file.py
+-rw-r--r--   0        0        0     1377 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/bdcdbb4b5b3f_added_user_data_to_several_entities.py
+-rw-r--r--   0        0        0      880 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/befa07ac5d1c_changed_tool_version_to_string.py
+-rw-r--r--   0        0        0     3622 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/cb7654d57bca_added_systems_table_and_host_info_user_.py
+-rw-r--r--   0        0        0    11177 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/ce05198f524a_convert_char_n_to_text.py
+-rw-r--r--   0        0        0      562 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/cea0e48abb5a_added_retention_policy_to_branch.py
+-rw-r--r--   0        0        0      461 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/d2b23f410d02_added_label_to_flow.py
+-rw-r--r--   0        0        0      714 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/d45087b62027_move_trigger_data_to_flow.py
+-rw-r--r--   0        0        0     1542 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/d524cbcbf19c_added_users_and_users_session.py
+-rw-r--r--   0        0        0      530 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/dae910bd9587_added_repo_data_to_run.py
+-rw-r--r--   0        0        0      719 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/e0d8421619c2_removed_unique_constraint_agent_non_.py
+-rw-r--r--   0        0        0      814 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/e404f52562c2_added_unique_constraints_on_branch_name_.py
+-rw-r--r--   0        0        0     1638 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/f566580fd139_added_test_case_comment_table.py
+-rw-r--r--   0        0        0      476 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/ff4a425a6070_added_last_seen_to_executor.py
+-rw-r--r--   0        0        0      582 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/__init__.py
+-rw-r--r--   0        0        0    12197 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/access.py
+-rw-r--r--   0        0        0     2919 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/agentblob.py
+-rw-r--r--   0        0        0    10192 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/authn.py
+-rw-r--r--   0        0        0    22134 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/backend.py
+-rw-r--r--   0        0        0     4378 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/badge.py
+-rw-r--r--   0        0        0        0 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/bg/__init__.py
+-rw-r--r--   0        0        0    44857 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/bg/jobs.py
+-rw-r--r--   0        0        0     6287 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/chops.py
+-rw-r--r--   0        0        0        0 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/cloud/__init__.py
+-rw-r--r--   0        0        0     2003 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/cloud/aws.py
+-rw-r--r--   0        0        0     9147 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/cloud/aws_ec2.py
+-rw-r--r--   0        0        0     7191 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/cloud/aws_ecs.py
+-rw-r--r--   0        0        0    17629 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/cloud/azure.py
+-rw-r--r--   0        0        0     3244 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/cloud/cloud.py
+-rw-r--r--   0        0        0     1892 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/cloud/common.py
+-rw-r--r--   0        0        0     9421 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/cloud/k8s.py
+-rw-r--r--   0        0        0        0 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/config.py
+-rw-r--r--   0        0        0     5127 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/consts.py
+-rw-r--r--   0        0        0     3772 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/datastore.py
+-rw-r--r--   0        0        0     1687 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/dbutils.py
+-rw-r--r--   0        0        0    18026 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/exec_utils.py
+-rw-r--r--   0        0        0    21211 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/execution.py
+-rw-r--r--   0        0        0     9981 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/gitops.py
+-rw-r--r--   0        0        0    27015 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/initdb.py
+-rw-r--r--   0        0        0     5460 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/job_log.py
+-rw-r--r--   0        0        0     4489 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/kkrq.py
+-rw-r--r--   0        0        0    14059 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/logs.py
+-rw-r--r--   0        0        0    46016 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/management.py
+-rw-r--r--   0        0        0     4435 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/minioops.py
+-rw-r--r--   0        0        0    47658 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/models.py
+-rw-r--r--   0        0        0    10039 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/notify.py
+-rwxr-xr-x   0        0        0     6478 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/planner.py
+-rw-r--r--   0        0        0     1248 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/pljobs.py
+-rw-r--r--   0        0        0     4440 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/qneck.py
+-rw-r--r--   0        0        0    11643 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/results.py
+-rwxr-xr-x   0        0        0     5714 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/scheduler.py
+-rw-r--r--   0        0        0    15415 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/schema.py
+-rw-r--r--   0        0        0    30836 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/schemaval.py
+-rwxr-xr-x   0        0        0     7508 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/server.py
+-rw-r--r--   0        0        0     2010 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/srvcheck.py
+-rw-r--r--   0        0        0     3908 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/storage.py
+-rw-r--r--   0        0        0    83344 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/swagger.yml
+-rw-r--r--   0        0        0     2222 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/toolops.py
+-rw-r--r--   0        0        0     3197 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/toolutils.py
+-rw-r--r--   0        0        0    10872 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/users.py
+-rw-r--r--   0        0        0     1032 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/utils.py
+-rw-r--r--   0        0        0    19687 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/watchdog.py
+-rw-r--r--   0        0        0    12005 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/webhooks.py
+-rw-r--r--   0        0        0       19 2023-04-14 16:38:17.608205 krakenci_server-1.1.44/kraken/version.py
+-rw-r--r--   0        0        0     2440 2023-04-14 16:38:18.460204 krakenci_server-1.1.44/pyproject.tml
+-rw-r--r--   0        0        0     5342 1970-01-01 00:00:00.000000 krakenci_server-1.1.44/setup.py
+-rw-r--r--   0        0        0     5709 1970-01-01 00:00:00.000000 krakenci_server-1.1.44/PKG-INFO
```

### Comparing `krakenci_server-1.0/README.md` & `krakenci_server-1.1.44/README.md`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/alembic.ini` & `krakenci_server-1.1.44/kraken/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/apply.py` & `krakenci_server-1.1.44/kraken/migrations/apply.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,16 @@
     alembic_ini_path = os.path.join(here, 'alembic.ini')
     alembic_args = [
         '-c', alembic_ini_path,
     ]
 
     if db_version is None:
         # create tables in db
-        models.db.create_all(app=app)
+        with app.app_context():
+            models.db.create_all()
 
         # stamp the alembic version of db schema in db
         alembic_args.extend(['stamp', 'head'])
         alembic.config.main(argv=alembic_args)
         print('alembic stamp completed')
     else:
         alembic_args.extend(['upgrade', 'head'])
```

### Comparing `krakenci_server-1.0/kraken/migrations/env.py` & `krakenci_server-1.1.44/kraken/migrations/env.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/050fbc3d126c_added_deployment_to_agents_group.py` & `krakenci_server-1.1.44/kraken/migrations/versions/050fbc3d126c_added_deployment_to_agents_group.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/0615faca43b1_added_url_tag_and_tool_file_to_tool.py` & `krakenci_server-1.1.44/kraken/migrations/versions/0615faca43b1_added_url_tag_and_tool_file_to_tool.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/19396769e240_added_extra_atrs_to_agents_group.py` & `krakenci_server-1.1.44/kraken/migrations/versions/19396769e240_added_extra_atrs_to_agents_group.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/1cf31ab18f84_create_secret_table.py` & `krakenci_server-1.1.44/kraken/migrations/versions/1cf31ab18f84_create_secret_table.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/1f5039135dd8_removed_enabled_from_projects.py` & `krakenci_server-1.1.44/kraken/migrations/versions/1f5039135dd8_removed_enabled_from_projects.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/26c6d691e7ce_added_last_flows_to_branch.py` & `krakenci_server-1.1.44/kraken/migrations/versions/26c6d691e7ce_added_last_flows_to_branch.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/2996b1b6e227_user_is_session_nullable.py` & `krakenci_server-1.1.44/kraken/migrations/versions/2996b1b6e227_user_is_session_nullable.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/29b96da53f09_added_reason_to_run.py` & `krakenci_server-1.1.44/kraken/migrations/versions/29b96da53f09_added_reason_to_run.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 branch_labels = None
 depends_on = None
 
 
 def upgrade():
     op.add_column('runs', sa.Column('reason', postgresql.JSONB(astext_type=sa.Text()), nullable=True))
 
-    conn = op.get_bind()
-    conn.execute("""UPDATE runs SET reason = '{"reason": "manual"}'::jsonb""")
+    op.execute("""UPDATE runs SET reason = '{"reason": "manual"}'::jsonb""")
 
     op.alter_column('runs', 'reason', nullable=False)
 
 
 def downgrade():
     op.drop_column('runs', 'reason')
```

### Comparing `krakenci_server-1.0/kraken/migrations/versions/2b5751b83fec_added_artifacts_to_flow.py` & `krakenci_server-1.1.44/kraken/migrations/versions/2b5751b83fec_added_artifacts_to_flow.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/2dd5cf2d12dc_added_new_repo_fields_to_stage.py` & `krakenci_server-1.1.44/kraken/migrations/versions/2dd5cf2d12dc_added_new_repo_fields_to_stage.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/3c1af14e0370_added_timeouts_to_stage_and_job.py` & `krakenci_server-1.1.44/kraken/migrations/versions/3c1af14e0370_added_timeouts_to_stage_and_job.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/411094f6b709_added_details_to_user.py` & `krakenci_server-1.1.44/kraken/migrations/versions/411094f6b709_added_details_to_user.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/42ea01a6cf31_convert_timestamps_to_with_timezones.py` & `krakenci_server-1.1.44/kraken/migrations/versions/42ea01a6cf31_convert_timestamps_to_with_timezones.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/4a7ac9143bb1_added_branch_sequences.py` & `krakenci_server-1.1.44/kraken/migrations/versions/4a7ac9143bb1_added_branch_sequences.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/5b13b262b132_added_repo_changes.py` & `krakenci_server-1.1.44/kraken/migrations/versions/5b13b262b132_added_repo_changes.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/5c16623f4d55_added_fields_masked_to_step.py` & `krakenci_server-1.1.44/kraken/migrations/versions/5c16623f4d55_added_fields_masked_to_step.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/5e38f55beb11_added_summary_to_flow.py` & `krakenci_server-1.1.44/kraken/migrations/versions/5e38f55beb11_added_summary_to_flow.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/6745adaf40e5_added_schema_repo_to_stage.py` & `krakenci_server-1.1.44/kraken/migrations/versions/6745adaf40e5_added_schema_repo_to_stage.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/735e81eedae4_change_project_id_in_executorgroup_to_.py` & `krakenci_server-1.1.44/kraken/migrations/versions/735e81eedae4_change_project_id_in_executorgroup_to_.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/818e190ca142_move_webhook_to_project.py` & `krakenci_server-1.1.44/kraken/migrations/versions/818e190ca142_move_webhook_to_project.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/8200318b9e18_added_several_stats_fields_to_run.py` & `krakenci_server-1.1.44/kraken/migrations/versions/8200318b9e18_added_several_stats_fields_to_run.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/87358b464400_added_casbin_rules_table.py` & `krakenci_server-1.1.44/kraken/migrations/versions/87358b464400_added_casbin_rules_table.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/899dadc28f9c_added_missing_indexes.py` & `krakenci_server-1.1.44/kraken/migrations/versions/899dadc28f9c_added_missing_indexes.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,36 +23,34 @@
     ('uq_system_name_executor', 'systems', 'name, executor'),
     ('ix_test_case_results_comment_id', 'test_case_results', 'comment_id'),
     ('ix_test_case_results_job_id', 'test_case_results', 'job_id')
 ]
 
 
 def upgrade():
-    conn = op.get_bind()
     for name, table, columns in INDEXES:
         if name.startswith('uq'):
             uq = ' UNIQUE '
             cmd = 'ALTER TABLE %s ADD CONSTRAINT %s UNIQUE (%s)' % (table, name, columns)
             with op.get_context().autocommit_block():
                 try:
-                    conn.execute(cmd)
+                    op.execute(cmd)
                 except Exception:
                     pass
         else:
             uq = ''
         cmd = "CREATE %s INDEX IF NOT EXISTS %s ON public.%s USING btree (%s);" % (uq, name, table, columns)
         print(cmd)
-        conn.execute(cmd)
+        op.execute(cmd)
     print('migration completed')
 
 
 def downgrade():
-    conn = op.get_bind()
     for name, table, _ in INDEXES:
         if name.startswith('uq'):
             cmd = 'ALTER TABLE %s DROP CONSTRAINT %s' % (table, name)
-            conn.execute(cmd)
+            op.execute(cmd)
         print('dropping index %s' % name)
         cmd = "DROP INDEX IF EXISTS %s;" % name
-        conn.execute(cmd)
+        op.execute(cmd)
         #op.drop_index(name, table_name=table)
     print('migration completed')
```

### Comparing `krakenci_server-1.0/kraken/migrations/versions/89ffd52f1f00_rename_executor_to_agent.py` & `krakenci_server-1.1.44/kraken/migrations/versions/89ffd52f1f00_rename_executor_to_agent.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/9666bf8c1bb0_added_details_to_user_session.py` & `krakenci_server-1.1.44/kraken/migrations/versions/9666bf8c1bb0_added_details_to_user_session.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/98af95844f27_added_results_change_stats_to_run.py` & `krakenci_server-1.1.44/kraken/migrations/versions/98af95844f27_added_results_change_stats_to_run.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/a0741baf2dbc_added_indexes_to_test_case_results.py` & `krakenci_server-1.1.44/kraken/migrations/versions/a0741baf2dbc_added_indexes_to_test_case_results.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/a26a02d0ac01_added_extra_atrs_to_agents.py` & `krakenci_server-1.1.44/kraken/migrations/versions/a26a02d0ac01_added_extra_atrs_to_agents.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/a35aec7afa0a_added_processed_at_in_run_and_index_to_.py` & `krakenci_server-1.1.44/kraken/migrations/versions/a35aec7afa0a_added_processed_at_in_run_and_index_to_.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/ab9326d5fc02_added_index_to_flows.py` & `krakenci_server-1.1.44/kraken/migrations/versions/ab9326d5fc02_added_index_to_flows.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,24 +25,22 @@
     ['ix_artifacts_run_id', 'artifacts', 'run_id'],
     # create INDEX ix_artifacts_flow_id on artifacts(flow_id);
     ['ix_artifacts_flow_id', 'artifacts', 'flow_id'],
 ]
 
 
 def upgrade():
-    conn = op.get_bind()
     for name, table, columns in INDEXES:
         print('creating index %s' % name)
         cmd = "CREATE INDEX IF NOT EXISTS %s ON %s (%s);" % (name, table, columns)
-        conn.execute(cmd)
+        op.execute(cmd)
         #op.create_index(name, table, columns)
     print('migration completed')
 
 
 def downgrade():
-    conn = op.get_bind()
     for name, _, _ in INDEXES:
         print('dropping index %s' % name)
         cmd = "DROP INDEX IF EXISTS %s;" % name
-        conn.execute(cmd)
+        op.execute(cmd)
         #op.drop_index(name, table_name=table)
     print('migration completed')
```

### Comparing `krakenci_server-1.0/kraken/migrations/versions/af348b43d9d5_extended_tool.py` & `krakenci_server-1.1.44/kraken/migrations/versions/af348b43d9d5_extended_tool.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/b2c9024746f5_added_unique_constraint_for_system_name_.py` & `krakenci_server-1.1.44/kraken/migrations/versions/b2c9024746f5_added_unique_constraint_for_system_name_.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/b5cc62f79980_add_extra_to_issue.py` & `krakenci_server-1.1.44/kraken/migrations/versions/b5cc62f79980_add_extra_to_issue.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/b84bdc5d3c67_uniqued_agent_address.py` & `krakenci_server-1.1.44/kraken/migrations/versions/b84bdc5d3c67_uniqued_agent_address.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/b908e219f07f_longer_message_in_issue.py` & `krakenci_server-1.1.44/kraken/migrations/versions/b908e219f07f_longer_message_in_issue.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/bb0d4908ba49_added_artifact_and_file.py` & `krakenci_server-1.1.44/kraken/migrations/versions/bb0d4908ba49_added_artifact_and_file.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/befa07ac5d1c_changed_tool_version_to_string.py` & `krakenci_server-1.1.44/kraken/migrations/versions/befa07ac5d1c_changed_tool_version_to_string.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 def upgrade():
     op.alter_column('tools', 'version',
                existing_type=sa.INTEGER(),
                type_=sa.UnicodeText(),
                existing_nullable=True)
     op.create_unique_constraint('uq_tool_name_version', 'tools', ['name', 'version'])
 
-    conn = op.get_bind()
-    conn.execute("UPDATE tools SET version = '1'")
+    op.execute("UPDATE tools SET version = '1'")
 
 
 def downgrade():
     op.drop_constraint('uq_tool_name_version', 'tools', type_='unique')
     op.alter_column('tools', 'version',
                existing_type=sa.UnicodeText(),
                type_=sa.INTEGER(),
```

### Comparing `krakenci_server-1.0/kraken/migrations/versions/cb7654d57bca_added_systems_table_and_host_info_user_.py` & `krakenci_server-1.1.44/kraken/migrations/versions/cb7654d57bca_added_systems_table_and_host_info_user_.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/ce05198f524a_convert_char_n_to_text.py` & `krakenci_server-1.1.44/kraken/migrations/versions/ce05198f524a_convert_char_n_to_text.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/cea0e48abb5a_added_retention_policy_to_branch.py` & `krakenci_server-1.1.44/kraken/migrations/versions/cea0e48abb5a_added_retention_policy_to_branch.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/d45087b62027_move_trigger_data_to_flow.py` & `krakenci_server-1.1.44/kraken/migrations/versions/d45087b62027_move_trigger_data_to_flow.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/d524cbcbf19c_added_users_and_users_session.py` & `krakenci_server-1.1.44/kraken/migrations/versions/d524cbcbf19c_added_users_and_users_session.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/dae910bd9587_added_repo_data_to_run.py` & `krakenci_server-1.1.44/kraken/migrations/versions/dae910bd9587_added_repo_data_to_run.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/e0d8421619c2_removed_unique_constraint_agent_non_.py` & `krakenci_server-1.1.44/kraken/migrations/versions/e0d8421619c2_removed_unique_constraint_agent_non_.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/e404f52562c2_added_unique_constraints_on_branch_name_.py` & `krakenci_server-1.1.44/kraken/migrations/versions/e404f52562c2_added_unique_constraints_on_branch_name_.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/migrations/versions/f566580fd139_added_test_case_comment_table.py` & `krakenci_server-1.1.44/kraken/migrations/versions/f566580fd139_added_test_case_comment_table.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/__init__.py` & `krakenci_server-1.1.44/kraken/server/__init__.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/access.py` & `krakenci_server-1.1.44/kraken/server/access.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/agentblob.py` & `krakenci_server-1.1.44/kraken/server/agentblob.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/authn.py` & `krakenci_server-1.1.44/kraken/server/authn.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/backend.py` & `krakenci_server-1.1.44/kraken/server/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from . import consts
 from .bg import jobs as bg_jobs
 from . import minioops
 from .. import version
 from . import kkrq
 from . import utils
 from . import dbutils
+from . import datastore
 
 log = logging.getLogger(__name__)
 
 JOB = {
     "name": "build-tarball",
     "id": 123,
     "steps": [{
@@ -306,15 +307,20 @@
     flag_modified(run, 'artifacts')
     db.session.commit()
 
     t1 = time.time()
     log.info('reporting %s artifacts took %ss', len(step.result['artifacts']), (t1 - t0))
 
 
-def destroy_machine_if_needed(agent, job):
+def _handle_data(job, step, result):
+    data = result['data']
+    return datastore.handle_data(job, step, data)
+
+
+def _destroy_machine_if_needed(agent, job):
     to_destroy = False
 
     # check if cloud machine should be destroyed now
     ag = dbutils.find_cloud_assignment_group(agent)
     if ag:
         # aws ec2
         if ag.deployment['method'] == consts.AGENT_DEPLOYMENT_METHOD_AWS_EC2:
@@ -407,18 +413,22 @@
     if 'test-results' in result:
         _store_results(job, step, result)
 
     # store issues
     if 'issues' in result:
         _store_issues(job, result)
 
-    # store issues
+    # store artifacts
     if 'artifacts' in result:
         _store_artifacts(job, step)
 
+    # set, update or get data
+    if 'data' in result:
+        _handle_data(job, step, result)
+
     # check if all steps are done so job is finised
     job_finished = True
     log.info('checking steps')
     for s in job.steps:
         log.info('%s: %s', s.index, consts.STEP_STATUS_NAME[s.status]
                  if s.status in consts.STEP_STATUS_NAME else s.status)
         if s.status == consts.STEP_STATUS_DONE:
@@ -429,15 +439,15 @@
         job_finished = False
         break
     if job_finished:
         job.state = consts.JOB_STATE_EXECUTING_FINISHED
         job.finished = utils.utcnow()
         agent.job = None
 
-        destroy_machine_if_needed(agent, job)
+        _destroy_machine_if_needed(agent, job)
 
         db.session.commit()
         kkrq.enq(bg_jobs.job_completed, job.id)
         log.info('job %s finished by %s', job, agent)
     else:
         response['timeout'] = _left_time(job)
```

### Comparing `krakenci_server-1.0/kraken/server/badge.py` & `krakenci_server-1.1.44/kraken/server/badge.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/bg/jobs.py` & `krakenci_server-1.1.44/kraken/server/bg/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import pytimeparse
 import redis
 
 from ..models import db, Run, Job, TestCaseResult, Branch, Flow, Stage, Project, get_setting
 from ..models import AgentsGroup, Agent, System, TestCaseComment, Tool
 from ..models import RepoChanges, Secret
 from ..schema import prepare_new_planner_triggers
-from ..schema import check_and_correct_stage_schema
+from ..schema import check_and_correct_stage_schema, prepare_context
 from ..cloud import cloud
 from .. import exec_utils  # pylint: disable=cyclic-import
 from .. import consts
 from .. import notify
 from .. import logs
 from .. import gitops
 from .. import kkrq
@@ -244,15 +244,15 @@
     q = q.filter_by(test_case_id=job_tcr.test_case_id)
     q = q.join('job')
     q = q.filter_by(covered=False)
     q = q.filter_by(agents_group=job.agents_group)
     q = q.filter_by(system=job.system)
     q = q.join('job', 'run', 'flow', 'branch')
     q = q.filter(Branch.id == job.run.flow.branch_id)
-    q = q.filter(Flow.kind == 0)  # CI
+    q = q.filter(Flow.kind == consts.FLOW_KIND_CI)
     q = q.filter(Flow.created < job.run.flow.created)
     q = q.order_by(desc(Flow.created))
     q = q.limit(10)
 
     # import sqlalchemy.dialects.postgresql
     # s = q.statement.compile(compile_kwargs={"literal_binds": True},
     #                         dialect=sqlalchemy.dialects.postgresql.dialect())
@@ -377,15 +377,15 @@
 
     counts = [0, 0, 0, 0]
     cnt = 0
     total = 0
     for job_tcr in q.all():
         t0 = time.time()
         # analyze history
-        if job.run.flow.kind == consts.FLOW_KIND_CI:  # CI
+        if job.run.flow.kind == consts.FLOW_KIND_CI:
             _analyze_ci_test_case_result(job, job_tcr)
         else:  # DEV
             _analyze_dev_test_case_result(job, job_tcr)
 
         db.session.commit()
 
         t1 = time.time()
@@ -409,15 +409,15 @@
     q = q.filter_by(completion_status=consts.JOB_CMPLT_ALL_OK)
     q = q.filter_by(system=job.system)
     q = q.filter_by(agents_group=job.agents_group)
     q = q.join('run')
     q = q.filter_by(stage=job.run.stage)
     q = q.join('run', 'flow')
     q = q.filter(Flow.created < job.run.flow.created)
-    q = q.filter(Flow.kind == 0)  # CI
+    q = q.filter(Flow.kind == consts.FLOW_KIND_CI)
     q = q.order_by(desc(Flow.created))
     prev_job = q.first()
     if prev_job is None:
         log.info('prev job for issues not found')
         return 0
 
     issues_new = 0
@@ -985,15 +985,16 @@
             else:
                 repo_access_token = None
 
             schema_code, version = gitops.get_schema_from_repo(stage.repo_url, stage.repo_branch, repo_access_token,
                                                                stage.schema_file, stage.git_clone_params)
 
             # check schema
-            schema_code, schema = check_and_correct_stage_schema(stage.branch, stage.name, schema_code)
+            ctx = prepare_context(stage, stage.get_default_args())
+            schema_code, schema = check_and_correct_stage_schema(stage.branch, stage.name, schema_code, ctx)
         except Exception as e:
             stage.repo_error = str(e)
             stage.repo_state = consts.REPO_STATE_ERROR
             db.session.commit()
             log.exception('problem with schema, stage: %d, run: %s',
                           stage_id, complete_starting_run_id)
             return
```

### Comparing `krakenci_server-1.0/kraken/server/chops.py` & `krakenci_server-1.1.44/kraken/server/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-# Copyright 2023 The Kraken Authors
+# Copyright 2021 The Kraken Authors
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
 
+import logging
+import datetime
 
-import os
-from urllib.parse import urlparse
+import pytz
 
-import clickhouse_driver
+log = logging.getLogger(__name__)
 
-from . import consts
 
+def utcnow():
+    return datetime.datetime.now(pytz.utc)
 
-def get_clickhouse_url():
-    ch_url = os.environ.get('KRAKEN_CLICKHOUSE_URL', consts.DEFAULT_CLICKHOUSE_URL)
-    return ch_url
 
-
-def get_clickhouse():
-    ch_url = get_clickhouse_url()
-    o = urlparse(ch_url)
-    ch = clickhouse_driver.Client(host=o.hostname)
-    return ch
+def split_host_port(addr, default_port):
+    parts = addr.split(':')
+    host = parts[0]
+    if len(parts) == 1:
+        if default_port is None:
+            raise Exception("format of address '%s' is incorrect" % addr)
+        port = default_port
+    else:
+        port = int(parts[1])
+    return host, port
```

### Comparing `krakenci_server-1.0/kraken/server/cloud/aws.py` & `krakenci_server-1.1.44/kraken/server/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/cloud/aws_ec2.py` & `krakenci_server-1.1.44/kraken/server/cloud/aws_ec2.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/cloud/aws_ecs.py` & `krakenci_server-1.1.44/kraken/server/cloud/aws_ecs.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/cloud/azure.py` & `krakenci_server-1.1.44/kraken/server/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/cloud/cloud.py` & `krakenci_server-1.1.44/kraken/server/cloud/cloud.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/cloud/common.py` & `krakenci_server-1.1.44/kraken/server/cloud/common.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/cloud/k8s.py` & `krakenci_server-1.1.44/kraken/server/cloud/k8s.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/consts.py` & `krakenci_server-1.1.44/kraken/server/consts.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,14 +95,19 @@
     RUN_STATE_REPLAY: 'replay',
     RUN_STATE_CREATING: 'creating',
 }
 
 FLOW_KIND_CI = 0
 FLOW_KIND_DEV = 1
 
+FLOW_KINDS_NAME = {
+    FLOW_KIND_CI: 'CI',
+    FLOW_KIND_DEV: 'DEV'
+}
+
 FLOW_STATE_IN_PROGRESS = 1
 FLOW_STATE_COMPLETED = 2
 
 FLOW_STATES_NAME = {
     FLOW_STATE_IN_PROGRESS: 'in-progress',
     FLOW_STATE_COMPLETED: 'completed'
 }
```

### Comparing `krakenci_server-1.0/kraken/server/dbutils.py` & `krakenci_server-1.1.44/kraken/server/dbutils.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/exec_utils.py` & `krakenci_server-1.1.44/kraken/server/exec_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import logging
 
 from sqlalchemy.orm.attributes import flag_modified
 from sqlalchemy.sql.expression import desc
 
 from . import consts
 from .models import db, BranchSequence, Flow, Run, Job, Step, AgentsGroup, Tool, Agent, AgentAssignment, System
-from .schema import check_and_correct_stage_schema, prepare_secrets, substitute_vars, substitute_val
+from .schema import check_and_correct_stage_schema, prepare_secrets, substitute_vars, substitute_val, prepare_context
 from . import dbutils
 from . import kkrq
 from . import utils
 
 log = logging.getLogger(__name__)
 
 
@@ -57,28 +57,28 @@
     db.session.commit()
     kkrq.enq(bg_jobs.job_completed, job.id)
     log.info('job %s canceled because: %s', job, note, job=job.id)
 
 
 def _increment_sequences(branch, stage, kind):
     if stage is None:
-        if kind == 0:  # CI
+        if kind == consts.FLOW_KIND_CI:
             seq1_kind = consts.BRANCH_SEQ_FLOW
             seq1_name = 'KK_FLOW_SEQ'
             seq2_kind = consts.BRANCH_SEQ_CI_FLOW
         else:
             seq1_kind = consts.BRANCH_SEQ_FLOW
             seq1_name = 'KK_FLOW_SEQ'
-            seq2_kind = consts.BRANCH_SEQ_CI_FLOW
+            seq2_kind = consts.BRANCH_SEQ_DEV_FLOW
         seq2_name = 'KK_CI_DEV_FLOW_SEQ'
     else:
-        if kind == 0:  # CI
+        if kind == consts.FLOW_KIND_CI:
             seq1_kind = consts.BRANCH_SEQ_RUN
             seq1_name = 'KK_RUN_SEQ'
-            seq2_kind = consts.BRANCH_SEQ_DEV_RUN
+            seq2_kind = consts.BRANCH_SEQ_CI_RUN
         else:
             seq1_kind = consts.BRANCH_SEQ_RUN
             seq1_name = 'KK_RUN_SEQ'
             seq2_kind = consts.BRANCH_SEQ_DEV_RUN
         seq2_name = 'KK_CI_DEV_RUN_SEQ'
 
     seq1 = BranchSequence.query.filter_by(branch=branch, stage=stage, kind=seq1_kind).one()
@@ -86,15 +86,17 @@
     seq2 = BranchSequence.query.filter_by(branch=branch, stage=stage, kind=seq2_kind).one()
     seq2.value = BranchSequence.value + 1
     db.session.commit()
 
     vals = {}
     vals[seq1_name] = str(seq1.value)
     vals[seq2_name] = str(seq2.value)
-    return vals
+
+    vals2 = {'shared': seq1.value, 'own': seq2.value}
+    return vals, vals2
 
 
 def complete_starting_run(run_id):
     run = Run.query.filter_by(id=run_id).one_or_none()
     if run is None:
         raise Exception('run %d cannot be found' % run_id)
 
@@ -114,25 +116,27 @@
         run_args = run.stage.get_default_args()
         if run.flow.args:
             run_args.update(run.flow.args)
         if run.args is not None:
             run_args.update(run.args)
 
         # increment sequences
-        seq_vals = _increment_sequences(run.flow.branch, run.stage, run.flow.kind)
+        seq_vals, seq_vals2 = _increment_sequences(run.flow.branch, run.stage, run.flow.kind)
         run_args.update(seq_vals)
+        run.seq = seq_vals2
 
         # prepare flow label if needed
         lbl_vals = {}
         for lbl_field in ['flow_label', 'run_label']:
             label_pattern = run.stage.schema.get(lbl_field, None)
             if label_pattern:
                 lbl_vals[lbl_field] = label_pattern
         if lbl_vals:
-            lbl_vals, _ = substitute_vars(lbl_vals, run_args)
+            ctx = prepare_context(run, run_args)
+            lbl_vals, _ = substitute_vars(lbl_vals, run_args, ctx)
             if run.flow.label is None:
                 run.flow.label = lbl_vals.get('flow_label', None)
 
         # if currently there is not repo data copy it from previous run if it is there
         repo_data = run.repo_data
         if not repo_data:
             prev_run = dbutils.get_prev_run(run.stage.id, run.flow.kind)
@@ -191,33 +195,35 @@
         complete_starting_run(run.id)
 
     return run
 
 
 def create_a_flow(branch, kind, body, trigger_data=None):
     if kind == 'dev':
-        kind = 1
+        kind = consts.FLOW_KIND_DEV
     else:
-        kind = 0
+        kind = consts.FLOW_KIND_CI
 
     args = body.get('args', {})
     flow_args = args.get('Common', {})
     branch_name = flow_args.get('BRANCH', branch.branch_name)
     if 'BRANCH' in flow_args:
         del flow_args['BRANCH']
 
     # increment sequences
-    seq_vals = _increment_sequences(branch, None, kind)
+    seq_vals, seq_vals2 = _increment_sequences(branch, None, kind)
     flow_args.update(seq_vals)
 
-    flow_args['KK_FLOW_TYPE'] = 'CI' if kind == 0 else 'DEV'
+    flow_args['KK_FLOW_TYPE'] = 'CI' if kind == consts.FLOW_KIND_CI else 'DEV'
     flow_args['KK_BRANCH'] = branch_name if branch_name else 'master'
+    flow_args['branch'] = flow_args['KK_BRANCH']
 
     # create flow instance
-    flow = Flow(branch=branch, kind=kind, branch_name=branch_name, args=flow_args, trigger_data=trigger_data)
+    flow = Flow(branch=branch, kind=kind, branch_name=branch_name, args=flow_args, trigger_data=trigger_data,
+                seq=seq_vals2)
     db.session.commit()
 
     log.set_ctx(flow_kind=flow.kind, flow=flow.id)
 
     log.info('created %s flow %s in branch %s',
              'ci' if kind == 0 else 'dev',
              flow, branch)
@@ -235,28 +241,17 @@
             continue
 
         start_run(stage, flow, reason=reason, args=args.get(stage.name, {}))
 
     return flow
 
 
-def _setup_schema_context(run):
-    ctx = {
-        'is_ci': run.flow.kind == 0,
-        'is_dev': run.flow.kind == 1,
-        'run_label': run.label,
-        'flow_label': run.flow.label,
-    }
-    return ctx
-
-
 def _reeval_schema(run):
-    context = _setup_schema_context(run)
-
-    schema_code, schema = check_and_correct_stage_schema(run.stage.branch, run.stage.name, run.stage.schema_code, context)
+    ctx = prepare_context(run, run.args)
+    schema_code, schema = check_and_correct_stage_schema(run.stage.branch, run.stage.name, run.stage.schema_code, ctx)
 
     run.stage.schema = schema
     run.stage.schema_code = schema_code
     flag_modified(run.stage, 'schema')
     db.session.commit()
 
 
@@ -288,151 +283,166 @@
 
     return timeout
 
 
 def trigger_jobs(run, replay=False):
     log.info('triggering jobs for run %s', run)
 
-    # reevaluate schema code
-    _reeval_schema(run)
+    try:
 
-    schema = run.stage.schema
+        # reevaluate schema code
+        _reeval_schema(run)
 
-    # find any prev jobs that will be covered by jobs triggered here in this function
-    if replay:
-        covered_jobs = _find_covered_jobs(run)
-
-    # prepare secrets to pass them to substitute in steps
-    secrets = prepare_secrets(run)
-
-    # prepare missing group
-    missing_agents_group = AgentsGroup.query.filter_by(name='missing').one_or_none()
-    if missing_agents_group is None:
-        missing_agents_group = AgentsGroup(name='missing')
-        db.session.commit()
-
-    # count how many agents are in each group, if there is 0 for given job then return an error
-    agents_count = {}
-
-    agents_needed = set()
-    created_systems = {}
-
-    # trigger new jobs based on jobs defined in stage schema
-    all_started_erred = True
-    now = utils.utcnow()
-    for j in schema['jobs']:
-        # check tools in steps
-        tools = []
-        tool_not_found = None
-        for idx, s in enumerate(j['steps']):
-            if '@' in s['tool']:
-                name, ver = s['tool'].split('@')
-                tool = Tool.query.filter_by(name=name, version=ver).one_or_none()
-            else:
-                tool = Tool.query.filter_by(name=s['tool']).order_by(desc(Tool.created)).first()
-            if tool is None:
-                tool_not_found = s['tool']
-                break
-            tools.append(tool)
-        if tool_not_found is not None:
-            log.warning('cannot find tool %s', tool_not_found)
-
-        envs = j['environments']
-        for env in envs:
-            # get agents group
-            ag_name, _ = substitute_val(env['agents_group'], run.args)
-            q = AgentsGroup.query
-            q = q.filter_by(project=run.stage.branch.project, name=ag_name)
-            agents_group = q.one_or_none()
+        schema = run.stage.schema
+
+        # find any prev jobs that will be covered by jobs triggered here in this function
+        if replay:
+            covered_jobs = _find_covered_jobs(run)
+
+        # prepare secrets to pass them to substitute in steps
+        secrets = prepare_secrets(run)
+
+        # prepare missing group
+        missing_agents_group = AgentsGroup.query.filter_by(name='missing').one_or_none()
+        if missing_agents_group is None:
+            missing_agents_group = AgentsGroup(name='missing')
+            db.session.commit()
+
+        # count how many agents are in each group, if there is 0 for given job then return an error
+        agents_count = {}
+
+        agents_needed = set()
+        created_systems = {}
+
+        run_ctx = prepare_context(run, run.args)
+
+        # trigger new jobs based on jobs defined in stage schema
+        all_started_erred = True
+        now = utils.utcnow()
+        for j in schema['jobs']:
+            # check tools in steps
+            tools = []
+            tool_not_found = None
+            for idx, s in enumerate(j['steps']):
+                if '@' in s['tool']:
+                    name, ver = s['tool'].split('@')
+                    tool = Tool.query.filter_by(name=name, version=ver).one_or_none()
+                else:
+                    tool = Tool.query.filter_by(name=s['tool']).order_by(desc(Tool.created)).first()
+                if tool is None:
+                    tool_not_found = s['tool']
+                    break
+                tools.append(tool)
+            if tool_not_found is not None:
+                log.warning('cannot find tool %s', tool_not_found)
+
+            envs = j['environments']
+            for env in envs:
+                # get agents group
+                ag_name, _ = substitute_val(env['agents_group'], run.args, run_ctx)
+                q = AgentsGroup.query
+                q = q.filter_by(project=run.stage.branch.project, name=ag_name)
+                agents_group = q.one_or_none()
 
-            if agents_group is None:
-                agents_group = AgentsGroup.query.filter_by(name=ag_name).one_or_none()
                 if agents_group is None:
-                    log.warning("cannot find agents group '%s'", ag_name)
+                    agents_group = AgentsGroup.query.filter_by(name=ag_name).one_or_none()
+                    if agents_group is None:
+                        log.warning("cannot find agents group '%s'", ag_name)
+
+                # get count of agents in the group
+                if agents_group is not None and agents_group.name not in agents_count:
+                    q = AgentAssignment.query.filter_by(agents_group=agents_group)
+                    q = q.join('agent')
+                    q = q.filter(Agent.disabled.is_(False))
+                    q = q.filter(Agent.authorized.is_(True))
+                    cnt = q.count()
+                    #log.info("agents group '%s' count is %d", agents_group.name, cnt)
+                    agents_count[agents_group.name] = cnt
 
-            # get count of agents in the group
-            if agents_group is not None and agents_group.name not in agents_count:
-                q = AgentAssignment.query.filter_by(agents_group=agents_group)
-                q = q.join('agent')
-                q = q.filter(Agent.disabled.is_(False))
-                q = q.filter(Agent.authorized.is_(True))
-                cnt = q.count()
-                #log.info("agents group '%s' count is %d", agents_group.name, cnt)
-                agents_count[agents_group.name] = cnt
-
-            if not isinstance(env['system'], list):
-                systems = [substitute_val(env['system'], run.args)[0]]
-            else:
-                systems = [substitute_val(s, run.args)[0] for s in env['system']]
-
-            for system_name in systems:
-                # prepare system and executor
-                if 'executor' in env:
-                    executor = env['executor'].lower()
+                if not isinstance(env['system'], list):
+                    systems = [substitute_val(env['system'], run.args, run_ctx)[0]]
                 else:
-                    executor = 'local'
-                system = System.query.filter_by(name=system_name, executor=executor).one_or_none()
-                sys_key = (system_name, executor)
-                if system is None:
-                    system = created_systems.get(sys_key, None)
-                if system is None:
-                    system = System(name=system_name, executor=executor)
-                    db.session.flush()
-                    # this is to avoid doing flush for the same system
-                    created_systems[sys_key] = system
-
-                # get timeout
-                timeout = _establish_timeout_for_job(j, run, system, agents_group)
-
-                # create job
-                job = Job(run=run, name=j['name'], agents_group=agents_group, system=system, timeout=timeout)
-
-                erred_job = False
-                if tool_not_found:
-                    job.state = consts.JOB_STATE_COMPLETED
-                    job.completion_status = consts.JOB_CMPLT_MISSING_TOOL_IN_DB
-                    job.notes = "cannot find tool '%s' in database" % tool_not_found
-                    erred_job = True
-                if agents_group is None:
-                    job.agents_group = missing_agents_group
-                    if job.state != consts.JOB_STATE_COMPLETED:
-                        job.state = consts.JOB_STATE_COMPLETED
-                        job.completion_status = consts.JOB_CMPLT_MISSING_AGENTS_GROUP
-                        job.notes = "cannot find agents group '%s' in database" % ag_name
-                    erred_job = True
-                elif agents_group.deployment and agents_group.deployment['method'] > 0:
-                    agents_needed.add(agents_group.id)
-                elif agents_count[agents_group.name] == 0:
-                    if job.state != consts.JOB_STATE_COMPLETED:
-                        job.state = consts.JOB_STATE_COMPLETED
-                        job.completion_status = consts.JOB_CMPLT_NO_AGENTS
-                        job.notes = "there are no agents in group '%s' - add some agents" % agents_group.name
-                    erred_job = True
-
-                if not erred_job:
-                    all_started_erred = False
-                    # substitute vars in steps
-                    for idx, s in enumerate(j['steps']):
-                        args = secrets.copy()
-                        if run.args:
-                            args.update(run.args)
-                        fields, fields_masked = substitute_vars(s, args)
-                        del fields['tool']
-                        Step(job=job, index=idx, tool=tools[idx], fields=fields, fields_masked=fields_masked)
-
-                # if this is rerun/replay then mark prev jobs as covered
-                if replay:
-                    key = '%s-%s' % (j['name'], agents_group.id)
-                    if key in covered_jobs:
-                        for cj in covered_jobs[key]:
-                            cj.covered = True
-                            # TODO: we should cancel these jobs if they are still running
+                    systems = [substitute_val(s, run.args, run_ctx)[0] for s in env['system']]
+
+                for system_name in systems:
+                    # prepare system and executor
+                    if 'executor' in env:
+                        executor = env['executor'].lower()
+                    else:
+                        executor = 'local'
+                    system = System.query.filter_by(name=system_name, executor=executor).one_or_none()
+                    sys_key = (system_name, executor)
+                    if system is None:
+                        system = created_systems.get(sys_key, None)
+                    if system is None:
+                        system = System(name=system_name, executor=executor)
+                        db.session.flush()
+                        # this is to avoid doing flush for the same system
+                        created_systems[sys_key] = system
 
-                db.session.commit()
-                log.info('created job %s', job.get_json(mask_secrets=True))
+                    # get timeout
+                    timeout = _establish_timeout_for_job(j, run, system, agents_group)
+
+                    # create job
+                    job = Job(run=run, name=j['name'], agents_group=agents_group, system=system, timeout=timeout)
+
+                    erred_job = False
+                    if tool_not_found:
+                        job.state = consts.JOB_STATE_COMPLETED
+                        job.completion_status = consts.JOB_CMPLT_MISSING_TOOL_IN_DB
+                        job.notes = "cannot find tool '%s' in database" % tool_not_found
+                        erred_job = True
+                    if agents_group is None:
+                        job.agents_group = missing_agents_group
+                        if job.state != consts.JOB_STATE_COMPLETED:
+                            job.state = consts.JOB_STATE_COMPLETED
+                            job.completion_status = consts.JOB_CMPLT_MISSING_AGENTS_GROUP
+                            job.notes = "cannot find agents group '%s' in database" % ag_name
+                        erred_job = True
+                    elif agents_group.deployment and agents_group.deployment['method'] > 0:
+                        agents_needed.add(agents_group.id)
+                    elif agents_count[agents_group.name] == 0:
+                        if job.state != consts.JOB_STATE_COMPLETED:
+                            job.state = consts.JOB_STATE_COMPLETED
+                            job.completion_status = consts.JOB_CMPLT_NO_AGENTS
+                            job.notes = "there are no agents in group '%s' - add some agents" % agents_group.name
+                        erred_job = True
+
+                    if not erred_job:
+                        all_started_erred = False
+                        # substitute vars in steps
+                        for idx, s in enumerate(j['steps']):
+                            args = secrets.copy()
+                            if run.args:
+                                args.update(run.args)
+                            step = Step(job=job, index=idx, tool=tools[idx], fields={}, fields_masked={})
+                            step_ctx = prepare_context(step, args)
+                            fields, fields_masked = substitute_vars(s, args, step_ctx)
+                            del fields['tool']
+                            step.fields = fields
+                            step.fields_masked = fields_masked
+
+                    # if this is rerun/replay then mark prev jobs as covered
+                    if replay:
+                        key = '%s-%s' % (j['name'], agents_group.id)
+                        if key in covered_jobs:
+                            for cj in covered_jobs[key]:
+                                cj.covered = True
+                                # TODO: we should cancel these jobs if they are still running
+
+                    db.session.commit()
+                    log.info('created job %s', job.get_json(mask_secrets=True))
+
+    except Exception as ex:
+        log.exception('Problem with starting jobs')
+        now = utils.utcnow()
+        run.started = now
+        run.note = "Triggering run's jobs failed: %s" % str(ex)
+        complete_run(run, now)
+        return
 
     run.started = now
     run.state = consts.RUN_STATE_IN_PROGRESS  # need to be set in case of replay
     db.session.commit()
 
     from .bg import jobs as bg_jobs  # pylint: disable=import-outside-toplevel
```

### Comparing `krakenci_server-1.0/kraken/server/execution.py` & `krakenci_server-1.1.44/kraken/server/execution.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import time
+import json
 import logging
 from urllib.parse import urljoin
 
 from flask import abort
 from sqlalchemy.sql.expression import asc, desc
 from sqlalchemy.orm import joinedload
 
 from . import consts
+from . import kkrq
 from . import utils
-from .models import db, Branch, Flow, Run, Stage, Job, Step
-from .models import Issue, Artifact, Agent
+from .models import db, Project, Branch, Flow, Run, Stage, Job, Step
+from .models import Issue, Artifact
 from .schema import SchemaError
 from . import exec_utils
 from . import access
 from . import chops
 
 log = logging.getLogger(__name__)
 
@@ -179,14 +181,33 @@
         abort(400, str(e))
 
     data = run.get_json()
 
     return data, 200
 
 
+def force_run_analysis(run_id, token_info=None):
+    run = Run.query.filter_by(id=run_id).one_or_none()
+    if run is None:
+        abort(404, "Run not found")
+    access.check(token_info, run.stage.branch.project_id, 'pwrusr',
+                 'only superadmin, project admin and project power roles can run jobs')
+
+    log.set_ctx(branch=run.flow.branch_id, flow_kind=run.flow.kind, flow=run.flow_id, run=run.id)
+
+    log.info('force analysis of run %s', run)
+
+    from .bg import jobs as bg_jobs  # pylint: disable=import-outside-toplevel
+    kkrq.enq_neck(bg_jobs.analyze_run, run.id)
+
+    data = run.get_json()
+
+    return data, 200
+
+
 def job_rerun(job_id, token_info=None):
     job = Job.query.filter_by(id=job_id).one_or_none()
     if job is None:
         abort(404, "Job not found")
     access.check(token_info, job.run.stage.branch.project_id, 'pwrusr',
                  'only superadmin, project admin and project power roles can rerun a job')
 
@@ -443,136 +464,43 @@
 
     return {'items': logs, 'total': total, 'job': job_json}, 200
 
 
 def get_logs(branch_id=None, flow_kind=None, flow_id=None, run_id=None, job_id=None, step_idx=None,
              agent_id=None, services=None, level=None,
              start=0, limit=200, order=None, token_info=None):  # pylint: disable=unused-argument
-    if order not in [None, 'asc', 'desc']:
-        abort(400, "incorrect order value: %s" % str(order))
-
     if start < 0:
         abort(400, "incorrect start value: %s" % str(start))
 
     if limit < 0:
         abort(400, "incorrect limit value: %s" % str(limit))
 
-    if branch_id is None and flow_id is None and run_id is None and job_id is None and agent_id is None:
-        access.check(token_info, '', 'admin',
-                     'only superadmin can get services logs')
-
-    if branch_id is None and flow_kind is not None:
-        abort(400, "if flow_kind is provided then branch_id must be provided as well")
-
-    if job_id is None and step_idx is not None:
-        abort(400, "if step_idx is provided then job_id must be provided as well")
-
-    if job_id is not None:
-        job = Job.query.filter_by(id=job_id).one_or_none()
-        if job is None:
-            abort(404, "Job not found")
-        access.check(token_info, job.run.stage.branch.project_id, 'view',
-                     'only superadmin, project admin, project power and project viewer user roles can get job logs')
-
-    elif run_id is not None:
-        run = Run.query.filter_by(id=run_id).one_or_none()
-        if run is None:
-            abort(404, "Run not found")
-        access.check(token_info, run.stage.branch.project_id, 'view',
-                     'only superadmin, project admin, project power and project viewer user roles can get run logs')
-
-    elif flow_id is not None:
-        flow = Flow.query.filter_by(id=flow_id).one_or_none()
-        if flow is None:
-            abort(404, "Flow not found")
-        access.check(token_info, flow.branch.project_id, 'view',
-                     'only superadmin, project admin, project power and project viewer user roles can get flow logs')
-
-    elif branch_id is not None:
-        branch = Branch.query.filter_by(id=branch_id).one_or_none()
-        if branch is None:
-            abort(404, "Branch not found")
-        access.check(token_info, branch.project_id, 'view',
-                     'only superadmin, project admin, project power and project viewer user roles can get branch logs')
-
-    if agent_id is not None:
-        agent = Agent.query.filter_by(id=agent_id).one_or_none()
-        if agent is None:
-            abort(404, "Agent not found")
-        access.check(token_info, '', 'admin',
-                     'only superadmin can get agent logs')
-
-    ch = chops.get_clickhouse()
+    if order not in [None, 'asc', 'desc']:
+        abort(400, "incorrect order value: %s" % str(order))
 
     if order is None:
         order = 'asc'
 
-    params = dict(start=start, limit=limit)
+    _, where_clause, params = chops.prepare_logs_query(
+        branch_id, flow_kind, flow_id, run_id, job_id, step_idx,
+        agent_id, services, level, token_info)
 
-    where_clauses = []
-    if branch_id is not None:
-        where_clauses.append('branch = %(branch_id)d')
-        params['branch_id'] = branch_id
-        if flow_kind is not None:
-            where_clauses.append('flow_kind = %(flow_kind)d')
-            params['flow_kind'] = flow_kind
-    if flow_id is not None:
-        where_clauses.append('flow = %(flow_id)d')
-        params['flow_id'] = flow_id
-    if run_id is not None:
-        where_clauses.append('run = %(run_id)d')
-        params['run_id'] = run_id
-    if job_id is not None:
-        where_clauses.append('job = %(job_id)d')
-        params['job_id'] = job_id
-        if step_idx is not None:
-            where_clauses.append('step_idx = %(step_idx)d')
-            params['step_idx'] = step_idx
-    if agent_id is not None:
-        where_clauses.append('agent = %(agent_id)d')
-        params['agent_id'] = agent_id
-
-    where_services = []
-    if services:
-        for idx, s in enumerate(services):
-            param = 'service%d' % idx
-            if '/' in s:
-                s, t = s.split('/')
-                tparam = 'tool%d' % idx
-                where_services.append("(service = %%(%s)s and tool = %%(%s)s)" % (param, tparam))
-                params[param] = s
-                params[tparam] = t
-            else:
-                where_services.append("service = %%(%s)s" % param)
-                params[param] = s
-        where = " or ".join(where_services)
-        where = "(" + where + ") "
-        where_clauses.append(where)
-
-    if level:
-        level = level.upper()
-        if level == 'ERROR':
-            lq = "level = 'ERROR'"
-        elif level == 'WARNING':
-            lq = "level in ('WARNING', 'ERROR')"
-        else:
-            lq = "level in ('INFO', 'WARNING', 'ERROR')"
-        where_clauses.append(lq)
+    params['start'] = start
+    params['limit'] = limit
 
-    where_clause = 'where ' + ' and '.join(where_clauses)
+    ch = chops.get_clickhouse()
 
     # get total first
     total_query = "SELECT count(*) FROM logs %s" % where_clause
     resp = ch.execute(total_query, params)
     total = resp[0][0]
 
     # get logs now
     query = "SELECT time,message,service,host,path,lineno,level,branch,flow_kind,flow,run,job,tool,step,agent "
-    query += " FROM logs %s ORDER BY time %s, seq %s LIMIT %%(start)d, %%(limit)d"
-    query %= (where_clause, order, order)
+    query += f" FROM logs {where_clause} ORDER BY time {order}, seq {order} LIMIT %(start)d, %(limit)d"
     log.info('CH query %s', query)
     log.info('CH params %s', params)
     rows = ch.execute(query, params)
 
     logs = []
     for r in rows:
         entry = dict(time=r[0],
@@ -650,7 +578,34 @@
     total = q.count()
     q = q.order_by(desc('id'))
     q = q.offset(start).limit(limit)
     jobs = []
     for j in q.all():
         jobs.append(j.get_json())
     return {'items': jobs, 'total': total}, 200
+
+
+def get_user_data(scope, entity_id, token_info=None):
+    if scope == 'flow':
+        flow = Flow.query.filter_by(id=entity_id).one_or_none()
+        data = flow.user_data
+        project_id = flow.branch.project_id
+    elif scope.startswith('branch'):
+        branch = Branch.query.filter_by(id=entity_id).one_or_none()
+        if scope == 'branch-ci':
+            data = branch.user_data_ci
+        elif scope == 'branch-dev':
+            data = branch.user_data_dev
+        elif scope == 'branch':
+            data = branch.user_data
+        project_id = branch.project_id
+    elif scope == 'project':
+        project = Project.query.filter_by(id=entity_id).one_or_none()
+        data = project.user_data
+        project_id = project.id
+
+    access.check(token_info, project_id, 'view',
+                 'only superadmin, project admin, project power and project viewer user roles can get branch logs')
+
+    resp = dict(data=json.dumps(data, indent=4))
+
+    return resp, 200
```

### Comparing `krakenci_server-1.0/kraken/server/gitops.py` & `krakenci_server-1.1.44/kraken/server/gitops.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/initdb.py` & `krakenci_server-1.1.44/kraken/server/initdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from passlib.hash import pbkdf2_sha256
 
 from .models import db, Branch, Stage, AgentsGroup, Setting, Tool, Project
 from .models import User, BranchSequence, System
-from .schema import execute_schema_code
+from .schema import execute_schema_code, prepare_context
 from . import consts
 
 
 # pylint: disable=line-too-long
 
 
 INITIAL_SETTINGS = {
@@ -532,14 +532,60 @@
                 "cwd": {
                     "description": "A current working directory where the step is executed.",
                     "default": ".",
                     "type": "string"
                 }
             }
         }
+    }, {
+        "name": "data",
+        "description": "A tool that allows for storing (setting and updating) JSON data server-side.",
+        "location": "",
+        "entry": "",
+        "version": "1",
+        "parameters": {
+            "properties": {
+                "file": {
+                    "description": "A file with data with JSON format in case of `set` and `jsonpatch` operations and JQ expression in case of `jq` operation.",
+                    "type": "string"
+                },
+                "cwd": {
+                    "description": "A current working directory where the step is executed.",
+                    "default": ".",
+                    "type": "string"
+                },
+                "value": {
+                    "description": "The sama data as in file field but provided directly. Alternative to file field.",
+                    "default": "",
+                    "type": "string"
+                },
+                "operation": {
+                    "description":
+                        "An operation that should be performed. `set` sets data, `jq` executes JQ expression on server-side data,"
+                        " `jsonpatch` patches server-side data, `get` retrieve data from server in JSON format.",
+                    "default": "set",
+                    "type": "string",
+                    "enum": ["set", "jq", "jsonpatch", "get"]
+                },
+                "json_pointer": {
+                    "description": "A JSON pointer that indicates data (see RFC 6901). If `/` then whole data is taken, if key name is provided then data under this key is taken.",
+                    "default": "/",
+                    "type": "string"
+                },
+                "scope": {
+                    "description":
+                       "A scope of data: `flow` - data attached to a flow, `branch-ci` - data attached to a branch but related with CI flows,"
+                       " `branch-dev` - data attached to a branch but related with CI flows, `branch` - data attached to a branch,"
+                       " `project` - data attached to a project",
+                    "default": "flow",
+                    "type": "string",
+                    "enum": ["flow", "branch-ci", "branch-dev", "branch", "project"]
+                }
+            }
+        }
     }]
     for td in tool_defs:
         tool = Tool.query.filter_by(name=td['name'], version=td['version']).one_or_none()
         if tool is None:
             tool = Tool(name=td['name'],
                         description=td['description'],
                         location=td['location'],
@@ -616,22 +662,23 @@
             "environments": [{
                 "system": "any",
                 "agents_group": "all",
                 "config": "default"
             }]
         }]
     }'''
+    ctx = prepare_context(branch, {})
     if stage is None:
         stage = Stage(name='Tests', description="This is a stage of tests.", branch=branch,
-                      schema_code=schema_code, schema=execute_schema_code(branch, schema_code))
+                      schema_code=schema_code, schema=execute_schema_code(schema_code, ctx))
         db.session.commit()
         print("   created Stage record 'Tests'")
     else:
         stage.schema_code = schema_code
-        stage.schema = execute_schema_code(branch, schema_code)
+        stage.schema = execute_schema_code(schema_code, ctx)
         db.session.commit()
 
 
     for seq_type in [consts.BRANCH_SEQ_RUN, consts.BRANCH_SEQ_CI_RUN, consts.BRANCH_SEQ_DEV_RUN]:
         bs = BranchSequence.query.filter_by(branch=branch, stage=stage, kind=seq_type).one_or_none()
         if bs is None:
             BranchSequence(branch=branch, stage=stage, kind=seq_type, value=0)
```

### Comparing `krakenci_server-1.0/kraken/server/kkrq.py` & `krakenci_server-1.1.44/kraken/server/kkrq.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,20 +76,20 @@
     jobs_ids = q.deferred_job_registry.get_job_ids()
     deferred_jobs = rq.job.Job.fetch_many(jobs_ids, connection=rds)
 
     return scheduled_jobs, started_jobs, finished_jobs, failed_jobs, deferred_jobs
 
 
 # TODO: it does not work because rq always traces the exception
-# def _exception_handler(job, exc_type, exc_value, traceback):  # pylint: disable=unused-argument
-#     ignore_excs = ['ix_agents_address']
-#     for ex in ignore_excs:
-#         if ex in str(exc_value) or ex in str(traceback):
-#             return
-#     log.exception('IGNORED')
+def _exception_handler(job, exc_type, exc_value, traceback):  # pylint: disable=unused-argument
+    ignore_excs = ['ix_agents_address']
+    for ex in ignore_excs:
+        if ex in str(exc_value) or ex in str(traceback):
+            return
+    log.exception('IGNORED')
 
 
 def main():
     # check deps
     planner_url = os.environ.get('KRAKEN_PLANNER_URL', consts.DEFAULT_PLANNER_URL)
     srvcheck.wait_for_service('planner', planner_url, 7997)
 
@@ -114,13 +114,13 @@
     db.init_app(app)
 
     # setup sentry
     with app.app_context():
         sentry_url = get_setting('monitoring', 'sentry_dsn')
         logs.setup_sentry(sentry_url)
 
-    worker = rq.Worker('kq', connection=rds)  # , exception_handlers=[_exception_handler])  TODO: see above
+    worker = rq.Worker('kq', connection=rds, exception_handlers=[_exception_handler])
     worker.work(with_scheduler=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `krakenci_server-1.0/kraken/server/logs.py` & `krakenci_server-1.1.44/kraken/server/logs.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/management.py` & `krakenci_server-1.1.44/kraken/server/management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020-2022 The Kraken Authors
+# Copyright 2020-2023 The Kraken Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -31,15 +31,15 @@
 from azure.mgmt.compute import ComputeManagementClient
 
 from . import consts, srvcheck, kkrq
 from .models import db, Branch, Stage, Agent, AgentsGroup, Secret, AgentAssignment, Setting
 from .models import Project, BranchSequence, System, Flow, duration_to_txt
 from .models import Tool
 from .schema import check_and_correct_stage_schema, SchemaError, execute_schema_code
-from .schema import prepare_new_planner_triggers
+from .schema import prepare_new_planner_triggers, prepare_context
 from .cloud import aws, azure, k8s
 from ..version import version as server_version
 from . import toolutils
 from . import notify
 from . import utils
 from . import minioops
 from . import schemaval
@@ -360,14 +360,16 @@
         rsp['avg_duration_last_month'] = None
         rsp['avg_duration_last_week'] = None
         rsp['durations'] = []
         if rsp['flows_last_month'] > 0:
             q2 = q.filter(Flow.finished.is_not(None))
             q2 = q2.with_entities(func.avg(extract('epoch', Flow.finished) - extract('epoch', Flow.created)).label('average'))
             secs = q2.filter(Flow.created >= month_ago).all()[0][0]
+            if secs is None:
+                secs = 0
             dur = datetime.timedelta(seconds=secs)
             rsp['avg_duration_last_month'] = duration_to_txt(dur)
             if rsp['flows_last_week'] > 0:
                 secs = q2.filter(Flow.created >= week_ago).all()[0][0]
                 if secs:
                     dur = datetime.timedelta(seconds=secs)
                     rsp['avg_duration_last_week'] = duration_to_txt(dur)
@@ -475,16 +477,17 @@
     access.check(token_info, branch.project_id, 'pwrusr',
                  'only superadmin, project admin and project power user roles can create a stage')
 
     schema_code = None
     if 'schema_code' in body:
         schema_code = body['schema_code']
 
+    ctx = prepare_context(branch, {})
     try:
-        schema_code, schema = check_and_correct_stage_schema(branch, body['name'], schema_code)
+        schema_code, schema = check_and_correct_stage_schema(branch, body['name'], schema_code, ctx)
     except SchemaError as e:
         abort(400, str(e))
 
     # create record
     stage = Stage(branch=branch, name=body['name'], schema=schema, schema_code=schema_code)
     BranchSequence(branch=branch, stage=stage, kind=consts.BRANCH_SEQ_RUN, value=0)
     BranchSequence(branch=branch, stage=stage, kind=consts.BRANCH_SEQ_CI_RUN, value=0)
@@ -527,16 +530,17 @@
         stage.description = body['description']
 
     if 'enabled' in body:
         stage.enabled = body['enabled']
 
     if 'schema_code' in body:
         prev_triggers = stage.schema['triggers']
+        ctx = prepare_context(stage, stage.get_default_args())
         try:
-            schema_code, schema = check_and_correct_stage_schema(stage.branch, body['name'], body['schema_code'])
+            schema_code, schema = check_and_correct_stage_schema(stage.branch, body['name'], body['schema_code'], ctx)
         except SchemaError as e:
             abort(400, str(e))
         stage.schema = schema
         stage.schema_code = schema_code
         flag_modified(stage, 'schema')
         if stage.triggers is None:
             stage.triggers = {}
@@ -553,15 +557,15 @@
     db.session.commit()
 
     if schema_from_repo_enabled:
         if 'repo_url' in body:
             stage.repo_url = body['repo_url']
         if 'repo_branch' in body:
             stage.repo_branch = body['repo_branch']
-        if 'repo_access_token' in body:
+        if 'repo_access_token' in body and body['repo_access_token']:
             repo_access_token = body['repo_access_token']
             secret = Secret.query.filter_by(project=stage.branch.project, name=repo_access_token).one_or_none()
             if secret is None:
                 abort(400, "Secret '%s' for access token does not exist" % repo_access_token)
             if secret.kind != consts.SECRET_KIND_SIMPLE:
                 abort(400, "Type of '%s' access token secret should be Simple Secret" % repo_access_token)
             stage.repo_access_token = repo_access_token
@@ -621,15 +625,16 @@
     if stage is None:
         abort(404, "Stage not found")
 
     access.check(token_info, stage.branch.project_id, 'view',
                  'only superadmin, project admin, project power user and project viewer roles can get a stage')
 
     try:
-        schema = execute_schema_code(stage.branch, schema_code['schema_code'])
+        ctx = prepare_context(stage.branch, {})
+        schema = execute_schema_code(schema_code['schema_code'], ctx)
     except Exception as e:
         return dict(stage_id=stage_id, error=str(e)), 200
 
     schema = json.dumps(schema, indent=4, separators=(',', ': '))
 
     return dict(stage_id=stage_id, schema=schema), 200
 
@@ -1173,14 +1178,41 @@
                      level=r[4],
                      tool=r[5])
         logs.append(entry)
 
     return {'items': logs, 'total': len(logs)}, 200
 
 
+def create_rq_entry(body, token_info=None):
+    access.check(token_info, '', 'admin',
+                 'only superadmin can create RQ entry')
+
+    func_name = body['func_name']
+    args = body['args']
+
+    from .bg import jobs as bg_jobs  # pylint: disable=import-outside-toplevel
+    func_ptr = getattr(bg_jobs, func_name, None)
+    if func_ptr is None:
+        abort(400, 'Unknown function %s' % func_name)
+
+    args = args.split(',')
+    args = [a.strip() for a in args]
+    args2 = []
+    for a in args:
+        try:
+            a = int(a)
+        except Exception:
+            pass
+        args2.append(a)
+
+    kkrq.enq_neck(func_ptr, *args2)
+
+    return {}, 201
+
+
 def get_live_data():
     redis_addr = os.environ.get('KRAKEN_REDIS_ADDR', consts.DEFAULT_REDIS_ADDR)
     redis_host, redis_port = utils.split_host_port(redis_addr, 6379)
     rds = redis.Redis(host=redis_host, port=redis_port, db=consts.REDIS_KRAKEN_DB)
 
     counters = {
         'error_logs_count': 0,
```

### Comparing `krakenci_server-1.0/kraken/server/minioops.py` & `krakenci_server-1.1.44/kraken/server/minioops.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/models.py` & `krakenci_server-1.1.44/kraken/server/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,27 +63,34 @@
     id = Column(Integer, primary_key=True)
     name = Column(UnicodeText)
     description = Column(UnicodeText)
     branches = relationship("Branch", back_populates="project", order_by="Branch.created")
     secrets = relationship("Secret", back_populates="project", order_by="Secret.name")
     agents_groups = relationship("AgentsGroup", back_populates="project")
     webhooks = Column(JSONB)
+    user_data = Column(JSONB, default={})
 
-    def get_json(self, with_results=False, with_last_results=False):
-        branches = [b.get_json(with_results=with_results, with_last_results=with_last_results) for b in self.branches if b.deleted is None]
-        branches.sort(key=lambda b: b['name'])
-        return dict(id=self.id,
+    def get_json(self, with_branches=True, with_results=False, with_last_results=False, with_user_data=False):
+        data = dict(id=self.id,
                     created=self.created.strftime("%Y-%m-%dT%H:%M:%SZ") if self.created else None,
                     deleted=self.deleted.strftime("%Y-%m-%dT%H:%M:%SZ") if self.deleted else None,
                     name=self.name,
                     description=self.description,
-                    branches=branches,
                     secrets=[s.get_json() for s in self.secrets if s.deleted is None],
                     webhooks=self.webhooks if self.webhooks else {})
 
+        if with_branches:
+            branches = [b.get_json(with_results=with_results, with_last_results=with_last_results) for b in self.branches if b.deleted is None]
+            branches.sort(key=lambda b: b['name'])
+            data['branches'] = branches
+
+        if with_user_data:
+            data['data'] = self.user_data
+
+        return data
 
 class Branch(db.Model, DatesMixin):
     __tablename__ = "branches"
     id = Column(Integer, primary_key=True)
     name = Column(UnicodeText)  # display name
     project_id = Column(Integer, ForeignKey('projects.id'), nullable=False)
     project = relationship('Project', back_populates="branches")
@@ -96,18 +103,21 @@
     ci_last_completed_flow = relationship('Flow', foreign_keys=[ci_last_completed_flow_id])
     ci_last_incomplete_flow_id = Column(Integer, ForeignKey('flows.id'))
     ci_last_incomplete_flow = relationship('Flow', foreign_keys=[ci_last_incomplete_flow_id])
     stages = relationship("Stage", back_populates="branch", order_by="Stage.name")
     sequences = relationship("BranchSequence", back_populates="branch")
     comments = relationship("TestCaseComment", back_populates="branch")
     retention_policy = Column(JSONB)
+    user_data = Column(JSONB, default={})
+    user_data_ci = Column(JSONB, default={})
+    user_data_dev = Column(JSONB, default={})
 
     #base_branch = relationship('BaseBranch', uselist=False, primaryjoin="or_(Branch.id==BaseBranch.ci_branch_id, Branch.id==BaseBranch.dev_branch_id)")
 
-    def get_json(self, with_results=False, with_cfg=False, with_last_results=False):
+    def get_json(self, with_results=False, with_cfg=False, with_last_results=False, with_user_data=False):
         if self.retention_policy:
             retention_policy = self.retention_policy
         else:
             retention_policy = dict(ci_logs=6,
                                     dev_logs=3,
                                     ci_artifacts=6,
                                     dev_artifacts=3)
@@ -143,14 +153,20 @@
                               label=f.label,
                               created=f.created.strftime("%Y-%m-%dT%H:%M:%SZ"),
                               errors=any((r.jobs_error > 0 for r in f.runs)))
                 data['last_incomplete_flow'] = f_json
 
         if with_cfg:
             data['stages'] = [s.get_json() for s in self.stages if s.deleted is None]
+
+        if with_user_data:
+            data['data'] = self.user_data
+            data['data_ci'] = self.user_data_ci
+            data['data_dev'] = self.user_data_dev
+
         return data
 
 Index('ix_branches_name_project_id_not_deleted', Branch.name, Branch.project_id, postgresql_where=Branch.deleted.is_(None), unique=True)
 
 
 # Sequence kinds:
 # 0. KK_FLOW_SEQ
@@ -324,21 +340,29 @@
     artifacts = Column(JSONB, default={})
     label = Column(UnicodeText)
     trigger_data_id = Column(Integer, ForeignKey('repo_changes.id'))
     trigger_data = relationship('RepoChanges')
     artifacts_files = relationship('Artifact', back_populates="flow")
     comments = relationship("TestCaseComment", back_populates="last_flow")
     summary = Column(JSONB, default={})
+    user_data = Column(JSONB, default={})
+    seq = Column(JSONB, default={})
 
     Index('ix_flows_branch_id_kind', branch_id, kind)
 
+    def __repr__(self):
+        return "<Flow %s, label %s, kind %s, state %s>" % (self.id,
+                                                           self.get_label(),
+                                                           consts.FLOW_KINDS_NAME.get(self.kind, 'unknown %d' % self.kind),
+                                                           consts.FLOW_STATES_NAME.get(self.state, 'unknown %d' % self.state))
+
     def get_label(self):
         return self.label if self.label else ("%d." % self.id)
 
-    def get_json(self, with_project=True, with_branch=True, with_schema=True):
+    def get_json(self, with_project=True, with_branch=True, with_schema=True, with_user_data=False, with_stages=True, with_runs=True):
         if self.state == consts.FLOW_STATE_COMPLETED:
             duration = self.finished - self.created
         else:
             duration = utils.utcnow() - self.created
 
         trigger = None
         if self.trigger_data:
@@ -346,34 +370,44 @@
 
         data = dict(id=self.id,
                     label=self.get_label(),
                     created=self.created.strftime("%Y-%m-%dT%H:%M:%SZ") if self.created else None,
                     finished=self.finished.strftime("%Y-%m-%dT%H:%M:%SZ") if self.finished else None,
                     deleted=self.deleted.strftime("%Y-%m-%dT%H:%M:%SZ") if self.deleted else None,
                     state=consts.FLOW_STATES_NAME[self.state],
-                    kind='ci' if self.kind == 0 else 'dev',
+                    kind='ci' if self.kind == consts.FLOW_KIND_CI else 'dev',
                     duration=duration_to_txt(duration),
                     branch_name=self.branch_name,
                     args=self.args,
-                    stages=[s.get_json(with_schema=with_schema) for s in self.branch.stages if s.deleted is None],
-                    runs=[r.get_json(with_project=False, with_branch=False, with_artifacts=False) for r in self.runs],
                     trigger=trigger,
-                    artifacts=self.artifacts)
+                    artifacts=self.artifacts,
+                    seq=self.seq)
 
         infix = 'f/%d' % self.id
         data['report_entries'] = _get_report_entries(self.artifacts, infix)
 
+        if with_stages:
+            stages = [s.get_json(with_schema=with_schema) for s in self.branch.stages if s.deleted is None]
+            data['stages'] = stages
+
+        if with_runs:
+            runs = [r.get_json(with_project=False, with_branch=False, with_artifacts=False) for r in self.runs]
+            data['runs'] = runs
+
         if with_project:
             data['project_id'] = self.branch.project_id
             data['project_name'] = self.branch.project.name
 
         if with_branch:
             data['branch_id'] = self.branch_id
             data['base_branch_name'] = self.branch.name
 
+        if with_user_data:
+            data['data'] = self.user_data
+
         return data
 
 
 Index('ix_flows_created', Flow.created)
 
 
 class Run(db.Model, DatesMixin):
@@ -408,35 +442,43 @@
     tests_total = Column(Integer, default=0)
     artifacts = Column(JSONB, default={})
     label = Column(UnicodeText)
     reason = Column(JSONB, nullable=False)
     repo_data_id = Column(Integer, ForeignKey('repo_changes.id'))
     repo_data = relationship('RepoChanges')
     processed_at = Column(DateTime(timezone=True))    # time when results analysis completed
+    seq = Column(JSONB, default={})
 
-    def get_json(self, with_project=True, with_branch=True, with_artifacts=True):
+    def __repr__(self):
+        return "<Run %s, state %s>" % (self.id, consts.RUN_STATES_NAME.get(self.state, 'unknown %d' % self.state))
+
+    def get_json(self, with_project=True, with_branch=True, with_artifacts=True, with_counts=True):
         jobs_processing = 0
         jobs_executing = 0
         jobs_waiting = 0
         jobs_error = 0
         jobs_total = 0
+        duration = ''
 
         if self.state == consts.RUN_STATE_PROCESSED:
             jobs_total = self.jobs_total
             jobs_error = self.jobs_error
             if self.started:
                 begin = self.started
             else:
                 begin = self.created
             if self.finished is None:
                 log.error('PROBLEM WITH NONE TIMESTAMP in run %s', self)
                 duration = utils.utcnow() - begin
             else:
                 duration = self.finished - begin
-        else:
+
+            duration = duration_to_txt(duration)
+
+        elif with_counts:
             non_covered_jobs = Job.query.filter_by(run=self).filter_by(covered=False).all()
             jobs_total = len(non_covered_jobs)
             jobs_completed = 0
             last_time = None
             for job in non_covered_jobs:
                 if job.state == consts.JOB_STATE_EXECUTING_FINISHED:
                     jobs_processing += 1
@@ -453,27 +495,29 @@
                     jobs_error += 1
 
             if jobs_total == jobs_completed and last_time:
                 duration = last_time - self.created
             else:
                 duration = utils.utcnow() - self.created
 
+            duration = duration_to_txt(duration)
+
         data = dict(id=self.id,
                     label=self.label,
                     created=self.created.strftime("%Y-%m-%dT%H:%M:%SZ") if self.created else None,
                     deleted=self.deleted.strftime("%Y-%m-%dT%H:%M:%SZ") if self.deleted else None,
                     started=self.started.strftime("%Y-%m-%dT%H:%M:%SZ") if self.started else None,
                     finished=self.finished.strftime("%Y-%m-%dT%H:%M:%SZ") if self.finished else None,
                     processed_at=self.processed_at.strftime("%Y-%m-%dT%H:%M:%SZ") if self.processed_at else None,
-                    duration=duration_to_txt(duration),
+                    duration=duration,
                     state=consts.RUN_STATES_NAME[self.state],
                     stage_name=self.stage.name,
                     stage_id=self.stage_id,
                     flow_id=self.flow_id,
-                    flow_kind='ci' if self.flow.kind == 0 else 'dev',
+                    flow_kind='ci' if self.flow.kind == consts.FLOW_KIND_CI else 'dev',
                     flow_label=self.flow.get_label(),
                     args=self.args,
                     jobs_total=jobs_total,
                     jobs_waiting=jobs_waiting,
                     jobs_executing=jobs_executing,
                     jobs_processing=jobs_processing,
                     jobs_error=jobs_error,
@@ -484,15 +528,16 @@
                     issues_new=self.issues_new,
                     new_cnt=self.new_cnt,
                     no_change_cnt=self.no_change_cnt,
                     regr_cnt=self.regr_cnt,
                     fix_cnt=self.fix_cnt,
                     repo_data=self.repo_data.data if self.repo_data else None,
                     reason=self.reason['reason'],
-                    note=self.note)
+                    note=self.note,
+                    seq=self.seq)
 
         if with_project:
             data['project_id'] = self.flow.branch.project_id
             data['project_name'] = self.flow.branch.project.name
 
         if with_branch:
             data['branch_id'] = self.flow.branch_id
@@ -516,46 +561,47 @@
     tool = relationship("Tool", back_populates="steps")
     fields = Column(JSONB, nullable=False)
     result = Column(JSONB)
     status = Column(Integer)
     fields_masked = Column(JSONB, nullable=True)
     # services
 
-    def get_json(self, mask_secrets=False):
+    def get_json(self, with_fields=True, mask_secrets=False):
         data = dict(id=self.id,
                     index=self.index,
                     tool=self.tool.name,
                     tool_id=self.tool_id,
                     tool_location=self.tool.location,
                     tool_entry=self.tool.entry,
                     tool_version=self.tool.version,
                     job_id=self.job_id,
                     status=self.status,
                     result=self.result)
 
-        if mask_secrets and self.fields_masked:
-            fields = self.fields_masked
-        else:
-            fields = self.fields
+        if with_fields:
+            if mask_secrets and self.fields_masked:
+                fields = self.fields_masked
+            else:
+                fields = self.fields
 
-        name = self.tool.name
-        if 'name' in fields:
-            name = fields['name']
-        elif self.tool.name == 'shell':
-            if 'script' in fields and fields['script']:
-                name = fields['script'].strip().splitlines()[0] + '...'
-            elif 'cmd' in fields and fields['cmd']:
-                name = fields['cmd']
-        elif self.tool.name == 'git':
-            name = 'checkout: ' + fields['checkout']
+            name = self.tool.name
+            if 'name' in fields:
+                name = fields['name']
+            elif self.tool.name == 'shell':
+                if 'script' in fields and fields['script']:
+                    name = fields['script'].strip().splitlines()[0] + '...'
+                elif 'cmd' in fields and fields['cmd']:
+                    name = fields['cmd']
+            elif self.tool.name == 'git':
+                name = 'checkout: ' + fields['checkout']
 
-        data['name'] = name
+            data['name'] = name
 
-        for f, v in fields.items():
-            data[f] = v
+            for f, v in fields.items():
+                data[f] = v
 
         return data
 
 
 class Job(db.Model, DatesMixin):
     __tablename__ = "jobs"
     id = Column(Integer, primary_key=True)
@@ -580,30 +626,25 @@
     agents_group = relationship('AgentsGroup', back_populates="jobs")
     timeout = Column(Integer)
     system_id = Column(Integer, ForeignKey('systems.id', name='fk_systems_jobs'), nullable=False) # match name fk_systems_jobs with name in alembic migration
     system = relationship('System', back_populates="jobs")
     results = relationship('TestCaseResult', back_populates="job")
     issues = relationship('Issue', back_populates="job")
 
-    def get_json(self, mask_secrets=False):
+    def get_json(self, with_steps=True, mask_secrets=False):
         if self.started:
             if self.finished:
                 duration = self.finished - self.started
             else:
                 duration = utils.utcnow() - self.started
             duration = duration_to_txt(duration)
         else:
             duration = ''
 
-        steps = []
-        for s in sorted(self.steps, key=lambda s: s.index):
-            s = s.get_json(mask_secrets=mask_secrets)
-            steps.append(s)
-
-        return dict(id=self.id,
+        data = dict(id=self.id,
                     created=self.created.strftime("%Y-%m-%dT%H:%M:%SZ") if self.created else None,
                     deleted=self.deleted.strftime("%Y-%m-%dT%H:%M:%SZ") if self.deleted else None,
                     started=self.started.strftime("%Y-%m-%dT%H:%M:%SZ") if self.started else None,
                     finished=self.finished.strftime("%Y-%m-%dT%H:%M:%SZ") if self.finished else None,
                     completed=self.completed.strftime("%Y-%m-%dT%H:%M:%SZ") if self.completed else None,
                     # processing_started=self.processing_started.strftime(
                     #     "%Y-%m-%dT%H:%M:%SZ") if self.processing_started else None,
@@ -617,16 +658,25 @@
                     system_id=self.system_id,
                     system=self.system.name,
                     executor=self.system.executor,
                     run_id=self.run_id,
                     agents_group_id=self.agents_group_id,
                     agents_group_name=self.agents_group.name,
                     agent_id=self.agent_used_id if self.agent_used else 0,
-                    agent_name=self.agent_used.name if self.agent_used else '',
-                    steps=steps)
+                    agent_name=self.agent_used.name if self.agent_used else '')
+
+        if with_steps:
+            steps = []
+            for s in sorted(self.steps, key=lambda s: s.index):
+                s = s.get_json(mask_secrets=mask_secrets)
+                steps.append(s)
+            data['steps'] = steps
+
+        return data
+
 
     def __repr__(self):
         txt = 'Job %s, state:%s' % (self.id, consts.JOB_STATES_NAME[self.state])
         txt += ', g:%s' % self.agents_group_id
         if self.agent_used_id:
             txt += ', ag:%s' % self.agent_used_id
         return "<%s>" % txt
@@ -695,15 +745,15 @@
 
         if with_extra:
             data['project_id'] = self.job.run.flow.branch.project_id
             data['project_name'] = self.job.run.flow.branch.project.name
             data['branch_id'] = self.job.run.flow.branch_id
             data['branch_name'] = self.job.run.flow.branch.name
             data['flow_id'] = self.job.run.flow_id
-            data['flow_kind'] = 'ci' if self.job.run.flow.kind == 0 else 'dev'
+            data['flow_kind'] = 'ci' if self.job.run.flow.kind == consts.FLOW_KIND_CI else 'dev'
             data['flow_label'] = self.job.run.flow.get_label()
             created_at = self.job.run.flow.created
             data['flow_created_at'] = created_at.strftime("%Y-%m-%dT%H:%M:%SZ") if created_at else None
             data['run_id'] = self.job.run_id
             data['stage_id'] = self.job.run.stage_id
             data['stage_name'] = self.job.run.stage.name
```

### Comparing `krakenci_server-1.0/kraken/server/notify.py` & `krakenci_server-1.1.44/kraken/server/notify.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from urllib.parse import urljoin
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
 
 import requests
 
 from .models import get_setting
-from .schema import prepare_secrets, substitute_vars
+from .schema import prepare_secrets, substitute_vars, prepare_context
 
 
 log = logging.getLogger(__name__)
 
 
 SLACK_URL = 'https://slack.com/api/chat.postMessage'
 
@@ -246,16 +246,17 @@
     notification = run.stage.schema.get('notification', None)
     if notification is None:
         return
 
     # prepare secrets to pass them to substitute in notifications definitions
     args = prepare_secrets(run)
     args.update(run.args)
+    ctx = prepare_context(run, args)
     # log.info('notification1 %s', notification)
-    notification, _ = substitute_vars(notification, args)
+    notification, _ = substitute_vars(notification, args, ctx)
     # log.info('notification2 %s', notification)
 
     # slack
     slack = notification.get('slack', None)
     try:
         _notify_slack(run, event, slack)
     except Exception:
```

### Comparing `krakenci_server-1.0/kraken/server/planner.py` & `krakenci_server-1.1.44/kraken/server/planner.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/pljobs.py` & `krakenci_server-1.1.44/kraken/server/pljobs.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/qneck.py` & `krakenci_server-1.1.44/kraken/server/qneck.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/results.py` & `krakenci_server-1.1.44/kraken/server/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,22 +120,22 @@
                   joinedload('job.agent_used'))
     q = q.filter_by(test_case_id=tcr.test_case_id)
     q = q.join('job')
     q = q.filter_by(agents_group=tcr.job.agents_group)
     q = q.filter_by(system=tcr.job.system)
     q = q.join('job', 'run', 'flow', 'branch')
     q = q.filter(Branch.id == tcr.job.run.flow.branch_id)
-    q = q.filter(Flow.kind == 0)  # CI
+    q = q.filter(Flow.kind == consts.FLOW_KIND_CI)
     q = q.filter(Flow.created <= tcr.job.run.flow.created)
     q = q.order_by(desc(Flow.created))
 
     total = q.count()
     q = q.offset(start).limit(limit)
     results = []
-    if tcr.job.run.flow.kind == 1:  # DEV
+    if tcr.job.run.flow.kind == consts.FLOW_KIND_DEV:
         results.append(tcr.get_json(with_extra=True))
     for tcr in q.all():
         results.append(tcr.get_json(with_extra=True))
     return {'items': results, 'total': total}, 200
 
 
 def get_result(test_case_result_id, token_info=None):
```

### Comparing `krakenci_server-1.0/kraken/server/scheduler.py` & `krakenci_server-1.1.44/kraken/server/scheduler.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/schema.py` & `krakenci_server-1.1.44/kraken/server/schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,70 +13,65 @@
 # limitations under the License.
 
 import os
 import re
 import logging
 import xmlrpc.client
 
+import addict
 import pytimeparse
 import dateutil.parser
 import RestrictedPython
 from RestrictedPython import compile_restricted
 from RestrictedPython import limited_builtins
+from jinja2.sandbox import SandboxedEnvironment
 
 from . import consts
 from . import schemaval
-from .models import Secret
+from .models import Secret, Step, Run, Stage, Branch
 
 
 log = logging.getLogger(__name__)
 
 
 class SchemaError(Exception):
     pass
 
 
-class SchemaCodeContext:
-    def __init__(self, branch_name, context):
-        self.branch_name = branch_name
-        for k, v in context.items():
-            setattr(self, k, v)
+class SchemaCodeContext(addict.Dict):
+    pass
 
 
-def execute_schema_code(branch, schema_code, context=None):
+def execute_schema_code(schema_code, context=None):
     # TODO: use starlark-go for executing schema code
     # for now RestrictedPython is used
     try:
         byte_code = compile_restricted(schema_code, '<inline>', 'exec')
     except Exception as e:
         log.exception('schema compilation exception')
         msg = 'compilation error: ' + str(e)
         raise SchemaError(msg) from e
 
     my_locals = {}
     my_globals = {'__builtins__': limited_builtins,
                   '_getattr_': RestrictedPython.Guards.safer_getattr,
                   '_getiter_': RestrictedPython.Eval.default_guarded_getiter,
-                  '_iter_unpack_sequence_': RestrictedPython.Guards.guarded_iter_unpack_sequence}
+                  '_iter_unpack_sequence_': RestrictedPython.Guards.guarded_iter_unpack_sequence,
+                  'log': log}
 
 
     try:
         exec(byte_code, my_globals, my_locals)  # pylint: disable=exec-used
     except Exception as e:
         log.exception('schema compilation exception')
         msg = 'compilation error: ' + str(e)
         raise SchemaError(msg) from e
 
     my_globals.update(my_locals)
-    if context is None:
-        context = {
-            'is_ci': True,
-            'is_dev': False,
-        }
-    ctx = SchemaCodeContext(branch.name, context)
+    ctx = SchemaCodeContext(context)
     my_globals['ctx'] = ctx
 
     my_locals2 = {}
     try:
         exec('schema = stage(ctx)', my_globals, my_locals2)  # pylint: disable=exec-used
     except Exception as e:
         log.exception('schema compilation exception')
@@ -115,15 +110,15 @@
             }]
         }]
     }'''
     log.info('schema_code %s', schema_code)
 
     # execute schema code
     try:
-        schema = execute_schema_code(branch, schema_code, context)
+        schema = execute_schema_code(schema_code, context)
     except SchemaError:
         raise
     except Exception:
         log.exception('unkown error in schema execution')
         raise
 
     # fill missing parts in schema
@@ -192,28 +187,29 @@
         elif s.kind == consts.SECRET_KIND_SIMPLE:
             name = "KK_SECRET_SIMPLE_" + s.name
             secrets[name] = s.data['secret']
 
     return secrets
 
 
-def substitute_val(val, args):
+def substitute_val(val, args, ctx):
     if isinstance(val, dict):
-        return substitute_vars(val, args)
+        return substitute_vars(val, args, ctx)
     if isinstance(val, list):
         list2 = []
         list2_masked = []
         for e in val:
-            e2, e2_masked = substitute_val(e, args)
+            e2, e2_masked = substitute_val(e, args, ctx)
             list2.append(e2)
             list2_masked.append(e2_masked)
         return list2, list2_masked
     if not isinstance(val, str):
         return val, val
 
+    # old way of interpolating vars in fields
     val_masked = val
     secret_present = False
     for var in re.findall(r'#{[A-Za-z0-9_ ]+}', val):
         name = var[2:-1]
         if name in args:
             arg_val = args[name]
             if  not isinstance(arg_val, str):
@@ -221,29 +217,104 @@
             val = val.replace(var, arg_val)
             if name.startswith('KK_SECRET_'):
                 val_masked = val_masked.replace(var, '******')
                 secret_present = True
             else:
                 val_masked = val_masked.replace(var, arg_val)
 
+    # new way of exposing context in fields
+    env = SandboxedEnvironment()
+    for var in re.findall(r'#{[A-Za-z0-9_\. ]+}', val):
+        expr = var[2:-1].strip()
+
+        tpl = env.from_string("{{ %s }}" % expr)
+        new_str = tpl.render(**ctx)
+        val = val.replace(var, new_str)
+
+        if expr.startswith('secrets.'):
+            secret_present = True
+            val_masked = val_masked.replace(var, '******')
+        else:
+            val_masked = val_masked.replace(var, new_str)
+
     if secret_present:
         return val, val_masked
     return val, val
 
 
-def substitute_vars(fields, args):
+def substitute_vars(fields, args, ctx):
     new_fields = {}
     new_fields_masked = {}
     for f, val in fields.items():
-        val, val_masked = substitute_val(val, args)
+        val, val_masked = substitute_val(val, args, ctx)
         new_fields[f] = val
         new_fields_masked[f] = val_masked
     return new_fields, new_fields_masked
 
 
+def prepare_context(entity, args):
+    if isinstance(entity, Step):
+        step = entity
+        run = step.job.run
+        stage = run.stage
+        branch = stage.branch
+    elif isinstance(entity, Run):
+        step = None
+        run = entity
+        stage = run.stage
+        branch = stage.branch
+    elif isinstance(entity, Stage):
+        step = None
+        run = None
+        stage = entity
+        branch = stage.branch
+    elif isinstance(entity, Branch):
+        step = None
+        run = None
+        stage = None
+        branch = entity
+
+    ctx = {}
+    ctx['args'] = args
+    ctx['project'] = branch.project.get_json(with_branches=False, with_user_data=True)
+    ctx['branch'] = branch.get_json(with_user_data=True)
+    ctx['branch_name'] = branch.name
+
+    ctx['secrets'] = {}
+    for s in branch.project.secrets:
+        if s.deleted:
+            continue
+        if s.kind == consts.SECRET_KIND_SSH_KEY:
+            ctx['secrets'][s.name] = {
+                'user': s.data['username'],
+                'key': s.data['key'],
+                'password': s.data['key']
+            }
+        elif s.kind == consts.SECRET_KIND_SIMPLE:
+            ctx['secrets'][s.name] = s.data['secret']
+
+    if stage:
+        ctx['stage'] = stage.get_json(with_schema=False)
+
+    if run:
+        ctx['flow'] = run.flow.get_json(with_project=False, with_branch=False, with_schema=False, with_user_data=True,
+                                        with_stages=False, with_runs=False)
+        ctx['run'] = run.get_json(with_project=False, with_branch=False, with_artifacts=False, with_counts=False)
+        ctx['is_ci'] = run.flow.kind == consts.FLOW_KIND_CI
+        ctx['is_dev'] = run.flow.kind == consts.FLOW_KIND_DEV
+        ctx['run_label'] = run.label
+        ctx['flow_label'] = run.flow.label
+
+    if step:
+        ctx['job'] = step.job.get_json(with_steps=False)
+        ctx['step'] = step.get_json(with_fields=False)
+
+    return ctx
+
+
 def prepare_new_planner_triggers(stage_id, new_triggers, prev_triggers, triggers):
     planner_url = os.environ.get('KRAKEN_PLANNER_URL', consts.DEFAULT_PLANNER_URL)
     planner = xmlrpc.client.ServerProxy(planner_url, allow_none=True)
 
     log.info('stage: %d, triggers: new: %s, old: %s', stage_id, new_triggers, prev_triggers)
 
     # set up interval trigger
```

### Comparing `krakenci_server-1.0/kraken/server/schemaval.py` & `krakenci_server-1.1.44/kraken/server/schemaval.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/server.py` & `krakenci_server-1.1.44/kraken/server/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,19 +158,21 @@
     connex_app.add_url_rule("/bk/artifacts/<store_type>/r/<run_id>/<path:path>", view_func=storage.serve_run_artifact, methods=['GET'])
 
     # serve job log
     connex_app.add_url_rule("/job_log/<job_id>", view_func=job_log.serve_job_log, methods=['GET'])
     connex_app.add_url_rule("/bk/job_log/<job_id>", view_func=job_log.serve_job_log, methods=['GET'])
     connex_app.add_url_rule("/job_log/<job_id>/<step_idx>", view_func=job_log.serve_step_log, methods=['GET'])
     connex_app.add_url_rule("/bk/job_log/<job_id>/<step_idx>", view_func=job_log.serve_step_log, methods=['GET'])
+    connex_app.add_url_rule("/any_log", view_func=job_log.serve_any_log, methods=['GET'])
+    connex_app.add_url_rule("/bk/any_log", view_func=job_log.serve_any_log, methods=['GET'])
 
     # install webhooks
     webhooks_bp = webhooks.create_blueprint()
-    app.register_blueprint(webhooks_bp, url_prefix='/webhooks')
-    app.register_blueprint(webhooks_bp, url_prefix='/bk/webhooks')
+    app.register_blueprint(webhooks_bp, url_prefix='/webhooks', name='webhooks1')
+    app.register_blueprint(webhooks_bp, url_prefix='/bk/webhooks', name='webhooks2')
 
     # branch status badge
     app.add_url_rule("/branch-badge/<branch_id>", view_func=badge.get_branch_badge, methods=['GET'], defaults={'what': None})
     app.add_url_rule("/branch-badge/<branch_id>/<what>", view_func=badge.get_branch_badge, methods=['GET'])
     app.add_url_rule("/bk/branch-badge/<branch_id>", view_func=badge.get_branch_badge, methods=['GET'], defaults={'what': None})
     app.add_url_rule("/bk/branch-badge/<branch_id>/<what>", view_func=badge.get_branch_badge, methods=['GET'])
```

### Comparing `krakenci_server-1.0/kraken/server/srvcheck.py` & `krakenci_server-1.1.44/kraken/server/srvcheck.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/storage.py` & `krakenci_server-1.1.44/kraken/server/storage.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/swagger.yml` & `krakenci_server-1.1.44/kraken/server/swagger.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1415,14 +1415,40 @@
                 $ref: '#/components/schemas/Run'
         default:
           description: unexpected error
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ApiError'
+    post:
+      tags:
+      - Execution
+      summary: Start manual run or replay existing run ie. start again same jobs
+      operationId: force_run_analysis
+      parameters:
+      - name: run_id
+        in: path
+        description: ID of pet to return
+        required: true
+        schema:
+          type: integer
+          format: int64
+      responses:
+        200:
+          description: A paged array of runs
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/Run'
+        default:
+          description: unexpected error
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ApiError'
     delete:
       tags:
       - Execution
       summary: Cancel a run
       description: Cancel a run
       operationId: cancel_run
       parameters:
@@ -2479,14 +2505,60 @@
                 contentType: application/json
               file:
                 contentType: application/zip
       responses:
         201:
           description: Successfully created group
           content: {}
+  /user_data:
+    get:
+      tags:
+      - Execution
+      summary: Get user data.
+      description: Get user data.
+      operationId: get_user_data
+      parameters:
+      - name: scope
+        in: query
+        description: Scope of user data
+        schema:
+          type: string
+      - name: entity_id
+        in: query
+        description: Entity ID
+        schema:
+          type: integer
+          format: int32
+      responses:
+        200:
+          description: Successfully
+          content:
+            application/json:
+              schema:
+                type: object
+                properties:
+                  data:
+                    type: string
+  /rq/queue:
+    post:
+      tags:
+      - Management
+      summary: Create new entry in RQ
+      description: Create new entry in RQ
+      operationId: create_rq_entry
+      requestBody:
+        description: RQ Entry
+        content:
+          application/json:
+            schema:
+              $ref: '#/components/schemas/RQEntry'
+      responses:
+        201:
+          description: Successfully created group
+          content: {}
 
 
 components:
   securitySchemes:
     bearerAuth:
       type: http
       scheme: bearer
@@ -2995,14 +3067,17 @@
           type: string
     Branch:
       type: object
       properties:
         id:
           type: integer
           format: int64
+        created:
+          type: string
+          format: date-time
         name:
           type: string
         branch_name:
           type: string
         project_id:
           type: integer
           format: int64
@@ -3347,14 +3422,21 @@
       type: object
       properties:
         id:
           type: integer
           format: int64
         name:
           type: string
+    RQEntry:
+      type: object
+      properties:
+        func_name:
+          type: string
+        args:
+          type: string
     ServerVersion:
       type: object
       properties:
         version:
           type: string
     ApiError:
       required:
```

### Comparing `krakenci_server-1.0/kraken/server/toolops.py` & `krakenci_server-1.1.44/kraken/server/toolops.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/toolutils.py` & `krakenci_server-1.1.44/kraken/server/toolutils.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/users.py` & `krakenci_server-1.1.44/kraken/server/users.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/kraken/server/watchdog.py` & `krakenci_server-1.1.44/kraken/server/watchdog.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,15 @@
 
         for flow_kind in [0, 1]:
             query = "ALTER TABLE logs DELETE WHERE branch = %(branch_id)s AND flow_kind = %(flow_kind)s AND time < (now() - toIntervalMonth(%(months)s))"
             params = dict(branch_id=branch.id,
                           flow_kind=flow_kind,
                           months=months[flow_kind])
             resp = ch.execute(query, params)
-            log.info('DELETED LOGS %s', resp)
+            log.info('deleted logs %s', resp)
             # TODO: trace number of deleted logs
 
     log.reset_ctx()
 
 
 def _main_loop():
     t0 = time.time()
```

### Comparing `krakenci_server-1.0/kraken/server/webhooks.py` & `krakenci_server-1.1.44/kraken/server/webhooks.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.0/pyproject.tml` & `krakenci_server-1.1.44/pyproject.tml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "krakenci-server"
-version="1.0"
+version="1.1.44"
 description = "Kraken CI server."
 authors = ["Michal Nowikowski <godfryd@gmail.com>"]
 readme = "README.md"
 homepage = "https://kraken.ci/"
 repository = "https://github.com/kraken-ci/kraken"
 documentation = "https://kraken.ci/docs"
 keywords = ["building", "testing", "continuous-integration", "ci", "cd", "cicd"]
@@ -22,18 +22,18 @@
   { include = "kraken" },
 ]
 
 include = ["kraken/version.py"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-connexion = "^2.13.1"
-MarkupSafe = "2.0.1"  # 2.1 is broken that is used by Jinja2 by connextion
-Flask = "^1.1.4" # 2.0.1
-Flask-SQLAlchemy = "^2.5.1"
+connexion = "^2.14.2"
+MarkupSafe = "2.1.2"
+Flask = "^2.2.3"
+Flask-SQLAlchemy = "^3.0.3"
 psycopg2-binary = "^2.9.1"
 redis = "^3.5.3"
 requests = "^2.26.0"
 SQLAlchemy = "^1.4.25"
 swagger-ui-bundle = "^0.0.9"
 apscheduler = "^3.8.0"
 tzlocal = "2.1"  # this is required by apscheduler that still relies on pytz; aps 4.x will have this fixed and then this line can be removed
@@ -59,14 +59,18 @@
 azure-mgmt-subscription = "^1.0.0"
 kubernetes = "^20.13.0"
 casbin = "^1.17.1"
 python-ldap = "^3.4.3"
 Authlib = "^1.1.0"
 setuptools = "^66.0.0"  # required by apscheduler
 furl = "^2.1.3"
+jq = "^1.4.0"
+jsonpatch = "^1.32"
+jinja2 = "^3.1.2"
+addict = "^2.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pylint = "2.13.9"
 pudb = "^2021.1"
 PyHamcrest = "^2.0.3"
```

### Comparing `krakenci_server-1.0/setup.py` & `krakenci_server-1.1.44/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,35 +10,39 @@
  'kraken.server.cloud']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Authlib>=1.1.0,<2.0.0',
- 'Flask-SQLAlchemy>=2.5.1,<3.0.0',
- 'Flask>=1.1.4,<2.0.0',
- 'MarkupSafe==2.0.1',
+ 'Flask-SQLAlchemy>=3.0.3,<4.0.0',
+ 'Flask>=2.2.3,<3.0.0',
+ 'MarkupSafe==2.1.2',
  'RestrictedPython==5.0',
  'SQLAlchemy>=1.4.25,<2.0.0',
+ 'addict>=2.4.0,<3.0.0',
  'alembic>=1.7.3,<2.0.0',
  'apscheduler>=3.8.0,<4.0.0',
  'azure-identity>=1.6.1,<2.0.0',
  'azure-mgmt-compute>=23.0.0,<24.0.0',
  'azure-mgmt-monitor>=2.0.0,<3.0.0',
  'azure-mgmt-network>=19.0.0,<20.0.0',
  'azure-mgmt-resource>=19.0.0,<20.0.0',
  'azure-mgmt-storage>=18.0.0,<19.0.0',
  'azure-mgmt-subscription>=1.0.0,<2.0.0',
  'boto3>=1.18.52,<2.0.0',
  'casbin>=1.17.1,<2.0.0',
  'clickhouse-driver>=0.2.5,<0.3.0',
- 'connexion>=2.13.1,<3.0.0',
+ 'connexion>=2.14.2,<3.0.0',
  'furl>=2.1.3,<3.0.0',
  'giturlparse>=0.10.0,<0.11.0',
  'gunicorn>=20.1.0,<21.0.0',
+ 'jinja2>=3.1.2,<4.0.0',
+ 'jq>=1.4.0,<2.0.0',
+ 'jsonpatch>=1.32,<2.0',
  'jsonschema>=4.5.0,<5.0.0',
  'kubernetes>=20.13.0,<21.0.0',
  'minio>=7.1.0,<8.0.0',
  'passlib>=1.7.4,<2.0.0',
  'psycopg2-binary>=2.9.1,<3.0.0',
  'python-dateutil>=2.8.2,<3.0.0',
  'python-ldap>=3.4.3,<4.0.0',
@@ -57,15 +61,15 @@
                      'kkqneck = kraken.server.qneck:main',
                      'kkrq = kraken.server.kkrq:main',
                      'kkscheduler = kraken.server.scheduler:main',
                      'kkwatchdog = kraken.server.watchdog:main']}
 
 setup_kwargs = {
     'name': 'krakenci-server',
-    'version': '1.0',
+    'version': '1.1.44',
     'description': 'Kraken CI server.',
     'long_description': '# Kraken CI\n\n![Release Version](https://img.shields.io/github/v/release/Kraken-CI/kraken)\n![Release Date](https://img.shields.io/github/release-date/Kraken-CI/kraken)\n\n![Kraken Build](https://lab.kraken.ci/bk/branch-badge/2)\n![Kraken Tests](https://lab.kraken.ci/bk/branch-badge/2/tests)\n![Kraken Issues](https://lab.kraken.ci/bk/branch-badge/2/issues)\n\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/be770bd29e374ece9e6f2782a1de99fc)](https://www.codacy.com/gh/Kraken-CI/kraken/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Kraken-CI/kraken&amp;utm_campaign=Badge_Grade)\n[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Kraken-CI/kraken.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Kraken-CI/kraken/context:python)\n[![Language grade: JavaScript](https://img.shields.io/lgtm/grade/javascript/g/Kraken-CI/kraken.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Kraken-CI/kraken/context:javascript)\n[![Total alerts](https://img.shields.io/lgtm/alerts/g/Kraken-CI/kraken.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Kraken-CI/kraken/alerts/)\n[![codebeat badge](https://codebeat.co/badges/556ac028-2390-4093-839e-a509f5678cf1)](https://codebeat.co/projects/github-com-kraken-ci-kraken-master)\n\n[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4758/badge)](https://bestpractices.coreinfrastructure.org/projects/4758)\n[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/kraken-ci)](https://artifacthub.io/packages/search?repo=kraken-ci)\n\n\n<!-- ABOUT THE PROJECT -->\n## About Kraken CI\n\n![Kraken CI Results Page](https://kraken.ci/img/slide-branch-results.png)\n\nKraken CI is a modern, open-source, on-premise CI/CD system\nthat is highly scalable and focused on testing.\n\nMore information can be found on https://kraken.ci\n\n\n<!-- GETTING STARTED -->\n## Getting Started\n\nQuick start guide is here: https://kraken.ci/docs/quick-start\n\nFull installation manual: https://kraken.ci/docs/installation\n\nAnd here is developers guide: https://kraken.ci/docs/dev-guide\n\n\n<!-- USAGE EXAMPLES -->\n## Usage\n\nGuides can be found here: https://kraken.ci/docs/guide-intro\n\nDemo site is available here: https://lab.kraken.ci/\n\n\n<!-- ROADMAP -->\n## Roadmap\n\nSee the [open issues](https://github.com/kraken-ci/kraken/issues) for a list of proposed features (and known issues).\n\n\n<!-- CONTRIBUTING -->\n## Contributing\n\nContributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.\n\nDetails on https://kraken.ci/docs/contrib-kraken\n\n\n<!-- LICENSE -->\n## License\n\nDistributed under the Apache 2.0 License. See `LICENSE` for more information.\n\n\n<!-- CONTACT -->\n## Contact\n\nMichal Nowikowski - godfryd@gmail.com\n\nProject Link: [https://kraken.ci](https://kraken.ci)\n',
     'author': 'Michal Nowikowski',
     'author_email': 'godfryd@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kraken.ci/',
```

### Comparing `krakenci_server-1.0/PKG-INFO` & `krakenci_server-1.1.44/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krakenci-server
-Version: 1.0
+Version: 1.1.44
 Summary: Kraken CI server.
 Home-page: https://kraken.ci/
 License: Apache-2.0
 Keywords: building,testing,continuous-integration,ci,cd,cicd
 Author: Michal Nowikowski
 Author-email: godfryd@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -16,35 +16,39 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Requires-Dist: Authlib (>=1.1.0,<2.0.0)
-Requires-Dist: Flask (>=1.1.4,<2.0.0)
-Requires-Dist: Flask-SQLAlchemy (>=2.5.1,<3.0.0)
-Requires-Dist: MarkupSafe (==2.0.1)
+Requires-Dist: Flask (>=2.2.3,<3.0.0)
+Requires-Dist: Flask-SQLAlchemy (>=3.0.3,<4.0.0)
+Requires-Dist: MarkupSafe (==2.1.2)
 Requires-Dist: RestrictedPython (==5.0)
 Requires-Dist: SQLAlchemy (>=1.4.25,<2.0.0)
+Requires-Dist: addict (>=2.4.0,<3.0.0)
 Requires-Dist: alembic (>=1.7.3,<2.0.0)
 Requires-Dist: apscheduler (>=3.8.0,<4.0.0)
 Requires-Dist: azure-identity (>=1.6.1,<2.0.0)
 Requires-Dist: azure-mgmt-compute (>=23.0.0,<24.0.0)
 Requires-Dist: azure-mgmt-monitor (>=2.0.0,<3.0.0)
 Requires-Dist: azure-mgmt-network (>=19.0.0,<20.0.0)
 Requires-Dist: azure-mgmt-resource (>=19.0.0,<20.0.0)
 Requires-Dist: azure-mgmt-storage (>=18.0.0,<19.0.0)
 Requires-Dist: azure-mgmt-subscription (>=1.0.0,<2.0.0)
 Requires-Dist: boto3 (>=1.18.52,<2.0.0)
 Requires-Dist: casbin (>=1.17.1,<2.0.0)
 Requires-Dist: clickhouse-driver (>=0.2.5,<0.3.0)
-Requires-Dist: connexion (>=2.13.1,<3.0.0)
+Requires-Dist: connexion (>=2.14.2,<3.0.0)
 Requires-Dist: furl (>=2.1.3,<3.0.0)
 Requires-Dist: giturlparse (>=0.10.0,<0.11.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: jq (>=1.4.0,<2.0.0)
+Requires-Dist: jsonpatch (>=1.32,<2.0)
 Requires-Dist: jsonschema (>=4.5.0,<5.0.0)
 Requires-Dist: kubernetes (>=20.13.0,<21.0.0)
 Requires-Dist: minio (>=7.1.0,<8.0.0)
 Requires-Dist: passlib (>=1.7.4,<2.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.1,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-ldap (>=3.4.3,<4.0.0)
```

