---
filename: access-favorites-and-recent-items-from-slack
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Access your favorites and recent items from Slack
description: After you have installed and configured Adobe Workfront for Slack, you can view your Workfront Favorites and Recent Items and access items from either list from Slack.
---

# Access your favorites and recent items from Slack

After you have installed and configured Adobe Workfront for Slack, you can view your Workfront Favorites and Recent Items and access items from either list from Slack.

For more information about configuring Workfront with Slack, see [Configure Adobe Workfront for Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Access requirements

You must have the following:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront plan</a>*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
    <td> <p>Plan</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.\

## Prerequisites

Before you can access your favorites and recent items from Slack, you must

* Configure Workfront for Slack  
  For instructions on configuring Workfront for Slack, see [Configure Adobe Workfront for Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Access your Favorites list from Slack

1. Log in to your Slack instance and log in to Workfront from Slack.  
   For more information about logging in to Workfront from Slack, see the "Logging In to Workfront from Slack" section in [Access Adobe Workfront from Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. From any channel, start typing the following command in the message field:&nbsp;

   ```
   /workfront favorites
   ```

   >[!NOTE]
   >
   >Commands are case sensitive. You can start your command with    >
   >
   >```   >
   >/wf
   >```   >
   >
   >instead of    >
   >
   >```   >
   >/workfront
   >```   >
   >
   >.

   A list of your Favorites displays.

* ![slack_favorites_with_show_more_button.png](assets/slack-favorites-with-show-more-button-350x202.png)

1. (Optional) Click **Show more** to list more Favorites.
1. Click the name of a favorite to open it in Workfront in a new browser tab.

## Access your recent items list from Slack

1. Log in to your Slack instance and log in to Workfront from Slack.  
   For more information about logging in to Workfront from Slack, see the "Logging In to Workfront from Slack" section in [Access Adobe Workfront from Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. From any channel, start typing the following command in the message field:&nbsp;

   ```
   /workfront recent
   ```

   >[!NOTE]
   >
   >Commands are case sensitive. You can start your command with    >
   >
   >```   >
   >/wf
   >```   >
   >
   >instead of    >
   >
   >```   >
   >/workfront
   >```   >
   >
   >.

   A list of your Recent Items displays, in the order they were accessed last, with the most recent at the top. The items are listed three at a time and are grouped by object type.  
   ![slack_recent_items.png](assets/slack-recent-items-350x249.png)

1. (Optional) Click **Show more** to list more Recent Items.
1. (Optional)&nbsp;Click the name of an item you have recently accessed to open it in Workfront in a new browser tab.

