---
product-area: projects
navigation-topic: financials
title: Override Project-Level Billing Rates with Company-Level Billing Rates
description: Override Project-Level Billing Rates with Company-Level Billing Rates
author: Alina
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
---
# Override Project-Level Billing Rates with Company-Level Billing Rates

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

You can configure a project to use company-level billing rates instead of project-level billing rates.

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Financial&nbsp;Data</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project with permissions to Manage Finance</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Enable the Company-level Billing Rates override option

When a company is associated with a project and this option is enabled, changes made to the company-level billing rates override the billing rate set on the project.

When a user manually recalculates finances on the project, any changes to the company-level billing rates are applied. Historical revenue calculations are also overridden unless they are marked as billed.

1. Go to a project. 
1. Click the **More** menu ![](assets/qs-more-icon-on-an-object.png) next to the name of the project in the header, then click **Edit**. 
1. In the **Finance** section, enable the **Allow company-level billing rates to override project-level billing rates**.

   >[!CAUTION]
   >
   >Enabling this option overrides historical revenue calculations unless they are marked as billed. You can preserve the historical revenue calculations by creating a billing record. For more information, see the article [Create billing records](../../../manage-work/projects/project-finances/create-billing-records.md)

1. Click **Save Changes**.

## Update Company-level Billing Rates and apply them to a project

After you have enabled the company-level billing rates override option on a project, changes made to the company billing rates apply to the project any time the finances are recalculated.

>[!NOTE]
>
>Users must have access to Companies in their access level to update company-level billing rates.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup**. 
1. Click **Companies**. 
1. Click the name of the company that is associated with the project for which you enabled company-level billing rates override.
1. Click **Billing Rates** in the left panel.
1. Update the **Company Billing Rate** and start/end dates for an existing job role, then press Enter.

   To add a new date effective company billing rate, select a billing rate for the job role and click **Edit**. For more information on date effective company billing rates, see [Override job role billing rates at the company level](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

1. To update company rates for one or more projects, do one of the following:

   * Multiple projects:

     1. Go to a list of projects. 
     1. Select the checkbox in line with the projects you want to update.
     1. Click **Edit**.
     1. In the Settings section, enable the **Recalculate Costs And Revenues** option. 
     1. Click **Save Changes**.

   * Single project:

     1. Go to the project for which you enabled company-level billing rates override.
     1. Click the **More** menu ![](assets/qs-more-icon-on-an-object.png) next to the project name in the header, then click **Recalculate Finance**.
