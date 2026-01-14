---
title: Submit Adobe Workfront Planning requests
description: After someone shares a link to a request form with you from a record type page in Adobe Workfront Planning, you can add a request to create records for the record type associated with the request form.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
---
# Submit Adobe Workfront Planning requests to create records

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

After a workspace manager builds a request form for a record type in Adobe Workfront Planning, you can use the form to submit requests that will create records for the record type associated with the form. 

You can submit a Workfront Planning request from the following areas: 

* From the Requests area of Workfront. 
* From a direct link to the request form that was shared. 
* From the record type page, when you add or request a new record. For information, see [Create records](/help/quicksilver/planning/records/create-records.md). 

This article describes how you can submit a request to add new records to a record type from the Requests area of Workfront, or from a shared link.


Workfront users and external users can submit requests to Planning record types and create records. <!--double check on the external users-->

For information about how a workspace manager can create a request form and associate it with a record type, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

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
<p>Any Workfront package and any Planning package</p>
Or
<p>Any Workflow package and any Planning package</p>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account representative.</p>
   </td> </tr>

  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Any</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>View or higher permissions to a workspace and record type, if you are a Workfront user</p>  </td> 
  </tr>  
</tbody> 
</table> 

For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisites

The following must be in place before you can submit a request to a Workfront Planning request form: 

