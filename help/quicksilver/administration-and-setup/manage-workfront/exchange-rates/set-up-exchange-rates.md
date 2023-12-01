---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Set up exchange rates
description: As an Adobe Workfront administrator, you can set up currency exchange rates in Workfront.
feature: System Setup and Administration
role: Admin
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
---
# Set up exchange rates

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

As an Adobe Workfront administrator, you can set up currency exchange rates in Workfront. This includes the following:

* Setting the default currency for the Workfront system
* Updating exchange rates in Workfront to match current exchange rates
* Configuring the exchange rates for multiple currencies (doing so enables users to choose a default currency for individual projects)

Exchange rates impact all financial elements in Workfront. The Base Currency is the default currency for all projects throughout the system, unless it is overridden for a given project or job role. You can also select to display financial information in currencies available in your system that are different than the base currency or that of the project when viewing them in a report or list. For more information, see [Create financial data reports with unique exchange rates](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

For more information about overriding the Base Currency in Workfront for projects and job roles, see the following articles:

* [Change the project currency](../../../manage-work/projects/project-finances/change-project-currency.md) 
* [Create and manage job roles](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

The way that you set up exchange rates affects whether users can modify exchange rates for a given project.

>[!IMPORTANT]
>
>Exchange rates in Workfront are not dynamic; the value that you set must be updated when changes in exchange rates occur. 

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Set up exchange rates

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).  

1. Click **Project Preferences** > **Exchange Rates.** 

1. Click **Add Currency.**
1. Begin typing the name of the currency, then click it when it appears in the drop-down list.  

1. In the provided field, specify the rate for the currency that you selected, as it relates to the currency that is set as the base currency in the system.
1. (Optional) Set the currency as the base (default) currency for Workfront.

   This is the currency that is used as the default for all projects and reports throughout the system.

1. Click **Save** to save your changes. 

## Enable users to modify the default currency for a project

Users can modify the default currency for a project when the following conditions are met:

* The user has a Plan license with the administrative access to Exchange Rates.

  For more information, see [Grant users administrative access to certain areas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* More than one currency is enabled on the Workfront system.

For information about how users can change the default currency on a given project, see [Change the project currency](../../../manage-work/projects/project-finances/change-project-currency.md).

## Enable users to modify the default currency for a job role

Users can modify the currency for a job role when the following conditions are met:

* The user has a Plan license with administrative access to Job Roles.

  For more information, see [Grant users administrative access to certain areas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* More than one currency is enabled in the Workfront system.

For information about how users can change the default currency on a given job role, see [Create and manage job roles](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
