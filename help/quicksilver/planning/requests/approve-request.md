---
title: Approve a Request in Adobe Workfront Planning
description: When a user submits a request to a request form associated with an approval in Adobe Workfront Planning, approvers receive a notification and an email about the pending approval. They must approve the request before Workfront Planning creates an object.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: aca9b313-3420-43f6-8f6c-dd74888bd120
---
# Approve a request in Adobe Workfront Planning

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

When a user submits a request to a request form associated with an approval in Adobe Workfront Planning, approvers receive a notification and an email about the pending approval. They must approve the request before Workfront Planning creates an object. 

This article describes how a workspace manager can approve a request submitted for Workfront Planning to create a record. 

We recommend that you also see the following articles:

* [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md)
* [Add an approval to a request form](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## Considerations about approving requests and request statuses

Submitted requests display in the Planning tab of the Submitted section in the Requests area of Workfront  with one of the following request statuses: 

* **Pending review**: This status is shown when none of the approvers has opened the request object.
* **In review**: The **Pending review** status changes to **In review** when at least one approver opens the request object. The status of the request remains **In review** until all approvers have approved the request.
* **Approved**: When an approver approves the request object, their individual status becomes **Approved**, but the overall request object status remains **In review** until all approvers have made their decisions. When all approvers approve a request, the request status becomes **Approved**.
* **Completed**: If all approvers approve the request object, its status changes to **Completed**, or if the request did not need an approval.
* **Rejected**: If any approver rejects the request object, the status becomes **Rejected**. No record is created and a new request must be submitted to create the record. 

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Products</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any of the following Workfront plans:</p>
<ul><li>Select</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning is not available for legacy Workfront plans</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td>
   <td>
<p>Any </p>  
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning.</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td>
   <ul>
   <li><p>Manage permissions to a workspace</p></li>
    <li><p>System Administrators can manage workspaces they did not create. </p></li>
    </ul>
   <p>For information about sharing permissions for Workfront Planning objects, see  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Overview of sharing permissions in Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p>  
</td>
  </tr>
 </tbody>
</table>

*For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).  

+++

## Approve a request to create a record

After users add requests to a record type request form that is associated with an approval, the request is sent to the approvers. 

Approvers receive the following notifications about a request pending their approval: 

* An in-app notification
* An email notification

>[!NOTE]
>
>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience for users to be able to receive email and in-app notifications.

To approve a request:

1. Do one of the following: 

    * If you have access to Workfront Planning and can view at least one workspace, click **Main Menu** ![](assets/dots-menu.png) in the upper-right corner of the screen, or the **Main Menu** ![](assets/lines-menu.png) in the upper-left corner, if available, then click **Requests** > **Submitted** > **Planning**, and click the request with the status of **Pending review** or **In review**.

      >[!TIP]
      >
      >If you don't have access to Workfront Planning, or if you don't have access to view any workspaces, you can only access a request to approve it using your email or in-app notifications. 
   
    * Click the **Notifications** area icon ![](assets/notifications-area-icon-unified-shell.png) in the upper-right corner of the screen and click the notification about a request pending your approval to open the request.
    * Go to the email notification in your email that notifies you about a request pending your approval, then click **Open request** to open the request. <!--add the name of the button here, from the email-->

    The request page opens in read-only mode.

    ![](assets/read-only-reqeust-page-in-review-status.png) 

1. (Optional) Click the **Approvals** icon ![](assets/approvals-icon.png) in the upper-right corner of the request to view the approvers.
1. Click **Review and approve**, then choose one of the following: <!--did they fix the button and removed the &??-->

    * **Approve**: This approves the request. A record is immediately created for the record type associated with the request form after all approvers approve the request.
    * **Reject**: This rejects the request, even when you are the only approver that rejects it. No record is created for the record type associated with the request form. 

    The user who submitted the request receives an email and in an-app notifications when their request is approved or rejected. 

    The status of the request changes to the following, depending on the approval decision: 
    
    * **Completed**: The request is approved.
    * **Rejected**: The request is rejected. 

    The request remains in the Planning tab of the Submitted section in the Requests area of Workfront.
