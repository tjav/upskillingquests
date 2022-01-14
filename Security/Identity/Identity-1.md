# Identity-1 Hybrid-Identity

## Description

Constoso needs to extend its existing on-premises Active Directory identiy management solution to Azure AD. They leverage Active Directory to manage identities in their on premises worlds. To be able to allow their users to consume cloud services, including Office 365, and Azure based applications they need to syncronize their AD objects to the Azure AD. They know that in the future they will move most of their workloads to the cloud, therefore they want to minimize the dependency on their on-premises infrastructure when extending their Active Directory to the cloud. They want to leverage Microsoft best practices and ise Azure AD Connect (AAD Connect) to achieve this. 



## Outcome

Create Windows Server 2019 VM in your subscription and promote it to a Domain Controller (DC). After the DC was promoted, create a new Organizational Unit (OU) in the domain and under that OU create a test user and a test group. Add the user to the group. Then install Azure AD Connect on the domain controller (even though it is not a recommended practice, it suits the purposes of this quest). Then setup AAD Connect with a configuration that best matches the goals and requirements. Ensure that the test user and group is synchronized to the Azure AD. Check if you can authenticate to the Azure Portal with the user (the authentication must succeed even if the user has no access to resources in Azure).

As a bonus or extra add-on to this challenge: customize the Azure AD logon experiences for the users for your own branding.

![AAD Connect](../../.images/identity/aadconnect.png)

## Review and discussion
What type of integration did you choose for the AAD Connect? Why did you choose that method?
What pros and cons can you think of regarding the different methods?
What what would be the questions or requirements that you would investigate or discuss with your customer regarding extending their AD to AAD?

If you want to talk through or validate your quest after you completed, contact [Matyas Safranka](mailto:matyas@microsoft.com) via email or Teams.

## References

It is not mandatory to use these references.

- [Install Active Directory Domain Services (Level 100)](https://docs.microsoft.com/en-us/windows-server/identity/ad-ds/deploy/install-active-directory-domain-services--level-100-)
- [What is Azure AD Connect?](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/whatis-azure-ad-connect)
- [Microsoft Azure Active Directory Connect](https://www.microsoft.com/en-us/download/details.aspx?id=47594)
- [Azure AD Connect and Azure AD Connect Health installation roadmap](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-install-roadmap)
- [Tutorial: Integrate a single AD forest using password hash sync (PHS)](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/tutorial-password-hash-sync)
- [Tutorial: Integrate a single AD forest using pass-through authentication (PTA)](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/tutorial-passthrough-authentication)
- [Tutorial: Federate a single AD forest environment to the cloud](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/tutorial-federation)
- [https://docs.microsoft.com/en-us/azure/active-directory/hybrid/tutorial-phs-backup](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/tutorial-phs-backup)
- [Add branding to your organization's Azure Active Directory sign-in page](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/customize-branding)
- [Add your custom domain name using the Azure Active Directory portal](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/add-custom-domain)

[back](../Security.md) <--- * ---> [next](./Identity-2.md)
