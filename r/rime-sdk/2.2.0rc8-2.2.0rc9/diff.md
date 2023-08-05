# Comparing `tmp/rime_sdk-2.2.0rc8.tar.gz` & `tmp/rime_sdk-2.2.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rime_sdk-2.2.0rc8.tar", last modified: Wed Aug  2 15:58:16 2023, max compression
+gzip compressed data, was "rime_sdk-2.2.0rc9.tar", last modified: Fri Aug  4 00:45:48 2023, max compression
```

## Comparing `rime_sdk-2.2.0rc8.tar` & `rime_sdk-2.2.0rc9.tar`

### file list

```diff
@@ -1,512 +1,512 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:58:16.377707 rime_sdk-2.2.0rc8/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-02 15:58:16.377707 rime_sdk-2.2.0rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:58:16.309699 rime_sdk-2.2.0rc8/rime_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64243 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:58:16.309699 rime_sdk-2.2.0rc8/rime_sdk/data_format_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/data_format_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/data_format_check/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/data_format_check/data_format_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/data_format_check/nlp_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/data_format_check/tabular_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    27942 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/generative_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/image_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:58:16.309699 rime_sdk-2.2.0rc8/rime_sdk/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15781 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/internal/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/internal/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/internal/file_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/internal/rest_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/internal/security_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/internal/swagger_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/internal/swagger_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/internal/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/internal/throttle_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    73896 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    27443 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:58:16.309699 rime_sdk-2.2.0rc8/rime_sdk/swagger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:58:16.309699 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)    49575 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:58:16.313700 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31606 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/config_validator_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25305 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/data_collector_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/detection_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23001 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18198 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/file_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/firewall_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/firewall_configuration_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22570 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28418 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/image_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27020 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/integration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27071 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/job_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21740 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19359 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/model_testing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    34851 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19832 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    56145 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/project_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    57583 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/registry_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    72694 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/results_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/rime_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    40405 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25630 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/validation_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    46222 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:58:16.373706 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    47261 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/detection_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/detection_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_configure_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_get_file_upload_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_validation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_validation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/model_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/notification_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/notification_object_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    10410 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/protobuf_any.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_config_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_float_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_int_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_language.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_named_double.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_str_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_table_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_token_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/role_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16800 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    16128 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/user_private_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/user_user_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/validate_request_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/validate_request_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-08-02 15:58:12.000000 rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14833 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/rime_sdk/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:58:16.309699 rime_sdk-2.2.0rc8/rime_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-02 15:58:16.000000 rime_sdk-2.2.0rc8/rime_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34138 2023-08-02 15:58:16.000000 rime_sdk-2.2.0rc8/rime_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:58:16.000000 rime_sdk-2.2.0rc8/rime_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-02 15:58:16.000000 rime_sdk-2.2.0rc8/rime_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-02 15:58:16.000000 rime_sdk-2.2.0rc8/rime_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 15:58:16.000000 rime_sdk-2.2.0rc8/rime_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 15:58:16.377707 rime_sdk-2.2.0rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-02 15:57:30.000000 rime_sdk-2.2.0rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:45:48.096384 rime_sdk-2.2.0rc9/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-04 00:45:48.096384 rime_sdk-2.2.0rc9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:45:48.048383 rime_sdk-2.2.0rc9/rime_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64962 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:45:48.048383 rime_sdk-2.2.0rc9/rime_sdk/data_format_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/data_format_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/data_format_check/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/data_format_check/data_format_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/data_format_check/nlp_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/data_format_check/tabular_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27942 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/generative_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/image_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:45:48.048383 rime_sdk-2.2.0rc9/rime_sdk/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15781 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/internal/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/internal/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/internal/file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/internal/rest_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/internal/security_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/internal/swagger_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/internal/swagger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/internal/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/internal/throttle_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73896 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27443 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:45:48.048383 rime_sdk-2.2.0rc9/rime_sdk/swagger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:45:48.048383 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    49575 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:45:48.052383 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31606 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/config_validator_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25305 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/data_collector_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/detection_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23001 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/file_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/firewall_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/firewall_configuration_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22570 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28766 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/image_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27020 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/integration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27071 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/job_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21740 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19359 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/model_testing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34851 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19832 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56145 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/project_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57583 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/registry_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72694 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/results_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/rime_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40405 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25630 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/validation_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46222 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:45:48.096384 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    47261 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/detection_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/detection_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_configure_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_get_file_upload_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_validation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_validation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/model_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/notification_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/notification_object_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10410 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/protobuf_any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_config_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_float_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_int_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_job_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_job_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_job_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_model_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_named_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_str_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_table_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_token_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/role_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16800 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16128 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/user_private_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/user_user_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/validate_request_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/validate_request_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-08-04 00:45:43.000000 rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14833 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/rime_sdk/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:45:48.048383 rime_sdk-2.2.0rc9/rime_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-04 00:45:47.000000 rime_sdk-2.2.0rc9/rime_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34138 2023-08-04 00:45:48.000000 rime_sdk-2.2.0rc9/rime_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 00:45:47.000000 rime_sdk-2.2.0rc9/rime_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-04 00:45:47.000000 rime_sdk-2.2.0rc9/rime_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-04 00:45:47.000000 rime_sdk-2.2.0rc9/rime_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-04 00:45:47.000000 rime_sdk-2.2.0rc9/rime_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 00:45:48.096384 rime_sdk-2.2.0rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-08-04 00:45:08.000000 rime_sdk-2.2.0rc9/setup.py
```

### Comparing `rime_sdk-2.2.0rc8/LICENSE` & `rime_sdk-2.2.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/PKG-INFO` & `rime_sdk-2.2.0rc9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime_sdk
-Version: 2.2.0rc8
+Version: 2.2.0rc9
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.2.0rc8/README.md` & `rime_sdk-2.2.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/__init__.py` & `rime_sdk-2.2.0rc9/rime_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/client.py` & `rime_sdk-2.2.0rc9/rime_sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,15 +265,15 @@
             )
         return rime_info_response.customer_name
 
     def __str__(self) -> str:
         """Pretty-print the object."""
         return f"RIME Client [{self._domain}]"
 
