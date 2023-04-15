# Comparing `tmp/krakenci_server-1.1.44.tar.gz` & `tmp/krakenci_server-1.1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krakenci_server-1.1.44.tar", max compression
+gzip compressed data, was "krakenci_server-1.1.45.tar", max compression
```

## Comparing `krakenci_server-1.1.44.tar` & `krakenci_server-1.1.45.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0     2900 2023-04-14 16:38:17.608205 krakenci_server-1.1.44/README.md
--rw-r--r--   0        0        0        0 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/__init__.py
--rw-r--r--   0        0        0       38 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/README
--rw-r--r--   0        0        0        0 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/__init__.py
--rw-r--r--   0        0        0     2032 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/alembic.ini
--rw-r--r--   0        0        0     2041 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/apply.py
--rw-r--r--   0        0        0     2703 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/env.py
--rw-r--r--   0        0        0      494 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/script.py.mako
--rw-r--r--   0        0        0      560 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/050fbc3d126c_added_deployment_to_agents_group.py
--rw-r--r--   0        0        0      707 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/0615faca43b1_added_url_tag_and_tool_file_to_tool.py
--rw-r--r--   0        0        0      433 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/0731897c862e_add_enabled_to_stage.py
--rw-r--r--   0        0        0      448 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/0ad7507aa6d0_added_age_to_issue.py
--rw-r--r--   0        0        0      562 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/19396769e240_added_extra_atrs_to_agents_group.py
--rw-r--r--   0        0        0      461 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/1982be95e79f_added_system_to_job.py
--rw-r--r--   0        0        0     1173 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/1cf31ab18f84_create_secret_table.py
--rw-r--r--   0        0        0     1485 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/1f5039135dd8_removed_enabled_from_projects.py
--rw-r--r--   0        0        0     1122 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/26c6d691e7ce_added_last_flows_to_branch.py
--rw-r--r--   0        0        0      587 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/2996b1b6e227_user_is_session_nullable.py
--rw-r--r--   0        0        0      654 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/29b96da53f09_added_reason_to_run.py
--rw-r--r--   0        0        0      533 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/2b5751b83fec_added_artifacts_to_flow.py
--rw-r--r--   0        0        0     1035 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/2dd5cf2d12dc_added_new_repo_fields_to_stage.py
--rw-r--r--   0        0        0      482 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/38088514157a_removed_cancel_from_agent.py
--rw-r--r--   0        0        0      656 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/3c1af14e0370_added_timeouts_to_stage_and_job.py
--rw-r--r--   0        0        0      527 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/411094f6b709_added_details_to_user.py
--rw-r--r--   0        0        0    21962 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/42ea01a6cf31_convert_timestamps_to_with_timezones.py
--rw-r--r--   0        0        0      458 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/466de256799e_added_label_to_run.py
--rw-r--r--   0        0        0     1867 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/4a7ac9143bb1_added_branch_sequences.py
--rw-r--r--   0        0        0      492 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/54efe873f88f_added_git_clone_params_to_stage.py
--rw-r--r--   0        0        0     3897 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/5b13b262b132_added_repo_changes.py
--rw-r--r--   0        0        0      545 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/5c16623f4d55_added_fields_masked_to_step.py
--rw-r--r--   0        0        0      527 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/5e38f55beb11_added_summary_to_flow.py
--rw-r--r--   0        0        0      407 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/66808ea51a72_delete_setting_records_with_no_group.py
--rw-r--r--   0        0        0     1028 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/6745adaf40e5_added_schema_repo_to_stage.py
--rw-r--r--   0        0        0      478 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/67d4f5a5ee98_added_authorized_to_executor.py
--rw-r--r--   0        0        0      638 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/735e81eedae4_change_project_id_in_executorgroup_to_.py
--rw-r--r--   0        0        0      457 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/73db0f22e1e6_added_cancel_to_agent.py
--rw-r--r--   0        0        0      500 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/770cfcc80cfb_added_relevancy_to_test_case_result.py
--rw-r--r--   0        0        0      706 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/818e190ca142_move_webhook_to_project.py
--rw-r--r--   0        0        0     1732 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/8200318b9e18_added_several_stats_fields_to_run.py
--rw-r--r--   0        0        0     1317 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/87358b464400_added_casbin_rules_table.py
--rw-r--r--   0        0        0     1737 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/899dadc28f9c_added_missing_indexes.py
--rw-r--r--   0        0        0     5629 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/89ffd52f1f00_rename_executor_to_agent.py
--rw-r--r--   0        0        0      490 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/8b4adeca953d_added_group_to_setting.py
--rw-r--r--   0        0        0      551 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/9666bf8c1bb0_added_details_to_user_session.py
--rw-r--r--   0        0        0      826 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/98af95844f27_added_results_change_stats_to_run.py
--rw-r--r--   0        0        0      509 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/9d8d8713c1ad_added_unique_index_for_address_of_non_.py
--rw-r--r--   0        0        0        0 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/__init__.py
--rw-r--r--   0        0        0      700 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/a0741baf2dbc_added_indexes_to_test_case_results.py
--rw-r--r--   0        0        0      542 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/a26a02d0ac01_added_extra_atrs_to_agents.py
--rw-r--r--   0        0        0      698 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/a35aec7afa0a_added_processed_at_in_run_and_index_to_.py
--rw-r--r--   0        0        0      469 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/a7de4bdee425_added_section_to_artifact.py
--rw-r--r--   0        0        0     1385 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/ab9326d5fc02_added_index_to_flows.py
--rw-r--r--   0        0        0      690 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/af348b43d9d5_extended_tool.py
--rw-r--r--   0        0        0      626 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/b2c9024746f5_added_unique_constraint_for_system_name_.py
--rw-r--r--   0        0        0      859 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/b510fae321ba_added_seq_to_flow_and_run.py
--rw-r--r--   0        0        0      522 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/b5cc62f79980_add_extra_to_issue.py
--rw-r--r--   0        0        0      604 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/b84bdc5d3c67_uniqued_agent_address.py
--rw-r--r--   0        0        0      698 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/b908e219f07f_longer_message_in_issue.py
--rw-r--r--   0        0        0      384 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/ba436d491bf8_update_stage_enabled_to_true.py
--rw-r--r--   0        0        0     1478 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/bb0d4908ba49_added_artifact_and_file.py
--rw-r--r--   0        0        0     1377 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/bdcdbb4b5b3f_added_user_data_to_several_entities.py
--rw-r--r--   0        0        0      880 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/befa07ac5d1c_changed_tool_version_to_string.py
--rw-r--r--   0        0        0     3622 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/cb7654d57bca_added_systems_table_and_host_info_user_.py
--rw-r--r--   0        0        0    11177 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/ce05198f524a_convert_char_n_to_text.py
--rw-r--r--   0        0        0      562 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/cea0e48abb5a_added_retention_policy_to_branch.py
--rw-r--r--   0        0        0      461 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/d2b23f410d02_added_label_to_flow.py
--rw-r--r--   0        0        0      714 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/d45087b62027_move_trigger_data_to_flow.py
--rw-r--r--   0        0        0     1542 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/d524cbcbf19c_added_users_and_users_session.py
--rw-r--r--   0        0        0      530 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/dae910bd9587_added_repo_data_to_run.py
--rw-r--r--   0        0        0      719 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/e0d8421619c2_removed_unique_constraint_agent_non_.py
--rw-r--r--   0        0        0      814 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/e404f52562c2_added_unique_constraints_on_branch_name_.py
--rw-r--r--   0        0        0     1638 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/f566580fd139_added_test_case_comment_table.py
--rw-r--r--   0        0        0      476 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/migrations/versions/ff4a425a6070_added_last_seen_to_executor.py
--rw-r--r--   0        0        0      582 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/__init__.py
--rw-r--r--   0        0        0    12197 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/access.py
--rw-r--r--   0        0        0     2919 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/agentblob.py
--rw-r--r--   0        0        0    10192 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/authn.py
--rw-r--r--   0        0        0    22134 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/backend.py
--rw-r--r--   0        0        0     4378 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/badge.py
--rw-r--r--   0        0        0        0 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/bg/__init__.py
--rw-r--r--   0        0        0    44857 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/bg/jobs.py
--rw-r--r--   0        0        0     6287 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/chops.py
--rw-r--r--   0        0        0        0 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/cloud/__init__.py
--rw-r--r--   0        0        0     2003 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/cloud/aws.py
--rw-r--r--   0        0        0     9147 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/cloud/aws_ec2.py
--rw-r--r--   0        0        0     7191 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/cloud/aws_ecs.py
--rw-r--r--   0        0        0    17629 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/cloud/azure.py
--rw-r--r--   0        0        0     3244 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/cloud/cloud.py
--rw-r--r--   0        0        0     1892 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/cloud/common.py
--rw-r--r--   0        0        0     9421 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/cloud/k8s.py
--rw-r--r--   0        0        0        0 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/config.py
--rw-r--r--   0        0        0     5127 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/consts.py
--rw-r--r--   0        0        0     3772 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/datastore.py
--rw-r--r--   0        0        0     1687 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/dbutils.py
--rw-r--r--   0        0        0    18026 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/exec_utils.py
--rw-r--r--   0        0        0    21211 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/execution.py
--rw-r--r--   0        0        0     9981 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/gitops.py
--rw-r--r--   0        0        0    27015 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/initdb.py
--rw-r--r--   0        0        0     5460 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/job_log.py
--rw-r--r--   0        0        0     4489 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/kkrq.py
--rw-r--r--   0        0        0    14059 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/logs.py
--rw-r--r--   0        0        0    46016 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/management.py
--rw-r--r--   0        0        0     4435 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/minioops.py
--rw-r--r--   0        0        0    47658 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/models.py
--rw-r--r--   0        0        0    10039 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/notify.py
--rwxr-xr-x   0        0        0     6478 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/planner.py
--rw-r--r--   0        0        0     1248 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/pljobs.py
--rw-r--r--   0        0        0     4440 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/qneck.py
--rw-r--r--   0        0        0    11643 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/results.py
--rwxr-xr-x   0        0        0     5714 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/scheduler.py
--rw-r--r--   0        0        0    15415 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/schema.py
--rw-r--r--   0        0        0    30836 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/schemaval.py
--rwxr-xr-x   0        0        0     7508 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/server.py
--rw-r--r--   0        0        0     2010 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/srvcheck.py
--rw-r--r--   0        0        0     3908 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/storage.py
--rw-r--r--   0        0        0    83344 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/swagger.yml
--rw-r--r--   0        0        0     2222 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/toolops.py
--rw-r--r--   0        0        0     3197 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/toolutils.py
--rw-r--r--   0        0        0    10872 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/users.py
--rw-r--r--   0        0        0     1032 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/utils.py
--rw-r--r--   0        0        0    19687 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/watchdog.py
--rw-r--r--   0        0        0    12005 2023-04-14 16:36:33.000000 krakenci_server-1.1.44/kraken/server/webhooks.py
--rw-r--r--   0        0        0       19 2023-04-14 16:38:17.608205 krakenci_server-1.1.44/kraken/version.py
--rw-r--r--   0        0        0     2440 2023-04-14 16:38:18.460204 krakenci_server-1.1.44/pyproject.tml
--rw-r--r--   0        0        0     5342 1970-01-01 00:00:00.000000 krakenci_server-1.1.44/setup.py
--rw-r--r--   0        0        0     5709 1970-01-01 00:00:00.000000 krakenci_server-1.1.44/PKG-INFO
+-rw-r--r--   0        0        0     2900 2023-04-15 05:25:01.742745 krakenci_server-1.1.45/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/__init__.py
+-rw-r--r--   0        0        0       38 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/README
+-rw-r--r--   0        0        0        0 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/__init__.py
+-rw-r--r--   0        0        0     2032 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/alembic.ini
+-rw-r--r--   0        0        0     2041 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/apply.py
+-rw-r--r--   0        0        0     2703 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/env.py
+-rw-r--r--   0        0        0      494 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/script.py.mako
+-rw-r--r--   0        0        0      560 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/050fbc3d126c_added_deployment_to_agents_group.py
+-rw-r--r--   0        0        0      707 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/0615faca43b1_added_url_tag_and_tool_file_to_tool.py
+-rw-r--r--   0        0        0      433 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/0731897c862e_add_enabled_to_stage.py
+-rw-r--r--   0        0        0      448 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/0ad7507aa6d0_added_age_to_issue.py
+-rw-r--r--   0        0        0      562 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/19396769e240_added_extra_atrs_to_agents_group.py
+-rw-r--r--   0        0        0      461 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/1982be95e79f_added_system_to_job.py
+-rw-r--r--   0        0        0     1173 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/1cf31ab18f84_create_secret_table.py
+-rw-r--r--   0        0        0     1485 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/1f5039135dd8_removed_enabled_from_projects.py
+-rw-r--r--   0        0        0     1122 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/26c6d691e7ce_added_last_flows_to_branch.py
+-rw-r--r--   0        0        0      587 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/2996b1b6e227_user_is_session_nullable.py
+-rw-r--r--   0        0        0      654 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/29b96da53f09_added_reason_to_run.py
+-rw-r--r--   0        0        0      533 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/2b5751b83fec_added_artifacts_to_flow.py
+-rw-r--r--   0        0        0     1035 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/2dd5cf2d12dc_added_new_repo_fields_to_stage.py
+-rw-r--r--   0        0        0      482 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/38088514157a_removed_cancel_from_agent.py
+-rw-r--r--   0        0        0      656 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/3c1af14e0370_added_timeouts_to_stage_and_job.py
+-rw-r--r--   0        0        0      527 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/411094f6b709_added_details_to_user.py
+-rw-r--r--   0        0        0    21962 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/42ea01a6cf31_convert_timestamps_to_with_timezones.py
+-rw-r--r--   0        0        0      458 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/466de256799e_added_label_to_run.py
+-rw-r--r--   0        0        0     1867 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/4a7ac9143bb1_added_branch_sequences.py
+-rw-r--r--   0        0        0      492 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/54efe873f88f_added_git_clone_params_to_stage.py
+-rw-r--r--   0        0        0     3897 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/5b13b262b132_added_repo_changes.py
+-rw-r--r--   0        0        0      545 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/5c16623f4d55_added_fields_masked_to_step.py
+-rw-r--r--   0        0        0      527 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/5e38f55beb11_added_summary_to_flow.py
+-rw-r--r--   0        0        0      407 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/66808ea51a72_delete_setting_records_with_no_group.py
+-rw-r--r--   0        0        0     1028 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/6745adaf40e5_added_schema_repo_to_stage.py
+-rw-r--r--   0        0        0      478 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/67d4f5a5ee98_added_authorized_to_executor.py
+-rw-r--r--   0        0        0      638 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/735e81eedae4_change_project_id_in_executorgroup_to_.py
+-rw-r--r--   0        0        0      457 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/73db0f22e1e6_added_cancel_to_agent.py
+-rw-r--r--   0        0        0      500 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/770cfcc80cfb_added_relevancy_to_test_case_result.py
+-rw-r--r--   0        0        0      706 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/818e190ca142_move_webhook_to_project.py
+-rw-r--r--   0        0        0     1732 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/8200318b9e18_added_several_stats_fields_to_run.py
+-rw-r--r--   0        0        0     1317 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/87358b464400_added_casbin_rules_table.py
+-rw-r--r--   0        0        0     1737 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/899dadc28f9c_added_missing_indexes.py
+-rw-r--r--   0        0        0     5629 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/89ffd52f1f00_rename_executor_to_agent.py
+-rw-r--r--   0        0        0      490 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/8b4adeca953d_added_group_to_setting.py
+-rw-r--r--   0        0        0      551 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/9666bf8c1bb0_added_details_to_user_session.py
+-rw-r--r--   0        0        0      826 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/98af95844f27_added_results_change_stats_to_run.py
+-rw-r--r--   0        0        0      509 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/9d8d8713c1ad_added_unique_index_for_address_of_non_.py
+-rw-r--r--   0        0        0        0 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/__init__.py
+-rw-r--r--   0        0        0      700 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/a0741baf2dbc_added_indexes_to_test_case_results.py
+-rw-r--r--   0        0        0      542 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/a26a02d0ac01_added_extra_atrs_to_agents.py
+-rw-r--r--   0        0        0      698 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/a35aec7afa0a_added_processed_at_in_run_and_index_to_.py
+-rw-r--r--   0        0        0      469 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/a7de4bdee425_added_section_to_artifact.py
+-rw-r--r--   0        0        0     1385 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/ab9326d5fc02_added_index_to_flows.py
+-rw-r--r--   0        0        0      690 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/af348b43d9d5_extended_tool.py
+-rw-r--r--   0        0        0      626 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/b2c9024746f5_added_unique_constraint_for_system_name_.py
+-rw-r--r--   0        0        0      859 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/b510fae321ba_added_seq_to_flow_and_run.py
+-rw-r--r--   0        0        0      522 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/b5cc62f79980_add_extra_to_issue.py
+-rw-r--r--   0        0        0      604 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/b84bdc5d3c67_uniqued_agent_address.py
+-rw-r--r--   0        0        0      698 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/b908e219f07f_longer_message_in_issue.py
+-rw-r--r--   0        0        0      384 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/ba436d491bf8_update_stage_enabled_to_true.py
+-rw-r--r--   0        0        0     1478 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/bb0d4908ba49_added_artifact_and_file.py
+-rw-r--r--   0        0        0     1377 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/bdcdbb4b5b3f_added_user_data_to_several_entities.py
+-rw-r--r--   0        0        0      880 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/befa07ac5d1c_changed_tool_version_to_string.py
+-rw-r--r--   0        0        0     3622 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/cb7654d57bca_added_systems_table_and_host_info_user_.py
+-rw-r--r--   0        0        0    11177 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/ce05198f524a_convert_char_n_to_text.py
+-rw-r--r--   0        0        0      562 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/cea0e48abb5a_added_retention_policy_to_branch.py
+-rw-r--r--   0        0        0      461 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/d2b23f410d02_added_label_to_flow.py
+-rw-r--r--   0        0        0      714 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/d45087b62027_move_trigger_data_to_flow.py
+-rw-r--r--   0        0        0     1542 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/d524cbcbf19c_added_users_and_users_session.py
+-rw-r--r--   0        0        0      530 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/dae910bd9587_added_repo_data_to_run.py
+-rw-r--r--   0        0        0      719 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/e0d8421619c2_removed_unique_constraint_agent_non_.py
+-rw-r--r--   0        0        0      814 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/e404f52562c2_added_unique_constraints_on_branch_name_.py
+-rw-r--r--   0        0        0     1638 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/f566580fd139_added_test_case_comment_table.py
+-rw-r--r--   0        0        0      476 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/migrations/versions/ff4a425a6070_added_last_seen_to_executor.py
+-rw-r--r--   0        0        0      582 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/__init__.py
+-rw-r--r--   0        0        0    12197 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/access.py
+-rw-r--r--   0        0        0     2919 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/agentblob.py
+-rw-r--r--   0        0        0    10192 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/authn.py
+-rw-r--r--   0        0        0    22134 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/backend.py
+-rw-r--r--   0        0        0     4378 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/badge.py
+-rw-r--r--   0        0        0        0 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/bg/__init__.py
+-rw-r--r--   0        0        0    44857 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/bg/jobs.py
+-rw-r--r--   0        0        0     6287 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/chops.py
+-rw-r--r--   0        0        0        0 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/cloud/__init__.py
+-rw-r--r--   0        0        0     2003 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/cloud/aws.py
+-rw-r--r--   0        0        0     9147 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/cloud/aws_ec2.py
+-rw-r--r--   0        0        0     7191 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/cloud/aws_ecs.py
+-rw-r--r--   0        0        0    17629 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/cloud/azure.py
+-rw-r--r--   0        0        0     3244 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/cloud/cloud.py
+-rw-r--r--   0        0        0     1892 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/cloud/common.py
+-rw-r--r--   0        0        0     9421 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/cloud/k8s.py
+-rw-r--r--   0        0        0        0 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/config.py
+-rw-r--r--   0        0        0     5127 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/consts.py
+-rw-r--r--   0        0        0     3772 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/datastore.py
+-rw-r--r--   0        0        0     1687 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/dbutils.py
+-rw-r--r--   0        0        0    18026 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/exec_utils.py
+-rw-r--r--   0        0        0    21211 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/execution.py
+-rw-r--r--   0        0        0     9981 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/gitops.py
+-rw-r--r--   0        0        0    27015 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/initdb.py
+-rw-r--r--   0        0        0     5460 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/job_log.py
+-rw-r--r--   0        0        0     4489 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/kkrq.py
+-rw-r--r--   0        0        0    14059 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/logs.py
+-rw-r--r--   0        0        0    46016 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/management.py
+-rw-r--r--   0        0        0     4435 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/minioops.py
+-rw-r--r--   0        0        0    47658 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/models.py
+-rw-r--r--   0        0        0    10039 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/notify.py
+-rwxr-xr-x   0        0        0     6478 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/planner.py
+-rw-r--r--   0        0        0     1248 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/pljobs.py
+-rw-r--r--   0        0        0     4440 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/qneck.py
+-rw-r--r--   0        0        0    11643 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/results.py
+-rwxr-xr-x   0        0        0     5714 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/scheduler.py
+-rw-r--r--   0        0        0    15415 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/schema.py
+-rw-r--r--   0        0        0    30836 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/schemaval.py
+-rwxr-xr-x   0        0        0     7508 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/server.py
+-rw-r--r--   0        0        0     2010 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/srvcheck.py
+-rw-r--r--   0        0        0     3908 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/storage.py
+-rw-r--r--   0        0        0    83344 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/swagger.yml
+-rw-r--r--   0        0        0     2222 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/toolops.py
+-rw-r--r--   0        0        0     3197 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/toolutils.py
+-rw-r--r--   0        0        0    10872 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/users.py
+-rw-r--r--   0        0        0     1032 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/utils.py
+-rw-r--r--   0        0        0    19687 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/watchdog.py
+-rw-r--r--   0        0        0    12005 2023-04-15 05:22:58.000000 krakenci_server-1.1.45/kraken/server/webhooks.py
+-rw-r--r--   0        0        0       19 2023-04-15 05:25:01.738745 krakenci_server-1.1.45/kraken/version.py
+-rw-r--r--   0        0        0     2440 2023-04-15 05:25:02.866779 krakenci_server-1.1.45/pyproject.tml
+-rw-r--r--   0        0        0     5342 1970-01-01 00:00:00.000000 krakenci_server-1.1.45/setup.py
+-rw-r--r--   0        0        0     5709 1970-01-01 00:00:00.000000 krakenci_server-1.1.45/PKG-INFO
```

### Comparing `krakenci_server-1.1.44/README.md` & `krakenci_server-1.1.45/README.md`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/alembic.ini` & `krakenci_server-1.1.45/kraken/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/apply.py` & `krakenci_server-1.1.45/kraken/migrations/apply.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/env.py` & `krakenci_server-1.1.45/kraken/migrations/env.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/050fbc3d126c_added_deployment_to_agents_group.py` & `krakenci_server-1.1.45/kraken/migrations/versions/050fbc3d126c_added_deployment_to_agents_group.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/0615faca43b1_added_url_tag_and_tool_file_to_tool.py` & `krakenci_server-1.1.45/kraken/migrations/versions/0615faca43b1_added_url_tag_and_tool_file_to_tool.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/19396769e240_added_extra_atrs_to_agents_group.py` & `krakenci_server-1.1.45/kraken/migrations/versions/19396769e240_added_extra_atrs_to_agents_group.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/1cf31ab18f84_create_secret_table.py` & `krakenci_server-1.1.45/kraken/migrations/versions/1cf31ab18f84_create_secret_table.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/1f5039135dd8_removed_enabled_from_projects.py` & `krakenci_server-1.1.45/kraken/migrations/versions/1f5039135dd8_removed_enabled_from_projects.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/26c6d691e7ce_added_last_flows_to_branch.py` & `krakenci_server-1.1.45/kraken/migrations/versions/26c6d691e7ce_added_last_flows_to_branch.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/2996b1b6e227_user_is_session_nullable.py` & `krakenci_server-1.1.45/kraken/migrations/versions/2996b1b6e227_user_is_session_nullable.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/29b96da53f09_added_reason_to_run.py` & `krakenci_server-1.1.45/kraken/migrations/versions/29b96da53f09_added_reason_to_run.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/2b5751b83fec_added_artifacts_to_flow.py` & `krakenci_server-1.1.45/kraken/migrations/versions/2b5751b83fec_added_artifacts_to_flow.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/2dd5cf2d12dc_added_new_repo_fields_to_stage.py` & `krakenci_server-1.1.45/kraken/migrations/versions/2dd5cf2d12dc_added_new_repo_fields_to_stage.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/3c1af14e0370_added_timeouts_to_stage_and_job.py` & `krakenci_server-1.1.45/kraken/migrations/versions/3c1af14e0370_added_timeouts_to_stage_and_job.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/411094f6b709_added_details_to_user.py` & `krakenci_server-1.1.45/kraken/migrations/versions/411094f6b709_added_details_to_user.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/42ea01a6cf31_convert_timestamps_to_with_timezones.py` & `krakenci_server-1.1.45/kraken/migrations/versions/42ea01a6cf31_convert_timestamps_to_with_timezones.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/4a7ac9143bb1_added_branch_sequences.py` & `krakenci_server-1.1.45/kraken/migrations/versions/4a7ac9143bb1_added_branch_sequences.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/5b13b262b132_added_repo_changes.py` & `krakenci_server-1.1.45/kraken/migrations/versions/5b13b262b132_added_repo_changes.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/5c16623f4d55_added_fields_masked_to_step.py` & `krakenci_server-1.1.45/kraken/migrations/versions/5c16623f4d55_added_fields_masked_to_step.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/5e38f55beb11_added_summary_to_flow.py` & `krakenci_server-1.1.45/kraken/migrations/versions/5e38f55beb11_added_summary_to_flow.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/6745adaf40e5_added_schema_repo_to_stage.py` & `krakenci_server-1.1.45/kraken/migrations/versions/6745adaf40e5_added_schema_repo_to_stage.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/735e81eedae4_change_project_id_in_executorgroup_to_.py` & `krakenci_server-1.1.45/kraken/migrations/versions/735e81eedae4_change_project_id_in_executorgroup_to_.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/818e190ca142_move_webhook_to_project.py` & `krakenci_server-1.1.45/kraken/migrations/versions/818e190ca142_move_webhook_to_project.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/8200318b9e18_added_several_stats_fields_to_run.py` & `krakenci_server-1.1.45/kraken/migrations/versions/8200318b9e18_added_several_stats_fields_to_run.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/87358b464400_added_casbin_rules_table.py` & `krakenci_server-1.1.45/kraken/migrations/versions/87358b464400_added_casbin_rules_table.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/899dadc28f9c_added_missing_indexes.py` & `krakenci_server-1.1.45/kraken/migrations/versions/899dadc28f9c_added_missing_indexes.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/89ffd52f1f00_rename_executor_to_agent.py` & `krakenci_server-1.1.45/kraken/migrations/versions/89ffd52f1f00_rename_executor_to_agent.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/9666bf8c1bb0_added_details_to_user_session.py` & `krakenci_server-1.1.45/kraken/migrations/versions/9666bf8c1bb0_added_details_to_user_session.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/98af95844f27_added_results_change_stats_to_run.py` & `krakenci_server-1.1.45/kraken/migrations/versions/98af95844f27_added_results_change_stats_to_run.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/a0741baf2dbc_added_indexes_to_test_case_results.py` & `krakenci_server-1.1.45/kraken/migrations/versions/a0741baf2dbc_added_indexes_to_test_case_results.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/a26a02d0ac01_added_extra_atrs_to_agents.py` & `krakenci_server-1.1.45/kraken/migrations/versions/a26a02d0ac01_added_extra_atrs_to_agents.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/a35aec7afa0a_added_processed_at_in_run_and_index_to_.py` & `krakenci_server-1.1.45/kraken/migrations/versions/a35aec7afa0a_added_processed_at_in_run_and_index_to_.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/ab9326d5fc02_added_index_to_flows.py` & `krakenci_server-1.1.45/kraken/migrations/versions/ab9326d5fc02_added_index_to_flows.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/af348b43d9d5_extended_tool.py` & `krakenci_server-1.1.45/kraken/migrations/versions/af348b43d9d5_extended_tool.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/b2c9024746f5_added_unique_constraint_for_system_name_.py` & `krakenci_server-1.1.45/kraken/migrations/versions/b2c9024746f5_added_unique_constraint_for_system_name_.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/b510fae321ba_added_seq_to_flow_and_run.py` & `krakenci_server-1.1.45/kraken/migrations/versions/b510fae321ba_added_seq_to_flow_and_run.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/b5cc62f79980_add_extra_to_issue.py` & `krakenci_server-1.1.45/kraken/migrations/versions/b5cc62f79980_add_extra_to_issue.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/b84bdc5d3c67_uniqued_agent_address.py` & `krakenci_server-1.1.45/kraken/migrations/versions/b84bdc5d3c67_uniqued_agent_address.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/b908e219f07f_longer_message_in_issue.py` & `krakenci_server-1.1.45/kraken/migrations/versions/b908e219f07f_longer_message_in_issue.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/bb0d4908ba49_added_artifact_and_file.py` & `krakenci_server-1.1.45/kraken/migrations/versions/bb0d4908ba49_added_artifact_and_file.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/bdcdbb4b5b3f_added_user_data_to_several_entities.py` & `krakenci_server-1.1.45/kraken/migrations/versions/bdcdbb4b5b3f_added_user_data_to_several_entities.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/befa07ac5d1c_changed_tool_version_to_string.py` & `krakenci_server-1.1.45/kraken/migrations/versions/befa07ac5d1c_changed_tool_version_to_string.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/cb7654d57bca_added_systems_table_and_host_info_user_.py` & `krakenci_server-1.1.45/kraken/migrations/versions/cb7654d57bca_added_systems_table_and_host_info_user_.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/ce05198f524a_convert_char_n_to_text.py` & `krakenci_server-1.1.45/kraken/migrations/versions/ce05198f524a_convert_char_n_to_text.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/cea0e48abb5a_added_retention_policy_to_branch.py` & `krakenci_server-1.1.45/kraken/migrations/versions/cea0e48abb5a_added_retention_policy_to_branch.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/d45087b62027_move_trigger_data_to_flow.py` & `krakenci_server-1.1.45/kraken/migrations/versions/d45087b62027_move_trigger_data_to_flow.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/d524cbcbf19c_added_users_and_users_session.py` & `krakenci_server-1.1.45/kraken/migrations/versions/d524cbcbf19c_added_users_and_users_session.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/dae910bd9587_added_repo_data_to_run.py` & `krakenci_server-1.1.45/kraken/migrations/versions/dae910bd9587_added_repo_data_to_run.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/e0d8421619c2_removed_unique_constraint_agent_non_.py` & `krakenci_server-1.1.45/kraken/migrations/versions/e0d8421619c2_removed_unique_constraint_agent_non_.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/e404f52562c2_added_unique_constraints_on_branch_name_.py` & `krakenci_server-1.1.45/kraken/migrations/versions/e404f52562c2_added_unique_constraints_on_branch_name_.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/migrations/versions/f566580fd139_added_test_case_comment_table.py` & `krakenci_server-1.1.45/kraken/migrations/versions/f566580fd139_added_test_case_comment_table.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/__init__.py` & `krakenci_server-1.1.45/kraken/server/__init__.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/access.py` & `krakenci_server-1.1.45/kraken/server/access.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/agentblob.py` & `krakenci_server-1.1.45/kraken/server/agentblob.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/authn.py` & `krakenci_server-1.1.45/kraken/server/authn.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/backend.py` & `krakenci_server-1.1.45/kraken/server/backend.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/badge.py` & `krakenci_server-1.1.45/kraken/server/badge.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/bg/jobs.py` & `krakenci_server-1.1.45/kraken/server/bg/jobs.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/chops.py` & `krakenci_server-1.1.45/kraken/server/chops.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/cloud/aws.py` & `krakenci_server-1.1.45/kraken/server/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/cloud/aws_ec2.py` & `krakenci_server-1.1.45/kraken/server/cloud/aws_ec2.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/cloud/aws_ecs.py` & `krakenci_server-1.1.45/kraken/server/cloud/aws_ecs.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/cloud/azure.py` & `krakenci_server-1.1.45/kraken/server/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/cloud/cloud.py` & `krakenci_server-1.1.45/kraken/server/cloud/cloud.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/cloud/common.py` & `krakenci_server-1.1.45/kraken/server/cloud/common.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/cloud/k8s.py` & `krakenci_server-1.1.45/kraken/server/cloud/k8s.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/consts.py` & `krakenci_server-1.1.45/kraken/server/consts.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/datastore.py` & `krakenci_server-1.1.45/kraken/server/datastore.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/dbutils.py` & `krakenci_server-1.1.45/kraken/server/dbutils.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/exec_utils.py` & `krakenci_server-1.1.45/kraken/server/exec_utils.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/execution.py` & `krakenci_server-1.1.45/kraken/server/execution.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/gitops.py` & `krakenci_server-1.1.45/kraken/server/gitops.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/initdb.py` & `krakenci_server-1.1.45/kraken/server/initdb.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/job_log.py` & `krakenci_server-1.1.45/kraken/server/job_log.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/kkrq.py` & `krakenci_server-1.1.45/kraken/server/kkrq.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/logs.py` & `krakenci_server-1.1.45/kraken/server/logs.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/management.py` & `krakenci_server-1.1.45/kraken/server/management.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/minioops.py` & `krakenci_server-1.1.45/kraken/server/minioops.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/models.py` & `krakenci_server-1.1.45/kraken/server/models.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/notify.py` & `krakenci_server-1.1.45/kraken/server/notify.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/planner.py` & `krakenci_server-1.1.45/kraken/server/planner.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/pljobs.py` & `krakenci_server-1.1.45/kraken/server/pljobs.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/qneck.py` & `krakenci_server-1.1.45/kraken/server/qneck.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/results.py` & `krakenci_server-1.1.45/kraken/server/results.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/scheduler.py` & `krakenci_server-1.1.45/kraken/server/scheduler.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/schema.py` & `krakenci_server-1.1.45/kraken/server/schema.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/schemaval.py` & `krakenci_server-1.1.45/kraken/server/schemaval.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/server.py` & `krakenci_server-1.1.45/kraken/server/server.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/srvcheck.py` & `krakenci_server-1.1.45/kraken/server/srvcheck.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/storage.py` & `krakenci_server-1.1.45/kraken/server/storage.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/swagger.yml` & `krakenci_server-1.1.45/kraken/server/swagger.yml`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/toolops.py` & `krakenci_server-1.1.45/kraken/server/toolops.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/toolutils.py` & `krakenci_server-1.1.45/kraken/server/toolutils.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/users.py` & `krakenci_server-1.1.45/kraken/server/users.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/utils.py` & `krakenci_server-1.1.45/kraken/server/utils.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/watchdog.py` & `krakenci_server-1.1.45/kraken/server/watchdog.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/kraken/server/webhooks.py` & `krakenci_server-1.1.45/kraken/server/webhooks.py`

 * *Files identical despite different names*

### Comparing `krakenci_server-1.1.44/pyproject.tml` & `krakenci_server-1.1.45/pyproject.tml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "krakenci-server"
-version="1.1.44"
+version="1.1.45"
 description = "Kraken CI server."
 authors = ["Michal Nowikowski <godfryd@gmail.com>"]
 readme = "README.md"
 homepage = "https://kraken.ci/"
 repository = "https://github.com/kraken-ci/kraken"
 documentation = "https://kraken.ci/docs"
 keywords = ["building", "testing", "continuous-integration", "ci", "cd", "cicd"]
