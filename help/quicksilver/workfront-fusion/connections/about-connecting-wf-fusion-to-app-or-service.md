---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Connections overview
description: For most apps, it is necessary to create a connection, through which [!DNL Adobe Workfront Fusion] can communicate with the given third-party service according to the settings of the specific scenario.
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
---
# Connections overview

<!-- Audited: 3/2024-->

For most apps, [!DNL Workfront Fusion] requires a connection, through which it can communicate with the given third-party service according to the settings of the specific scenario.

For example, if you want to create a scenario that retrieves information from [!DNL Workfront], you must grant access permission for [!DNL Workfront Fusion] to access your [!DNL Workfront] account.

A connection represents the authorization and permissions that Fusion uses to access the application. You can create one or more connections for each application, and can use the same connection in multiple modules or scenarios. 

Most connections are used only for a single application. For example, a [!DNL Workfront] connection cannot be used in a [!UICONTROL Salesforce] module. Some [!DNL Adobe] applications can share connections. For details, see the articles for those applications, listed in [Apps and their modules](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md). 

Connections are managed on the team level. All members of a team have access to the team's connections, and users outside of a team do not have access to the team's connections.

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>New: [!UICONTROL Standard]</p><p>Or</p><p>Current: [!UICONTROL Work] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy: Any </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>New:</p> <ul><li>[!UICONTROL Select] or [!UICONTROL Prime] [!DNL Workfront] Plan: Your organization must purchase [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] is included.</li></ul>
   <p>Or</p>
   <p>Current: Your organization must purchase [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Access rights

For every connection, [!DNL Workfront Fusion] requires only those access rights that are necessary to successfully complete a given scenario. For example, if you create a scenario to list documents from [!DNL Google Docs], [!DNL Workfront Fusion] does not ask for permission to get the content of the documents. Later, if you find that you need to access the content of the documents, you can update the connection or create a new one that can access that content.

Not all services allow you to limit access to specific tasks. In these cases, [!DNL Workfront Fusion] must require full access rights. For more information on how to restrict [!DNL Workfront Fusion] access to your account registered to those services, see the application-specific documentationlisted in [Apps and their modules](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

## Manage connections

You can manage all connections from the [!UICONTROL Connections] area. 

>[!NOTE]
>
>Connections are owned by teams. If you cannot find the connection you are looking for, check that you are viewing the correct team.
>
>To select a new team:
>
>* Click the team name in the left navigation and select a new team.
>
>    Or
>
>* Click Team overview in the left navigation, then click the dropdown arrow next to the team name near the top of the page. Select a new team.

1. To open the [!UICONTROL Connections] area, click <b>[!UICONTROL Connections]</b> in the left navigation.
1. (Optional) Indicate the environment and type of connection by clicking the Environment and Type dropdown and selecting an option.
1. (Optional) To view which permissions were given to [!DNL Workfront Fusion] for a connection, click the View icon ![View connection permissions](assets/view-connection-permissions.png) for that connection.
1. (Optional) To rename a connection, highlight the connection name and type the new name.
1. (Optional) To reauthorize a connection, click **Reauthorize** for that connection.
1. (Optional) To delete a connection, click **Delete** for that connection.
1. (Optional) To verify that the connection to the service was established successfully, click **Verify** for the connection.



## Renew a connection

[!DNL Workfront Fusion] usually obtains access rights to a given service for an unlimited period of time. Some applications require the access permission to be renewed after a certain period of time. In these cases, [!DNL Workfront Fusion] notifies you via email shortly before its access rights expire.

To renew a connection:

1. Click the **[!UICONTROL Reauthorize]** button in the **[!UICONTROL Connections]** area.
