# demoTenant 


## Azure Environments:

  In MS, we can have 2 types of demo environments : 
     1. An internal subscription in MS Tenant (Always under the MS Tenant so you're not the owner of anything, only deployment is possible.)
     2. A demo tenant for own demo environment with full rights, through making a request in "CDX" portal and MSDN subscription in "Visual Studio Subscription" portal.

Follow the below steps to get a demo tenant and MSDN subscription for demo environment:

## Get Demo Tenant:

1. Visit this link to get a Demo Tenant: https://cdx.transform.microsoft.com/
2. Go to "My Environments" and create a tenant (Quick Tenant/Custom Tenant) and wait for 1-2 days to get the tenant ready.


## Get MSDN subscription:

1. To Build an infrastructure inside the demo tenant, we need to pay and hence we need a subscription.
2. To get a subscription visit: https://my.visualstudio.com/subscriptions 
3. Click on "Benefits" and activate Azure monthly credit (150§). Activate the account using personal MSA, not the corporate credentials (@microsoft.com). It might take few hours to get the subscription in place.

## Setting up the Environment using the new demo tenant and MSDN subscription:

1. In CDX portal you will find your new tenant in "My Environments". There will be an admin account and some demo accounts to login to your demo tenant environment in Azure. 
2. Login to your demo environment.
3. Assign the following roles to yourself/user : "Global admin" and "User admin" to have the permission (From AAD-->User-->Assigned Roles--> Add Assignments) to  manage everything in your AAD/demo tenant.
4. There is no subscription in this tenant. To add a subscription manually you need to invite a guest user account. In this case, invite the user account (email id) that has been used to create the MSDN subscription.
5. Switch to the account where you have the MSDN subscription. The subscription is not in any domain or tenant yet. It shows up as default directory but it's not managed anywhere yet. Therefore, we need the proper rights on the subscription to change the tenant from default directory to the demo tenant.
6. Accept the invitation from the demo tenant.	
7. Assign the following roles to yourself/user: "Owner" and "User Access Administrator"  on the subscription (From Subscriptions-->IAM-->Add role assignments) to have the permission to grants full access to manage all resources, including the ability to assign roles in Azure RBAC.
8. Click on the subscription and change the directory. Select the new directory and select the demo tenant/directory from the drop down list. It takes almost 1 hour to map. 
9. Switch back to the demo tenant account and look for the subscription that has been moved here.
10. Again Assign the following roles to yourself/user: "Owner" and "User Access Administrator" on the subscription (From Subscriptions-->IAM-->Add role assignments) to have the permission to grants full access to manage all resources, including the ability to assign roles in Azure RBAC. Please note, when we move a subscription, it loses all the previously assigned roles.


### Create Management Group in Demo tenant:

1. Go to the Management group to manage the hierarchy and apply rules and policies.
2. Before you create a management group, check if you have the "Owner" right (From Subscriptions-->IAM-->Add role assignments) to the management group.
3. Then go to AAD--> Properties--> Access management for azure resources--> toggle to "Yes" so that you can manage access to all Azure subscriptions and management groups in this tenant.
4. Create a new Management group under the root MgMt group (Ex: DemoOrg) by your organization's name.
5. Create another management group "Platform" below the DemoOrg MgMt group.
6. Then  click on "Add subscription" in Management Groups. It will give you an option to add the existing subscriptions to the management groups. Add the MSDN subscription.
7. The subscription will be visible under the root management group. It needs to be moved to the "Platform" MgMt group so that the applied policies on root MgMt can flow to the bottom (subscription). Click on the "three dots" beside the subscription to move it from one MgMt to another MgMt.


### Create Service Connection for ADO:

An app registration needs to be created in Azure to make a connection between Azure and ADO.

1. Go to AAD-->App Registration--> Give it a name without spaces--> Register.
2. Then give proper permission to the App registration. Hence, go to Azure Portal-->MgMt group--> Select the 2nd level MgMt group(DemoOrg)-->IAM-->Add Role Assignment--> Select "Owner" and assign it to the App Registration.
3. Go to the App registration --> API Permissions--> Add a permission--> "User.Read". Also grant "admin consent" for default directory.
4. Go to ADO.
5. Create a new project.
6. Go to project settings--> Service Connections--> Create Service Connection--> New Service Connection--> Azure Resource Manager--> Service Principal (Manual).
7. Select Management Group ID--> Put MgMt ID and Name (Find in Portal MgMt group overview).
8. In Authentication section, put the "Service Principal Id" (Find it in portal: Go to the App registration--Certificates & Secrets--Add a New Client Secret-->Add--> copy the value from the newly created Secret and past it.)
9. Put the tenant id (Find it in portal through the overview section of the App Registration) and click on "Verify".
10. In "Details" section put the Service Connection Name and then "Verify and Save".

Try to create a pipeline in ADO and push some codes to check if you can deploy a new resource in Azure through the ADO pipeline.