---
title: Add an Approval to a Request Form in Adobe Workfront Planning
description: You can add an approval process to an Adobe Workfront Planning request form, to initiate an approval for every submitted request, before it creates a record.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
---
# Add an approval to a request form in Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

You can add an approval process to an Adobe Workfront Planning request form, to initiate an approval for every submitted request, before it creates a record. 

This article describes how a workspace manager can add an approval to a request form associated with a record type. 

For information about creating a request form in Workfront Planning, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

For information about submitting a request to a record type to create a record, see [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md). 

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront packages</p></td> 
   <td> 
<ul><li><p>Any Workfront package</p></li>
And
<li><p>Any Planning package</p></li></ul>
Or
<ul><li><p>Any Workflow package</p></li>
And
<li><p>Any Planning package</p></li></ul>
   </td> </tr>

  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and  record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table> 

For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerations about adding approvals to a request form

* You can add one or multiple approvers to a request form. You can add only users as approvers. 
* You can display approval information on a record created by submitting a request form in the Approved by and Approved date fields. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).
* When you add multiple approvers to a request form, all approvers must accept the request before a record is created in Workfront Planning. 
* If all approvers approve the request, a record is created for the record type associated with the request form. 
* If at least one approver rejects the request, and all others approve it, a request is created for the Requests area in Workfront, but no record is created for the record type associated with the request form. 
* Adding approvals to a request form is optional. Workfront Planning immediately creates a record when a request is submitted, if the request form is not associated with an approval. 

## Add an approval to a request form

1. Start creating a request form for a record type, as described in [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Click **Configuration**.

    The **Configuration** area displays.

    ![Configuration tab](assets/configuration-tab.png)
1. In the **Approvers** field, click the drop-down icon and select one or several users or teams in the list

    Or

    Start typing the name of a user or team that you want to set as an approver, then select it when it displays in the list. 

    <!--most of the Note below is duplicated in the Create a request form article-->

      >[!NOTE]
      >
      >
      >* You can add one or several approvers to a request form.
      >
      >* If you add more than one approver, all approvers must approve the request before Workfront Planning creates a record.
      >
      >* If at least one approver rejects the request, the request is rejected and the record is not created. The request remains in the Planning tab of the Submitted section in the Requests area of Workfront.
      >
      >* All approvers must make a decision before a request is either approved or rejected.
      >
      >* If a team is set as an approver, only one decision is required from the team.


1. (Optional) Click **Publish** if you have never shared the request form before

    Or

    Click **Share** to share the form, then **Copy link**. 
1. (Optional) After a user uses the link you share and submits a request, Workfront Planning sends an approval in-app notification and an email to the approvers. 

   >[!NOTE]
   >
   >   Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience for users to be able to receive email and in-app notifications.


    For information about approving requests, see [Approve a request](/help/quicksilver/planning/requests/approve-request.md).
