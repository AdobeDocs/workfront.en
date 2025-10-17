---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: display parent tasks'
description: You can apply the task filters below to display working tasks. Working tasks are tasks that can be worked independently and are not parent tasks to other tasks. In one example, a filter identifies children tasks that could be parents themselves. In this case, they are not working tasks.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
---
# Filter: display parent tasks

<!--Audited: 10/2024-->

You can apply the task filters below to display working tasks. Working tasks are tasks that can be worked independently and are not parent tasks to other tasks. In one example, a filter identifies children tasks that could be parents themselves. In this case, they are not working tasks.

>[!TIP]
>
>* If you consider adding more than one filter to a report, we recommend that you add all your filters using the report builder interface, and clicking Switch to Text Mode after all the other filter rules have been added. Then, you can add the code for the parent task filter as noted above.&nbsp;
>* We also recommend that you add a grouping for Project Name to make the report easier to read. For more information about adding groupings to your reports, see the article [Groupings overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md). 
>

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Contributor or Request to modify a filter </p>
   <p>Standard or Plan to modify a report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a filter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Display tasks with no children (they could have a parent)

You can apply the following filter to a task report to display tasks with no children. They could have parents of their own and be children of other tasks.

1. From the **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, or the **Main Menu** ![Main Menu lines](assets/lines-main-menu.png) in the upper-left corner, if available, click **Reports**. 

1. Click **New Report**.
1. Select a **Task Report**.
1. Click **Filters**.
1. Click **Add a Filter Rule**.
1. In the **Start typing field name ...** line, start typing **Number of Children**, then click **Task >> Number of Children** when it displays in the list.

1. Select **Equal (Case Sensitive)** for your modifier, then enter **0** for the number of children.  
   ![Parent task filter](assets/parent-task-filter-from-the-ui-350x76.png)

   Or

   Click **Switch to Text Mode**, and in the text editing window, copy and paste the following text

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```
   

1. Click **Save + Close**.

   This pulls a report for all tasks which are working tasks in your system. Some of these tasks could have a parent, but they are not parent tasks themselves.

## Display tasks with parents (they could have children)

You can apply the following filter to a task report to display tasks with parents, meaning they are children tasks. However, these tasks could also have children of their own because the filter does not exclude their children. Children tasks that are also parents for other tasks are not considered working tasks.

1. From the **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, or the **Main Menu** ![Main Menu lines](assets/lines-main-menu.png) in the upper-left corner, if available, click **Reports**. 

1. Click **New Report**.
1. Select a **Task Report**.
1. Click **Filters**.
1. Click **Add a Filter Rule**.
1. In the **Start typing field name ...** line, start typing **Parent ID**, then select **Task >> Parent ID** when it displays in the list.
1. Select **Is Not Blank** for your modifier.
    
    ![Parent ID is not blank](assets/filter-parent-id-not-blank-350x100.png)  
    
    Or
    
    Click **Switch to Text Mode**, and in the text editing window, copy and paste the following text: 
    
    `parentID_Mod=notblank`
    
1. Click **Save + Close**.
    
    This pulls a report for all tasks in your system that have parents and are children tasks of those parents. Some of these tasks could be a parent themselves.

## Display tasks with no children and no parents (standalone tasks)

You can apply the following filter to a task report to display standalone working tasks. These tasks don't have a parent and they have no children of their own.

1. From the **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, or the **Main Menu** ![Main Menu lines](assets/lines-main-menu.png) in the upper-left corner, if available, click **Reports**. 

1. Click **New Report**.
1. Select a **Task Report**.
1. Click **Filters**.
1. Click **Add a Filter Rule**.
1. In the **Start typing field name ...** line start typing **Number of Children**, then select **Task >> Number of Children** from the list.
1. Select **Equal (Case Sensitive)** for your modifier, then enter **0** for the number of children.
1. Click **Add another Filter Rule**. 
1. In the **Start typing field name ...** line start typing **Parent ID**, then select **Task >> Parent ID** from the list.
1. Select **Is Blank** for the modifier.

   ![Parent ID is blank and no children](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   Or

   Instead of steps 6-10 <!--ensure steps above stay accurate-->, click **Switch to Text Mode** and in the text editing window, copy and paste the following text:

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. Click **Save + Close**.

   This pulls a report for all tasks in your system that have no parents nor children. These are standalone working tasks.
