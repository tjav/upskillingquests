# Identity-1 Hybrid-Identity

## Description

Constoso needs to extend its existing on-premises Active Directory identiy management solution to Azure AD. They leverage Active Directory to manage identities in their on premises worlds. To be able to allow their users to consume cloud services, including Office 365, and Azure based applications they need to syncronize their AD objects to the Azure AD. They know that in the future they will move most of their workloads to the cloud, therefore they want to minimize the dependency on their on-premises infrastructure when extending their Active Directory to the cloud. They want to leverage Microsoft best practices and ise Azure AD Connect (AAD Connect) to achieve this. 



## Outcome

Create Windows Server 2019 VM in your subscription and promote it to a Domain Controller (DC). After the DC was promoted, creat a new Organizational Unit (OU) in the domain and under that OU create a test user and a testgroup. Add the user to the group. Then install Azure AD Connect on the domain controller (eventhough it is not a recommended practce, it suits the purposes of this quest). Then setup AAD Connect with a configuration that best matches the goals and requirements. Ensure that the test user and group is synchronized to the Azure AD. Check if you can authenticate to the Azure Portal with the user (the authenticatin must sucseed even if the user has no access to resources in Azure).

![AAD Connect](../../.images/identity/aadconnect.png)

## References

It is not mandantory to use these references.

- [Install Active Directory Domain Services (Level 100)](https://docs.microsoft.com/en-us/windows-server/identity/ad-ds/deploy/install-active-directory-domain-services--level-100-)
- [What is Azure AD Connect?](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/whatis-azure-ad-connect)

[back](../Security.md) <--- * ---> [next](./Identity-2.md)
