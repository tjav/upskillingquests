# infra-networking-2 - design and connect multiple Azure Virtual Networks

## Description

Contoso requested us to provision a second Azure Virtual Network. They require that those 2 network are connected with each other, meaning if you deploy a client in those that they can communicate in a secure manner. 

## Outcome

  - A Hub Virtual Network deployed, consisting out of: <br>
    - 1 subnet for an IaaS workloads (e.g. a Windows Server)
      - Name the VNet `hub01-vnet`, to make it suitable for upcoming quests.
      - Name the subnet `dns01-subnet`, to make it suitable for upcoming quests.
    - 1 subnet for a VPN Virtual Network Gateway
    - That uses Azure Provided DNS
  - How can we connect the Hub to the spoke(s) in an efficient manner?
  - Implement a security to filter traffic between the Virtual Networks/Subnets
  - Working connectivity, preferrable filtered (e.g. only RDP or HTTPS)
  
The solution should look like something as this:

![image](tjav/upskillingquests/Infrastructure/Networking/Network-quest02.jpg)

## Review and discussion

If you want to discuss the outcome, or have a validation of your quest, contact Dwaine Ridderhof. 

## References

It is not mandatory to use these references.

  - [Quickstart: Create a virtual network - Resource Manager template](https://docs.microsoft.com/en-us/azure/virtual-network/quick-create-template)
  - [Cross-network connectivity](https://docs.microsoft.com/en-us/azure/expressroute/cross-network-connectivity?toc=/azure/virtual-network/toc.json#cross-connecting-vnets)
  - [Azure network security groups](https://docs.microsoft.com/en-us/azure/virtual-network/network-security-groups-overview)
  - [Azure Hub-spoke network topology](https://docs.microsoft.com/en-us/azure/architecture/reference-architectures/hybrid-networking/hub-spoke?tabs=cli)