-    # TODO(QuantumWombat): do this check server-side
+    # TODO(RAT-2173): do this check server-side
     def _project_exists(self, project_id: str) -> bool:
         """Check if `project_id` exists.
 
         Args:
             project_id: the id of the Project to be checked.
 
         Returns:
@@ -467,14 +467,18 @@
         automatically upgrade when the installed version of RIME upgrades.
         Note: Images take a few minutes to be built.
 
         This method returns an object that can be used to track the progress of the
         image building job. The new custom image is only available for use in a stress
         test once it has status ``READY``.
 
+        **Managed images are not currently supported in a Cloud deployment.
+        Please reach out to Robust Intelligence for support if this functionality is required
+        for your deployment.**
+
         Args:
             name: str
                 The name of the new Managed Image. This name serves as the unique
                 identifier of the Managed Image. The call fails when an image with
                 the specified name already exists.
             requirements: List[ManagedImagePipRequirement]
                 List of additional pip requirements to be installed on the managed
@@ -863,15 +867,15 @@
             if not res.has_more:
                 break
             # Advance to the next page of Test Cases.
             page_token = res.next_page_token
 
     def _validate_config(self, test_run_config: Dict, project_id: str) -> None:
         """Validate the test run config."""
-        # TODO(blaine): Add config validation service.
+        # TODO(VAL-2437): Add config validation service.
         if not isinstance(test_run_config, dict):
             raise ValueError("The configuration must be a dictionary")
         # TODO(VAL-316): do proper runtime validation of all of the types in the config
         if project_id and not self._project_exists(project_id):
             raise ValueError(f"Project id {project_id} does not exist")
         if "model_id" in test_run_config:
             if isinstance(test_run_config["model_id"], str):
@@ -1122,14 +1126,17 @@
         self, file_path: Union[Path, str], upload_path: Optional[str] = None
     ) -> str:
         """Upload a file to make it accessible to the RIME cluster.
 
         The uploaded file is stored in the RIME cluster in a blob store
         using its file name.
 
+        **File uploading is not currently supported in a Cloud deployment.
+        Please use an external data source instead.**
+
         Args:
             file_path: Union[Path, str]
                 Path to the file to be uploaded to RIME's blob store.
             upload_path: Optional[str] = None
                 Name of the directory in the blob store file system. If omitted,
                 a unique random string will be the directory.
 
@@ -1177,14 +1184,17 @@
         with an image_features that reference an image (either an absolute path
         or a relative path to an image file stored locally).
         Every image within the file is also uploaded to blob store,
         and the final file is also uploaded.
         If your image paths already reference an external blob storage,
         then use `upload_file` instead to upload the dataset file.
 
+        **File uploading is not currently supported in a Cloud deployment.
+        Please use an external data source instead.**
+
         Args:
             file_path: Union[Path, str]
                 Path to the file to be uploaded to RIME's blob store.
             image_features: List[str]
                 Keys to image file paths.
             upload_path: Optional[str]
                 Name of the directory in the blob store file system. If omitted,
