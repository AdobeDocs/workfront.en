---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Change Your Adobe Workfront Domain
description: As an Adobe Workfront administrator and an authorized Workfront Support contact, you can request help from the Workfront Support team to change your organization's Workfront domain.
author: Becky
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

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Request a domain change

1. Begin creating a support ticket on Experience League.
1. In the **Description** box, include the new new domain you want, as well as the timeframe when you want the new domain to go live.
1. Finish filling out the boxes for the support case, then click **Submit**.

You can also call Workfront Support to get help changing your domain.

## Update the new domain if you are an SSO customer

If your company utilizes SSO, the following steps are required after you have your Workfront domain changed.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

{{step-1-to-setup}}

1. In the left sidebar, click **System** > **Customer Info** and make sure that your domain is updated on the Customer Info page.

1. In the left sidebar, click **System** > **Single Sign-On (SSO)**.

1. Click **Download SAML 2.0 Metadata**.
1. After the file is downloaded, open it and make sure of the following:

   1. **entityID** is pointing to the new domain.
   1. All locations within **`<md:AssertionConsumerService>`** point to the new domain.

1. Provide the downloaded metadata file to your Identity Provider so that they can update it on their end.
1. Make sure the domain is updated for all Workfront integrations used by your organization.
