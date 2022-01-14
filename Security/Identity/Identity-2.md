# Identity-2 Securing Identities in the Cloud

## Description

This quest assumes that you already completed the [extend Active Directory to Azure AD](./Identity-1.md) quest.

Now that Contoso extended its identity infrastructure to Azure AD, they realized that their user credentials can be used to log on to Azure AD enabled services from anywhere in the internet. A weak, leaked or stolen password based credential can easily expose their infrastructure. They want to secure their identities, both cloud only accounts and accounts synchronized from their on-premises AD. They want to leverage cloud native solutions for this.



## Outcome

Setup and configure Multi-Factor Authentication (MFA) and Identity Protection (IP) for the synchronized account(s) and for a cloud-only account(s) as well. Securing identities also requires that the user can change their password in a self service way, also configure Self-Service Password Reset (SSPR) for the accounts as well. Make sure that in case of the on-prem synchronized account the SSPR changes the password in the on-premises AD as well. At the end of this quest, you should have MFA configured for at least one cloud only account and one synchronized account. When they attempt to access the Azure Portal they should be be prompted to MFA. Users should be able to reset their passwords.

## Review and discussion
Why would it be necessary to have MFA or other forms of protection of credentials in the cloud?
How or why does it differ from the traditional on-premsise approaches?
What if MFA is nto working? What is a 'break glass account'?
What would be your 'elevator pitch' for a customer on Azure MFA, IP and SSPR? What would be the top 3-5 things that would highlight to a customer executive on the necessity of these?

If you want to talk through or validate your quest after you completed, contact [Matyas Safranka](mailto:matyas@microsoft.com) via email or Teams.

## References

It is not mandantory to use these references.

- [How it works: Azure AD Multi-Factor Authentication](https://docs.microsoft.com/en-us/azure/active-directory/authentication/concept-mfa-howitworks)
- [Plan an Azure Active Directory Multi-Factor Authentication deployment](https://docs.microsoft.com/en-us/azure/active-directory/authentication/howto-mfa-getstarted)
- [What is Identity Protection?](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/overview-identity-protection)
- [Plan an Azure Active Directory self-service password reset deployment](https://docs.microsoft.com/en-us/azure/active-directory/authentication/howto-sspr-deployment)
- [Tutorial: Secure user sign-in events with Azure AD Multi-Factor Authentication](https://docs.microsoft.com/en-us/azure/active-directory/authentication/tutorial-enable-azure-mfa)
- [Tutorial: Configure custom banned passwords for Azure Active Directory password protection](https://docs.microsoft.com/en-us/azure/active-directory/authentication/tutorial-configure-custom-password-protection)
- [Tutorial: Use risk detections for user sign-ins to trigger Azure AD Multi-Factor Authentication or password changes](https://docs.microsoft.com/en-us/azure/active-directory/authentication/tutorial-risk-based-sspr-mfa)
- [Tutorial: Enable users to unlock their account or reset passwords using Azure Active Directory self-service password reset](https://docs.microsoft.com/en-us/azure/active-directory/authentication/tutorial-enable-sspr)
- [Tutorial: Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/en-us/azure/active-directory/authentication/tutorial-enable-sspr-writeback)

[back](./Identity-1.md) <--- * ---> [next](./Identity-3.md)