@@ -1266,14 +1276,17 @@
         upload_path: Optional[str] = None,
     ) -> str:
         """Upload a pandas DataFrame to make it accessible to the RIME cluster.
 
         The uploaded file is stored in the RIME cluster in a blob store
         using its file name.
 
+        **File uploading is not currently supported in a Cloud deployment.
+        Please use an external data source instead.**
+
         Args:
             data_frame: pd.DataFrame
                 Path to the file to be uploaded to RIME's blob store.
             name: Optional[str] = None
                 Name of the file in the blob store file system. If omitted,
                 a unique random string will be assigned as the file name.
             upload_path: Optional[str] = None
@@ -1316,14 +1329,17 @@
 
         The uploaded directory is stored in the RIME cluster in a blob store.
         All files contained within ``dir_path`` and its subdirectories are uploaded
         according to their relative paths within ``dir_path``. When
         `upload_hidden` is set to False, all hidden files and subdirectories
         that begin with a '.' are not uploaded.
 
+        **File uploading is not currently supported in a Cloud deployment.
+        Please use an external data source instead.**
+
         Args:
             dir_path: Union[Path, str]
                 Path to the directory to be uploaded to RIME's blob store.
             upload_hidden: bool = False
                 Whether to upload hidden files or subdirectories
                 (i.e. those beginning with a '.').
             upload_path: Optional[str] = None
```

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/data_collector.py` & `rime_sdk-2.2.0rc9/rime_sdk/data_collector.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/data_format_check/cli.py` & `rime_sdk-2.2.0rc9/rime_sdk/data_format_check/cli.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/data_format_check/data_format_checker.py` & `rime_sdk-2.2.0rc9/rime_sdk/data_format_check/data_format_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/data_format_check/nlp_checker.py` & `rime_sdk-2.2.0rc9/rime_sdk/data_format_check/nlp_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/data_format_check/tabular_checker.py` & `rime_sdk-2.2.0rc9/rime_sdk/data_format_check/tabular_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/detection_event.py` & `rime_sdk-2.2.0rc9/rime_sdk/detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/firewall.py` & `rime_sdk-2.2.0rc9/rime_sdk/firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/generative_firewall.py` & `rime_sdk-2.2.0rc9/rime_sdk/generative_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/image_builder.py` & `rime_sdk-2.2.0rc9/rime_sdk/image_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,11 +119,11 @@
                 )
             if wait_until_finish:
                 time.sleep(poll_rate_sec)
             else:
                 repeat = False
             poll_count += 1
 
-            # TODO(blaine): Add ability to get and print logging information from a
+            # TODO(VAL-2433): Add ability to get and print logging information from a
             # failed build.
 
         return image.to_dict()
```

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/internal/config_parser.py` & `rime_sdk-2.2.0rc9/rime_sdk/internal/config_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/internal/constants.py` & `rime_sdk-2.2.0rc9/rime_sdk/internal/constants.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/internal/decorators.py` & `rime_sdk-2.2.0rc9/rime_sdk/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/internal/file_upload.py` & `rime_sdk-2.2.0rc9/rime_sdk/internal/file_upload.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/internal/rest_error_handler.py` & `rime_sdk-2.2.0rc9/rime_sdk/internal/rest_error_handler.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/internal/security_config_parser.py` & `rime_sdk-2.2.0rc9/rime_sdk/internal/security_config_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/internal/swagger_parser.py` & `rime_sdk-2.2.0rc9/rime_sdk/internal/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/internal/swagger_utils.py` & `rime_sdk-2.2.0rc9/rime_sdk/internal/swagger_utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/internal/test_helpers.py` & `rime_sdk-2.2.0rc9/rime_sdk/internal/test_helpers.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/internal/throttle_queue.py` & `rime_sdk-2.2.0rc9/rime_sdk/internal/throttle_queue.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/internal/utils.py` & `rime_sdk-2.2.0rc9/rime_sdk/internal/utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/job.py` & `rime_sdk-2.2.0rc9/rime_sdk/job.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/monitor.py` & `rime_sdk-2.2.0rc9/rime_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/project.py` & `rime_sdk-2.2.0rc9/rime_sdk/project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/registry.py` & `rime_sdk-2.2.0rc9/rime_sdk/registry.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/__init__.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/__init__.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/agent_manager_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/agent_manager_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/config_validator_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/config_validator_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/data_collector_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/data_collector_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/detection_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/detection_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/feature_flag_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/feature_flag_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/file_scanning_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/file_scanning_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/file_upload_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/file_upload_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,15 +126,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def file_upload_get_dataset_file_upload_url(self, file_name, **kwargs):  # noqa: E501
         """GetDatasetFileUploadURL  # noqa: E501
 
