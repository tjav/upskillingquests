# infra-advanced-1

## Description

An application team needs to use get Windows VMs in Azure that will be used to created Jupyter notebooks on the vm. This means that the vms should have software being preinstalled. The company is already a heavily user of *Ansible Playbooks*, and this would be the prefered way to deploy the software.

## Outcome

Enable application team members to work by creating vms through code with preinstalled software through code. Make sure you end up with at least:
  
- Architecture drawing
- pipline that deploys the vm (windows 10)
- make sure the following is installed:
  - Git
  - Python
  - pip
  - WSL (v2.*)
  - VSCode
  - Visual Studio Jupyter VSCode Extension
  - Microsoft Azure Storage Explorer
  - Postman

## References

It is not mandantory to use these references.

- [Ansible playbooks on windows](https://docs.ansible.com/ansible/latest/user_guide/windows_usage.html)
- [GitHub Actions](https://docs.github.com/en/actions)
- [Azure Pipelines](https://docs.microsoft.com/en-us/azure/devops/pipelines/get-started/what-is-azure-pipelines?view=azure-devops)
- [Azure Resource Manager documentation](https://docs.microsoft.com/en-us/azure/azure-resource-manager/)
- [Terraform on Azure](https://docs.microsoft.com/en-gb/azure/developer/terraform/)
- [Terraform Azure provider](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs)
- [VS Code documentation](https://code.visualstudio.com/Docs)

[back](../Infrastructure.md) <--- * ---> [next](./infra-advanced-2.md)
