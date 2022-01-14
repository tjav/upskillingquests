# Security-Basics-7 Custom Policies

## Description

Following up on the quests for Azure Policy this final quests takes it to custom coding. This quest expects that you already completed the previous quests related to Azure Policies. The goal of this quest is to create a custom policy definition. If your role will be working with Azure Governance it is strongly recommended to get familiar with the [Policy as Code Framework](https://dev.azure.com/servicescode/infra-as-code-source/_git/Components?path=/Utilities/PolicyAsCodeFramework) in the infra-as-code-source offering that is accessible at [aka.ms/iacs](https://aka.ms/iacs).


## Outcome

Create a custom policy that enforces a shut down of virtual machines at a predefined time of every day. Assign it to your environment and validate that it configures the auto-shutdown for VMs.

Optional: Deploy the [Policy as Code Framework](https://dev.azure.com/servicescode/infra-as-code-source/_git/Components?path=/Utilities/PolicyAsCodeFramework) and use pipelines in your environment to deploy and assign your custom policy.

## Review and discussion
When would you create a custom policies?
What are the pros and cons for creating custom policies?
What operational concerns would you have for leveraging custom policies?
How would you maintain custom policies from an operational perspective?
What are the pros and cons for the pipeline based depolyments of Azure Policies using the Policy as Code Framework?

If you want to talk through or validate your quest after you completed, contact [Matyas Safranka](mailto:matyas@microsoft.com) via email or Teams.

## References

It is not mandatory to use these references.

- [Tutorial: Create a custom policy definition](https://docs.microsoft.com/en-us/azure/governance/policy/tutorials/create-custom-policy-definition)
- [Azure Policy definition structure](https://docs.microsoft.com/en-us/azure/governance/policy/concepts/definition-structure)
- [Azure Policy initiative definition structure](https://docs.microsoft.com/en-us/azure/governance/policy/concepts/initiative-definition-structure)
- [Wilfried Woivré - Azure Policy - Auto shutdown your virtual machines](https://dev.to/wilfriedwoivre/azure-policy-auto-shutdown-your-virtual-machines-22m7#:~:text=Auto-shutdown%20%3A%20Available%20as%20built-in%20feature%20in%20Azure%2C,VM%20separatly%2C%20and%20define%20custom%20hour%20for%20each.)
- [Azure Policy on GitHub](https://github.com/Azure/azure-policy)
- [Policy as Code Framework](https://dev.azure.com/servicescode/infra-as-code-source/_git/Components?path=/Utilities/PolicyAsCodeFramework)
- [infra-as-code-source offering](https://aka.ms/iacs)
- [Programmatically create policies](https://docs.microsoft.com/en-us/azure/governance/policy/how-to/programmatically-create)

[back](./security-basics-6.md) <--- * ---> [back to security](../Security.md)
