# Infrastructure

Infra track:

- [basics](Basics/infra-basics-1.md)
  - you can choose to use the [arm](Basics/infra-basics-1.md)/[bicep](Basics/infra-basics-6.md)/[terraform](Basics/infra-basics-10.md) ones. Or do all of them.
  - from [14](Basics/infra-basics-14.md) onwards, you can choose which IaC code you use.
- [networking](Networking/readme.md)
- [advanced](Advanced/infra-advanced-1.md)

```markdown
.
   ├──. Infrastructure
   ├──. Basics
   |  ├── infra-basics-1  # create storageaccount arm (arm)
   |  ├── infra-basics-2  # deploy storageaccount template to storageaccount (arm)
   |  ├── infra-basics-3  # deploy linked template from a storageaccount (arm)
   |  ├── infra-basics-4  # create keyvault to store SAS-token (arm)
   |  ├── infra-basics-5  # deploy using the keyvault SAS-token (arm)
   |  ├── infra-basics-6  # use bicep to deploy full setup  (bicep)
   |  ├── infra-basics-7  # create modules for bicep (bicep)
   |  ├── infra-basics-8  # create a azure devops pipeline to deploy (bicep)
   |  ├── infra-basics-9  # create a github flow to deploy (bicep)
   |  ├── infra-basics-10 # use terraform to deploy (terraform)
   |  ├── infra-basics-11 # use terraform with Azure AD (terraform)
   |  ├── infra-basics-12 # use terraform with modules and variables (terraform)
   |  ├── infra-basics-13 # use terraform in a github flow with statefile (terraform)
   |  ├── infra-basics-14 # create vm template design
   |  ├── infra-basics-15 # implement vm template 
   |  ├── infra-basics-16 # create vm with kv via a github workflow
   |  ├── infra-basics-17 # connect to a private storage account
   |  ├── infra-basics-18 # create an Node.js app with MongoDB (like https://docs.microsoft.com/en-us/azure/app-service/tutorial-nodejs-mongodb-app?pivots=platform-linux)
   |  ├── infra-basics-19 # create a data lake with synapse like https://docs.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-use-sql
   |  ├── infra-basics-20 # create a pwsh script that calls the ms graph
   |  ├── infra-basics-21 # create a function app that executes the calls the script
   |  └── infra-basics-22 # create a durable function
   ├──. Networking
      ├──. Create a Hub-Spoke network
   |     ├── infra-networking-1 # deploy an Azure Virtual Network via ARM/Bicep
   |     ├── infra-networking-2 # use Azure Bastion to remotely access a VM
   |     ├── infra-networking-3 # design and connect multiple Azure Virtual Networks
      ├──. Secure and isolate
   |    ├── infra-networking-4 # filter traffic between Azure Private and Azure Public using a firewall
   |    ├── infra-networking-5 # use a Service Endpoint to restrict access to a Storage Account
   |    ├── infra-networking-6 # use Private Link to restrict access to your Storage Account
      ├──. Hybrid Connectivity
   |    ├── infra-networking-7 # connect a PC via VPN to your Virtual Networks
      ├──. DNS
   |    ├── infra-networking-8 # create your own DNS Forwarder
   |    ├── infra-networking-9 # create an Azure Private DNS Zone and use the forwarder to resolve an A-record
   |    ├── infra-networking-10 # use Private Link to connect to a Storage Account, leveraging your own DNS Forwarder
   |    ├── infra-networking-11 # make your DNS Forwarder highly available using an Azure Load Balancer
   ├──. Monitoring
   |  ├── monitoring-basics-1 # create a workbook with Azure Resource metrics of your Lab environment
   |  ├── monitoring-basics-2 # explore security center
   |  ├── monitoring-networking-3 # use Network Watcher capabilities to troubleshoot
   |  ├── monitoring-networking-4 # use Network Watcher capabilities to troubleshoot
   ├──. Advanced
   |  ├── infra-advanced-1 # create vm with software using ansible
   |  ├── infra-advanced-2 # routing with Virtual WAN (Microhack - https://github.com/mddazure/azure-vwan-microhack)
   |  ├── infra-advanced-3 # Azure Private Link DNS (Microhack - https://github.com/dmauser/azure-privatelink-dns-microhack)
   |  ├── infra-advanced-4
   |  ├── infra-advanced-5
   |  ├── infra-advanced-6
   |  ├── infra-advanced-7
   |  ├── infra-advanced-8
   |  └── infra-advanced-9
```
