## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| admin\_create\_user\_config | \(Optional\) - The configuration for AdminCreateUser requests. | map | `{}` | no |
| alias\_attributes | Possible values in list: phone\_number, email, preferred\_username | list | `"null"` | no |
| auto\_verified\_attributes | \(Optional\) The attributes to be auto-verified. Possible values: email, phone\_number. | list | `[]` | no |
| certificate\_arn | \(Optional\) The ARN of an ISSUED ACM certificate in us-east-1 for a custom domain. | string | `"null"` | no |
| device\_configuration | \(Optional\) - The configuration for the user pool's device tracking. | map | `{}` | no |
| domain | Cognito User Pool Domain string | string | `"null"` | no |
| email\_configuration | \(Optional\) - The Email Configuration. | map | `{}` | no |
| email\_verification\_message | \(Optional\) A string representing the email verification message. Conflicts with verification\_message\_template configuration block email\_message argument. | string | `"null"` | no |
| email\_verification\_subject | \(Optional\) A string representing the email verification subject. Conflicts with verification\_message\_template configuration block email\_subject argument. | string | `"null"` | no |
| invite\_message\_template |  | map | `{}` | no |
| lambda\_config | \(Optional\) - A container for the AWS Lambda triggers associated with the user pool. | map | `{}` | no |
| mfa\_configuration | Possible string values: ON, OFF, OPTIONAL | string | `"OFF"` | no |
| name |  | string | `"cognito-default-name"` | no |
| password\_policy | \(Optional\) - A container for information about the user pool password policy. | map | `{}` | no |
| schema | \(Optional\) - A container with the schema attributes of a user pool. Maximum of 50 attributes. | list | `[]` | no |
| sms\_authentication\_message | \(Optional\) A string representing the SMS authentication message. | string | `"null"` | no |
| sms\_configuration | \(Optional\) - The SMS Configuration. | map | `{}` | no |
| sms\_verification\_message | \(Optional\) A string representing the SMS verification message. Conflicts with verification\_message\_template configuration block sms\_message argument. | string | `"null"` | no |
| user\_pool\_add\_ons | \(Optional\) Configuration block for user pool add-ons to enable user pool advanced security mode features. | map | `{}` | no |
| user\_pool\_client | Cognito User Pool app client configuration | list | `[]` | no |
| user\_pool\_group | Cognito User Pool group | list | `[]` | no |
| user\_pool\_identity\_provider | Cognito User Pool Identity Provider | list | `[]` | no |
| user\_pool\_resource\_server | Cognito User Pool Resource Server | list | `[]` | no |
| username\_attributes | Possible values in list: phone\_number, email | list | `"null"` | no |
| verification\_message\_template | \(Optional\) - The verification message templates configuration. | map | `{}` | no |

## Outputs

| Name | Description |
|------|-------------|
| arn | The ARN of the user pool. |
| endpoint | The endpoint name of the user pool. Example format: cognito-idp.REGION.amazonaws.com/xxxx\_yyyyy |
| id | The id of the user pool |
