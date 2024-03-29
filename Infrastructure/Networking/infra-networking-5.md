# infra-networking-5 - use a Service Endpoint to restrict access to a Storage Account

## Description

End-user reported an issue while accessing their Storage Account that had a PaaS firewall enabled, when both services (Azure Firewall and Storage Account) are deployed in the same region. Microsoft Support requested the enablement of a Virtual Network Service Endpoint on the Azure Firewall to fix this issue. Can you help them?

## Outcome

  - Enable a Storage Account Service Endpoint on the firewall subnets
  - Describe the impact of using a Service Endpoint, what is the difference?
  - Advice the end-user on their PaaS firewall settings, how can they enable and restrict connectivity?
    
The solution should look like something as this:

![image](https://user-images.githubusercontent.com/25753877/150859155-2d282796-5b0d-4a8f-8000-aa2a30db3ea2.png)

## Review and discussion

If you want to discuss the outcome, or have a validation of your quest, contact Dwaine Ridderhof. 

## References

It is not mandatory to use these references.

  - [Virtual Network service endpoints](https://docs.microsoft.com/en-us/azure/virtual-network/virtual-network-service-endpoints-overview)
  - [Virtual Network traffic routing](https://docs.microsoft.com/en-us/azure/virtual-network/virtual-networks-udr-overview)

[back](./infra-networking-4.md) <--- [TO OVERVIEW](../Infrastructure.md) ---> [next](../Infrastructure.md)
