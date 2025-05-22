---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: View the Jira Activity Log
description: As a [!DNL Jira] administrator, you can view the exceptions and errors that occur during the synchronization or creation of the tickets between [!DNL Adobe Workfront] and [!DNL Jira] in an Activity Log.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
---
# View the [!UICONTROL [!DNL Jira] Activity Log]

As a [!DNL Jira] administrator, you can view the exceptions and errors that occur during the synchronization or creation of the tickets between [!DNL Adobe Workfront] and [!DNL Jira] in an [!UICONTROL Activity Log]. 

You can see up to 500 items in the Activity Log, and they are listed starting with the most recent ones.

## Access requirements

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL Adobe Workfront] plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] licenses overview</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>System administrator access</p> <p>Important:  We recommend that you create separate system administrator accounts in [!DNL Jira] and [!DNL Workfront] to dedicate to this integration, rather than using existing ones that might be attached to users.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a [!DNL Workfront] administrator. For information on [!DNL Workfront] administrators, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

## Prerequisites

Before you can link items between [!DNL Workfront] and [!DNL Jira], you must

* Install [!DNL Workfront for Jira]

   For instructions on installing [!DNL Workfront for Jira], see [Install [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Access the [!UICONTROL [!DNL Jira] Activity Log]: 

1. Log into Jira as a system administrator.
1. Click **[!UICONTROL Settings]** in the main [!DNL Jira] menu.
1. Click **[!UICONTROL Add-ons]**, then **[!UICONTROL Manage add-ons]**.

1. Expand the **[!DNL Workfront]** add-on.
1. Click **[!UICONTROL Configure]**.
1. Log in to [!DNL Workfront] as a system administrator.
1. Select the **[!UICONTROL Activity Log]** tab.

   View information about exceptions and errors that occurred during the creation of items or synchronization of fields between the two applications.

   The log includes the following fields:

   * Date of the occurrence
   * The name of the user in Jira
   * Jira issue number
   * A brief description of the error that occurred.
