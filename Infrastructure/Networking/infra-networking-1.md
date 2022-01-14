# infra-networking-1 - deploy an Azure Virtual Network via ARM

## Description

Contoso requested us to provision an Azure Virtual Network that can be used for multiple solutions. They want to store everything as Infrastructure as Code (IaC) including a BICEP/ARM template that is reusable within the organization. They also requested a manner to keep track on IP space usage within the Virtual Networks, to make sure there is not overlap in IP space. 

## Outcome

  1. Create a Virtual Network with: <br>
    - 2 subnets, one for IaaS workloads (e.g. Virtual Machine) and one for Private Link Endpoints <br>
    - That uses Azure Provided DNS <br>
    - Configured with an Azure Storage West Europe Service Endpoint
  1. Deployed in a separate Resource Group
  1. A BICEP or ARM Template and Parameter file
  1. A release pipeline from where the Virtual Network is deployed
  1. IP Address schema
  
The solution should look like something as this:

![image](https://user-images.githubusercontent.com/25753877/144612702-a0124aeb-8ef0-4a8e-9aed-bf35edd12f86.png)

IP Schema example:

|IP Space|Subnet Mask|CIDR|First usable IP|Last usable IP|VNet Name|Subnet|Purpose|Reservation Date|
|-|-|-|-|-|-|-|-|-|
|192.168.1.0|255.255.255.0|/24|192.168.1.4|192.168.1.254|spoke01-d-vnet|dev01-subnet|IaaS Subnet|03-Dec-2021|
|192.168.2.0|255.255.255.0|/24|192.168.2.4|192.168.2.254|spoke01-d-vnet|ple01-subnet|Private Link Endpoints Subnet|03-Dec-2021|
|192.168.3.0|255.255.255.128|/25|192.168.3.4|192.168.3.127|Free|Free|To be assigned|-|-|
|192.168.3.128|255.255.255.128|/25|192.168.3.132|192.168.3.254|Free|Free|To be assigned|-|-|
|192.168.4.0|255.255.255.192|/26|192.168.4.4|192.168.4.63|Free|Free|To be assigned|-|-|
|192.168.4.64|255.255.255.192|/26|192.168.4.68|192.168.4.127|Free|Free|To be assigned|-|-|
|192.168.4.128|255.255.255.192|/26|192.168.4.132|192.168.4.191|Free|Free|To be assigned|-|-|
|192.168.4.192|255.255.255.192|/26|192.168.4.196|192.168.4.254|Free|Free|To be assigned|-|-|

## References

It is not mandatory to use these references.

  - [Quickstart: Create a virtual network - Resource Manager template](https://docs.microsoft.com/en-us/azure/virtual-network/quick-create-template)
  - [Manage network policies for private endpoints](https://docs.microsoft.com/en-us/azure/private-link/disable-private-endpoint-network-policy)
  - [Virtual Network service endpoints](https://docs.microsoft.com/en-us/azure/virtual-network/virtual-network-service-endpoints-overview)
  - [What address ranges can I use in my VNets?](https://docs.microsoft.com/en-us/azure/virtual-network/virtual-networks-faq#what-address-ranges-can-i-use-in-my-vnets)
