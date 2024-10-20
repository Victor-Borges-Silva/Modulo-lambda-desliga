<!-- BEGIN_TF_DOCS -->
## Requirements

No requirements.

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | 5.57.0 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_lambda_function.DesligaEC2](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lambda_function) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_armazenamento_temporario"></a> [armazenamento\_temporario](#input\_armazenamento\_temporario) | Espaço do disco temporario de armazenamento | `number` | n/a | yes |
| <a name="input_instancia_id"></a> [instancia\_id](#input\_instancia\_id) | lista de instancia a ser iniciada | `list(string)` | <pre>[<br>  "Default_Variabletf"<br>]</pre> | no |
| <a name="input_nome_funcao_desliga"></a> [nome\_funcao\_desliga](#input\_nome\_funcao\_desliga) | Nome da função lambda | `string` | `"Default_Variabletf"` | no |
| <a name="input_rastreio_log"></a> [rastreio\_log](#input\_rastreio\_log) | Ativar ou Desativar rastreio | `string` | n/a | yes |
| <a name="input_role"></a> [role](#input\_role) | ARN da função IAM | `string` | `"Default_Variabletf"` | no |
| <a name="input_tamanho_memoria"></a> [tamanho\_memoria](#input\_tamanho\_memoria) | Tamanho max para armezenar a função | `number` | n/a | yes |
| <a name="input_timeout"></a> [timeout](#input\_timeout) | Tempo max de execução da função | `number` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_lambda_function_arn"></a> [lambda\_function\_arn](#output\_lambda\_function\_arn) | n/a |
| <a name="output_lambda_function_name_desliga"></a> [lambda\_function\_name\_desliga](#output\_lambda\_function\_name\_desliga) | n/a |
<!-- END_TF_DOCS -->