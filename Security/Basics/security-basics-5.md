# Security-Basics-5 Governance with Policies

## Description

One of the [design principles](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/ready/enterprise-scale/design-principles) of the [Enterprise Scale Landing Zones](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/ready/enterprise-scale/architecture#:~:text=Enterprise-scale%20is%20an%20architectural%20approach%20and%20a%20reference,roadmap%20and%20the%20Cloud%20Adoption%20Framework%20for%20Azure.) is the Policy driven governance. The idea is to enable democratization of subscriptions and therefore application owner DevOps teams to be able to choose their way of work, tooling etc. by enforcing guardrails instead of restricting them on their choices of tooling or describing how and what they can do. [Azure Policy](https://docs.microsoft.com/en-us/azure/governance/policy/overview) helps with defining such guardrails.

The purpose of this quest is to explore the capabilities of Azure Policies.


## Outcome

Use the built-in 'Secure transfer to storage accounts should be enabled' Azure Policy to achieve the following:
- Assign the Policy to your subscription or to a resource group in your environment in Audit mode
- Create a Storage Account. After deployment go to the 'Configuration' point under 'Settings' for the Storage account and select 'Disabled' for 'Secure transfer required'.
- Go back to Azure Policies in the Portal and select the Compliance section. Wait until the non-compliant resources show up, you might need to refresh and wait up to an hour or so. Then change the setting back to 'Enabled'.
- Change the Policy assignment to 'Deny'
- Go back to the storage account and go to the 'Configuration' point under 'Settings' for the Storage account and select 'Disabled' for 'Secure transfer required'.

## Review and discussion
When would you use Audit? When would you use Deny? 
What is the difference between a Policy and an Initiative?
When would you assign a Policy? When would you assign an Initiative?

If you want to talk through or validate your quest after you completed, contact [Matyas Safranka](mailto:matyas@microsoft.com) via email or Teams.

## References

It is not mandatory to use these references.

- [What is Azure Policy?](https://docs.microsoft.com/en-us/azure/governance/policy/overview)
- [Understand Azure Policy effects](https://docs.microsoft.com/en-us/azure/governance/policy/concepts/effects)
- [Quickstart: Create a policy assignment to identify non-compliant resources](https://docs.microsoft.com/en-us/azure/governance/policy/assign-policy-portal)
- [Azure Policy built-in policy definitions](https://docs.microsoft.com/en-us/azure/governance/policy/samples/built-in-policies)
- [Azure Policy built-in initiative definitions](https://docs.microsoft.com/en-us/azure/governance/policy/samples/built-in-initiatives)
- [Tutorial: Create and manage policies to enforce compliance](https://docs.microsoft.com/en-us/azure/governance/policy/tutorials/create-and-manage)


[back](./security-basics-4.md) <--- * ---> [next](./security-basics-6.md)
