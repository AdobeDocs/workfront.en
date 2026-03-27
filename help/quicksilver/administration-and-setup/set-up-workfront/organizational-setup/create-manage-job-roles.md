---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Create and Manage Job Roles
description: As an [!DNL Adobe Workfront] administrator or a user with administrative access to Job Roles, you can create job roles which can be assigned to users and delete default job roles that are not relevant to your organization.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
---
# Create and manage job roles

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

{{highlighted-preview}}

>[!IMPORTANT]
>
>With the 25.11 release, the Override Currency for job roles was deprecated in Production. (The deprecation took place on October 30 in the Preview environment.) Instead of having a base currency and override currencies, one currency is now available for job roles, and the cost and billing rates are defined using that currency.

As an [!DNL Adobe Workfront] administrator or a user with administrative access to Job Roles, you can create job roles that can be assigned to users and delete default job roles that are not relevant to your organization. For information about administrative access in [!DNL Workfront], see [Grant users administrative access to certain areas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!TIP]
>
>Job roles are an integral part of managing resources. To use the resource planning tools, job roles need a cost and billing rate associated with them. For information, see [Get started with Resource Management](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>To create or edit a job role: Any Workfront or Workflow package</p>
   <p>To apply rate attributes and add custom forms to the job role: Workflow Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>Administrative access to Job Roles</td>
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Create a job role

To create a job role:

{{step-1-to-setup}}

1. In the left panel, click **[!UICONTROL Job Roles]**.
1. Click **[!UICONTROL New Job Role]**.
<!-- 1. Click **New Job Role > Create new job role**.  -->
1. Enter information in the following fields:

   * **Name**: Indicate a name for the job role. This is the name that displays everywhere in Workfront where the Job Role field displays.

      >[!TIP]
      >
      >The name of a job role may contain up to 255 characters. However, longer names might be truncated in certain areas of Workfront.

   * **Description**: Enter a description for the role that indicates what is unique about it.
   * **Is Active**: Select **Yes** if you want the role to be active and available everywhere in Workfront to be associated with users, work items, etc. Select **No** if you want the role to be deactivated and not available to assign to users, work items, etc.

      For information about deactivating job roles, see [Deactivate job roles](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

   * **Currency**: The Base Currency is shown by default. The Workfront administrator adds the Base Currency in the Setup area. You can change the selection to another available currency, and you can change the currency on effective dated time ranges.

      >[!TIP]
      >
      >Only currencies available in the Exchange Rates area in your system are available in this field. If you only have one currency set up, only that currency is available.

      For information about setting up the Base Currency in Workfront, see [Set up exchange rates](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

      For information about changing the currency of a project, see [Change the project currency](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).
   
   * **Cost Rate**: This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the selected currency.

      For date effective cost rates, click **Add Rate**. Enter the value of the cost/hour for the time period, and assign a Start Date and End Date as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.

      Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, 2025, an end date of April 30, 2025 is added to the first cost rate so that no gaps exist.

      For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

      >[!TIP]
      >
      >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

   * **Billing Rate**: This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the selected currency.

      For date effective billing rates, click **Add Rate**. Enter the value of the billing/hour for the time period, and assign a Start Date and End Date as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.

      Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, 2025, an end date of April 30, 2025 is added to the first billing rate so that no gaps exist.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

      >[!TIP]
      >
      >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

<!-- Remove or hide the billing rate and cost rate bullets on April 16 for GA -->

1. Click **[!UICONTROL Create Job Role]**. The job role is now available to be assigned to tasks, issues, approvals, or you can share layout templates or other objects with it. For information about all uses of job roles in [!DNL Workfront], see [Job role overview](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). For information about deleting a job role, see [Delete job roles](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

<div class="preview">

## Add rates and attributes to a job role

Billing and cost rates on a job role are used in financial calculations.

Rate attributes are supported in areas of Workfront where rates exist, such as job roles and users. When attributes are applied on a job role, their assignments resolve automatically to the correct rates.

For more information, see [Define rate attributes](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

{{step-1-to-setup}}

1. In the left panel, click **[!UICONTROL Job Roles]**.
1. Click the name of an existing job role to edit it.
1. To update the job role details, click **Details** in the left panel.
1. (Optional) To attach a custom form to the job role, click the **Add custom form** field in the upper-right corner of the Details page, and select a custom form from the list that displays.

   For more information on attaching a custom form, see [Add a custom form to an object](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Click [!UICONTROL **Rates**] in the left panel.
1. Click [!UICONTROL **Billing**] or [!UICONTROL **Cost**] to select the rate type.
1. Click [!UICONTROL **Add Rates**] to add a new rate.

   Or

   Select an existing rate and click the **Edit** icon ![Edit icon](assets/edit-icon.png) to update it.

   >[!NOTE]
   >
   >Because each rate is associated with the combination of the role and attributes to create a unique rate, the attributes cannot be changed when you edit a rate.

1. On the **New Rate** box, select attributes for the rate such as Agency, Location, or Cost Center.

   >[!NOTE]
   >
   >These attributes are defined separately and may affect revenue and cost calculations. For more information, see [Define rate attributes](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

1. Select the **Currency** for the rate. The Workfront administrator adds the Base Currency in the Setup area. You can change the selection to another available currency, and you can change the currency on effective dated time ranges.

   >[!TIP]
   >
   >Only currencies available in the Exchange Rates area in your system are available in this field. If you only have one currency set up, only that currency is available.

   For information about setting up the Base Currency in Workfront, see [Set up exchange rates](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

   For information about changing the currency of a project, see [Change the project currency](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).

1. (Conditional) For a billing rate, enter the **Billing Rate** for this job role.

   This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the selected currency.

   If you use attributes, the attributes and the job role combine to define a unique rate. For example, a Designer role in New York for Agency A can have a separate rate from a Designer role in Paris for Agency B.

   For date effective billing rates, click **Add Rate**. Enter the value of the billing/hour for the time period, and assign a Start Date and End Date as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.

   Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, an end date of April 30 is added to the first billing rate so that no gaps exist.

   For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

   >[!TIP]
   >
   >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

1. (Conditional) For a cost rate, enter the **Cost Rate** for this job role.

   This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the selected currency.

   If you use attributes, the attributes and the job role combine to define a unique rate. For example, a Designer role in New York for Agency A can have a separate rate from a Designer role in Paris for Agency B.

   For date effective cost rates, click **Add Rate**. Enter the value of the cost/hour for the time period, and assign a Start Date and End Date as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.

   Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, an end date of April 30 is added to the first cost rate so that no gaps exist.

   For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

   >[!TIP]
   >
   >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

1. Click [!UICONTROL **Save**].

</div>

<!--
   * **Override Currency Cost Rate**: This is the cost per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role.

     Enter the rate in the Override Currency specified above. This also updates the Cost Rate for this job role when using the Base Currency.

     For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a cost rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Cost Rate, the cost rate of the job role also updates automatically.

   * **Override Currency Billing Rate**: This is the billing per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role.

      Enter the rate in the Override Currency specified above. This also updates the Billing Rate for this job role when using the Base Currency.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a billing rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the billing rate of the job role also updates automatically.

-->   



