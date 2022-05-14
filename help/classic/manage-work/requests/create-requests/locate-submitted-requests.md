---
filename: locate-submitted-requests
product-area: requests
navigation-topic: create-requests
title: Locate submitted requests
description: You can locate the following types of requests that you or someone else submitted, or requests you started but you never finished submitting. You can locate these requests in the following areas of Adobe Workfront - EDIT ME.
---

# Locate submitted requests

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

You can locate the following types of requests that you or someone else submitted, or requests you started but you never finished submitting. You can locate these requests in the following areas of Adobe Workfront:

* Requests I've Submitted tab: Requests that you submitted.
* All&nbsp;Requests tab: All requests that you or someone else submitted and you have access to at least View. 
* Draft tab: All requests that you started but you never finished and you never submitted. For more information about draft requests, see [Create and submit Adobe Workfront requests](../../../manage-work/requests/create-requests/create-submit-requests.md).

  >[!TIP]
  >
  >You can only view your own draft requests.

## Access requirements

You must have the following to perform the steps in this article:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses overview*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions on the requests or higher</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Locate submitted requests

To locate requests that you or other users have submitted:

1. Go to the **Requests** area in the Global Navigation Bar.
1. Click&nbsp;**Requests I've Submitted** to view all the requests that you have submitted.

   Or  
   Click&nbsp;**All Requests**&nbsp;to view all requests that other users have submitted and which you have permissions to at least View.

   You can display up to 100 requests in the **Requests I've Submitted** and **All Requests** tabs.   
   Requests that are pending approval do not display.

1. Click the&nbsp;**Open**&nbsp;subtab to view requests that are open.  
   Requests without an Actual Completion Date or whose resolving object does not have an Actual Completion Date are listed in the Open subtab.&nbsp;

1. Click the&nbsp;**Complete** subtab to view requests that have been completed.   
   Requests with an Actual Completion Date or whose resolving object has an Actual Completion Date are listed in the Complete subtab.  
   Once a request receives an Actual Completion Date, it stays in the Recently Completed area for 10 business days. After that, it is moved to the Completed area.   
   For information about resolving and resolvable objects, see the article [Overview of Resolving and Resolvable Objects](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

1. (Optional) Select an option from the **Sort by** drop-down menu to sort the requests by the following criteria:&nbsp;

   * **Assigned To**: Requests are sorted alphabetically by the name of the assignee using the following criteria:&nbsp;

      * All requests assigned to users are sorted first, in the order of the users' names.
      * Requests assigned to job roles are sorted secondly, in the order of the job roles' names and are listed after all the requests assigned to users.
      * Requests that are assigned to teams are sorted last, in the order of the teams' names and are listed after all the requests assigned to users and those assigned to job roles.
      * All unassigned requests are listed last, in the order of their Entry Date.

   * **Submitted On**: Requests are sorted chronologically by the date when they were submitted.
   * **Recently Updated** (this is the default): Requests are sorted chronologically by the date of their last update.
   * **Name**: Requests are sorted alphabetically by name.&nbsp;
   * **Priority**: Requests are sorted in the order of their priority.
   * **Queue**: Requests are sorted alphabetically by the name of the requests queue where they were submitted.&nbsp;
   * **Status**: Requests are sorted alphabetically by their status.&nbsp;

1. Click **Drafts** to view all drafted requests. Workfront saves an unlimited number of drafts for each request queue in this folder. When you enter a new request for a queue topic that already has a draft, you will be prompted to use an existing draft. For more information about drafted requests, see [Create and submit Adobe Workfront requests](../../../manage-work/requests/create-requests/create-submit-requests.md).
