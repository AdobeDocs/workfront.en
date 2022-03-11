---
filename: report-which-users-have-proofing-license-in-wf
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: List users with a proofing license in Adobe Workfront
description: You can view which users in Adobe Workfront currently have the option "User can generate proofs" enabled in either of the following ways below.
---

# List users with a proofing license in Adobe Workfront

You can view which users in Adobe Workfront currently have the option "User can generate proofs" enabled in either of the following ways below.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Legacy plan: Select or Premium</p> <p>For more information about proofing access with the different plans, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Edit access to:</p> 
    <ul> 
     <li> <p>Create Reports, Dashboards, and Calendars</p> </li> 
     <li> <p>Create Filters, Views, and Groupings</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or Proof Permission Profile you have, contact your Workfront or Workfront Proof administrator.

## Create a user report

You can create a user report&nbsp;to view which users can generate proofs:

<ol> 
 <li value="1">Navigate to <span class="bold">Reporting</span> area.</li> 
 <li value="2">Click the&nbsp;<span class="bold">New Report</span>&nbsp;drop-down menu, then click&nbsp;<span class="bold">User Report</span>.</li> 
 <li value="3">On the <span class="bold">Filters</span> tab, click <span class="bold">Add a Filter Rule</span>.</li> 
 <li value="4">In the available field, expand <span class="bold">User</span>, then click <span class="bold">Has&nbsp;Proof License</span>.</li> 
 <li value="5"> <p>Select <span class="bold">Equal</span> > <span class="bold">True</span>.</p> <p> <img src="assets/report-prooflicenses-350x135.png" alt="report_prooflicenses.png" style="width: 350;height: 135;"> </p> </li> 
 <li value="6"> <p>Click <span class="bold">Save+Close</span>.<br></p> <p>The report displays all users in Workfront who have a proofing license assigned to them.</p> </li> 
</ol>

## Update the People view

You can add a new column in the People view to view which users can generate proofs:

1. Go to the `People`&nbsp;area.
1. Click the `People` tab.
1. In the `View` drop-down menu, do either of the following:

  * To add this information to an existing view, select the view you want to customize, then click `Customize View`.
  * To add this information to a new view, click `New View`.

1. Click `Add Column`.
1. In the available field, expand `User`, then click `Has Proof License`.

1. Click `Done`, then click `Save View` or `Save as New View`.

   The view displays `True` or `False` depending on whether the user has a proofing license assigned to them.

