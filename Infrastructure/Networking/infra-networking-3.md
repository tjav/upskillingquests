# infra-networking-3 - use Azure Bastion to remotely access a VM

## Description

[TO BE COMPLETED]

Contoso is very happy with there first Virtual Network and wants to get value out of it, by deploying a Virtual Machine that they can access remotely. They have the requirement that Virtual Machine may not have a direct Public IP Address assigned, but still it needs to be possible to RDP remotely into the VM.

## Outcome

  - Programmatically deploy a Virtual Machine into a Virtual Network.
  - Deploy the prerequisites for Azure Bastion into the same or a separate Virtual Network. Note that a seperate Virtual Network requires a connect (Virtual Network Peering) with the destinated VM. 
  - Take security into account. Is there a manner to increase security of Azure Bastion? If so, how? 
    - Think about Identity & Access Management, and Networking Security Whitelisting.
  - RDP (or SSH) into the VM.
  
The solution should look like something as this:

![image](tjav/upskillingquests/Infrastructure/Networking/Network-quest02.jpg)

## Review and discussion

If you want to discuss the outcome, or have a validation of your quest, contact Dwaine Ridderhof. 

## References

It is not mandatory to use these references.

  - [What is Azure Bastion?](https://docs.microsoft.com/en-us/azure/bastion/bastion-overview)
  - [Azure Bastion nsg](https://docs.microsoft.com/en-us/azure/bastion/bastion-nsg)
  - [Vnet peering and Azure Bastion](https://docs.microsoft.com/en-us/azure/bastion/vnet-peering)
