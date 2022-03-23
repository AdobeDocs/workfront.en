---
filename: locate-submitted-requests
product-area: requests
navigation-topic: create-requests
title: Locate submitted requests
description: You can locate the following types of requests that you or someone else submitted, or requests you started but you never finished submitting. You can locate these requests in the following areas of Adobe Workfront:
---

# Locate submitted requests

You can locate the following types of requests that you or someone else submitted, or requests you started but you never finished submitting. You can locate these requests in the following areas of Adobe Workfront:

* Requests I've Submitted tab: Requests that you submitted.
* All&nbsp;Requests tab: All requests that you or someone else submitted and you have access to at least View. 
* Draft tab: All requests that you started but you never finished and you never submitted. For more information about draft requests, see [Create and submit Adobe Workfront requests](../../../manage-work/requests/create-requests/create-submit-requests.md).

  >[!TIP]
  >
  >You can only view your own draft requests.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
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
   <td> <p>View permissions on the requests or higher</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
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

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Locate submitted requests in Production</h2>
<p>To locate requests that you or other users have submitted :</p>
<ol>
<li value="1"> <p>Go to the <strong>Requests</strong> area in the Global Navigation Bar.</p> <p>Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</p> </li>
<li value="2"> <p>Click&nbsp;<strong>Requests I've Submitted</strong> to view all the requests that you have submitted. </p> <p>Or<br>Click&nbsp;<strong>All Requests</strong>&nbsp;to view all requests that other users have submitted and which you have permissions to at least View. </p> <p>You can display up to 100 requests in the <strong>Requests I've Submitted</strong> and <strong>All Requests</strong> tabs.<br>Requests that are pending approval do not display.</p> </li>
<li value="3">Click the&nbsp;<strong>Open</strong>&nbsp;subtab to view requests that are open.<br>Requests without an Actual Completion Date or whose resolving object does not have an Actual Completion Date are listed in the Open subtab.</li>
<li value="4">Click the&nbsp;<strong>Complete</strong> subtab to view requests that have been completed. <br>Requests with an Actual Completion Date or whose resolving object has an Actual Completion Date are listed in the Complete subtab.<br>Once a request receives an Actual Completion Date, it stays in the Recently Completed area for 10 business days. After that, it is moved to the Completed area. <br>For information about resolving and resolvable objects, see the article <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</li>
<li value="5">(Optional) Select an option from the <strong>Sort by</strong> drop-down menu to sort the requests by the following criteria:&nbsp;
<ul>
<li><p><strong>Assigned To</strong>: Requests are sorted alphabetically by the name of the assignee using the following criteria:&nbsp;</p>
<ul>
<li>All requests assigned to users are sorted first, in the order of the users' names.</li>
<li>Requests assigned to job roles are sorted secondly, in the order of the job roles' names and are listed after all the requests assigned to users.</li>
<li>Requests that are assigned to teams are sorted last, in the order of the teams' names and are listed after all the requests assigned to users and those assigned to job roles.</li>
<li>All unassigned requests are listed last, in the order of their Entry Date. </li>
</ul></li>
<li><strong>Submitted On</strong>: Requests are sorted chronologically by the date when they were submitted.</li>
<li><strong>Recently Updated</strong> (this is the default): Requests are sorted chronologically by the date of their last update.</li>
<li><strong>Name</strong>: Requests are sorted alphabetically by name.&nbsp;</li>
<li><strong>Priority</strong>: Requests are sorted in the order of their priority.</li>
<li><strong>Queue</strong>: Requests are sorted alphabetically by the name of the requests queue where they were submitted.&nbsp;</li>
<li><strong>Status</strong>: Requests are sorted alphabetically by their status.&nbsp;</li>
</ul></li>
<li value="6"> <p>Click <strong>Draft Requests</strong> to view all drafted requests. Workfront saves an unlimited number of drafts for each request queue in this folder. When you enter a new request for a queue topic that already has a draft, you will be prompted to use an existing draft. For more information about drafted requests, see the <a href="#create-requests-in-the-web-app" class="MCXref xref">Locate submitted requests</a> section in this article. </p> </li>
</ol>
</div>
-->

&nbsp;

&nbsp;

&nbsp;