* The following must exist in Workfront Planning:

   * A workspace
   * A record type
   * A request form associated with a record type. 
   
      For information, see [Create a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
   
* The request form must be shared in a way you can access it. The following scenarios exist: 

   * Internally, the form must be shared with users who have View or higher permissions to the workspace. 

      Workfront users can either access the form from a link or find the request form in the Requests area of Workfront. 

   * If you don't have a Workfront account, a link to the form has been shared with external people. 
   
      Workfront users can also access a link shared with external people. 

* The link to the form must not be expired.

## Considerations about submitting requests to Workfront Planning

* You cannot edit a request in Workfront after you submit it.
* Each submitted request creates a record for the record type associated with the form you use, if the form is not associated with an approval, or if the approval has been granted by all approvers.
* Records created by submitting request forms cannot be differentiated from records added through any other method in Workfront Planning. 

   For information, see [Create records](/help/quicksilver/planning/records/create-records.md). 
* Submitted requests display in the Requests area of Workfront.
* Submitted Planning requests are visible only in the new requesting experience. You cannot see Planning requests in the legacy request experience.
* There are limitations in how certain field types display in a request form, or the request details page after a form is submitted. 

   For information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Submit a request to Workfront Planning in the Requests area of Workfront

{{step1-to-requests}}

1. Enable the **Switch to a new experience** setting, in the upper-right corner of he screen. 
   Enabling this setting makes the Workfront Planning request forms available in the **Requests** area of Workfront.

   >[!TIP]
   >
   >This setting is available only when the following are in place:
   >
   >* Your company has purchased a Workfront Planning package. 
   >* Your Workfront instance is onboarded to the Adobe Unified Experience. 
   >* You have access to view at least one workspace. 
   >

1. Click into the **What request do you want to submit** bar to open a list of request forms. 
1. Select a request form from the list, or begin typing the request form name, then select it when it appears in the list.

   A window opens with the request form name at the top.
1. Update the fields available in the request form. Fields with a red asterisk are required. 
1. Click **Submit**.
    
   The request form closes and you return to the **Requests** area. 

   Your form is submitted and the following things occur:

   * If the request form was not associated with an approval, the request is added to the Requests list in the Workfront Requests area and My Requests widget, and a new record is added to the record type associated with the form.
   
   * If the request form was associated with an approval, the request is added to tthe Requests list in the Workfront Requests area and My Requests widget. A new record is added to the record type page only after the approvers have approved it.
   
      For information, see [Add an approval to a request form](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

   * The request is visible only to the owner, approver, and the people who have at least View permissions to the workspace. Workfront administrators can view all requests submitted to any workspace in the system. 

   * You receive an in-app and an email notification that the request has either been submitted successfully or has been sent for review.
   * If the request form was associated with an approval, the approvers receive an in-app and an email notification to review and approve the request.

      >[!NOTE]
      >
      >The email and in-app notifications are visible only when your organization's instance of Workfront is onboarded to the Adobe Unified Experience.
      >
      >There is a link to the request in the email confirmation or approval notification. 

1. (Optional) Click **View your request** in the confirmation message, to open the request, or click the **X** icon to close the confirmation.
1. (Optional) Do any of the following:

   * Click **Filters** and start adding conditions for what requests you want to view in the Requests list. 

      ![Editing filters in the Planning requests tab](assets/filters-editing-box-in-requests-planning-tab.png)

      You can filter by the following fields:  

      * **Workspace**: The workspace the request form is associated with.
      * **Record type**: The record type the request form is associated with.
      * **Entry date**: The date when the request was submitted.
      * **Request form**: The name of the request form used to submit the request.
      * **Status**: The status of the request.
      * **Entered by**: The name of the user who added the request. If the request was added by someone outside of Workfront, the **Entered by** field shows `N/A`.

         You can have multiple filters joined by either **And** or **Or**.
         The request list is filtered automatically, as you add the filter conditions. 
 
   * Click **Columns** and hide, show, or rearrange the columns in the request list. 
 
      >[!TIP]
      >
      >You cannot add any more columns. 
      >
      >You cannot display the **Subject** field.
 
      ![Columns editing box in Requests area](assets/columns-editing-box-in-requests-planning-tab.png)


1. Click the name of a request in the list. 

      The request details page opens. 
   
      ![Request page with comment](assets/new-request-page-with-comment.png)
    
1. (Optional) Enter a comment in the Comments area.
1. (Conditional) If the request form is not associated with an approval, or if the request has been approved, click the name of the request, then click the name of the record in the **Record** field. 

   The record's page opens in Workfront Planning. 

   >[!TIP]
   >
   >* If the record's primary field was not updated in the request form, the name of the record in the Record field of the request displays as **Untitled**. 
   >
   >* If the request form is associated with an approval, the approval must be granted before you can access the record from the request page. 

1. (Optional) Click the name of the **Record type**. 

   The record type page opens in Workfront Planning. 

## Submit a request to Workfront Planning from a shared link to a request form

1. Go to the link shared with you from a Workfront Planning record type. 

1. Update the fields available in the form. Fields with an asterisk are required. 

   >[!TIP]
   >
   >   If the **Subject** field is available, it will not be visible in Workfront Planning, after the request is submitted. 
   >
   >We recommend that you update as many fields in your request as possible to make the new record identifiable when it is added to the record type in Workfront Planning.

1. Click **Submit**.

   Your form is submitted and the following things occur:

   * If the request form was not associated with an approval, the request is added to the Requests list in the Workfront Requests area and My Requests widget, and a new record is added to the record type associated with the form.
   
   * If the request form was associated with an approval, the request is added to the Requests list in the Workfront Requests area and My Requests widget. A new record is added to the record type page only after all the approvers have approved it.
   
      For information, see [Add an approval to a request form](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

      >[!IMPORTANT]
      >
      >You can view only the requests submitted by you or anyone else to the workspaces that you have at least permissions to View. Workfront administrators can view all requests submitted to any workspace in the system. <!--ensure this is correct; asking team in slack-->
   
   * You receive an in-app and an email notification that the request has either been submitted successfully or has been sent for review.
   * If the request form was associated with an approval, the approvers receive an in-app and an email notification to review and approve the request.

      >[!NOTE]
      >
      >The email and in-app notifications are visible only when your organization's instance of Workfront is onboarded to the Adobe Unified Experience.
   
   <!-- <span class="preview"> After the request was approved and the record was created, the Approved by and Approved date fields display information about the approval on the record.</span>-->

1. (Optional) Click **View your request** to open the request in Workfront.

      <!--Or-->

      <!--Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.-->

1. (Optional) Click **Main menu** > **Requests** to view your request, then click the name of the request. 

   The request details page opens. 

   ![Request page with comment](assets/new-request-page-with-comment.png)

1. (Optional) Enter a comment in the Comments area.
1. (Conditional) If the request form is not associated with an approval, or if the request has been approved, click the name of the request, then click the name of the record in the **Created object** field. 

   The record's page opens in Workfront Planning. 

   >[!TIP]
   >
   >* If the record name was not added to the request form, the name of the record in the Record field of the request displays as **Untitled**. 
   >
   >* If the request form is associated with an approval, the approval must be granted before you can access the record from the request page. 

1. (Optional) Click the name of the **Object type**. 

   The record type page opens in Workfront Planning. 

## Create a request by copying an existing request

You can copy a request in the requests list in Workfront, then edit the details and submit it as a new request.

This is available only in the new requesting experience.

For instructions, see [Copy and submit requests](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Create drafts and requests from existing drafts

You can create a draft of a request, then return to the draft and submit it as a request later.

This is available only in the new requesting experience.

For instructions, see [Create requests from drafts](/help/quicksilver/manage-work/requests/create-requests/create-requests-from-drafts.md).

  