-        Returns a pre-signed upload URL for a dataset.  # noqa: E501
+        Returns a pre-signed upload URL for a dataset.  File uploading is not currently supported in a Cloud deployment. Please use an external data source instead.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.file_upload_get_dataset_file_upload_url(file_name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str file_name: Path of dataset file on the local file system. (required)
@@ -149,15 +149,15 @@
         else:
             (data) = self.file_upload_get_dataset_file_upload_url_with_http_info(file_name, **kwargs)  # noqa: E501
             return data
 
     def file_upload_get_dataset_file_upload_url_with_http_info(self, file_name, **kwargs):  # noqa: E501
         """GetDatasetFileUploadURL  # noqa: E501
 
-        Returns a pre-signed upload URL for a dataset.  # noqa: E501
+        Returns a pre-signed upload URL for a dataset.  File uploading is not currently supported in a Cloud deployment. Please use an external data source instead.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.file_upload_get_dataset_file_upload_url_with_http_info(file_name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str file_name: Path of dataset file on the local file system. (required)
@@ -225,15 +225,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def file_upload_get_model_directory_upload_urls(self, directory_name, relative_file_paths, **kwargs):  # noqa: E501
         """GetModelDirectoryUploadURL  # noqa: E501
 
-        Returns a pre-signed upload URL for a model directory.  # noqa: E501
+        Returns a pre-signed upload URL for a model directory.  File uploading is not currently supported in a Cloud deployment. Please use an external data source instead.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.file_upload_get_model_directory_upload_urls(directory_name, relative_file_paths, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str directory_name: Path of model directory on local file system. (required)
@@ -249,15 +249,15 @@
         else:
             (data) = self.file_upload_get_model_directory_upload_urls_with_http_info(directory_name, relative_file_paths, **kwargs)  # noqa: E501
             return data
 
     def file_upload_get_model_directory_upload_urls_with_http_info(self, directory_name, relative_file_paths, **kwargs):  # noqa: E501
         """GetModelDirectoryUploadURL  # noqa: E501
 
-        Returns a pre-signed upload URL for a model directory.  # noqa: E501
+        Returns a pre-signed upload URL for a model directory.  File uploading is not currently supported in a Cloud deployment. Please use an external data source instead.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.file_upload_get_model_directory_upload_urls_with_http_info(directory_name, relative_file_paths, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str directory_name: Path of model directory on local file system. (required)
@@ -333,15 +333,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def file_upload_list_uploaded_file_urls(self, **kwargs):  # noqa: E501
         """ListUploadedFileURLs  # noqa: E501
 
-        List all blob store URLs for uploaded files.  # noqa: E501
+        List all blob store URLs for uploaded files.  File uploading is not currently supported in a Cloud deployment. Please use an external data source instead.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.file_upload_list_uploaded_file_urls(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :return: RimeListUploadedFileURLsResponse
@@ -354,15 +354,15 @@
         else:
             (data) = self.file_upload_list_uploaded_file_urls_with_http_info(**kwargs)  # noqa: E501
             return data
 
     def file_upload_list_uploaded_file_urls_with_http_info(self, **kwargs):  # noqa: E501
         """ListUploadedFileURLs  # noqa: E501
 
-        List all blob store URLs for uploaded files.  # noqa: E501
+        List all blob store URLs for uploaded files.  File uploading is not currently supported in a Cloud deployment. Please use an external data source instead.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.file_upload_list_uploaded_file_urls_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :return: RimeListUploadedFileURLsResponse
```

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/firewall_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/firewall_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/firewall_configuration_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/firewall_configuration_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/firewall_service_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/firewall_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/image_registry_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/image_registry_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def image_registry_create_image(self, body, **kwargs):  # noqa: E501
         """CreateImage  # noqa: E501
 
-        Creates a new Managed Image with a unique name.  # noqa: E501
+        Creates a new Managed Image with a unique name.  Managed images are not currently supported in a Cloud deployment. Please reach out to Robust Intelligence for support if this functionality is required for your deployment.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.image_registry_create_image(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param RimeCreateImageRequest body: (required)
@@ -53,15 +53,15 @@
         else:
             (data) = self.image_registry_create_image_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
     def image_registry_create_image_with_http_info(self, body, **kwargs):  # noqa: E501
         """CreateImage  # noqa: E501
 
-        Creates a new Managed Image with a unique name.  # noqa: E501
+        Creates a new Managed Image with a unique name.  Managed images are not currently supported in a Cloud deployment. Please reach out to Robust Intelligence for support if this functionality is required for your deployment.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.image_registry_create_image_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param RimeCreateImageRequest body: (required)
```

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/integration_service_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/integration_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/job_reader_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/job_reader_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/model_card_service_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/model_card_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/model_testing_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/model_testing_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/monitor_service_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/monitor_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/notification_setting_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/notification_setting_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/project_service_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/project_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/registry_service_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/registry_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/results_reader_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/results_reader_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/rime_info_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/rime_info_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/user_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/validation_service_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/validation_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api/workspace_service_api.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api/workspace_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/api_client.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/configuration.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/__init__.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/dataset_dataset.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/dataset_dataset.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/detection_detection_event.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/detection_detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/detection_event_detail.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/detection_event_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/detection_event_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/detection_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/detection_resolution.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/detection_resolution.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/firewall_firewall.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/firewall_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_configure_firewall_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_configure_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_get_file_upload_url_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_get_file_upload_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_validation_result.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_validation_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_validation_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_validation_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/googlerpc_status.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_level.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/integration_integration_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/integration_integration_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/model_model.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/model_model.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_monitor.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_threshold.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_threshold.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitor_transform.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitor_transform.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/notification_digest_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/notification_digest_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/notification_notification.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/notification_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/notification_notification_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/notification_notification_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/notification_object_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/notification_object_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_create_project_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_create_project_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_create_project_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_create_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_get_project_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_get_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_owner_details.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_project.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_project_with_details.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_project_with_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_update_project_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_update_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/protobuf_any.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_connection_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_connection_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_params.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_metadata.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_model_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_pred_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_pred_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registry_validity_status.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registry_validity_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_actor_role.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_actor_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_agent.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent_status.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_agent_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_category_metric.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_category_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_config_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_config_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_failing_row.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_failing_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_feature_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_feature_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_float_list.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_float_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_image_reference.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_image_reference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_int_list.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_int_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_integration_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_integration_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_data.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_job_data.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_job_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_view.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_job_view.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_language.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_language.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_license_feature.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_license_feature.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_license_limit.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_license_limit.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_limit_status.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_limit_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_managed_image.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_managed_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_card.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_task.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_model_task.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_named_double.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_named_double.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_order.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_order.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_safe_url.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_safe_url.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_severity.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_str_list.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_str_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_subject_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_subject_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_suggestion.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_suggestion.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_table_column.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_table_column.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_metric.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_time_interval.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_time_interval.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_token_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_token_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_role.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_uuid.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_uuid.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_workspace.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/role_users_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/role_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/role_workspace_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/role_workspace_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/schemanotification_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/schemanotification_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/statedb_job_status.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/statedb_job_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/user_private_info.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/user_private_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/user_role.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/user_user_detail.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/user_user_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/validate_request_input.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/validate_request_input.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/validate_request_output.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/validate_request_output.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/swagger/swagger_client/rest.py` & `rime_sdk-2.2.0rc9/rime_sdk/swagger/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/test_batch.py` & `rime_sdk-2.2.0rc9/rime_sdk/test_batch.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk/test_run.py` & `rime_sdk-2.2.0rc9/rime_sdk/test_run.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/rime_sdk.egg-info/PKG-INFO` & `rime_sdk-2.2.0rc9/rime_sdk.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime-sdk
-Version: 2.2.0rc8
+Version: 2.2.0rc9
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.2.0rc8/rime_sdk.egg-info/SOURCES.txt` & `rime_sdk-2.2.0rc9/rime_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc8/setup.py` & `rime_sdk-2.2.0rc9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 setup(
     name="rime_sdk",
     packages=find_packages(include=["rime_sdk*"]),
     description="Package to programmatically access a RIME deployment",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    # TODO(blaine): upgrade to semver 3 when it is released.
+    # TODO(VAL-2432): upgrade to semver 3 when it is released.
     setuptools_git_versioning={"enabled": True},
     setup_requires=["setuptools-git-versioning"],
     install_requires=[
         # Note: click is a dependency of `requests` but has to be pinned here
         # due to https://github.com/psf/black/issues/2964 .
         "click==8.0.1",
         "deprecated>=1.0.0,<2.0.0",
```

