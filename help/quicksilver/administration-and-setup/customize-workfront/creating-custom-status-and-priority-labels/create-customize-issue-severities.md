---
filename: create-customize-issue-severities
title: Create and customize issue severities
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Create or customize issue severities
description: Your users can use severities to define how serious an issue is. You can customize any of the five default severities existing in Adobe Workfront, or create a new severity for your users.
---

# Create or customize issue severities

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **Linked to Understanding Issue Severity.</p>
-->

Your users can use severities to define how serious an issue is. You can customize any of the five default severities existing in Adobe Workfront, or create a new severity for your users.

>[!NOTE]
>
>Tasks and projects do not have severities.

## Access requirements

You must have the following access to perform the steps in this article: 

<table> 
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
   <td> <p>You must be a Workfront administrator.</p> <p><b>Note<>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Built-in issue severities

Workfront has five built-in issue&nbsp;severities:

* Cosmetic
* Causes Confusion
* Bug with workaround
* Bug with no workaround
* Fatal error

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>You can edit the following for these severities:</p>
<ul>
<li>Name</li>
<li> <p>Color</p> <note type="note">
The color of your severity is preserved in a chart report, if you group your results by
<strong>Issue Severity</strong>. For more information on chart reports, see
<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Add a chart to a report</a>.
</note> </li>
<li> <p>Change the default severity
-->

<!--
<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">STOPPED&nbsp;HERE</span>
</p> <p>For more information about default severities, see <a href="#create-or-edit-an-issue-severity" class="MCXref xref">Create or edit an issue severity</a> in this article.</p> </li>
<li>Edit the description of the severities</li>
<li> <p>Hide a severity</p> <p>For more information about&nbsp;hiding a severity, see <a href="#create-or-edit-an-issue-severity" class="MCXref xref">Create or edit an issue severity</a> in this article.</p> </li>
<li> <p>Delete a severity</p> <p>When you delete an existing severity, you must select a replacement one.</p> </li>
</ul>
</div>
-->

## Create or edit an issue severity {#create-or-edit-an-issue-severity}

As a Workfront administrator, you can create and edit issue severities to suit the needs of your users.&nbsp;

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).  

1. In the left panel, click **Project Preferences** > **Severities**.

1. If you are creating a new severity, click **Add a New Severity**.
1. Configure the following options for the new severity or edit them for an existing one:

   <table> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Severity Name</td> 
      <td>Type a name</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Importance</td> 
      <td> <p>When you create a severity, Workfront assigns a number to it. Edit this number, if it does not match your needs. The <strong>Importance</strong> number for each severity&nbsp;must be unique. The number of the severity reflects the seriousness of the issue: the highest number corresponds to the highest severity.</p> <p>Note: You cannot edit the <strong>Importance</strong> number, after you save the severity.</p> </td> 
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
