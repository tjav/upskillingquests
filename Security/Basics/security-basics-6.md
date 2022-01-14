# Security-Basics-6 Remediation with Policies

## Description

This quest assumes that you already completed the [Governance with Policies](./security-basics-5.md) quest.

One of the strenghts of Azure Policies to implement the previously mentioned guardrails is that it supports the [Deny](https://docs.microsoft.com/en-us/azure/governance/policy/concepts/effects#deny) but also the [DeployIfNotExists](https://docs.microsoft.com/en-us/azure/governance/policy/concepts/effects#deployifnotexists) and [Modify](https://docs.microsoft.com/en-us/azure/governance/policy/concepts/effects#modify) effects. This means that Policies can configure deployed resources as well and not only audit compliance or prevent changes through settings. Theoretically since Policies are using the same resource model as ARM it can be used to deploy custom resources as well, but more about that in custom policies in the next quest.

Azure Policies with `DeployIfNotExists` conditions allow administrators to configure resources to a compliant state. This is 


## Outcome
Use the built-in 'Configure Storage account to use a private link connection' Azure Policy
- Asign it to the same scope that you have used in the previous quest
- On the Azure Portal go to the Policy section and Select remediation. Wait until the non-compliant resources show up, you might need to refresh and wait up to an hour or so. Then apply the remediation.
- After the remediation is completed check the results.

## Review and discussion
What is the main difference between DeployIfNotExists and Modify?
When would you use Deny and when would you use DeployIfNotExists policy?
What are the pros and cons of using Azure Policy remediation (from operational and from security perspectives)?

If you want to talk through or validate your quest after you completed, contact [Matyas Safranka](mailto:matyas@microsoft.com) via email or Teams.

## References

It is not mandatory to use these references.

- [Remediate non-compliant resources with Azure Policy](https://docs.microsoft.com/en-us/azure/governance/policy/how-to/remediate-resources)
- [Deploy Azure Policy to delegated subscriptions at scale](https://docs.microsoft.com/en-us/azure/lighthouse/how-to/policy-at-scale?toc=/azure/governance/policy/toc.json&bc=/azure/governance/policy/breadcrumb/toc.json)
- [Troubleshoot errors with using Azure Policy](https://docs.microsoft.com/en-us/azure/governance/policy/troubleshoot/general)

- [Understand the guest configuration feature of Azure Policy](https://docs.microsoft.com/en-us/azure/governance/policy/concepts/guest-configuration)



[back](./security-basics-5.md) <--- * ---> [next](./security-basics-7.md)
