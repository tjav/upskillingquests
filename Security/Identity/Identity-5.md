# Identity-5 B2B

## Description

Constoso business and IT works very much with external parties and consultants. Traditionally Contoso IT was creating user accounts and distributing passwords to the external users. Often, depending on the system the external party needed to have access Contoso distributed Contoso owend laptops to the external parties. In other scenarios they provided a VPN and a Citrix virtual desktop environment for the externals to access Contoso systems. This extra devices and virtual desktop environments mean constantly growing costs for the IT department, as Contoso leverage more and more external contracted workforce. The creation, management and permission granting for externals is a burden for the central IT, the IT experts often struggle to make a decision whether they should grant access to an external on a given resource or not, this information is often with the business team. This requires extra coordination that takes lots of time from COntoso IdM administrators. The extra IT costs of externals are also visible in support costs as external vendors who access Contoso systems infrequently often require password and MFA authenticator application resets from IT support. This was one of the main reason, why Contoso earlier was eager to implement self-service password reset capability.



## Outcome

As more and more of the IT applications and services are moving to the cloud, IT management now want to further decouple dependency on on-premises services especially for externals. IT management would prefer to rethink the approach how externals are managed: Central IT should be an enable and not a gate keeper for external accounts. Central would like to delegate the management of externals to as much as possible to the business application owners. They should be able to invite externals and manage external's access on Contoso systems. Contoso IT team want to stay in control on users of what organizations can be invited to the Contoso environment. For the time being Contoso IT approved only Microsoft as an external collaboration party, with the `@microsoft.com` email domain. Contoso IT also want to make sure that only strong authentication is accepted for external entities.


## Review and discussion
If you want to talk through or validate your quest after you completed, contact [Matyas Safranka](mailto:matyas@microsoft.com) via email or Teams.

## References

It is not mandantory to use these references.

- [What is guest user access in Azure Active Directory B2B?](https://docs.microsoft.com/en-us/azure/active-directory/external-identities/what-is-b2b)
- [Quickstart: Add guest users to your directory in the Azure portal](https://docs.microsoft.com/en-us/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)
- [Azure Active Directory B2B best practices](https://docs.microsoft.com/en-us/azure/active-directory/external-identities/b2b-fundamentals)
- [Microsoft 365 external sharing and Azure Active Directory (Azure AD) B2B collaboration](https://docs.microsoft.com/en-us/azure/active-directory/external-identities/o365-external-user)
- [Tutorial: Bulk invite Azure AD B2B collaboration users](https://docs.microsoft.com/en-us/azure/active-directory/external-identities/tutorial-bulk-invite)
- [Tutorial: Enforce multi-factor authentication for B2B guest users](https://docs.microsoft.com/en-us/azure/active-directory/external-identities/b2b-tutorial-require-mfa)
- [Enable B2B external collaboration and manage who can invite guests](https://docs.microsoft.com/en-us/azure/active-directory/external-identities/delegate-invitations)
= [Allow or block invitations to B2B users from specific organizations](https://docs.microsoft.com/en-us/azure/active-directory/external-identities/allow-deny-list)
- [How users in your organization can invite guest users to an app](https://docs.microsoft.com/en-us/azure/active-directory/external-identities/add-users-information-worker)
- [Conditional Access for B2B collaboration users](https://docs.microsoft.com/en-us/azure/active-directory/external-identities/conditional-access)
- [Ideneity provides: Azure Active Directory (Azure AD) identity provider for External Identities](https://docs.microsoft.com/en-us/azure/active-directory/external-identities/azure-ad-account)
- [Ideneity provides: Microsoft account (MSA) identity provider for External Identities](https://docs.microsoft.com/en-us/azure/active-directory/external-identities/microsoft-account)
- [Ideneity provides: Add Google as an identity provider for B2B guest users](https://docs.microsoft.com/en-us/azure/active-directory/external-identities/google-federation)
- [Ideneity provides: Add Facebook as an identity provider for External Identities](https://docs.microsoft.com/en-us/azure/active-directory/external-identities/facebook-federation)
- [Email one-time passcode authentication](https://docs.microsoft.com/en-us/azure/active-directory/external-identities/one-time-passcode)

[back](./Identity-3.md) <--- * ---> [back to security](../Security.md)

