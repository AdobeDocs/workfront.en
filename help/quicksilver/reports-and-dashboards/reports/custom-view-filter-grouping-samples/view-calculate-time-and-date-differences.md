---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: calculate time and date differences'
description: Learn to calculate time and date differences.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 548dd91f-02bc-43ed-8322-d0facf3488f0
---
# View: calculate time and date differences

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>You cannot calculate the time and date difference in Adobe Workfront between two different objects of the same kind. For example, you cannot calculate the time and date difference between two dates on two different projects, tasks, or issues.

You can calculate the difference between the following:

* The time and date difference between two date fields on the same object
* The time and date difference between a field on an object and another field on the parent object

>[!TIP]
>
>These calculations display the number of days between the two dates. The result displays in days. The timestamp on the date field is also taken into account, and the number of days might be followed by decimals if the timestamps don't match. If the task was completed late, the number of days displays as a negative value.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: </p><ul><li><p>Contributor to modify a view </p></li><li>
   <p>Standard to modify a report</p></li></ul><p>Or</p><p>Current:</p><ul><li><p>Request to modify a view </p></li><li>
   <p>Plan to modify a report</p> </li><ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a view</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Calculate the time and date difference between two date fields on the same object

For example, you can calculate the difference between the Planned Completion Date and the Actual Completion Date of a task.

![](assets/view-planned-actual-completion-dates-datediff-column-new.png)

1. Go to a list of tasks. 
1. From the **View** drop-down menu, click **New View**.

1. Click **Add Column** and start typing "Planned Completion Date" in the **Show in this column** field then select it when it displays in the list.

1. Click **Add Column** and start typing "Actual Completion Date" in the **Show in this column** field then select it when it displays in the list.

1. Click **Add Column**, then click **Switch to Text Mode**.

1. Hover over the text mode area, and click **Click to edit text**.
1. Remove the text you find in the **Text Mode** box, and replace it with the following code:

   ```
    displayname=Planned-Actual Completion Date
    linkedname=direct
    querysort=plannedCompletionDate
    textmode=true
    valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)
    valueformat=HTML
   ```

1. Click **Save**, then **Save View**.

## Calculate the time and date difference between the field on an object and another field on a parent object

For a list of objects and their parents, see the "Understanding the Interdependency and Hierarchy of Objects" section in [Understand objects in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).  
For example, you can calculate the difference between the Planned Completion Date of a task and the Planned Completion Date of its parent task, or of the project that the task is on.

![](assets/view-project-planned-task-planned-completion-dates-datediff-column-new.png)

1. Go to a list of tasks. 
1. From the **View** drop-down menu, click **New View**.

1. Click **Add Column** and start typing " Project Planned Completion Date" or "Parent Completion Date" in the **Show in this column** field then select it when it displays in the list.

1. Click **Add Column** and start typing "Planned Completion Date" in the **Show in this column** field then select it when it displays in the list.

1. Click **Add Column**, then click **Switch to Text Mode**.

1. Hover over the text mode area, and click **Click to edit text**.
1. Remove the text you find in the **Text Mode** box, and replace it with one of the following codes:

   * To display the difference between the Planned Completion Date of the project and that of the task:

     ```   
      displayname=Project Planned Completion - Task Planned Completion (Days)
      textmode=true
      valueexpression=ROUND(DATEDIFF({project}.{plannedCompletionDate},{plannedCompletionDate}),2)
      valueformat=HTML
     ```

   * To display the difference between the Planned Completion Date of the parent task and that of the task:

     ```   
      valueexpression=ROUND(DATEDIFF({parent}.{plannedCompletionDate},{plannedCompletionDate}),2)
      textmode=true<br>valueformat=HTML
      displayname=Parent Planned Completion - Planned Completion (Days)
     ```

1. Click **Save**, then **Save View**.
