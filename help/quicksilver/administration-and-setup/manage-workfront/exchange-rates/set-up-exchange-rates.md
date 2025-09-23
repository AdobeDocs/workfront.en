---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Set Up Exchange Rates
description: Exchange rates impact all financial elements in Workfront. The base currency is the default currency for all projects throughout the system.
feature: System Setup and Administration
role: Admin
author: Lisa
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

Exchange rates impact all financial elements in Workfront. The base currency is the default currency for all projects throughout the system, unless it is overridden for a given project or job role. The current base or default currency is indicated with an icon ![Default currency icon](assets/default-icon.png) in the list. You can also select to display financial information in currencies available in your system that are different than the base currency or that of the project when viewing them in a report or list. For more information, see [Create financial data reports with unique exchange rates](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

For more information about overriding the base currency in Workfront for projects and job roles, see the following articles:

* [Change the project currency](../../../manage-work/projects/project-finances/change-project-currency.md) 
* [Create and manage job roles](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

The way that you set up exchange rates affects whether users can modify exchange rates for a given project.

>[!IMPORTANT]
>
>Exchange rates in Workfront are not dynamic; the value that you set must be updated when changes in exchange rates occur.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

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
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>New: Standard</p>
       <p>Or</p>
       <p>Current: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Set up exchange rates

{{step-1-to-setup}}

1. Click **Project Preferences** > **Exchange Rates**.

1. Click **Add currency**.
1. In the **Add currency** box, begin typing the name of the currency, then click it when it appears in the drop-down list.
1. In the **Exchange rate** field, enter the rate for the currency that you selected, compared to the currency that is set as the base currency in the system.
1. Click **Add** to add the new currency and its exchange rate.
1. (Optional) To change the base (default) currency, do one of the following:

   * Select the check box next to the currency name and select **Make Default** in the action bar at the bottom of the screen.
   * Hover over the currency name and click the **More** menu that appears. Then, select **Make Default**.

     The new default currency is updated with the icon.

     >[!NOTE]
     >
     >The default currency always appears first in the list, regardless of how the list is sorted.

1. (Optional) To delete a currency, select the check box next to the currency name and select **Delete** in the action bar at the bottom of the screen. You cannot delete the default currency.

## Enable users to modify the default currency for a project

Users can modify the default currency for a project when the following conditions are met:

* The user has a Standard or Plan license with the administrative access to Exchange Rates.

  For more information, see [Grant users administrative access to certain areas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* More than one currency is enabled on the Workfront system.

For information about how users can change the default currency on a given project, see [Change the project currency](../../../manage-work/projects/project-finances/change-project-currency.md).

## Enable users to modify the default currency for a job role

Users can modify the currency for a job role when the following conditions are met:

* The user has a Standard or Plan license with administrative access to Job Roles.

  For more information, see [Grant users administrative access to certain areas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* More than one currency is enabled in the Workfront system.

For information about how users can change the default currency on a given job role, see [Create and manage job roles](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).


   <!--The default currency is the currency that is used as the default for all projects and reports throughout the system. The current default is indicated with an icon ![Default currency icon](assets/default-icon.png).-->
