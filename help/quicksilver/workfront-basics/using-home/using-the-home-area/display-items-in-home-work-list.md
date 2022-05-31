---
filename: display-items-in-home-work-list
product-area: projects
navigation-topic: use-the-home-area
title: Display items in the Work List in the Home area
description: The Work List in the Home area displays all work items that are assigned to you. You can control which items display in the Work List as described below.
---

# Display items in the Work List in the Home area

The Work List in the Home area displays all work items that are assigned to you. You can control which items display in the Work List as described below.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects,&nbsp;Tasks, Issues, and Documents</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions or higher to the tasks and issues you need to work on</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Filter the Work List {#filter-the-work-list}

You can filter items in the Work List to see only specific types of items. For example, you can filter the work list to display only issues or requests.

>[!NOTE]
>
>The filter options are stored in the browser. If you consistently use the same browser on the same computer (and do not clear the site data) the selected filters do not change. If you switch browsers or computers then the filters revert to the default option which is with all filters deselected.

1. Click the **Main Menu** ![](assets/main-menu-icon.png) in the upper-right corner, then click&nbsp;**Home**. 
1. Click the **Filter** ![](assets/filter-nwepng.png) drop-down menu. 
1. Select from the following filter options to specify the type of items you want to display:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">All</td> 
      <td><span>Displays and selects all items. This includes tasks, </span><span data-mc-edit-date="2022-02-16T13:45:46.9712518-05:00" data-mc-editor="alinaw" data-mc-comment="this might need indenting when it goes to Preview" data-mc-initials="AL" data-mc-creator="alinaw" data-mc-create-date="2022-02-16T13:45:23.7889689-05:00">issues</span><span>, approvals, personal tasks and completed tasks and issues.</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tasks Working On</td> 
      <td> <p><span>Displays only tasks that you are actively working on.&nbsp;These are tasks assigned to you for which you have clicked the Work On&nbsp;It button.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tasks&nbsp;Ready to Start</td> 
      <td> 
       <div> 
        <p>Displays only tasks that are ready for you to start. Both of the following statements must be true:</p> 
        <ul style="list-style-type: square;"> 
         <li> <p>The tasks and their parents have no predecessors or task constraints preventing them from being worked on.</p> </li> 
        </ul> 
        <ul> 
         <li> <p>The Planned Start Date of the tasks is in the past or up to two weeks in the future.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tasks Not Ready</td> 
      <td> 
       <div> 
        <p>Displays only tasks that are not yet ready to start. Either one of the following statements must be true:</p> 
        <ul> 
         <li> <p>The tasks and their parents might have predecessors or task constraints that prevent them from being worked on.</p> </li> 
         <li> <p>The tasks have a Planned Start Date that is more than two weeks in the future.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Issues Working On</td> 
      <td> <p>Displays only issues that you are actively working on.&nbsp;These are issues assigned to you for which you have clicked the Work On&nbsp;It button.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Issues&nbsp;Requested</td> 
      <td><span>Displays only issues that you are assigned to but for which you have not clicked the Work On It button.</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Personal&nbsp;</td> 
      <td><span>Displays only personal tasks. These are tasks that you create as a To Do task, as described in the section</span><span href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#creating-a-personal-task">Create a personal task</span><span> in the article</span><span href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">Create work items from the Home area</span><span>.</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Approvals</td> 
      <td> 
       <div> 
        <p>Displays only approvals assigned or delegated to you and approvals you have submitted. Approvals include approvals on work items (projects, tasks, and issues), and approvals for documents, proofs, requests for access, and timesheets. For more information about approvals, see the following articles:</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">View approvals </a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">Manage approvals</a> </p> </li> 
        </ul> 
        <p>Note: Approvals that you submitted and where you are also one of the approvers are counted twice. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Completed</td> 
      <td> <p><span>Displays only completed tasks, issues, and personal tasks. Completed work displays for the previous two weeks and it is grouped in the Work List according to the week in which they were completed. Approvals are not included.</span> </p> <p><span>Completed work is hidden in the Work List unless you select this filter.</span> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* Filter options are based on objects (Tasks, Issues, Approvals, Personal tasks). 
   >* Tasks and issues are further filtered by their state in relationship with our readiness to work on them (Working On, Ready to Start, Not Ready for tasks, and Working On and Requested for issues). You can select to display tasks or issues in a specific state or click&nbsp;Tasks or Issues to select and display all states. 
   >* There is a separate filter for completed items and it includes both tasks and issues.&nbsp;This does not include approvals. The Completed filter includes Personal tasks. 
   >* You can select only one state at a time. For example, you can display only Working On tasks and only Requested issues.   
   >* You cannot apply filters for items assigned to one of your teams and they are not included in the items that are assigned directly to you. 

1. (Optional) Further organize the Work List, as described in the section [Group and sort by Date, Project, and Priority](#group-and-sort-by-date-project-and-priority) in this article.

## Group and sort by Date, Project, and Priority {#group-and-sort-by-date-project-and-priority}

You can group and sort the Work List by Planned Completion Date, Commit Date, Project, or My Priority. The option you choose determines how items are grouped in the Work List.

1. Click the **Main Menu** ![](assets/main-menu-icon.png) in the upper-right corner, then click&nbsp;**Home**. 
1. Click the **Group by** drop-down menu.

   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)

1. Select from the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Planned Completion</td> 
      <td> <p> Items display in the following groupings in the Work List, depending on their Planned Completion Date (the number of items contained within each grouping displays in parenthesis next to the heading title):</p> 
       <ul> 
        <li> <p>Late</p> </li> 
        <li> <p>No Planned Completion Date</p> </li> 
        <li> <p>This Week</p> </li> 
        <li> <p>This grouping is expanded by default.</p> </li> 
        <li> <p>Next Week</p> </li> 
        <li> <p>Planned, followed by various Planned Completion Dates (multiple groupings)</p> </li> 
        <li> <p>Complete</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Planned Start</td> 
      <td> <p>Items display in the following groupings in the Work List, depending on their Planned Start&nbsp;Date (the number of items contained within each grouping displays in parenthesis next to the heading title): </p> 
       <ul> 
        <li> <p>Late</p> </li> 
        <li> <p>This Week </p> </li> 
        <li> <p>This grouping is expanded by default.</p> </li> 
        <li> <p>Next Week</p> </li> 
        <li> <p>Planned, followed by various Planned Start Dates (multiple groupings)</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Commit Date</td> 
      <td> <p>Items display in the following groupings in the Work List (the number of items contained within each grouping displays in parenthesis next to the heading title): </p> 
       <ul> 
        <li> <p>No Commit Date</p> </li> 
        <li> <p>Committed Next Week</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Project</td> 
      <td>Items are grouped according to project, and projects appear alphabetically in the Work List.&nbsp;(The number of items contained within each grouping displays in parenthesis next to the heading title.)</td> 
     </tr> 
     <tr> 
      <td role="rowheader">My Priority</td> 
      <td>Items display&nbsp;in an order you choose. For more information, see <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">Prioritize work in the Home area</a>.</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>```The default sorting is ascending.```. If you change the sorting to ```descending``` , the selected sorting options are stored in the browser. If you consistently use the same browser on the same computer (and do not clear the site data) the sorting does not change, but if you switch browsers or computers then the sorting changes to the default sorting.

## View late items

Adobe Workfront uses the following dates to determine if work requests are late:

* **Tasks**: Planned Completion Date
* **Issues**: Planned Completion Date
* **Documents**: Submitted date
* **Timesheets**: Submitted date
* **Approvals**: Submitted date
* **Proof approvals**: Proof deadline

## Search the Work List&nbsp;

When you search the Work List, any items assigned to you are returned in the search (even items that are not currently loaded on the screen). If the Show complete option is selected, any items you marked complete within the past two weeks are also returned.

In addition, only the names of the work items are searched (information within the work item are not searched, neither are the names of the projects where the work item resides).

To search the Work List:

1. Click the **Main Menu** ![](assets/main-menu-icon.png) in the upper-right corner, then click&nbsp;**Home**. 
1. (Optional) Filter the Work List, as described in [Filter the Work List](#filter-the-work-list) and [Group and sort by Date, Project, and Priority](#group-and-sort-by-date-project-and-priority).

1. (Optional) If you are searching for a work item that is already complete, you must configure the Work List to display completed items before searching.
1. ![](assets/search-icon-highlighted-home-new-filters-and-sorting-nwe-350x238.png)

1. Begin typing the name of the item name you are searching for.   
   The Work List is automatically filtered as to include items with a matching name.

## Change the size of the Work List

You can change the size of the Work List so that it consumes anywhere between about a quarter of the Home area to about half of the Home area.

1. Click the **Main Menu** ![](assets/main-menu-icon.png) in the upper-right corner, then click&nbsp;**Home**. 
1. Mouse over the right edge of the Work List, then drag left or right until the Work List is the desired size.

## Collapse and expand groupings

Items in the Work List are displayed within groupings. You can collapse and expand groupings to control how much information is displayed on the page at a given time.&nbsp;

You can collapse and expand groupings within the Work List to better control what information is visible.  
By default, the This Week grouping is expanded and all other groupings are collapsed.&nbsp;Any changes you make are remembered the next time you access the Home area.&nbsp;

1. Click the **Main Menu** ![](assets/main-menu-icon.png) in the upper-right corner, then click&nbsp;**Home**. 
1. Click the **Expand** or **Collapse** arrow next to any grouping you want to expand or collapse.

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> </span>
   -->

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   Or  
   To expand or collapse all groupings simultaneously, click the **Expand** or **Collapse** arrow next to any grouping while holding down the Shift key.

