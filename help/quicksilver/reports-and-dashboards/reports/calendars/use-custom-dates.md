---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Use Custom Date Fields in a Calendar Report
description: A calendar report is a dynamic report that provides a visual representation of your work. You can use custom date fields in a calendar report for tasks, issues, and projects.
author: Jenny
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
---
# Use custom date fields in a calendar report

A [!UICONTROL calendar] report is a dynamic report that provides a visual representation of your work. You can use custom date fields in a calendar report for the following objects:

* Tasks
* Issues
* Projects

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, and Calendars</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td>Manage access to the calendar report</td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisites

1. You must have custom date fields and a value within the field available in your [!DNL Workfront] instance. If you don't have a custom form set up with custom dates, follow the instructions in [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
1. Attach the custom form to a project, task, or issue you plan to add to the calendar, and specify a date. For more information, see [Add a custom form to an object](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Set up the group of items

You can choose how you want the group of items to display on your calendar.

{{step1-to-calendars}}

1. Select the calendar you want to add a new group of items, click the More menu, then **Edit**.
   Or
   Click **[!UICONTROL + New Calendar]**, enter the project name, then click **[!UICONTROL Add advanced items]**.

   >[!NOTE]
   >
   >You must have [!UICONTROL Edit] access to [!UICONTROL Reports], [!UICONTROL Dashboards], and [!UICONTROL Calendars] in your access level to create a calendar report.

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
      <td>Choose <strong>[!UICONTROL Custom dates]</strong>.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL On the calendar, show]</strong></td>
      <td><p>Choose how you want the dates to show:</p>
       <ul>
        <li><strong>[!UICONTROL Single Date]</strong>: The calendar displays the object on a single date.</li>
        <li><strong>[!UICONTROL Duration] (Start to End)</strong>: The calendar displays the object over a span of days.<br><p>Note: If you choose <strong>[!UICONTROL Duration]</strong>, the end date specified must be after the start date or the item won't show on the calendar.</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Custom Dates]</strong></td>
      <td><p>Enter the custom date name attached to the object you want to track.</p><p><strong>NOTE:</strong> The search for the custom date name is limited to 50 results to avoid performance issues.</td>
     </tr>
    </tbody>
   </table>

1. Continue to the following section.

### Add objects to the group of items 

After you set up how you want items to display, you need to add the objects you want to see on the calendar to the grouping.

1. In the **[!UICONTROL What would you like to add to the calendar?]** section, select

   * **[!UICONTROL Tasks]**
   * **[!UICONTROL Projects]**
   * **[!UICONTROL Issues]**

1. Click **[!UICONTROL Add Tasks]**, **[!UICONTROL Add Projects]**, **[!UICONTROL Add Issues]**, or **Time Off** depending on the object type you are adding to the calendar.

1. In the drop-down menu, begin typing the field name, then select the field source of the object you want to display on the calendar (for example, **[!UICONTROL Late Tasks]**).
1. Set a condition statement for the calendar grouping.


   To learn about setting conditions, see [Filter and condition modifiers](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

    ![Select object for calendar](assets/calendar-field-name.png)

1. (Optional) Specify additional objects for the calendar grouping by repeating Steps 1-4.
1. In the **[!UICONTROL Set the Tasks/Projects/Issues labels to be the...]** field, select how the objects in this calendar grouping are labeled in the calendar.

   >[!NOTE]
   >
   >If the default label options are not available for a certain object, the object name is shown instead. For example, when the [!UICONTROL Parent Task] label is selected and there is no parent task associated with the object, [!DNL Adobe Workfront] displays the object name you are viewing in the calendar.

   ![set task labels](assets/set-task-labels.png)
1. Click **[!UICONTROL Save]**.

