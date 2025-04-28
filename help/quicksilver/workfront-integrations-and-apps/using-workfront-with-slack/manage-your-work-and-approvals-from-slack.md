---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Manage your work and approvals from Slack
description: You can access your Home Work List, review and agree to work on tasks and issues, and review or make decisions on approvals directly from Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 802a2f16-d827-455e-9e49-f58f4c5fc482
---
# Manage your work and approvals from [!DNL Slack]

After you have installed [!DNL Adobe Workfront for Slack], you can do the following:

* Access lists of your [!UICONTROL Home] items from [!DNL Slack]
* Review and accept to work on tasks and issues from [!DNL Slack]
* Review and make decisions on approvals from [!DNL Slack]

For more information about configuring [!DNL Workfront] with [!DNL Slack], see [Configure [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Access requirements

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL Adobe Workfront] plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

Before you can manage your work and approvals from [!DNL Slack], you must

* Configure [!DNL Workfront for Slack]  
  For instructions on configuring [!DNL Workfront for Slack], see [Configure [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Manage your work from [!DNL Slack]

1. Log in to your [!DNL Slack] instance and log in to [!DNL Workfront] from [!DNL Slack].  
   For more information about logging in to [!DNL Workfront] from [!DNL Slack], see the "Logging In to [!DNL Workfront] from [!DNL Slack]" section in [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. From any channel, start typing the following command in the message field: 

   `/workfront home`

   >[!NOTE]
   >
   >* Commands are case sensitive. 
   >* You can start your command with `/wf` instead of `/workfront`.

   The buttons from which you can access lists of your tasks, issues, and approvals display. Clicking one of the buttons displays the first 20 items of each list in [!DNL Slack].  

1. (Optional) Click **[!UICONTROL Tasks]** to display all your tasks.

   For more information about managing tasks in [!DNL Slack], see [Managing Your Tasks from [!DNL Slack]](#manage-your-tasks-from-slack-manage-your-tasks-from-slack).

1. (Optional) Click **[!UICONTROL Issues]** to display all your issues.

   For more information about managing issues in [!DNL Slack], see [Managing Your Issues from [!DNL Slack]](#manage-your-issues-from-slack-manage-your-issues-from-slack).

1. (Optional) Click **[!UICONTROL Approvals]** to display all the approvals waiting for your decision.  
   For more information about managing your approvals in [!DNL Slack], see [Manage your approvals from [!DNL Slack]](#manage-your-approvals-from-slack-manage-your-approvals-from-slack).

## Manage your tasks from [!DNL Slack] {#manage-your-tasks-from-slack}

1. Log in to your [!DNL Slack] instance and log in to [!DNL Workfront] from [!DNL Slack].  
   For information about logging in to [!DNL Workfront] from [!DNL Slack], see the "Logging In to [!DNL Workfront] from [!DNL Slack]" section in [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. From any channel, start typing either of the following commands in the message field:

   `/workfront home`, then click **[!UICONTROL Tasks]**

   Or

   `/workfront tasks`

   >[!NOTE]
   >
   >* Commands are case sensitive. 
   >* You can start your command with `/wf` instead of `/workfront`.

   The first 20 tasks on your list display.  

1. Click **[!UICONTROL +`<remaining number>` more]** to display additional tasks.
1. Consider reviewing the following information about your work items:

   * **[!UICONTROL Name]** 
   * **[!UICONTROL Project Name]** or **[!DNL Parent Object Name]**
   
   * **[!DNL Planned Completion Date]** of the work item.
   * **[!DNL Assigned By Name]**: this is the name of the user who assigned the task to you.
   * **[!UICONTROL Status]**

1. (Optional) Click the name of an item to open it in Workfront in a separate browser tab.
1. (Optional) In the **[!UICONTROL Status]** field, select a new Status.
1. (Optional) Click **[!UICONTROL Log Time]**, then select an **[!UICONTROL Hour Type]** and an hour amount to log time on the item.

   >[!NOTE]
   >
   >* You can only log hours in increments of a full or half hour, up to 12 hours and 30 minutes.
   >* The hours you log have an Entry Date of today. You cannot log time for a past or future date from [!DNL Slack].

   You receive a confirmation that the time has been logged.

1. (Optional) Click **[!UICONTROL Work on it]** to accept to work on a task. The [!UICONTROL Work on it] button disappears.

## Manage your issues from [!DNL Slack] {#manage-your-issues-from-slack}

1. Log in to your [!DNL Slack] instance and log in to [!DNL Workfront] from [!DNL Slack].  
   For more information about logging in to [!DNL Workfront] from [!DNL Slack], see the [Logging In to [!DNL Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront) section in [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. From any channel, start typing either of the following commands in the message field:   

   `/workfront home`, then click **[!UICONTROL Issues]** 

   Or

   `/workfront issues`

   >[!NOTE]
   >
   >* Commands are case sensitive. 
   >* You can start your command with `/wf` instead of `/workfront`.

   The first 20 issues in your list display.  

1. Click **[!UICONTROL + remaining `<number>` more]** to display additional items.
1. Consider reviewing the following information about your work items:

   * **[!UICONTROL Name]**
   * **[!UICONTROL Project]** Name or Parent Object Name
   * **[!UICONTROL Due on]** Date: This is the Planned Completion Date of the work item.
   * **[!DNL Requested by]** Name: This is the Primary Contact (for issues) or the user who made the assignment (for tasks). 

1. (Optional) Click the name of the issue to open it in Workfront in a separate browser tab.
1. (Optional) Click **[!DNL Work on it]** to start working on issues you have not accepted yet.

   The [!UICONTROL Work on it] button disappears.

## Manage your approvals from [!DNL Slack] {#manage-your-approvals-from-slack}

1. Log in to your [!DNL Slack] instance and log in to [!DNL Workfront] from [!DNL Slack].  
   For more information about logging in to [!DNL Workfront] from [!DNL Slack], see the "Logging In to [!DNL Workfront] from [!DNL Slack]" section in [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. From any channel, start typing either of the following commands in the message field:  

   `/workfront home`, then click **[!UICONTROL Approvals]**

   Or

   `/workfront approvals`

   >[!NOTE]
   >
   >* Commands are case sensitive. 
   >* You can start your command with `/wf` instead of `/workfront`.

   The first 20 items on your **[!UICONTROL Approvals]** list display. Additional information about the items also displays, like the name of the user who requested it or the name of the project the item belongs to. 

1. Click **[!UICONTROL + remaining `<number>` more]** to display additional items.
 
1. Consider managing approvals for the following objects: 

   * **Projects** 

     Click **[!UICONTROL Approve]** or **[!UICONTROL Reject]** to accept or reject the status change of a project.
   
   * **Tasks** 

     Click **[!UICONTROL Approve]** or **[!UICONTROL Reject]** to accept or reject the status change of a task.
   
   * **Issues** 

     Click **[!UICONTROL Approve]** or **[!DNL Reject]** to accept or reject the status change of an issue.
   
   * **Documents** 

     Click **[!UICONTROL Approve]** to approve a document, **[!UICONTROL Reject]** to reject it, or **[!UICONTROL Changes]** to indicate that you approve it, but that the document needs additional changes.  
     (Optional) Mouse over the document thumbnail to click the magnifying glass and preview the document. 
   
   * **Proofs**&#x200B;Click the proof name to open it in [!DNL Workfront] in a separate tab and manage the approval. 
   * **Access Requests** 

     Click **[!UICONTROL Grant Access]** to give enhanced permissions to the requested object, or **[!UICONTROL Ignore]** to ignore the request for more access.

1. (Optional) Click the name of the object submitted for approval to open it in [!DNL Workfront] in a new browser tab. 
