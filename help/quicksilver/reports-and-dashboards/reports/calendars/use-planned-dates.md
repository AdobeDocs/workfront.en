---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Use Planned Dates in a calendar report
description: A calendar report is a dynamic report that provides a visual representation of your work. You can use Planned Date fields in a calendar report for tasks, issues, and projects.
author: Lisa
feature: Reports and Dashboards
exl-id: 27bf6f03-2f6b-4556-a715-75c4a21bfbbb
---
# Use [!UICONTROL Planned Dates] in a calendar report

A calendar report is a dynamic report that provides a visual representation of your work. You can use [!UICONTROL Planned Date] fields in a calendar report for the following objects:

* Tasks
* Issues
* Projects

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>[!UICONTROL Edit] access to [!UICONTROL Reports], [!UICONTROL Dashboards], and [!UICONTROL Calendars]</p> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>[!UICONTROL Manage] access to the calendar report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

## Set up the group of items

You can choose how you want the group of items to display on your calendar.

1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of [!DNL Adobe Workfront], then click **[!UICONTROL Calendars]**.

1. Select the calendar you want to add a new group of items to.\
   Or\
   Click **[!UICONTROL + New Calendar]** and enter the calendar name.

   >[!NOTE]
   >
   >You must have Edit access to Reports, Dashboards, and Calendars in your access level to create a calendar report.

1. On the left, click **[!UICONTROL Add to Calendar]**, then click **[!UICONTROL Add advanced items]**.

1. Specify the following:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Name this group of items]</strong></td>
      <td>Type a name for the group of items.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>Select a color for the group of items. All items display in the selected color on the calendar report.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Date Field]</strong></td>
      <td><p>Choose <strong>[!UICONTROL Planned dates]</strong>. For more information on planned dates, see </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-start-date.md" class="MCXref xref">Overview of the project Planned Start Date</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Overview of the task Planned Start Date</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Overview of the task Planned Completion Date</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Set the project Planned Completion Date</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>On the calendar, show</strong></td>
      <td><p>Choose how you want the dates to show:</p>
       <ul>
        <li><strong>[!UICONTROL Start Date Only]</strong>: The calendar displays the object on a single date.</li>
        <li><strong>[!UICONTROL End Date Only]</strong>: The calendar displays the object on a single date.</li>
        <li><strong>[!UICONTROL Duration] (Start to End)</strong>: The calendar displays the object over a span of days.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Switch to actual dates when available]</strong></td>
      <td><p>The calendar automatically switches to actual dates when they are available. <br>Choose <strong>[!UICONTROL Yes]</strong> or <strong>[!UICONTROL No]</strong> to switch to actual dates when available. For more information on Actual Dates, see</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Overview of the project Actual Start Date </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Overview of the project Actual Completion Date </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. Continue to the following section.

## Add objects to the group of items

After you set up how you want items to display, you need to add the objects you want to see on the calendar to the grouping.

1. In the **[!UICONTROL What would you like to add to the calendar?]** section, select

   * **[!UICONTROL Tasks]**
   * **[!UICONTROL Projects]**
   * **[!UICONTROL Issues]**

1. Click **[!UICONTROL Add Tasks]**, **[!UICONTROL Add Projects]**, or **[!UICONTROL Add Issues]**, depending on the object type you are adding to the calendar.\
   ![Select object for calendar](assets/field-name.png)

1. In the drop-down menu, begin typing the field name, then select the field source of the object you want to display on the calendar (for example, **[!UICONTROL Late Tasks]**).
1. Set a condition statement for the calendar grouping.

   ![Condition statement](assets/condition-statement-calendar.png)

   To learn about setting conditions, see [Filter and condition modifiers](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Optional) Specify additional objects for the calendar grouping by repeating Steps 1-4.
1. In the **[!UICONTROL Set the Tasks/Projects/Issues labels to be the...]** field, select how the objects in this calendar grouping are labeled in the calendar.

   >[!NOTE]
   >
   >If the default label options are not available for a certain object, the object name is shown instead. For example, when the [!UICONTROL Parent Task] label is selected and there is no parent task associated with the object, [!DNL Adobe Workfront] displays the object name you are viewing in the calendar.

1. Click **[!UICONTROL Save]**.
