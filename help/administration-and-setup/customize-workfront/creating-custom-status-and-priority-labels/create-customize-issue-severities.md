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

As an *Adobe Workfront administrator*, you can customize the default severities existing in *Workfront* or create new severities that users can associate with issues in *Workfront*.

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
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Customizing issue severities

There are 5 default issue&nbsp;severities in *Workfront*:

* Cosmetic
* Causes Confusion
* Bug with workaround
* Bug with no workaround
* Fatal error

*Workfront administrators* can customize the following information on&nbsp;the default severities provided in *Workfront*:

<ul> 
 <li>Edit the severity name</li> 
 <li> <p>Change the color associated with the severity</p> <note type="note">
   The color of your severity is preserved in a chart report, if you group your results by 
   <span class="bold">Issue Severity</span>. For more information on chart reports, see 
   <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Add a chart to a report</a>.
  </note> </li> 
 <li> <p>Change the default severity</p> <p>For more information about default severities, see <a href="#creating-new-issue-severities" class="MCXref xref">Create new issue severities</a>.</p> </li> 
 <li>Edit the description of the severities</li> 
 <li> <p>Hide a severity</p> <p>For more information about&nbsp;hiding a severity, see <a href="#creating-new-issue-severities" class="MCXref xref">Create new issue severities</a>.</p> </li> 
 <li> <p>Delete a severity</p> <p>When you delete an existing severity, you must select a replacement one.</p> </li> 
</ul>

## Create new issue severities

As a *Workfront administrator*, you can create new issue severities to reflect the needs in your organization.&nbsp;

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="2">In the left panel, click <span class="bold">Project Preferences</span> > <span class="bold">Severities</span>.</li> 
 <li value="3">Click <span class="bold">Add a New Severity</span>.</li> 
 <li value="4"> <p>Fill in the following information for the new severity:</p> 
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
     <td> <p>When adding a new severity, a number is assigned to it by default. Edit this number, if it does not match your needs. The <span class="bold">Importance</span> number for each severity&nbsp;must be unique. The number of the severity reflects the seriousness of the issue: the highest number corresponds to the highest severity.</p> <note type="note">
       You cannot edit the 
       <span class="bold">Importance</span> number, after you save the severity.
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Color</td> 
     <td> <p>Choose a color for the severity.</p> <note type="note">
       The color of the severity is used in chart reports, when you group your results by 
       <span class="bold">Issue Severity</span>. For more information on chart reports, see 
       <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Add a chart to a report</a>.
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Default Severity</td> 
     <td>Decide whether this should be a default severity&nbsp;or not, by selecting the radio button.<br>If a severity is designated as the default severity, it is automatically selected for all newly created issues in <em>Workfront</em>. <span class="bold">Cosmetic</span>&nbsp;is the default severity for issues in <em>Workfront</em>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Description</td> 
     <td>Type a description for the severity&nbsp;to explain its function.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Hide</td> 
     <td> <p>Select this box if you want to hide the severity.</p> <p>When you check the <span class="bold">Hide</span> option, the severity&nbsp;does not display anywhere in <em>Workfront</em> and users are not able to choose it for their issues.</p> <note type="important">
       We recommend that you hide the severities&nbsp;that you no longer want to use, rather than deleting them.&nbsp;By hiding them, you still keep all your historic data, of objects that have been completed with this severity, while preventing people from choosing this severity&nbsp;in the future.
      </note> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5"> <p>(Optional) Change the listing order of your severities by dragging and dropping them in the order you want.</p> <p>This changes the order in which they display for issues. It does not change the <span class="bold">Importance</span> number.</p> </li> 
 <li value="6">Click <span class="bold">Save</span>.</li> 
</ol>

For more information on how to use severities while working with issues, see [Update issue severity](../../../manage-work/issues/issue-information/update-issue-severity.md).
