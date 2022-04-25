# infra-aks-1

## Description

In the past, Contoso has developed a big monolithic business application. Over the years they are not so happy anymore. Customers are complaining about the slowness and are running away to other suppliers, because the application hasn't been updated with new features for ages.
Contoso asked the help of a Microsoft consultant because they are at their wit's end. Your task is to help them out.

First you learn what is wrong with the monolith:

* They need to redeploy the whole application even for a small change
* As the size of the application increases, its start-up and deployment time also increases
* For any new developer joining the project, it is very difficult to understand the logic of large Monolithic application even if their responsibility is related to a single functionality
* Even if a single part of the application is facing a large load/traffic, they need to deploy the instances of the whole application in multiple servers. It is very inefficient and takes up more resources unnecessarily. Hence, horizontal scaling is not feasible in monolithic applications.
* It is very difficult to adopt any new technology which is well suited for a particular functionality as it affects the whole application, both in terms of time and cost.
* It is not very reliable as a single bug in any module can bring down the whole monolithic application.

You point Contoso to the advantages of Microservices:

* Easy to manage because they are smaller in size
* If there’s any update in one of the microservices, then they need to redeploy only that microservice
* Easy to onboard new developers
* Easier to scale out because only the particular microservice that generates a large load needs to scale
* If a particular microservices goes down for a bug then it does not affect other microservices.

After hearing this, Contoso expresses their intent that they indeed want to go the Microservices route. 
But on which platform should these microservices be deployed? These are Contoso's requirements:

* Contoso has partnered with Microsoft and has a preference for the Azure cloud.
* Contoso however wants the platform to be vendor agnostic.
* The application should also be able to run on-premises in the future (but not now)
* The platform should support horizontal scaling
* The use of open source is important for Contoso
* Developers must be enabled to test locally

So it is up to you to advise Contoso which solution could be a fit for the platform.
You advise to use (Kubernetes([https://docs.microsoft.com/en-us/azure/architecture/microservices/]). 

Contoso is very new to Kubernetes, so your first task is to build a small POC.

## Outcome

* Describe why Kubernetes would be a great platform fit to host their Microservices (or is there even a better alternative)?
* Describe how they can package the microservices to run on Kubernetes (hint: something with a Dockerfile)
* Describe some disadvantages of Kubernetes
* Use the Azure CLI to build a quick AKS cluster with these parameters:
    - resource group: contoso-lob-dev-we-rg
    - name: contoso-lob-dev-we-aks
    - node-count 1
    - location: westeurope
    (feel free to use your own resource names though)
* Once ready, check what is deployed in the Azure portal. Notice the weird resource group that starts with 'MC_' and what is in there.
* Install kubectl
* Get access to your cluster with `az aks get-credentials -n contoso-lob-dev-we-aks -g contoso-lob-dev-we-rg`
* Show the pods of all namespaces `kubectl get pods --all-namespaces`
* Deploy an nginx container to the default namespace using nginx-deployment.yaml (see cheatsheet in the references)
* Scale the nginx deployment to 3 replicas and show that there are 3 pods running
* Show it off to the customer
* Remove the cluster

The outcome is:
* The customer is aware of Kubernetes being a solution to host their application if they are going to refactor the monolith into microservices
* You were able to show them how quickly a Kubernetes cluster can be spun up in Azure and how quickly to deploy the Nginx webserver
* You were able to show them how quickly this webserver can be scaled
* Customer is sold to AKS. Next time we will take this a step further and deploy AKS with Terraform and Github Actions. 

## References

It is not mandantory to use these references.
- [create aks cluster](https://docs.microsoft.com/en-us/azure/aks/kubernetes-walkthrough#create-aks-cluster)
- [kubectl cheatsheet deploy](https://kubernetes.io/docs/reference/kubectl/cheatsheet/#creating-objects)
- [kubectl cheatsheat scale](https://kubernetes.io/docs/reference/kubectl/cheatsheet/#scaling-resources)
- [Azure Resource Manager documentation](https://docs.microsoft.com/en-us/azure/azure-resource-manager/)
- [Azure Architecture Center](https://docs.microsoft.com/en-us/azure/architecture/)
- [VS Code documentation](https://code.visualstudio.com/Docs)
- [Azure CLI](https://docs.microsoft.com/en-us/cli/azure/reference-index?view=azure-cli-latest)
- [WSL](https://docs.microsoft.com/en-us/windows/wsl/about)
- [Azure PowerShell](https://docs.microsoft.com/en-us/powershell/azure/?view=azps-6.6.0)

[back](../Infrastructure.md.md) <--- [TO OVERVIEW](../Infrastructure.md) ---> [next](./infra-basics-2.md)