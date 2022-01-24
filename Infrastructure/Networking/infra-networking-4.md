# infra-networking-4 - filter traffic between Azure Private and Azure Public using a firewall

## Description

Contoso her CISO department heard about the focus on Azure. They require an improvement to the security posture where all outbound connectivity towards Azure Public or Internet is filtered. They requested you to investigate Azure Firewall or a third-party firewall solution, including a rational. Can you advise them and implement a pilot? 

## Outcome

  - Deploy a Virtual Network and include the requirements of your firewall solution.
  - Deploy a firewall solution
  - Enforce **all** outbound connectivity via the firewall.
  - [_Optionally_] Update your IP Address Management scheme, see [infra-networking-1 - deploy an Azure Virtual Network via ARM](https://github.com/tjav/upskillingquests/blob/Dwaine/UpdateNetworkingQuests/Infrastructure/Networking/infra-networking-1.md)
  - Deploy whitelisting and take into account that some services _require_ specific whitelisting
  - Describe the reasoning (rational) of your chosen firewall solution.
  - Deploy everything via Infrastructure as Code, using a Release pipeline.
  - Any design decisions you want to capture?
  
The solution should look like something as this:

![image](https://user-images.githubusercontent.com/25753877/149521820-9a3464f0-aa53-4cd8-9e0e-5a17f7d838f6.png)

## Review and discussion

If you want to discuss the outcome, or have a validation of your quest, contact Dwaine Ridderhof. 

## References

It is not mandatory to use these references.

  - [Deploy and configure Azure Firewall](https://docs.microsoft.com/En-us/azure/firewall/tutorial-firewall-deploy-portal)
  - [Azure Firewall Manager](https://docs.microsoft.com/en-us/azure/firewall-manager/policy-overview)
  - [Azure Firewall architecture overview](https://docs.microsoft.com/en-us/azure/architecture/example-scenario/firewalls/)