---
product-area: projects
navigation-topic: financials
title: Manage information in the project Finance area
description: Manage information in the project Finance area
author: Alina
feature: Work Management
exl-id: 147f5d55-a827-4cca-9ab0-afb03a4bcd5a
---
# Manage information in the project Finance area

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

You can view or edit the financial information of a project by accessing the Finance area of the Project Details section. There is a limited number of fields that you can view or edit in this area. For information about editing all information for a project see [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects and Financial Data</p> <p>Edit access to Projects and Financial Data to edit financial information on the project</p> <p><b>NOTE</b></p>
   <p> If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a project or higher that include View Finance permissions</p> <p>Manage permissions to the project that include Manage Finance to edit financial information for the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Overview of the Finance area

Consider the following when viewing or editing information in the Finance area:

* The financial information you can find on the Finance area of Project Detailsrepresents values that roll up to the project level from tasks, as well as information entered directly on the project. Some financial information can be managed at the project as well as the task level. 
* You must have View permissions on the project as well as access to Financial Data from your access level in order to be able to view the Finance area on a project. 
* You must have Manage permissions on the project as well as access to Financial Data from your access level in order to be able to edit the information on the Finance area . However, we recommend that only the Project Owner should edit the information on this area .

## View Finance information on a project

1. Go to a project.
1. Click **Project Details** in the left panel.
1. Click the **Edit** icon ![](assets/edit-icon.png) in the upper-right corner of the Details section, then click **Finance**.

   ![](assets/finance-area-in-details-view-only-nwe-350x188.png)

   >[!NOTE]
   >
   >Depending on how your Workfront administrator configured your Layout Template, the Overview section might not be listed first, in which case it is collapsed. For information, see [Customize the Details view using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. View the following fields in the Finance area of the project:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Performance Index Method</td> 
      <td> Controls the method Workfront uses to calculate Earned Value metrics. It can be hours-based, or cost-based. <br>For more information about the PIM, see the article <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Set the Performance Index Method (PIM)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">CPI/SPI/CSI</td> 
      <td> <p>These are project performance metrics that show how your project is performing, at a given time. Their values are calculated based on the Performance Index Method.<br>For more information see the following articles: </p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Calculate Cost Performance Index (CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Calculate Schedule Performance Index (SPI) </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Calculate Cost Schedule Performance Index (CSI)</a> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estimate at Completion</td> 
      <td> Projected total cost of your project, represented in hours if the Performance Index Method (PIM) is hours-based, and it is represented in a currency value, if the Performance Index Method (PIM) is cost-based.<br>For more information about calculating the Estimate at Completion, see the article <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Calculate Estimate At Completion (EAC)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Budget</td> 
      <td>This is the budget set for the project. This is manually specified by the Project Owner.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fixed Cost</td> 
      <td>These are the fixed costs on the project, independent of other activities on the project. They are manually entered by the Project Owner.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planned Cost</td> 
      <td>The estimated cost of the project, based on Planned Hours and the rates associated with the task assignees (job roles or users).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Actual Cost</td> 
      <td>All of the costs accruing on the project. Actual Cost is the sum of all actual costs: labor cost (based on Actual Hours and the rates associated with the job roles or users logging them), expenses, and fixed costs, which can be associated with a project or task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fixed Revenue</td> 
      <td>Set income expected based on the project schedule. Fixed Revenue is manually specified by the Project Owner.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planned Revenue</td> 
      <td>Projected income expected based on the Planned Hours and the rates associated with the task assignees (job roles or users).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Actual Revenue</td> 
      <td>Actual income from the project based on the Actual Hours and the rates associated with the task assignees (job roles or users).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Billed Revenue</td> 
      <td> <p>Revenue billed to clients or other parties which is captured in Billing Records. For more information about billing records, see the article <a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">Create billing records</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">&nbsp;</td> 
      <td>&nbsp;</td> 
     </tr> 
     <tr> 
      <td role="rowheader">&nbsp;</td> 
      <td>&nbsp;</td> 
     </tr> 
    </tbody> 
   </table>

## Edit financial information on a project

As a Project Owner, you can edit the information on the Finance subtab of a project.

To edit information on the Project Finance subtab:

1. Go to a project which you are the owner of.

   >[!NOTE]
   >
   >You need Manage permissions to the project to perform the following steps. We also recommend that only the Project Owner should make changes to the Finance subtab of the project.

1. Click **Project Details** in the left panel.
1. Click the **Edit** icon ![](assets/edit-icon.png) in the upper-right corner of the Details section, then click&nbsp;**Finance** . This opens the Finance area for editing.
1. Edit any field that is available for editing, by single-clicking the field or click **+Add** to add information to an empty field.

   >[!TIP]
   >
   >Fields are not available for editing if they are automatically calculated by Workfront or if you don't have editing permissions on them.

   ![](assets/edit-finance-area-in-project-details-nwe-350x275.png)

1. Update any of the fields below.

   >[!NOTE]
   >
   >Depending on how your Workfront administrator sets up our Layout Template, the fields in the Project&nbsp;Details section might be different in your environment. For information, see [Customize the Details view using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Performance Index Method</td> 
      <td> <p>Controls the method Workfront uses to calculate project performance metrics. This is set up at the system level by your administrator, but you can also edit it at the project level. Consider selecting one of the following options:</p> 
       <ul> 
        <li><strong>Hour-Based:</strong>Workfront uses the Planned Hours in calculating the CPI and EAC of the project, and the EAC of the project displays as a number, in hours. </li> 
        <li><strong>Cost-Based:</strong>Workfront uses the Planned Labor Cost in calculating the CPI and EAC of the project, and the EAC displays as a currency value. When you select this option, ensure that your task assignees (job roles or users) are associated with cost rates.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estimate at Completion</td> 
      <td> <p>Represents the projected total cost of your project or task when it completes. This is set up at the system level by your administrator, but you can also edit it at the project level. Consider selecting one of the following options:</p> 
       <ul> 
        <li><strong>Calculate at Project Level</strong>: EAC for the parent task and project are determined by entering the actual hours/ actual labor cost into the EAC Formulas. This calculation includes Actual Hours/ costs and expenses added directly to the parent task or project.</li> 
        <li><strong>Roll up from Tasks/ Subtasks</strong>: EAC for the parent task and project are determined by summing up the EAC for each child task. This calculation excludes Actual Hours/ costs and expenses added directly to the parent task or project.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Budget</td> 
      <td>Specify the budget for this project.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fixed Cost</td> 
      <td>Specify the fixed cost for this project. This should not include any labor or expense costs.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fixed Revenue</td> 
      <td> <p>Specify the fixed revenue of this project. This should not include revenue coming from any billing records billed to partners or third parties.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Project Currency</td> 
      <td> <p>Specify a currency for this project, if it is different from the default currency in your system. The default currency in your system is defined by your Workfront administrator. For more information about setting up exchange rates in Workfront, see the article <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p> </td> 
     </tr>
    </tbody> 
   </table>

1. Click **Save Changes**.