```

### Comparing `krakenci_server-1.1.44/setup.py` & `krakenci_server-1.1.45/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                      'kkqneck = kraken.server.qneck:main',
                      'kkrq = kraken.server.kkrq:main',
                      'kkscheduler = kraken.server.scheduler:main',
                      'kkwatchdog = kraken.server.watchdog:main']}
 
 setup_kwargs = {
     'name': 'krakenci-server',
-    'version': '1.1.44',
+    'version': '1.1.45',
     'description': 'Kraken CI server.',
     'long_description': '# Kraken CI\n\n![Release Version](https://img.shields.io/github/v/release/Kraken-CI/kraken)\n![Release Date](https://img.shields.io/github/release-date/Kraken-CI/kraken)\n\n![Kraken Build](https://lab.kraken.ci/bk/branch-badge/2)\n![Kraken Tests](https://lab.kraken.ci/bk/branch-badge/2/tests)\n![Kraken Issues](https://lab.kraken.ci/bk/branch-badge/2/issues)\n\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/be770bd29e374ece9e6f2782a1de99fc)](https://www.codacy.com/gh/Kraken-CI/kraken/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Kraken-CI/kraken&amp;utm_campaign=Badge_Grade)\n[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Kraken-CI/kraken.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Kraken-CI/kraken/context:python)\n[![Language grade: JavaScript](https://img.shields.io/lgtm/grade/javascript/g/Kraken-CI/kraken.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Kraken-CI/kraken/context:javascript)\n[![Total alerts](https://img.shields.io/lgtm/alerts/g/Kraken-CI/kraken.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Kraken-CI/kraken/alerts/)\n[![codebeat badge](https://codebeat.co/badges/556ac028-2390-4093-839e-a509f5678cf1)](https://codebeat.co/projects/github-com-kraken-ci-kraken-master)\n\n[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4758/badge)](https://bestpractices.coreinfrastructure.org/projects/4758)\n[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/kraken-ci)](https://artifacthub.io/packages/search?repo=kraken-ci)\n\n\n<!-- ABOUT THE PROJECT -->\n## About Kraken CI\n\n![Kraken CI Results Page](https://kraken.ci/img/slide-branch-results.png)\n\nKraken CI is a modern, open-source, on-premise CI/CD system\nthat is highly scalable and focused on testing.\n\nMore information can be found on https://kraken.ci\n\n\n<!-- GETTING STARTED -->\n## Getting Started\n\nQuick start guide is here: https://kraken.ci/docs/quick-start\n\nFull installation manual: https://kraken.ci/docs/installation\n\nAnd here is developers guide: https://kraken.ci/docs/dev-guide\n\n\n<!-- USAGE EXAMPLES -->\n## Usage\n\nGuides can be found here: https://kraken.ci/docs/guide-intro\n\nDemo site is available here: https://lab.kraken.ci/\n\n\n<!-- ROADMAP -->\n## Roadmap\n\nSee the [open issues](https://github.com/kraken-ci/kraken/issues) for a list of proposed features (and known issues).\n\n\n<!-- CONTRIBUTING -->\n## Contributing\n\nContributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.\n\nDetails on https://kraken.ci/docs/contrib-kraken\n\n\n<!-- LICENSE -->\n## License\n\nDistributed under the Apache 2.0 License. See `LICENSE` for more information.\n\n\n<!-- CONTACT -->\n## Contact\n\nMichal Nowikowski - godfryd@gmail.com\n\nProject Link: [https://kraken.ci](https://kraken.ci)\n',
     'author': 'Michal Nowikowski',
     'author_email': 'godfryd@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kraken.ci/',
```

### Comparing `krakenci_server-1.1.44/PKG-INFO` & `krakenci_server-1.1.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krakenci-server
-Version: 1.1.44
+Version: 1.1.45
 Summary: Kraken CI server.
 Home-page: https://kraken.ci/
 License: Apache-2.0
 Keywords: building,testing,continuous-integration,ci,cd,cicd
 Author: Michal Nowikowski
 Author-email: godfryd@gmail.com
 Requires-Python: >=3.7,<4.0
```

