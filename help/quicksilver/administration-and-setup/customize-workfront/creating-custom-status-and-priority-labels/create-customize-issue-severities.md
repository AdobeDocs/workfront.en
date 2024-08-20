---
title: Create or Customize Issue Severities
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Your users can use severities to define how serious an issue is. You can customize any of the five default severities existing in Adobe Workfront, or create a new severity for your users.
author: Lisa
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

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Built-in issue severities

Workfront has five built-in issue severities:

* Cosmetic
* Causes Confusion
* Bug with workaround
* Bug with no workaround
* Fatal error

<p>You can edit the following for these severities:</p> 

* Name
* Color
     
     The color of a severity is preserved in a chart report, if you group your results by Issue Severity. For information on chart reports, see [Add a chart to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Which severity is the default
     
     For more information about default severities, see [Create or edit an issue severity](#create-or-edit-an-issue-severity) in this article.
* Description
* Whether a severity is hidden in Workfront
     
     For more information about hiding a severity, see [Create or edit an issue severity](#create-or-edit-an-issue-severity")

* Delete a severity
     
     When you do this, you must select a replacement severity.

## Create or edit an issue severity {#create-or-edit-an-issue-severity}

As a Workfront administrator, you can create and edit issue severities to suit the needs of your users. 

{{step-1-to-setup}}

1. In the left panel, click **Project Preferences** > **Severities**.

1. If you are creating a new severity, click **Add a New Severity**.
1. Configure the following options for the new severity or edit them for an existing one:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Severity Name</td> 
      <td>Type a name for the severity</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Importance</td> 
      <td>Increase or decrease the level of seriousness, originally assigned by Workfront, for the severity.
      <p>The Importance number for each severity must be unique. The highest number corresponds to the highest level of severity.</p> <p>You cannot edit this number after you save the severity.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Color</td> 
      <td> <p>Choose a color for the severity.</p> 
      <p>The color of the severity is used in chart reports when you group your results by Issue Severity. For  information on chart reports, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Add a chart to a report</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Default Severity</td> 
      <td>Select the severity you want Workfront to select automatically all newly created issues.</p>
      <p>Cosmetic is the default severity for issues in Workfront.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Type a description for the severity to explain its function.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hide</td> 
      <td> Hide a severity that is no longer needed. 
      <p>A hidden severity does not display anywhere in Workfront, so users can't choose it for their issues.</p> 
      <p><b>IMPORTANT</b>: Instead of deleting severities that you no longer want to use, we suggest that you hide them. This way, you keep all your historic data on objects already completed with the severity, while preventing people from using the severity in the future.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Change the listing order of your severities by dragging and dropping them in the order you want.

   This changes the order in which they display for issues. It does not change the **Importance** number.

1. Click **Save**.

For more information on how to use severities while working with issues, see [Update issue severity](../../../manage-work/issues/issue-information/update-issue-severity.md).
