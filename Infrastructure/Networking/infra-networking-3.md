# infra-networking-3 - use Azure Bastion to remotely access a VM

## Description

Contoso is very happy with there Hub-spoke architecture. They would like to improve there security posture and remove any Public IP's assigned to Virtual Machines and still be able to access them remotely. 

## Outcome

  - Deploy the prerequisites for Azure Bastion into the Hub Virtual Network. 
  - Take security into account. Is there a manner to increase security of Azure Bastion? If so, how? 
    - Think about Identity & Access Management, and Networking Security Whitelisting.
  - RDP (or SSH) into the VM through the Azure Portal or natively via Windows (mstsc.exe).
  
The solution should look like something as this:

![image](https://user-images.githubusercontent.com/25753877/149521820-9a3464f0-aa53-4cd8-9e0e-5a17f7d838f6.png)

## Review and discussion

If you want to discuss the outcome, or have a validation of your quest, contact Dwaine Ridderhof. 

## References

It is not mandatory to use these references.

  - [What is Azure Bastion?](https://docs.microsoft.com/en-us/azure/bastion/bastion-overview)
  - [Azure Bastion nsg](https://docs.microsoft.com/en-us/azure/bastion/bastion-nsg)
  - [Vnet peering and Azure Bastion](https://docs.microsoft.com/en-us/azure/bastion/vnet-peering)
  - [Connect to a VM using the native client on your Windows computer](https://docs.microsoft.com/en-us/azure/bastion/connect-native-client-windows)
