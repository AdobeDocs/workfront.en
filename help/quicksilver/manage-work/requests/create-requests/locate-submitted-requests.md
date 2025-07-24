---
product-area: requests
navigation-topic: create-requests
title: Locate Submitted Requests
description: Learn about the areas of Adobe Workfront where you can locate requests that you or someone else submitted or requests that you never submitted and were saved as drafts. 
author: Alina
feature: Requests
topic: Collaboration
role: User
exl-id: cfa2383a-9594-4867-9b48-11b8ea281486
---
# Locate submitted requests

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

You can locate the following types of requests that you or someone else submitted, or requests you started but you never finished submitting. You can locate these requests in the following areas of Adobe Workfront:

* The **Workfront** tab of the Requests area in Workfront: Locate requests submitted to Workfront request queues in the following sections: 
   * **Submitted section**: All requests that you or someone else submitted and you have access to at least View. 
   * **Draft section** : All requests that you started but you never finished and you never submitted. For more information about draft requests, see [Create and submit Adobe Workfront requests](../../../manage-work/requests/create-requests/create-submit-requests.md).

   >[!TIP]
   >
   >You can only view your own draft requests.

* The **Planning** tab of the Requests area in Workfront: Locate requests submitted to Workfront Planning request forms. Your organization must purchase a Workfront Planning package. For information, see the following articles:

   * [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
   * [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md)


## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Contributor or higher</p>
   Or
   <p>Current: Request or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td><p>Edit access to Issues</p></td> 
  </tr>
  <tr>
   <td role="rowheader">Object permissions</td> 
   <td><p>View permissions or higher on the requests</p></td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Locate submitted requests

To locate requests that you or other users have submitted:

{{step1-to-requests}}

1. (Conditional) If your organization purchased a Workfront Planning package, click the **Workfront** tab to view Workfront requests. 
1. Click **Submitted** in the left panel to view all submitted requests.

   You can view up to 2000 requests and they may display on multiple pages.

   >[!TIP]
   >
   >You cannot customize the columns in the Submitted request list.

   ![](assets/nwe-submitted-requests-new-list-350x57.png)

 
1. The following columns display by default:

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader">Name</td> 
         <td> <p>The name of the request.</p> <p>Click the name of a request to open it. </p> <p><b>TIP</b>
         
      If the issue was not preserved when it was converted to a task or a project, the name of the issue is dimmed and can no longer be clicked. For information about converting issues, see <a href="../../../manage-work/issues/convert-issues/convert-issues.md" class="MCXref xref">Overview of converting issues in Adobe Workfront</a>. </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Converted to</td> 
         <td> <p>The name of the resolving object which can be a task or project that the request was converted to. </p> <p>Click the name of the task or project to open them. </p> <p>If the request was not converted, this field is empty. </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Path</td> 
         <td>The name of the request queue, topic groups, and queue topics where the request was originally submitted. </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Status</td> 
         <td>The current status of the request or of the resolving object (task or project)</td> 
      </tr> 
      <tr> 
         <td role="rowheader">Entry Date</td> 
         <td>The date when the request was submitted or the date when the resolving object was created if the request was deleted when converted. </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Last Update Date</td> 
         <td> <p>The date when the request was updated last.</p> <p>The Submitted request list is sorted by this field, by default. </p> </td> 
      </tr> 
      </tbody> 
      </table>

1. (Optional) Click the header of a column to sort by it.

   >[!TIP]
   >
   >When you navigate away from the Submitted requests list, the selected sorting option is preserved.

1. (Optional) Select a request in the list, then click the **Open Summary** icon ![](assets/open-summary-with-text-nwe.png) to open the Summary panel and display additional information about the request, add comments, documents, or assign it. For information about the Summary panel, see [Summary overview](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

   >[!TIP]
   >
   >If the Summary panel is already opened, the Open Summary icon changes to Close Summary.

1. (Optional and conditional) Click the **X** icon in the upper-right corner or the **Close Summary** icon ![](assets/close-summary-with-text-nwe.png) to close the Summary Panel.

   If an issue was converted to a task or project and the issue was deleted in the conversion process, the Summary panel is blank. For information about converting issues, see [Overview of converting issues in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md). 

1. From the **Filter icon** ![](assets/filter-nwepng.png) in the top right of the list, select any of the filters listed in the table below.

   >[!TIP]
   >
   >You cannot modify filters in the Submitted section of the Requests area.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">All</td> 
      <td>All submitted requests, regardless of status or who submitted them.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Open</td> 
      <td> <p>All submitted requests that are currently open, regardless of who submitted them. Only requests you have at least permissions to view display here if you did not submit them yourself. </p> <p>Requests without an Actual Completion Date or whose resolving object does not have an Actual Completion Date are listed in the Open subtab.</p> <p><b>TIP</b> 
      
      Requests that are in any status that does not equate with Closed are considered open.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">My Requests</td> 
      <td>Requests you submitted regardless of their status. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">My Open Requests</td> 
      <td> <p>Requests you submitted that are still open. </p> <p>Requests without an Actual Completion Date or whose resolving object does not have an Actual Completion Date are listed in the My Open Requests subtab. </p> <p><b>TIP</b> 
      
      Requests that are not in a status that equates with Closed are considered open.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Click the **Filter page** icon ![](assets/search-icon.png) at the top of the list to search for a request by name. The list updates with results that match your search criteria.

   <!--
   <li value="9" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Click the <strong>Complete</strong> subtab to view requests that have been completed.</p> <p>(NOTE: this step will stay drafted even after release. We can't see Completed at this time!) <br>Requests with an Actual Completion Date or whose resolving object has an Actual Completion Date are listed in the Complete subtab.<br>Once a request receives an Actual Completion Date, it stays in the Recently Completed area for 10 business days. After that, it is moved to the Completed area. <br>For information about resolving and resolvable objects, see the article <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </li>
   -->

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Optional) Select an option from the <strong>Sort by</strong> drop-down menu to sort the requests by the following criteria:   (NOTE: this step will stay drafted even after release. We can't see Completed at this time!)  
   <ul>
   <li><strong>Assigned To</strong>: Requests are sorted alphabetically by the name of the assignee using the following criteria: 
   <ul>
   <li>All requests assigned to users are sorted first, in the order of the users' names.</li>
   <li>Requests assigned to job roles are sorted secondly, in the order of the job roles' names and are listed after all the requests assigned to users.</li>
   <li>Requests that are assigned to teams are sorted last, in the order of the teams' names and are listed after all the requests assigned to users and those assigned to job roles.</li>
   <li>All unassigned requests are listed last, in the order of their Entry Date. </li>
   </ul></li>
   <li><strong>Submitted On</strong>: Requests are sorted chronologically by the date when they were submitted.</li>
   <li><strong>Recently Updated</strong> (this is the default): Requests are sorted chronologically by the date of their last update.</li>
   <li><strong>Name</strong>: Requests are sorted alphabetically by name. </li>
   <li><strong>Priority</strong>: Requests are sorted in the order of their priority.</li>
   <li><strong>Queue</strong>: Requests are sorted alphabetically by the name of the requests queue where they were submitted. </li>
   <li><strong>Status</strong>: Requests are sorted alphabetically by their status. </li>
   </ul></li>
   -->

1. Click **Drafts** to view all drafted requests. Workfront saves an unlimited number of drafts for each request queue in this folder. When you enter a new request for a queue topic that already has a draft, you will be prompted to use an existing draft. For more information, see [Create requests from drafts](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).

1. (Optional and conditional) If your organization purchased a Workfront Planning package, click the **Planning** tab, then click **Submitted** in the left panel to view Workfront Planning requests. 

   Use **Filters** and **Columns** to update the information in the Planning request list. 

   ![](assets/workfront-planning-tab-submitted-section-in-requests-area.png)

   For information, see [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md).


