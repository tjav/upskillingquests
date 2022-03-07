# infra-basics-2

## Description

Now that there is a storage account, we can store an ARM template in it. As a starter we like to store the storage account template. Right now the template isn't ready to be deployed for other deployments. The template needs to be parameterized and a container should be deployed with the template. Contoso has the requirement that the storage account should always be in the same location as the resource group it is deployed to.

## Outcome

- Parametize the storage account template
- Deploy again creating a container
- Upload the template to the container using Azure CLI or PowerShell

## References

It is not mandantory to use these references.

- [Azure Resource Manager documentation](https://docs.microsoft.com/en-us/azure/azure-resource-manager/)
- [Azure Architecture Center](https://docs.microsoft.com/en-us/azure/architecture/)
- [VS Code documentation](https://code.visualstudio.com/Docs)
- [Azure CLI](https://docs.microsoft.com/en-us/cli/azure/reference-index?view=azure-cli-latest)
- [WSL](https://docs.microsoft.com/en-us/windows/wsl/about)
- [Azure PowerShell](https://docs.microsoft.com/en-us/powershell/azure/?view=azps-6.6.0)

[back](./infra-basics-1.md) <--- [TO OVERVIEW](../Infrastructure.md) ---> [next](./infra-basics-3.md)
