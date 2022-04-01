---
filename: create-customize-issue-severities
title: Create and customize issue severities
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Create and customize issue severities
description: As an Adobe Workfront administrator, you can customize the default severities existing in Workfront or create new severities that users can associate with issues in Workfront.
---

# Create and customize issue severities

As an Adobe Workfront administrator, you can customize the default severities existing in Workfront or create new severities that users can associate with issues in Workfront.

Issues are unexpected events that can prevent your projects from finishing on time or within budget. You can use severities to define how serious an issue is.

Tasks and projects do not have severities.

##  

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Customizing issue severities

There are 5 default issue&nbsp;severities in Workfront:

* Cosmetic
* Causes Confusion
* Bug with workaround
* Bug with no workaround
* Fatal error

Workfront administrators can customize the following information on&nbsp;the default severities provided in Workfront:

* Edit the severity name
* Change the color associated with the severity

  >[!NOTE]
  >
  >The color of your severity is preserved in a chart report, if you group your results by **Issue Severity**. For more information on chart reports, see [Add a chart to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Change the default severity

  For more information about default severities, see [Create new issue severities](#create-new-issue-severities).

* Edit the description of the severities
* Hide a severity

  For more information about&nbsp;hiding a severity, see [Create new issue severities](#create-new-issue-severities).

* Delete a severity

  When you delete an existing severity, you must select a replacement one.

## Create new issue severities {#create-new-issue-severities}

As a Workfront administrator, you can create new issue severities to reflect the needs in your organization.&nbsp;

1. Click **Setup** near the upper-right corner of Adobe Workfront on the Global Navigation Bar.  

1. In the left panel, click **Project Preferences** > **Severities**.

1. Click **Add a New Severity**.
1. Fill in the following information for the new severity:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Severity Name</td> 
      <td>Type a name</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Importance</td> 
      <td> <p>When adding a new severity, a number is assigned to it by default. Edit this number, if it does not match your needs. The <strong>Importance</strong> number for each severity&nbsp;must be unique. The number of the severity reflects the seriousness of the issue: the highest number corresponds to the highest severity.</p> <p>Note: You cannot edit the <strong>Importance</strong> number, after you save the severity.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Color</td> 
      <td> <p>Choose a color for the severity.</p> <p>Note: The color of the severity is used in chart reports, when you group your results by <strong>Issue Severity</strong>. For more information on chart reports, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Add a chart to a report</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Default Severity</td> 
      <td>Decide whether this should be a default severity&nbsp;or not, by selecting the radio button.<br>If a severity is designated as the default severity, it is automatically selected for all newly created issues in Workfront. <strong>Cosmetic</strong>&nbsp;is the default severity for issues in Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Type a description for the severity&nbsp;to explain its function.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hide</td> 
      <td> <p>Select this box if you want to hide the severity.</p> <p>When you check the <strong>Hide</strong> option, the severity&nbsp;does not display anywhere in Workfront and users are not able to choose it for their issues.</p> <p>Important: We recommend that you hide the severities&nbsp;that you no longer want to use, rather than deleting them.&nbsp;By hiding them, you still keep all your historic data, of objects that have been completed with this severity, while preventing people from choosing this severity&nbsp;in the future.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Change the listing order of your severities by dragging and dropping them in the order you want.

   This changes the order in which they display for issues. It does not change the **Importance** number.

1. Click **Save**.

For more information on how to use severities while working with issues, see [Update issue severity](../../../manage-work/issues/issue-information/update-issue-severity.md).
