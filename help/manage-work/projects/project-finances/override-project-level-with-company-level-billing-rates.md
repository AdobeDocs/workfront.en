---
filename: override-project-level-with-company-level-billing-rates
product-area: projects
navigation-topic: financials
title: Override Project-Level Billing Rates with Company-Level Billing Rates
description: You can configure a project to use company-level billing rates instead of project-level billing rates.
---

# Override Project-Level Billing Rates with Company-Level Billing Rates

You can configure a project to use company-level billing rates instead of project-level billing rates.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Financial&nbsp;Data</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project with permissions to Manage Finance</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Enable the Company-level Billing Rates override option

When a company is associated with a project and this option is enabled, changes made to the company-level billing rates override the billing rate set on the project.

When a user manually recalculates finances on the project, any changes to the company-level billing rates are applied. Historical revenue calculations are also overridden unless they are marked as billed.

<ol> 
 <li value="1">Go to a project. </li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">More</span> menu <img src="assets/qs-more-icon-on-an-object.png"> next to the name of the project in the header, then click <span class="bold">Edit</span>. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">More</span> menu <img src="assets/qs-more-icon-on-an-object.png"> next to the name of the project in the header, then click <span class="bold">Edit</span>. </p> </li> 
 <li value="3"> <p>In the <span class="bold">Finance</span> section, enable the <span class="bold">Allow company-level billing rates to override project-level billing rates</span>.</p> <p class="warning" data-mc-autonum="<b>Warning: </b>"><span class="autonumber"><span><b>Warning: </b></span></span>Enabling this option overrides historical revenue calculations unless they are marked as billed. You can preserve the historical revenue calculations by creating a billing record. For more information, see the article <a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">Create billing records</a></p> </li> 
 <li value="4">Click <span class="bold">Save Changes</span>.</li> 
</ol>

## Update Company-level Billing Rates and apply them to a project

After you have enabled the company-level billing rates override option on a project, changes made to the company billing rates apply to the project any time the finances are recalculated.

>[!NOTE]
>
>Users must have access to Companies in their access level to update company-level billing rates.

<ol> 
 <li value="1"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span>. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span>. </p> </li> 
 <li value="2">Click <span class="bold">Companies</span>. </li> 
 <li value="3">Click the name of the company that is associated with the project for which you enabled company-level billing rates override.</li> 
 <li value="4"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Billing Rates</span> in the left panel.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Billing Rates</span> in the left panel.</p> </li> 
 <li value="5"> <p>Enter the new billing rate for an existing job role in the <span class="bold">Company Billing Rate</span> field, then press Enter. </p> </li> 
 <li value="6">To update company rates for one or more projects, do one of the following:<br>
  <ul>
   <li>Multiple projects:</li>
  </ul>
  <ol>
   <li value="1">Go to a list of projects. </li>
   <li value="2">Select the checkbox in line with the projects you want to update.</li>
   <li value="3">Click <span class="bold">Edit</span>.</li>
   <li value="4">In the Settings section, enable the <span class="bold">Recalculate Costs And Revenues</span> option. </li>
   <li value="5"><p>Click <span class="bold">Save Changes</span>.</p></li>
  </ol>
  <ul>
   <li>Single project: 
    <ol style="list-style-type: lower-alpha;">
     <li value="1">Go to the project for which you enabled company-level billing rates override.</li>
     <li value="2">
      <draft-comment>
       <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">More</span> menu <img src="assets/qs-more-icon-on-an-object.png"> next to the project name in the header, then click <span class="bold">Recalculate Finance</span>. </p>
      </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">More</span> menu <img src="assets/qs-more-icon-on-an-object.png"> next to the project name in the header, then click <span class="bold">Recalculate Finance</span>. </p></li>
    </ol></li>
  </ul></li> 
</ol>

