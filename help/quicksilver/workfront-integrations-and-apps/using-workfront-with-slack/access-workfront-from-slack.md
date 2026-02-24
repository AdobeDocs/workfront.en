---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Access [!DNL Adobe Workfront] from [!DNL Slack]
description: Integrating [!DNL Adobe Workfront] with [!DNL Slack] allows you to access [!DNL Workfront] from Slack, or perform certain actions in [!DNL Workfront] using a slash command. The integration can be used from any [!DNL Slack] environment, including the [!DNL Slack] mobile app.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
---
# Access [!DNL Adobe Workfront] from [!DNL Slack]

Integrating [!DNL Adobe Workfront] with [!DNL Slack] allows you to access [!DNL Workfront] from [!DNL Slack], or perform certain actions in [!DNL Workfront] using a slash command. The integration can be used from any [!DNL Slack] environment, including the [!DNL Slack] mobile app.

You or your [!DNL Slack] administrator must install the [!DNL Workfront] app in your [!DNL Slack] instance before you can use [!DNL Workfront] from [!DNL Slack]. For more information, see [Configure Adobe Workfront for Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Any</p>
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## About slash commands {#about-slash-commands}

When using [!DNL Slack], you type messages inside of a message field. When you start your message with a slash, it becomes a command and it behaves differently than a simple message. The command tells [!DNL Slack] to perform an action.

You can access your [!DNL Workfront] instance from [!DNL Slack] by typing a slash command in any [!DNL Slack] channel.

Remember the following when using a slash command in [!DNL Slack] to access [!DNL Workfront]:

* Slash commands are case sensitive.
* The commands for [!DNL Workfront] are only visible to you, regardless of which channel you are typing them in.
* The command should always start with `/workfront` or `/wf`, followed by a space and the name of an action you want to perform in [!DNL Workfront].

   This indicates that your command is meant for the [!DNL Workfront] app. The commands for [!DNL Workfront] work only when you have already configured the [!DNL Workfront] app with your [!DNL Slack] instance.

For a list of all the commands you can run from Slack for [!DNL Workfront], see [Access [!DNL Workfront] from a slash command in [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## Log in to [!DNL Workfront] from [!DNL Slack] {#log-in-to-workfront-from-slack}

When you type any command in the message field in Slack, you will be asked to log in to [!DNL Workfront] first.\
For a complete list of [!DNL Workfront] commands from [!DNL Slack], see the [Access [!DNL Workfront] from a slash command in [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) section in this article. 

To log in to [!DNL Workfront] from [!DNL Slack]:

1. Log in to your [!DNL Slack] instance.
1. From any channel, type one of the following commands:\
   `/workfront log in`

   Or

   `/wf log in`

1. Click the [!DNL Workfront] **[!UICONTROL Log In]** link displayed in the response.\
   A new tab opens with fields for [!DNL Workfront] credentials.

1. Follow the prompts to log in to [!DNL Workfront] using Enhanced Authentication, OAuth 2.0, or your Security Assertion Markup Language (SAML) URL.

   >[!NOTE]
   >
   >* When you are prompted to enter the host of your [!DNL Workfront] account, type it using this format: *yourCompany'sDomain.my.workfront.com*. Your company's domain is usually the name of your company.
   >* Enhanced Authentication is not available until a [!DNL Workfront] administrator enables it for this integration.


   The configuration page for [!DNL Workfront] notifications in [!DNL Slack] opens.

1. (Optional) Disable any [!DNL Workfront] notifications that you do not want to receive in [!DNL Slack].

   For information about configuring [!DNL Workfront] settings for [!DNL Slack], see the [Configure settings](#configure-settings-configure-settings) section in this article

1. Navigate back to your [!DNL Slack] channel.

   You are logged in to [!DNL Workfront] from your [!DNL Slack] instance. 

## Access [!DNL Workfront] from [!DNL Slack]

* [About slash commands](#about-slash-commands-about-slash-commands)
* [Access [!DNL Workfront] from a shared link in [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## Access [!DNL Workfront] from a slash command in [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. Log in to your [!DNL Slack] instance and log in to [!DNL Workfront] from [!DNL Slack].\
   For more information about logging in to [!DNL Workfront] from [!DNL Slack], see [Log in to [!DNL Workfront] from [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. From any channel, start typing the following command in the message field: 

   `/workfront help`

   Or

   `/wf help`

1. Select from the following commands: 

   * `/wf home`

      Displays buttons from which you can access lists of your tasks, issues, and approvals. Clicking one of the buttons displays the first 20 items of each list in [!DNL Slack].

      For more information about managing [!DNL Workfront] work items from [!DNL Slack], see [Manage your work and approvals from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf add task <TaskName>`

      Include the name of the task as it will appear in the [!DNL Workfront] interface.

      Adds a task to [!DNL Workfront].

      For more information about adding tasks to [!DNL Workfront] from Slack, see the "Creating Tasks from [!DNL Slack]" section in [Create tasks and issues from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf add issue <Issue Name>`

      Include the name of the issue as it will appear in the [!DNL Workfront] interface.

      Adds an issue to [!DNL Workfront]

      For more information about adding issues to [!DNL Workfront] from [!DNL Slack], see the "Creating Issues from [!DNL Slack]" section in [Create tasks and issues from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf favorites`

      Displays the list of your [!DNL Workfront] Favorites.

      For more information about accessing your Favorites from [!DNL Slack], see the [Accessing Your [!UICONTROL Favorites] List from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) section in the [Accessing Your Favorites and Recent Items from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) article.

   * `/wf recent`

      Displays the list of your most recently accessed items in [!DNL Workfront].

      For more information about accessing your Recent Items from [!DNL Slack], see the [Accessing Your [!UICONTROL Recent Items] List from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites] and [!UICONTROL recent items from [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) article.

   * `wf tasks`

      Displays a list of your tasks.

      For more information about managing your tasks from [!DNL Slack], see the "Managing Your Tasks from [!DNL Slack]" section in [Managing Your Work and Approvals from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

      Displays a list of your issues.

      For more information about managing your issues from [!DNL Slack], see the "Managing Your Issues from [!DNL Slack]" section in [Managing Your Work and Approvals from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` Displays your [!DNL Workfront] approvals.\

      For more information about managing your approvals from [!DNL Slack], see the "Managing Your Approvals from [!DNL Slack]" section in [Manage your work and approvals from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf search <keyword>`

      Include keyword.

      Search for a specific keyword. You can search for the following types objects:

      * Project
      * Task 
      * Issue
      * Report
      * People
      * Template
      * Document
      * Portfolio
      * Program
      * Dashboard
      * Company
      * Note  \

         For more information about searching in [!DNL Slack], see [Search for [!DNL Adobe Workfront] items from Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

      Logs you in to [!DNL Workfront] from [!DNL Slack]. 

   * `/wf log out`

      Logs you out of [!DNL Workfront] from [!DNL Slack]. You remain logged in to [!DNL Workfront] if you have a separate [!DNL Workfront] instance open in another browser tab on in another application. 
   * `/wf settings`

      Gives you access to configuring your [!DNL Workfront] settings in [!DNL Slack].

      For information about configuring [!DNL Workfront] settings in Slack, see [Configure settings](#configure-settings-configure-settings).

   * `/wf help`
Displays a complete list of commands for [!DNL Workfront]. 


   * `Visit Workfront Help`: Opens the [!UICONTROL Slack] section on the [!DNL Workfront] Help Site in a new browser tab. 


1. (Optional) To delete the message of any command, mouse over the upper-right corner of the Slack message containing the command and click&#x200B;**[!UICONTROL Show message actions]**, then click **[!UICONTROL Delete message]**.

1. (Optional and conditional) Click **[!UICONTROL Delete]** to confirm you want to delete this message. 

### Access [!DNL Workfront] from a shared link in [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

You can access [!DNL Workfront] objects from a link to those objects that is shared with you in [!DNL Slack]. 

For more information about accessing [!DNL Workfront] from a shared link, see [Access [!DNL Adobe Workfront] objects from a shared link in [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## Configure settings {#configure-settings}

1. Inside a [!DNL Slack] message field, type the following command:

   `/workfront settings`

   Or

   `/wf settings`

   All settings are enabled by default.

1. Deselect from the following options, to disable your settings for Workfront:

   * In the **[!UICONTROL General Settings]** area, disable the **[!UICONTROL When pasting a [!DNL Workfront] URL in a [!DNL Slack] channel, show additional description, due date, or requestor name]**&#x200B;setting if you do not want [!DNL Slack] to add additional information about your [!DNL Workfront] objects when you share a URL to the object in [!UICONTROL Slack].

   * In the **[!UICONTROL Notifications Settings]** area, disable notifications that you want to stop receiving from Workfront.\

      For information about receiving [!DNL Workfront] notifications in [!DNL Slack], see [Receive [!DNL Adobe Workfront] notifications in [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Log out of [!DNL Workfront] from [!DNL Slack]

1. Inside a [!DNL Slack] message field, type the following command:\
   `/workfront log out` Or\
   `/wf log out`\
   You receive a confirmation that you have been logged out of [!DNL Workfront].\
   You remain logged in to [!DNL Workfront] if you have a separate [!DNL Workfront] instance open in another browser tab on in another application. 
