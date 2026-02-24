---
title: Create or Customize Issue Severities
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Your users can use severities to define how serious an issue is. You can customize any of the five default severities existing in Adobe Workfront, or create a new severity for your users.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
---
# Create or customize issue severities

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

Your users can use severities to define how serious an issue is. You can customize any of the five default severities existing in Adobe Workfront, or create a new severity for your users.

>[!NOTE]
>
>Tasks and projects do not have severities.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>System Administrator</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

## Built-in issue severities

Workfront has five built-in issue severities:

* Cosmetic
* Causes Confusion
* Bug with workaround
* Bug with no workaround
* Fatal error

You can edit the following for these severities:

* Name
* Color
     
     The color of a severity is preserved in a chart report, if you group your results by Issue Severity. For information on chart reports, see [Add a chart to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Which severity is the default
     
     For more information about default severities, see [Create or edit an issue severity](#create-or-edit-an-issue-severity) in this article.

* Description
* Whether a severity is hidden in Workfront
     
     For more information about hiding a severity, see [Create or edit an issue severity](#create-or-edit-an-issue-severity) in this article.

* Delete a severity
     
     When you do this, you must select a replacement severity.

## Create or edit an issue severity {#create-or-edit-an-issue-severity}

As a Workfront administrator, you can create and edit issue severities to suit the needs of your users. 

{{step-1-to-setup}}

1. In the left panel, click **Project Preferences** > **Severities**.

1. If you are creating a new severity, click **New row** at the bottom of the table.
1. Configure the following options for the new severity or edit them for an existing one:

   * **Severity Name**: Type a name for the severity.
   * **Importance**: Increase or decrease the level of seriousness, originally assigned by Workfront, for the severity.
     
     The Importance number for each severity must be unique. The highest number corresponds to the highest level of severity.

     You cannot edit this number after you save the severity.
   
   * **Color**: Choose a color for the severity.

     The color of the severity is used in chart reports when you group your results by Issue Severity. For information on chart reports, see [Add a chart to a report](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

   * **Default Severity**: Select the severity you want Workfront to apply automatically to all newly created issues.

     **Cosmetic** is the default severity for issues in Workfront.

     You cannot make a hidden severity the default.
     
     The default severity is indicated with an icon ![Default severity icon](assets/default-icon.png). To choose a new default, do one of the following:

       * Select the check box next to the severity name and select **Make Default** in the action bar at the bottom of the screen.
       * Hover over the severity name and click the **More** menu that appears. Then, select **Make Default**.

         The new default severity is labeled with the icon.

   * **Description**: Type a description for the severity to explain its function.
   * **Hide Choice**: Select **Yes** to hide a severity that is no longer needed.

     A hidden severity does not display anywhere in Workfront, so users can't choose it for their issues.

     >[!IMPORTANT]
     >
     >Instead of deleting severities that you no longer want to use, we suggest that you hide them. This way, you keep all your historic data on objects already completed with the severity, while preventing people from using the severity in the future.

1. (Optional) Change the listing order of your severities by dragging and dropping them in the order you want.

   This changes the order in which they display for issues. It does not change the **Importance** number.

1. Click **Save**.

For more information on how to use severities while working with issues, see [Update issue severity](../../../manage-work/issues/issue-information/update-issue-severity.md).
