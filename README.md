# Velero into Azure

![Tfsec](https://github.com/nlamirault/terraform-azurerm-velero/workflows/Tfsec/badge.svg)

## Usage

```hcl
module "velero" {
  source  = "nlamirault/velero/azurerm"
  version = "1.0.0"


}
```

and variables :

```hcl

```

## Documentation

<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Requirements

| Name | Version |
|------|---------|
| terraform | >= 1.0.0 |
| azurerm | >= 2.48.0 |

## Providers

| Name | Version |
|------|---------|
| azurerm | >= 2.48.0 |

## Modules

No Modules.

## Resources

| Name |
|------|
| [azurerm_resource_group](https://registry.terraform.io/providers/hashicorp/azurerm/2.48.0/docs/resources/resource_group) |
| [azurerm_role_assignment](https://registry.terraform.io/providers/hashicorp/azurerm/2.48.0/docs/resources/role_assignment) |
| [azurerm_storage_account](https://registry.terraform.io/providers/hashicorp/azurerm/2.48.0/docs/resources/storage_account) |
| [azurerm_storage_container](https://registry.terraform.io/providers/hashicorp/azurerm/2.48.0/docs/resources/storage_container) |
| [azurerm_user_assigned_identity](https://registry.terraform.io/providers/hashicorp/azurerm/2.48.0/docs/resources/user_assigned_identity) |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| resource\_group\_location | The Azure Region where the Resource Group should exist | `string` | n/a | yes |
| resource\_group\_name | The Name which should be used for this Resource Group | `string` | n/a | yes |
| tags | A mapping of tags to assign to the resource. | `map(string)` | <pre>{<br>  "made-by": "terraform"<br>}</pre> | no |

## Outputs

| Name | Description |
|------|-------------|
| user\_assigned\_identity\_id | ID of the user assigned identity |
| user\_assigned\_identity\_name | Name of the user assigned identity |
<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
