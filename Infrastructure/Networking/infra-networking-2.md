# infra-networking-2 - design and connect 2 Azure Virtual Networks to each other using automation

## Description

Contoso requested us to provision a second Azure Virtual Network. They require that those 2 network are connected with each other, meaning if you deploy a client in those that they can communicate in a secure manner. 

## Outcome

  - A second Virtual Network deployed, consisting out of: <br>
    - 1 subnet for an IaaS workloads (e.g. Virtual Machine)
      - Name the VNet `hub01-vnet`, to make it suitable for upcoming quests.
      - Name the subnet `dns01-subnet`, to make it suitable for upcoming quests.
    - That uses Azure Provided DNS
  - How can we connect the 2 Virtual Networks in an efficient manner?
  - Implement a security to filter traffic between the Virtual Networks/Subnets
  - Working connectivity, preferrable filtered (e.g. only RDP or HTTPS)
  
The solution should look like something as this:

![image](https://user-images.githubusercontent.com/25753877/149518922-4137a642-6d09-4b5e-a8e6-9a6e882cd59f.png)

## Review and discussion

If you want to discuss the outcome, or have a validation of your quest, contact Dwaine Ridderhof. 

## References

It is not mandatory to use these references.

  - [Quickstart: Create a virtual network - Resource Manager template](https://docs.microsoft.com/en-us/azure/virtual-network/quick-create-template)
  - [Cross-network connectivity](https://docs.microsoft.com/en-us/azure/expressroute/cross-network-connectivity?toc=/azure/virtual-network/toc.json#cross-connecting-vnets)
  - [Azure network security groups](https://docs.microsoft.com/en-us/azure/virtual-network/network-security-groups-overview)
