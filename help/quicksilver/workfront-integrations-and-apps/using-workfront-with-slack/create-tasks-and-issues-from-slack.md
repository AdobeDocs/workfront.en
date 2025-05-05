---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Create tasks and issues from Slack
description: After you have installed and configured [!DNL Adobe Workfront] for Slack, you can create tasks and issues from Slack and associate them with projects in Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
---
# Create tasks and issues from [!DNL Slack]

After you have installed and configured [!DNL Adobe Workfront for Slack], you can create tasks and issues from [!DNL Slack] and associate them with projects in [!DNL Workfront].

For more information about configuring [!DNL Workfront] with [!DNL Slack], see [Configure [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md). 

You must have access to create tasks and issues in your Access Level and you must have [!UICONTROL Contribute] permissions on the project that you are associating them with. 

For more information about Access Levels, see [Access levels overview](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md). For more information about permissions to objects, see [Overview of sharing permissions on objects](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Access requirements

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.\

## Prerequisites

Before you can create tasks and issues from [!DNL Slack], you must

* Configure [!DNL Workfront] for Slack\
   For instructions on configuring [!DNL Workfront for Slack], see [Configure [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Create tasks from [!DNL Slack]

1. Log in to your [!DNL Slack] instance and log in to [!DNL Workfront] from [!DNL Slack].\
   For more information about logging in to Workfront from [!DNL Slack], see the "Logging In to [!DNL Workfront] from [!DNL Slack]" section in [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. From any channel, start typing the following command in the message field:

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >Commands are case sensitive. You can start your command with `/wf` instead of `/workfront`.
   >  
   >The Task Name must be entered as it will appear in the [!DNL Workfront] interface, without brackets or quotation marks.                               

1. (Optional) Start typing the name of a project with which you want to associate the new task and select it when it appears in the list.\
   You receive a confirmation indicating that the task was added to the selected project.
1. (Optional) Click the name of the task in the confirmation message to open it in [!DNL Workfront], in a new browser tab.

## Create issues from [!DNL Slack]

1. Log in to your [!DNL Slack] instance and log in to [!DNL Workfront] from [!DNL Slack].\
   For more information about logging in to [!DNL Workfront] from [!DNL Slack], see the "Logging In to [!DNL Workfront] from [!DNL Slack]" section in [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. From any channel, start typing the following command in the message field: 

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >Commands are case sensitive. You can start your command with '/wf' instead of '/workfront.' \
   >The Issue Name must be entered as it will appear in the [!DNL Workfront] interface, without brackets or quotation marks.

1. (Optional) Start typing the name of a project with which you want to associate the new issue and select it when it appears in the list.\
   You receive a confirmation indicating that the issue was added to the selected project. 
1. (Optional) Click the name of the issue in the confirmation message to open it in [!DNL Workfront], in a new browser tab.
