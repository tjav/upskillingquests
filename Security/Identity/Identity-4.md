# Identity-4 Priviledged Identity Management

## Description

This quest assumes that you already completed the quest to [conditional access](./Identity-3.md)

In the day to day life of the Contoso administrators they find it time consuming that they are prompted for MFA prompts when they need to access environments in Azure. Most often their activity includes just to take a look on an item to read or check configurations or set values, but they do not need to change anything. The Security department has no problem of allowing a read only access to the Azure administrators, but any change or modification must be validated with an MFA. When investigating current security and operationl incidents the Contoso team finds that it would be ideal if admins would have to provide a justification (e.g.: a service desk ticket number and a description) when they do changes in the Azure environment. The opertaional team would also like to introduce a two-eye approach for changes on core parts of the infrastructure such as the central hub network.

## Outcome

Investgiate options that would allow to fulfill the requirements:
- Getting acces to the central hub RG in your subscription would need an approval from another administrator
- Getting modify rights (Owner or Contributor ) would require an MFA
- Global administrator role would also require MFA
- The high priviledged rights can not be active for more than 2 hours
- Provide access reviews to enable periodically check 

## Review and discussion
How would you articulate the difference between Conditional access and PIM?
How do you see Conditional access and PIM work together? Are they mutually exclusive? Is it enough to have only one? Should we recommend both? Why?
What scenarios do you consider relevant for PIM?
What would be your elevator pitch on PIM? What would be the 2-3 sentences why and when PIM is needed?

If you want to talk through or validate your quest after you completed, contact [Matyas Safranka](mailto:matyas@microsoft.com) via email or Teams.

## References

It is not mandatory to use these references.

- [What is Azure AD Privileged Identity Management?](https://docs.microsoft.com/en-us/azure/active-directory/privileged-identity-management/pim-configure)
- [Start using PIM](https://docs.microsoft.com/en-us/azure/active-directory/privileged-identity-management/pim-getting-started)
- [Plan a Privileged Identity Management deployment](https://docs.microsoft.com/en-us/azure/active-directory/privileged-identity-management/pim-deployment-plan)
- [Multifactor authentication and Privileged Identity Management](https://docs.microsoft.com/en-us/azure/active-directory/privileged-identity-management/pim-how-to-require-mfa)
- [Create an access review of Azure resource and Azure AD roles in PIM](https://docs.microsoft.com/en-us/azure/active-directory/privileged-identity-management/pim-create-azure-ad-roles-and-resource-roles-review)
- [Elevate access to manage all Azure subscriptions and management groups](https://docs.microsoft.com/en-us/azure/role-based-access-control/elevate-access-global-admin?toc=/azure/active-directory/privileged-identity-management/toc.json)



[back](./Identity-3.md) <--- * ---> [next](./Identity-5.md)
