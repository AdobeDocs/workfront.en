---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Change your Adobe Workfront domain
description: As an Adobe Workfront administrator and an authorized Workfront Support contact, you can request help from the Workfront Support team to change your organization's Workfront domain.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
---
# Change your Adobe Workfront domain

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, it is not possible to change your Workfront domain.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

As an Adobe Workfront administrator and an authorized Workfront Support contact, you can request help from the Workfront Support team to change your organization's Workfront domain.

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Request a domain change

1. Click the **Support** tab on the Workfront One page, then start creating a support case.
1. In the **Description** box, include the new new domain you want, as well as the timeframe when you want the new domain to go live.
1. Finish filling out the boxes for the support case, then click **Submit**.

You can also call Workfront Support to get help changing your domain.

## Update the new domain if you are an SSO customer

If your company utilizes SSO, the following steps are required after you have your Workfront domain changed.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. In the left sidebar, click **System** > **Customer Info** and make sure that your domain is updated on the Customer Info page.

1. In the left sidebar, click **System** > **Single Sign-On (SSO)**.

1. Click **Download SAML 2.0 Metadata**.
1. After the file is downloaded, open it and make sure of the following:

   1. **entityID** is pointing to the new domain.
   1. All locations within **`<md:AssertionConsumerService>`** point to the new domain.

1. Provide the downloaded metadata file to your Identity Provider so that they can update it on their end.
1. Make sure the domain is updated for all Workfront integrations used by your organization.
