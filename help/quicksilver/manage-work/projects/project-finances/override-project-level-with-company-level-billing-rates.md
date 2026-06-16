---
product-area: projects
navigation-topic: financials
title: Override Project-Level Billing Rates with Company-Level Billing Rates
description: Override Project-Level Billing Rates with Company-Level Billing Rates
author: Lisa
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
TQID: https://experienceleague.adobe.com/GQSQGGHBZsBLtI8IEUltVXzxmEtOxue0iE6fpHmYWP4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Override Project-Level Billing Rates with Company-Level Billing Rates

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

You can configure a project to use company-level billing rates instead of project-level billing rates.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>Edit access to Projects and Financial Data</td> 
  </tr> 
  <tr> 
   <td>Object permissions</td> 
   <td>Manage permissions to the project with permissions to Edit Billing Rates and General Finance</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Enable the Company-level Billing Rates override option

When a company is associated with a project and this option is enabled, changes made to the company-level billing rates override the billing rate set on the project.

When a user manually recalculates finances on the project, any changes to the company-level billing rates are applied. Historical revenue calculations are also overridden unless they are marked as billed.

1. Go to a project. 
1. Click the **More** menu ![More menu](assets/qs-more-icon-on-an-object.png) next to the name of the project in the header, then click **Edit**. 
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

{{step-1-to-setup}}

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
     1. Click the **More** menu ![More menu](assets/qs-more-icon-on-an-object.png) next to the project name in the header, then click **Recalculate Finance**.
