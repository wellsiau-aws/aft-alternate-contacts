<!-- BEGIN_TF_DOCS -->
## Requirements

No requirements.

## Providers

| Name | Version |
|------|---------|
| <a name="provider_archive"></a> [archive](#provider\_archive) | n/a |
| <a name="provider_aws"></a> [aws](#provider\_aws) | n/a |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_cloudwatch_log_group.aft_alternate_contacts_add_lambda_log](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_log_group) | resource |
| [aws_cloudwatch_log_group.aft_alternate_contacts_extract_lambda_log](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_log_group) | resource |
| [aws_cloudwatch_log_group.aft_alternate_contacts_validate_lambda_log](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/cloudwatch_log_group) | resource |
| [aws_iam_role.aft_alternate_contacts_add_lambda_role](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.aft_alternate_contacts_extract_lambda_role](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.aft_alternate_contacts_state_role](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role.aft_alternate_contacts_validate_lambda_role](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role) | resource |
| [aws_iam_role_policy.aft_alternate_contacts_add_lambda_role_policy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy) | resource |
| [aws_iam_role_policy.aft_alternate_contacts_state_role_policy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy) | resource |
| [aws_iam_role_policy_attachment.aft_alternate_contacts_add_lambda_role_policy_attachment](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.aft_alternate_contacts_extract_lambda_role_policy_attachment](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_iam_role_policy_attachment.aft_alternate_contacts_validate_lambda_role_policy_attachment](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |
| [aws_lambda_function.aft_alternate_contacts_add_lambda](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_function) | resource |
| [aws_lambda_function.aft_alternate_contacts_extract_lambda](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_function) | resource |
| [aws_lambda_function.aft_alternate_contacts_validate_lambda](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_function) | resource |
| [aws_sfn_state_machine.aft_alternate_contacts_state](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/sfn_state_machine) | resource |
| [archive_file.aft_alternate_contacts_add](https://registry.terraform.io/providers/hashicorp/archive/latest/docs/data-sources/file) | data source |
| [archive_file.aft_alternate_contacts_extract](https://registry.terraform.io/providers/hashicorp/archive/latest/docs/data-sources/file) | data source |
| [archive_file.aft_alternate_contacts_validate](https://registry.terraform.io/providers/hashicorp/archive/latest/docs/data-sources/file) | data source |
| [aws_caller_identity.aft_management_id](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/caller_identity) | data source |
| [aws_dynamodb_table.aft_request_metadata_table](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/dynamodb_table) | data source |
| [aws_iam_policy.AWSLambdaBasicExecutionRole](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy) | data source |
| [aws_region.aft_management_region](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/region) | data source |
| [aws_ssm_parameter.aft_request_metadata_table_name](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/ssm_parameter) | data source |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_aws_ct_mgt_account_id"></a> [aws\_ct\_mgt\_account\_id](#input\_aws\_ct\_mgt\_account\_id) | Control Tower Management Account Id | `string` | n/a | yes |
| <a name="input_aws_ct_mgt_org_id"></a> [aws\_ct\_mgt\_org\_id](#input\_aws\_ct\_mgt\_org\_id) | Control Tower Organization Id | `string` | n/a | yes |
| <a name="input_cloudwatch_log_group_retention"></a> [cloudwatch\_log\_group\_retention](#input\_cloudwatch\_log\_group\_retention) | Lambda CloudWatch log group retention period | `string` | `"0"` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_aft_alternate_contacts_add_lambda_arn"></a> [aft\_alternate\_contacts\_add\_lambda\_arn](#output\_aft\_alternate\_contacts\_add\_lambda\_arn) | aft-alternate-contacts-add Lambda ARN |
| <a name="output_aft_alternate_contacts_extract_lambda_arn"></a> [aft\_alternate\_contacts\_extract\_lambda\_arn](#output\_aft\_alternate\_contacts\_extract\_lambda\_arn) | aft-alternate-contacts-extract Lambda ARN |
| <a name="output_aft_alternate_contacts_state_machine_arn"></a> [aft\_alternate\_contacts\_state\_machine\_arn](#output\_aft\_alternate\_contacts\_state\_machine\_arn) | State machine ARN |
| <a name="output_aft_alternate_contacts_validate_lambda_arn"></a> [aft\_alternate\_contacts\_validate\_lambda\_arn](#output\_aft\_alternate\_contacts\_validate\_lambda\_arn) | aft-alternate-contacts-validate Lambda ARN |
<!-- END_TF_DOCS -->