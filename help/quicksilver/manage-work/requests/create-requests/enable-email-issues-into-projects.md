---
product-area: requests
navigation-topic: create-requests
title: Enable Users to Email an Issue into a Request Queue Project
description: You can configure a project to allow users to add issues to the project via email.
author: Becky
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
---
# Enable users to email an issue into a Request Queue project

<!-- Audited: 4/2025 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

You can configure a project to allow users to add issues to the project via email. You can only allow issues to be emailed into a project if the project is designated as a Request Queue. For more information about creating a Request Queue project, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Contributor or higher</p>
   <p>Request or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Issues</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

The following conditions are required to configure a project to allow users to add issues to the project via email:

* Users who are emailing issues to this account must be active users with a license for Workfront.  
* Users who are emailing issues to this account must have Add Issue permissions on the project. 
* External Users cannot email issues to a request queue because they do not have access to create issues.
* Only emails coming from an email address associated with an active Workfront user are allowed to send issues to the project. Emails that are forwarded to an active Workfront user email from an email not associated with a Workfront account are unable to create issues under the project, as the original sender's email address is required to be associated with an active Workfront account. 
* The project is set up as a Request Queue. 
* The email account associated with the project is not linked to a Workfront user account.

## Configure the project in Workfront

>[!NOTE]
>
>Keep the following in mind when enabling email queue settings:
>
>* Workfront allows one unique email per request queue across all clusters. If you choose to disable your request queue, you'll retain the email address you created as long as it is still in the Intake Email Address box. If you choose to discontinue use of the intake email, you must delete it from the Intake Email Field so it can be available for future use.
>
>* If the request queue has multiple queue topics or topic groups, Workfront will randomly select the queue topic that the emailed requests will go to, making emailed requests hard to manage.
>We recommend that the project that you set up to receive requests through emails should not have more than one queue topic. If the submitted requests are intended for different resources or projects you should route or move them manually, after they have been submitted. 

1. Go to the project that you want to enable to receive issues via email.
1. Click **Queue Details** in the left panel.
1. In the **Queue Type** area, select **Publish as Help Request Queue**.

1. Scroll down to the **Email Queue Settings** area, then select **Enable Request intake via email**.

1. Enter the beginning of the email address in the **Intake Email Address** box.

   You must create a unique email address. We recommend using your company name as part of your intake email address.

   >[!CAUTION]
   >
   >* This email address cannot be recovered from the recycle bin if the project containing the request queue is deleted.
   >
   >* Because this email address must be unique, it may not be available in the future if deleted.
   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. (Optional) Select the **Forward all issues that fail to submit via email**, then enter a forwarding email address in the box below.

   This email address receives information about emails that failed to submit to the project.

1. Click **Save**. Now, when users with an active Workfront account send an email to this email address, an issue is created in the Workfront project.

   >[!NOTE]
   >
   >Users must have access to create issues in the project in order to submit via email. You can grant this access in the Sharing dialog box under Advanced Settings.  
   >
   >External Users cannot email issues to a request queue because they do not have access to create issues.

## Receive the issue in Workfront

When a Workfront user sends an email to Workfront, the following things happen:

* The Subject line of the email becomes the Issue Name.
* The body of the email becomes the Description of the Issue.
* If there are any documents attached to the email, those documents are attached to the issue in Workfront.

   >[!NOTE]
   >
   > MSG files are not supported and won't be attached to the issue in Workfront.
   
* The user who is sending the email becomes the Primary Contact of the new issue in Workfront.
* The body text of the email cannot exceed 4,000 characters.
* Email attachments cannot exceed 7 MB total.
