<a href="https://lacework.com"><img src="https://techally-content.s3-us-west-1.amazonaws.com/public-content/lacework_logo_full.png" width="600"></a>

# terraform-gcp-agentless-scanning

[![GitHub release](https://img.shields.io/github/release/lacework/terraform-gcp-agentless-scanning.svg)](https://github.com/lacework/terraform-gcp-agentless-scanning/releases/)
[![Codefresh build status](https://g.codefresh.io/api/badges/pipeline/lacework/terraform-modules%2Ftest-compatibility?type=cf-1&key=eyJhbGciOiJIUzI1NiJ9.NWVmNTAxOGU4Y2FjOGQzYTkxYjg3ZDEx.RJ3DEzWmBXrJX7m38iExJ_ntGv4_Ip8VTa-an8gBwBo)](https://g.codefresh.io/pipelines/edit/new/builds?id=607e25e6728f5a6fba30431b&pipeline=test-compatibility&projects=terraform-modules&projectId=607db54b728f5a5f8930405d)

A Terraform Module to configure the Lacework Agentless Scanner.

## Requirements

| Name                                                                     | Version    |
| ------------------------------------------------------------------------ | ---------- |
| <a name="requirement_terraform"></a> [terraform](#requirement_terraform) | >= 0.12.31 |
| <a name="requirement_google"></a> [google](#requirement_google)          | ~> 4.46    |
| <a name="requirement_lacework"></a> [lacework](#requirement_lacework)    | ~> 1.3     |

## Providers

| Name                                                            | Version |
| --------------------------------------------------------------- | ------- |
| <a name="provider_google"></a> [google](#provider_google)       | 4.46.0  |
| <a name="provider_lacework"></a> [lacework](#provider_lacework) | 1.3.0   |
| <a name="provider_random"></a> [random](#provider_random)       | 3.4.3   |

## Modules

| Name                                                                                                                                         | Source                       | Version |
| -------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------- | ------- |
| <a name="module_lacework_agentless_scan_svc_account"></a> [lacework_agentless_scan_svc_account](#module_lacework_agentless_scan_svc_account) | lacework/service-account/gcp | ~> 1.0  |

## Resources

| Name                                                                                                                                                                                     | Type        |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- |
| [google_cloud_run_v2_job.agentless_orchestrate](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/cloud_run_v2_job)                                         | resource    |
| [google_cloud_scheduler_job.agentless_orchestrate](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/cloud_scheduler_job)                                   | resource    |
| [google_organization_iam_custom_role.agentless_orchestrate](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/organization_iam_custom_role)                 | resource    |
| [google_organization_iam_member.agentless_orchestrate](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/organization_iam_member)                           | resource    |
| [google_project_iam_custom_role.agentless_orchestrate](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/project_iam_custom_role)                           | resource    |
| [google_project_iam_custom_role.agentless_orchestrate_project](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/project_iam_custom_role)                   | resource    |
| [google_project_iam_custom_role.agentless_scan](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/project_iam_custom_role)                                  | resource    |
| [google_project_iam_member.agentless_orchestrate](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/project_iam_member)                                     | resource    |
| [google_project_iam_member.agentless_orchestrate_invoker](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/project_iam_member)                             | resource    |
| [google_project_iam_member.agentless_orchestrate_project](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/project_iam_member)                             | resource    |
| [google_project_iam_member.agentless_orchestrate_service_account](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/project_iam_member)                     | resource    |
| [google_project_iam_member.agentless_orchestrate_service_account_user](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/project_iam_member)                | resource    |
| [google_project_iam_member.agentless_scan](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/project_iam_member)                                            | resource    |
| [google_project_iam_member.lacework_svc_account](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/project_iam_member)                                      | resource    |
| [google_project_service.required_apis](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/project_service)                                                   | resource    |
| [google_secret_manager_secret.agentless_orchestrate](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/secret_manager_secret)                               | resource    |
| [google_secret_manager_secret_iam_member.member](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/secret_manager_secret_iam_member)                        | resource    |
| [google_secret_manager_secret_version.agentless_orchestrate](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/secret_manager_secret_version)               | resource    |
| [google_service_account.agentless_orchestrate](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/service_account)                                           | resource    |
| [google_service_account.agentless_scan](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/service_account)                                                  | resource    |
| [google_storage_bucket.lacework_bucket](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/storage_bucket)                                                   | resource    |
| [google_storage_bucket_iam_binding.lacework_bucket](https://registry.terraform.io/providers/hashicorp/google/latest/docs/resources/storage_bucket_iam_binding)                           | resource    |
| [lacework_integration_gcp_agentless_scanning.lacework_cloud_account](https://registry.terraform.io/providers/lacework/lacework/latest/docs/resources/integration_gcp_agentless_scanning) | resource    |
| [random_id.uniq](https://registry.terraform.io/providers/hashicorp/random/latest/docs/resources/id)                                                                                      | resource    |
| [google_compute_default_service_account.default](https://registry.terraform.io/providers/hashicorp/google/latest/docs/data-sources/compute_default_service_account)                      | data source |
| [google_project.selected](https://registry.terraform.io/providers/hashicorp/google/latest/docs/data-sources/project)                                                                     | data source |
| [lacework_user_profile.current](https://registry.terraform.io/providers/lacework/lacework/latest/docs/data-sources/user_profile)                                                         | data source |

## Inputs

| Name                                                                                                                                                               | Description                                                                                       | Type                                                                                                                                                                                                                                                                           | Default                                                                                                                                                                                                                                                | Required |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | :------: |
| <a name="input_agentless_orchestrate_service_account_email"></a> [agentless_orchestrate_service_account_email](#input_agentless_orchestrate_service_account_email) | The email of the service account for which to use during scan tasks.                              | `string`                                                                                                                                                                                                                                                                       | `""`                                                                                                                                                                                                                                                   |    no    |
| <a name="input_agentless_scan_secret_id"></a> [agentless_scan_secret_id](#input_agentless_scan_secret_id)                                                          | The ID of the Google Secret containing the Lacework Account and Auth Token                        | `string`                                                                                                                                                                                                                                                                       | `""`                                                                                                                                                                                                                                                   |    no    |
| <a name="input_agentless_scan_service_account_email"></a> [agentless_scan_service_account_email](#input_agentless_scan_service_account_email)                      | The email of the service account for which to use during scan tasks.                              | `string`                                                                                                                                                                                                                                                                       | `""`                                                                                                                                                                                                                                                   |    no    |
| <a name="input_bucket_enable_ubla"></a> [bucket_enable_ubla](#input_bucket_enable_ubla)                                                                            | Boolean for enabling Uniform Bucket Level Access on the created bucket. Default is `true`.        | `bool`                                                                                                                                                                                                                                                                         | `true`                                                                                                                                                                                                                                                 |    no    |
| <a name="input_bucket_force_destroy"></a> [bucket_force_destroy](#input_bucket_force_destroy)                                                                      | Force destroy bucket (Required when bucket not empty)                                             | `bool`                                                                                                                                                                                                                                                                         | `true`                                                                                                                                                                                                                                                 |    no    |
| <a name="input_bucket_lifecycle_rule_age"></a> [bucket_lifecycle_rule_age](#input_bucket_lifecycle_rule_age)                                                       | Number of days to keep agentless scan objects in bucket before deletion.                          | `number`                                                                                                                                                                                                                                                                       | `30`                                                                                                                                                                                                                                                   |    no    |
| <a name="input_global"></a> [global](#input_global)                                                                                                                | Whether or not to create global resources. Defaults to `false`.                                   | `bool`                                                                                                                                                                                                                                                                         | `false`                                                                                                                                                                                                                                                |    no    |
| <a name="input_global_module_reference"></a> [global_module_reference](#input_global_module_reference)                                                             | A reference to the global lacework_gcp_agentless_scanning module for this account.                | <pre>object({<br> agentless_orchestrate_service_account_email = string<br> agentless_scan_service_account_email = string<br> agentless_scan_secret_id = string<br> lacework_account = string<br> lacework_domain = string<br> prefix = string<br> suffix = string<br> })</pre> | <pre>{<br> "agentless_orchestrate_service_account_email": "",<br> "agentless_scan_secret_id": "",<br> "agentless_scan_service_account_email": "",<br> "lacework_account": "",<br> "lacework_domain": "",<br> "prefix": "",<br> "suffix": ""<br>}</pre> |    no    |
| <a name="input_image_url"></a> [image_url](#input_image_url)                                                                                                       | The container image url for Lacework Agentless Workload Scanning.                                 | `string`                                                                                                                                                                                                                                                                       | `"us-docker.pkg.dev/cloudrun/container/hello"`                                                                                                                                                                                                         |    no    |
| <a name="input_integration_type"></a> [integration_type](#input_integration_type)                                                                                  | Specify the integration type. Can only be PROJECT or ORGANIZATION. Defaults to PROJECT            | `string`                                                                                                                                                                                                                                                                       | `"PROJECT"`                                                                                                                                                                                                                                            |    no    |
| <a name="input_labels"></a> [labels](#input_labels)                                                                                                                | Set of labels which will be added to the resources managed by the module.                         | `map(string)`                                                                                                                                                                                                                                                                  | `{}`                                                                                                                                                                                                                                                   |    no    |
| <a name="input_lacework_account"></a> [lacework_account](#input_lacework_account)                                                                                  | The name of the Lacework account with which to integrate.                                         | `string`                                                                                                                                                                                                                                                                       | `""`                                                                                                                                                                                                                                                   |    no    |
| <a name="input_lacework_domain"></a> [lacework_domain](#input_lacework_domain)                                                                                     | The domain of the Lacework account with with to integrate.                                        | `string`                                                                                                                                                                                                                                                                       | `"lacework.net"`                                                                                                                                                                                                                                       |    no    |
| <a name="input_lacework_integration_name"></a> [lacework_integration_name](#input_lacework_integration_name)                                                       | The name of the Lacework cloud account integration.                                               | `string`                                                                                                                                                                                                                                                                       | `"google-cloud-agentless-scanning"`                                                                                                                                                                                                                    |    no    |
| <a name="input_organization_id"></a> [organization_id](#input_organization_id)                                                                                     | The organization ID, required if integration_type is set to ORGANIZATION                          | `string`                                                                                                                                                                                                                                                                       | `""`                                                                                                                                                                                                                                                   |    no    |
| <a name="input_prefix"></a> [prefix](#input_prefix)                                                                                                                | A string to be prefixed to the name of all new resources.                                         | `string`                                                                                                                                                                                                                                                                       | `"lacework-awls"`                                                                                                                                                                                                                                      |    no    |
| <a name="input_project_filter_list"></a> [project_filter_list](#input_project_filter_list)                                                                         | A list of projects to include/exclude for integration.                                            | `list(any)`                                                                                                                                                                                                                                                                    | `[]`                                                                                                                                                                                                                                                   |    no    |
| <a name="input_region"></a> [region](#input_region)                                                                                                                | The region in which to create resources.                                                          | `string`                                                                                                                                                                                                                                                                       | `"us-central1"`                                                                                                                                                                                                                                        |    no    |
| <a name="input_regional"></a> [regional](#input_regional)                                                                                                          | Whether or not to create regional resources. Defaults to `false`.                                 | `bool`                                                                                                                                                                                                                                                                         | `false`                                                                                                                                                                                                                                                |    no    |
| <a name="input_required_apis"></a> [required_apis](#input_required_apis)                                                                                           | n/a                                                                                               | `map(any)`                                                                                                                                                                                                                                                                     | <pre>{<br> "cloudscheduler": "cloudscheduler.googleapis.com",<br> "compute": "compute.googleapis.com",<br> "iam": "iam.googleapis.com",<br> "run": "run.googleapis.com",<br> "secretmanager": "secretmanager.googleapis.com"<br>}</pre>                |    no    |
| <a name="input_scan_containers"></a> [scan_containers](#input_scan_containers)                                                                                     | Whether to includes scanning for containers. Defaults to `true`.                                  | `bool`                                                                                                                                                                                                                                                                         | `true`                                                                                                                                                                                                                                                 |    no    |
| <a name="input_scan_frequency_hours"></a> [scan_frequency_hours](#input_scan_frequency_hours)                                                                      | How often in hours the scan will run in hours. Defaults to `24`.                                  | `number`                                                                                                                                                                                                                                                                       | `24`                                                                                                                                                                                                                                                   |    no    |
| <a name="input_scan_host_vulnerabilities"></a> [scan_host_vulnerabilities](#input_scan_host_vulnerabilities)                                                       | Whether to includes scanning for host vulnerabilities. Defaults to `true`.                        | `bool`                                                                                                                                                                                                                                                                         | `true`                                                                                                                                                                                                                                                 |    no    |
| <a name="input_scanning_project_id"></a> [scanning_project_id](#input_scanning_project_id)                                                                         | A project ID different from the default defined inside the provider - used for scanning resources | `string`                                                                                                                                                                                                                                                                       | `""`                                                                                                                                                                                                                                                   |    no    |
| <a name="input_service_account_name"></a> [service_account_name](#input_service_account_name)                                                                      | The name of the service account Lacework will use to access scan results.                         | `string`                                                                                                                                                                                                                                                                       | `""`                                                                                                                                                                                                                                                   |    no    |
| <a name="input_suffix"></a> [suffix](#input_suffix)                                                                                                                | A string to be appended to the end of the name of all new resources.                              | `string`                                                                                                                                                                                                                                                                       | `""`                                                                                                                                                                                                                                                   |    no    |

## Outputs

| Name                                                                                                                                                                 | Description                                                   |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------- |
| <a name="output_agentless_orchestrate_service_account_email"></a> [agentless_orchestrate_service_account_email](#output_agentless_orchestrate_service_account_email) | Output Cloud Run service account email.                       |
| <a name="output_agentless_scan_secret_id"></a> [agentless_scan_secret_id](#output_agentless_scan_secret_id)                                                          | Google Secret Manager ID for Lacework Account and Token.      |
| <a name="output_agentless_scan_service_account_email"></a> [agentless_scan_service_account_email](#output_agentless_scan_service_account_email)                      | Output Compute service account email.                         |
| <a name="output_bucket_name"></a> [bucket_name](#output_bucket_name)                                                                                                 | The storage bucket name for Agentless Workload Scanning data. |
| <a name="output_lacework_account"></a> [lacework_account](#output_lacework_account)                                                                                  | Lacework Account Name for Integration.                        |
| <a name="output_lacework_domain"></a> [lacework_domain](#output_lacework_domain)                                                                                     | Lacework Domain Name for Integration.                         |
| <a name="output_prefix"></a> [prefix](#output_prefix)                                                                                                                | Prefix used to add uniqueness to resource names.              |
| <a name="output_service_account_name"></a> [service_account_name](#output_service_account_name)                                                                      | The service account name for Lacework.                        |
| <a name="output_service_account_private_key"></a> [service_account_private_key](#output_service_account_private_key)                                                 | The base64 encoded private key in JSON format for Lacework.   |
| <a name="output_suffix"></a> [suffix](#output_suffix)                                                                                                                | Suffix used to add uniqueness to resource names.              |
