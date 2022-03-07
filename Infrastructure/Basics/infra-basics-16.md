# infra-basics-16

## Description

The vm is not deployed via code. If not already, the customer would like that the vm password is randomly generated and added to a kv. Next to this, they want it to be part of a github workflow so it is easy to deploy.

If you are looking for some additional setup of the vm please look [here](../Advanced/infra-advanced-1.md)

## Outcome

- make sure the password is randomly generated and stored in a keyvault
- deploy the solution via github workflow
- update the design if needed

## References

It is not mandantory to use these references.

- [Bicep documentation](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/)
- [Azure documentation](https://docs.microsoft.com/en-us/azure/)
- [Azure Architecture Center](https://docs.microsoft.com/en-us/azure/architecture/)
- [VS Code documentation](https://code.visualstudio.com/Docs)
- [Azure CLI](https://docs.microsoft.com/en-us/cli/azure/reference-index?view=azure-cli-latest)
- [WSL](https://docs.microsoft.com/en-us/windows/wsl/about)
- [Azure PowerShell](https://docs.microsoft.com/en-us/powershell/azure/?view=azps-6.6.0)
- [GitHub documentation](https://docs.github.com/en)
- [Terraform state in Azure](https://www.terraform.io/language/settings/backends/azurerm)
- [Terraform documentation](https://www.terraform.io/docs)
- [Terraform: Azure registry documentation (azurerm)](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs)
- [Terraform: Azure AD registry documentation (azuread)](https://registry.terraform.io/providers/hashicorp/azuread/latest/docs)

[back](./infra-basics-16.md) <--- [TO OVERVIEW](../Infrastructure.md) ---> [next](./infra-basics-17.md)