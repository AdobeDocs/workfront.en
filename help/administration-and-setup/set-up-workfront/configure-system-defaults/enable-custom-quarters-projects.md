---
filename: enable-custom-quarters-projects
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Enable custom quarters for projects
description: For reporting purposes, you might want to create custom quarters if your organization's quarters are based on specific criteria other than calendar dates (such as business days or shopping days).
---

# Enable custom quarters for projects

For reporting purposes, you might want to create custom quarters if your organization's quarters are based on specific criteria other than calendar dates (such as business days or shopping days).

You can configure up to eight custom quarters for your `Adobe Workfront` system.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <span>Workfront administrator</span>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Set up custom quarters for your `Workfront` system

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">Project Preferences</span> > <span class="bold">Projects.</span></li> 
 <li value="3">In the <span class="bold">Timelines</span> section, select <span class="bold">Enable Custom Quarters</span>.</li> 
 <li value="4"> <p>Type a name for the custom quarter, such as "Fiscal Q1 2021."</p> </li> 
 <li value="5"> <p>Select start and end dates for the custom quarter.</p> <p> <img src="assets/custom-quarters-nwe-350x107.png" style="width: 350;height: 107;"> </p> </li> 
 <li value="6"> <p>(Optional) Click <span class="bold">Add Custom Quarter</span> to add additional custom quarters to the system.</p> </li> 
 <li value="7"> <p>(Optional) Create a reporting element that refers to the fiscal quarters.</p> 
  <div class="example" data-mc-autonum="<b>Example: </b>">
   <span class="autonumber"><span><b>Example: </b></span></span> 
   <p>Create a filter for a project list and include the Planned Completion Date of a project referencing the custom quarters.</p> 
   <p> <img src="assets/example-of-project-filter-with-custom-quarters-350x406.png" style="width: 350;height: 406;"> </p> 
   <p>The references to "This Quarter", "Next Quarter", and "Last Quarter"&nbsp;are replaced with new references to the custom quarters. </p> 
   <p>For information about reporting elements, see <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Reporting elements: filters, views, and groupings</a>. </p> 
   <p>For information about creating filters, see <a href="../../../reports-and-dashboards/reports/reporting-elements/create-filters.md" class="MCXref xref">Create or edit filters in Adobe Workfront</a>. </p> 
  </div> </li> 
</ol>

