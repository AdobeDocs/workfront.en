---
filename: slack-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Slack modules
description: In a Adobe Workfront Fusion scenario, you can connect your Slack account to multiple third-party applications and services.
---

# Slack modules

In a *Adobe Workfront Fusion* scenario, you can connect your *Slack* account to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p><em>Pro</em> or higher</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
    <td> <p>Plan, Work</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront Fusion</em> license**</td> 
   <td> <p><em>Workfront Fusion for Work Automation and Integration</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <em>Adobe Workfront Fusion</em> as well as <em>Adobe Workfront</em> to use functionality described in this article.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

&#42;&#42;For information on *Adobe Workfront Fusion* licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use Slack modules, you must have a Slack account.

## Slack modules and their fields

When you configure *Slack* modules, *Workfront Fusion* displays the fields listed below. Along with these, additional *Slack* fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Messages](#messages) 
* [Files](#files) 
* [Channels](#conversa) 
* [Reactions](#reaction) 
* [Stars](#stars) 
* [Saved Items](#saved) 
* [Pins](#pins) 
* [Users](#users) 
* [Reminders](#reminder) 
* [Events](#events) 
* [Profile](#profile) 
* [Other](#other)

### Messages

* [Watch Public Channel Messages](#watch) 
* [Watch Private Channel Messages](#watch2) 
* [Watch Direct Messages](#watch3) 
* [Watch Multiparty Direct Messages](#watch4) 
* [Search for Message](#search2) 
* [Get a Private Channel Message](#get2) 
* [Get a Public Channel Message](#get) 
* [Create a Message](#create) 
* [Update a Message](#update) 
* [Delete a Message](#delete)

#### Watch Public Channel Messages

This trigger module starts the scenario when a new message is added to a public channel.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Channel </td> 
   <td> <p>Select the public channel you want to watch for new messages.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>Set the maximum number of messages <em>Workfront Fusion</em> will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Watch Private Channel Messages

This trigger module starts the scenario when a new message is added to a private channel (group).

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Channel </td> 
   <td> <p>Select the private channel you want to watch for new messages.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>Set the maximum number of messages <em>Workfront Fusion</em> will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Watch Direct Messages

This trigger module starts the scenario when a new message is added to a direct message.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Channel </td> 
   <td> <p>Select the direct message conversation you want to watch for new messages.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>Set the maximum number of messages <em>Workfront Fusion</em> will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Watch Multiparty Direct Messages

This trigger module starts the scenario when a new message is added to a multiparty direct message channel.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Channel </td> 
   <td> <p>Select the direct message conversation you want to watch for new messages.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>Set the maximum number of messages <em>Workfront Fusion</em> will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Search for Message

This search module returns messages matching a search query.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query</td> 
   <td> <p>Enter the query that you want to search by. </p> <p>For information on creating formulas from the mapping panel, see <a href="../../workfront-fusion/functions/map-using-functions.md" class="MCXref xref">Map items using functions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>Set the maximum number of messages <em>Workfront Fusion</em> will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a Private Channel Message

This action module retrieves the details of a message from a selected channel.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Channel ID</p> </td> 
   <td> <p>Enter (map) the Channel ID.</p> <p>Note: The Channel ID can be retrieved using the List Channels module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Message ID (Time stamp)</p> </td> 
   <td> <p> Enter or map the message time stamp of the message you want to retrieve information about.</p> <p>Note: The time stamp can be retrieved using another module, such as the Watch Public Channel Module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a Public Channel Message

This action module returns a message with a given ID from a specified public channel..

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Channel ID</p> </td> 
   <td> <p>Enter or map the Channel ID.</p> <p>Note: The Channel ID can be retrieved using the List Channels module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Message ID (Time stamp)</td> 
   <td> <p> Enter or map the message time stamp of the message you want to retrieve information about.</p> <p>Note: The time stamp can be retrieved using another module, such as the Watch Public Channel Module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List replies

This action module retrieves a thread of messages posted to a conversation.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Channel type</td> 
   <td>Select the type of channel that contains the message that you want to retrieve replies for, then select the channel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Parent message ID (Time stamp)</td> 
   <td> <p> Enter or map the message time stamp of the message you want to retrieve replies for.</p> <p>Note: The time stamp can be retrieved using another module, such as the Watch Public Channel Module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of <em>replie</em>s you want the module to <em>return</em> during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create a Message

This action module creates a new message.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Enter a channel ID or name</p> </td> 
   <td> <p>Choose how you want to select the channel where you want to create a message.</p> 
    <ul> 
     <li> <p><span class="bold">Enter manually</span> </p> <p>In the <span class="bold">Channel ID or name</span> field, enter or map the Channel ID or name of the channel where you want to post the message.</p> <p>Note: The Channel ID can be retrieved using the List Channels module.</p> </li> 
     <li> <p><span class="bold">Select from the list</span> </p> <p>Select the type of channel, then select the channel.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Text</p> </td> 
   <td> <p>Enter the text content of the message you want to create.</p> <p>Note: For detailed information about text formatting, see <a href="https://api.slack.com/reference/surfaces/formatting">Formatting text for app surfaces</a> in the Slack documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Blocks</td> 
   <td>Block are reusable components that you can use to customize and organize your messages. For more information on blocks, see <a href="https://api.slack.com/block-kit">Block Kit</a> in the Slack documentation.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"> <p>As user</p> </td> 
    <td> <p>Select <span class="bold">Yes</span> to create the message as the authenticated user instead of as a bot.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader"> <p>As user</p> </td> 
   <td> <p>Select <span class="bold">Yes</span> to create the message as the authenticated user instead of as a bot.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Thread message ID (time stamp)</td> 
   <td>If the new message is a reply, enter the time stamp of the message you want to reply to. Do not enter the time stamp of a message that is already a reply.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Reply broadcast</td> 
   <td> <p>Select <span class="bold">Yes</span> if both of the following apply:</p> 
    <ul> 
     <li> <p>The new message is a reply to another message</p> </li> 
     <li> <p>You want the new message to be visible to everyone in the channel</p> </li> 
    </ul> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"> <p>Attachments</p> </td> 
    <td> <p>Add any attachments that you want to include in the message. An attachment is required when the field Text is left empty.</p> <p>For more details about attachments, see <a href="https://api.slack.com/docs/message-attachments">Attaching content and links to messages</a> in the Slack documentation.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader"> <p>Attachments</p> </td> 
   <td> <p>Add any attachments that you want to include in the message. An attachment is required when the field Text is left empty.</p> <p>For more details about attachments, see <a href="https://api.slack.com/docs/message-attachments">Attaching content and links to messages</a> in the Slack documentation.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"> <p>Icon emoji</p> </td> 
    <td> <p>Enter or map the emoji you want to use for the posted message. </p> <p>For a list of emoji, see the <a href="https://www.webfx.com/tools/emoji-cheat-sheet/">Emoji cheat sheet</a>.</p> <p>If the As user option is enabled, this field is ignored.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader"> <p>Icon emoji</p> </td> 
   <td> <p>Enter or map the emoji you want to use for the posted message. </p> <p>For a list of emoji, see the <a href="https://www.webfx.com/tools/emoji-cheat-sheet/">Emoji cheat sheet</a>.</p> <p>If the As user option is enabled, this field is ignored.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"> <p>Icon URL</p> </td> 
    <td> <p>Enter or map the URL to an image you want to use as the icon for this message.</p> <p>If the As user option is enabled, this field is ignored. </p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader"> <p>Icon URL</p> </td> 
   <td> <p>Enter or map the URL to an image you want to use as the icon for this message.</p> <p>If the As user option is enabled, this field is ignored. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Link names</p> </td> 
   <td> <p>Enable this option to allow names and channels to use <code>@username</code> or <code>#channel</code> format. </p> <p>For more information, see <a href="https://api.slack.com/docs/formatting">Formatting text for app surfaces</a> in the Slack documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Parse message text</p> </td> 
   <td> <p>Enable this option to allow automatic parsing. </p> <p>For more information, see <a href="https://api.slack.com/docs/formatting">Formatting text for app surfaces</a> in the Slack documentation.</p> <p>Note: If you used Link names or Parse message text options in the original message, you should specify them when running the Update a Message module as well.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Use markdown</p> </td> 
   <td> <p>Enable this option to allow Slack to use markdown in the text.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Unfurl primarily text-based content</p> </td> 
   <td> <p>Enable this option to allow unfurling of primarily text-based content. </p> <p>For more information about unfurling in Slack, see <a href="https://api.slack.com/reference/messaging/link-unfurling">Unfurling links in messages</a> in the Slack documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Unfurl media content</p> </td> 
   <td> <p>Enable this option to allow unfurling of media content. </p> <p>For more information about unfurling in Slack, see <a href="https://api.slack.com/reference/messaging/link-unfurling">Unfurling links in messages</a> in the Slack documentation.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"> <p>User name</p> </td> 
    <td> <p>Enter the name of your bot. </p> <p>If the As user option is enabled, this field is ignored.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader"> <p>User name</p> </td> 
   <td> <p>Enter the name of your bot. </p> <p>If the As user option is enabled, this field is ignored.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Update a Message

This action module allows you to edit an existing message.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Enter a channel ID or name</p> </td> 
   <td> <p>Choose how you want to select the message you want to .</p> 
    <ul> 
     <li> <p><span class="bold">Enter manually</span> </p> <p>In the <span class="bold">Channel ID or name</span> field, enter or map the Channel ID or of the channel that contains the message, then enter the <span class="bold">Time Stamp (Message ID)</span> of the message. .</p> <p>Note: The Channel ID can be retrieved using the List Channels module.</p> </li> 
     <li> <p><span class="bold">Select from the list</span> </p> <p>Select the type of channel, then select the channel, then select the message.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Text</p> </td> 
   <td> <p>Enter the new text content of the message you want to update.</p> <p>For more information, see <a href="https://api.slack.com/docs/formatting">Formatting text for app surfaces</a> in the Slack documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Blocks</td> 
   <td>Block are reusable components that you can use to customize and organize your messages. For more information on blocks, see <a href="https://api.slack.com/block-kit">Block Kit</a> in the Slack documentation.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"> <p>As user</p> </td> 
    <td> <p>Select <span class="bold">Yes</span> to update the message as the authenticated user instead of as a bot.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader"> <p>As user</p> </td> 
   <td> <p>Select <span class="bold">Yes</span> to update the message as the authenticated user instead of as a bot.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"> <p>Attachments</p> </td> 
    <td> <p>Add any attachments that you want to include in the message. An attachment is required when the field Text is left empty.</p> <p>For more details about attachments, see <a href="https://api.slack.com/docs/message-attachments">Attaching content and links to messages</a> in the Slack documentation.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader"> <p>Attachments</p> </td> 
   <td> <p>Add any attachments that you want to include in the message. An attachment is required when the field Text is left empty.</p> <p>For more details about attachments, see <a href="https://api.slack.com/docs/message-attachments">Attaching content and links to messages</a> in the Slack documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Link names</p> </td> 
   <td> <p>Enable this option to allow names and channels to use <code>@username</code> or <code>#channel</code> format. </p> <p>For more information, see <a href="https://api.slack.com/docs/formatting">Formatting text for app surfaces</a> in the Slack documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Parse message text</p> </td> 
   <td> <p>Enable this option to allow automatic parsing. </p> <p> For more information, see <a href="https://api.slack.com/docs/formatting">Formatting text for app surfaces</a> in the Slack documentation.</p> <p>Note: If you used Link names or Parse message text options in the original message, you should specify them when running the Update a Message module as well.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a Message

This action module deletes a specified message.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Channel ID</p> </td> 
   <td> <p>Enter or map the Channel ID.</p> <p>Note: The Channel ID can be retrieved using the List Channels module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Message ID</td> 
   <td> <p> Enter or map the time stamp of the message you want to delete.</p> <p>Note: The time stamp can be retrieved using another module, such as the Watch Private Channel Module.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"> <p>As user</p> </td> 
    <td> <p>Select <span class="bold">Yes</span> to delete the message as the authenticated user instead of as a bot.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader"> <p>As user</p> </td> 
   <td> <p>Select <span class="bold">Yes</span> to delete the message as the authenticated user instead of as a bot.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Files

* [Watch Files](#watch5) 
* [List Files](#list5) 
* [Get a File](#get4) 
* [Download a File](#download) 
* [Upload a File](#upload) 
* [Create a Text File](#create3) 
* [Delete a File](#delete2)

#### Watch Files

This trigger module starts a scenario when a new file is added.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Type</td> 
   <td>Select the type of file that you want the module to watch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Channel type</td> 
   <td> <p>Select the type of channel you want to watch for files, then select the channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>Enter or map the maximum number of <em>file</em>s you want the module to <em>return</em> during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Files

This action module returns a list of files based on the specified filter.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Type </td> 
   <td> <p>Select the type(s) of files you want to retrieve.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Channel type</p> </td> 
   <td> <p>Select the type of channel representing the channel that you want to list files from, then select the channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Created by</td> 
   <td> <p>Select a user to return only files created by that user.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Date from</td> 
   <td>Enter the earliest date that you want to return files from. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Type coercion</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Date to</td> 
   <td>Enter the latest date that you want to return files from. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Type coercion</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td>Enter or map the maximum number of <em>file</em>s you want the module to <em>return</em> during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

#### Get a File

This action module returns details about the specified file.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">File ID</td> 
   <td> <p>Enter or map the ID&nbsp;of the file that you want to retrieve. </p> <p>Note: The file ID can be retrieved using another module, such as the Watch Files Module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Download a File

This action module downloads a file from a URL. It must follow the Slack > Get a File module in a scenario.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL private download</td> 
   <td> <p>Map the <b>URL Private download</b> value from the Slack &gt; Get a File module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Upload a File

This action module creates or uploads a file to Slack

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Channels</td> 
   <td> <p>For each channel you want to upload the file to, click <b>Add item</b>, then select the channel type and channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Source file</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Title</td> 
   <td>Enter a title for the file you want to upload</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Thread ID (timestamp)</td> 
   <td> <p>If you are uploading the file as a reply, enter or map the time stamp of the message you want to reply to.</p> <p>Note: The time stamp can be retrieved using another module, such as the Watch Private Channel Module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Initial Comment</td> 
   <td> <p>Enter or map the text of the message that introduces the file.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create a Text File

This action module creates a text file.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Channels</td> 
   <td> <p>For each channel you want to upload the file to, click <b>Add item</b>, then select the channel type and channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Source file</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Title</td> 
   <td>Enter a title for the file you want to upload</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Thread ID (timestamp)</td> 
   <td> <p>If you are uploading the file as a reply, enter or map the time stamp of the message you want to reply to.</p> <p>Note: The time stamp can be retrieved using another module, such as the Watch Private Channel Module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Initial Comment</td> 
   <td> <p>Enter or map the text of the message that introduces the file.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a File

This action module returns deletes the specified file.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">File ID</td> 
   <td> <p>Enter or map the ID&nbsp;of the file that you want to delete. </p> <p>Note: The file ID can be retrieved using another module, such as the Watch Files Module.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Channels

* [List Channels](#list) 
* [Get a Channel](#get3) 
* [List Members in Channel](#list2) 
* [Set the Topic of a Channel](#set) 
* [Set the Purpose of a Channel](#set2) 
* [Join a Channel](#join) 
* [Leave a Channel](#leave) 
* [Create a Channel](#create2) 
* [Archive a Channel](#archive) 
* [Unarchive a Channel](#unarchiv)

#### List Channels

This search module returns a list of all channels in a workspace.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Exclude archived</p> </td> 
   <td> <p>Select Yes to exclude archived channels in results.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Type </td> 
   <td> <p>Select the type(s) of channels you want to retrieve.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>Set the maximum number of channels <em>Workfront Fusion</em> will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a Channel

This action module returns information about a workspace channel.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Channel ID</p> </td> 
   <td> <p>Enter or map the ID&nbsp;of the channel that you want to retrieve information about.</p> <p>Note: The Channel ID can be retrieved using the List Channels module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Members in Channel

This search module returns a list of users in the selected channel.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"> <p>Enter a channel ID or name</p> </td> 
    <td> <p>Choose how you want to select the channel where you want to create a message.</p> 
     <ul> 
      <li> <p><span class="bold">Enter manually</span> </p> <p>In the <span class="bold">Channel ID or name</span> field, enter or map the Channel ID or name of the channel where you want to post the message.</p> <p>Note: The Channel ID can be retrieved using the List Channels module.</p> </li> 
      <li> <p><span class="bold">Select from the list</span> </p> <p>Select the type of channel, then select the channel.</p> </li> 
     </ul> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader"> <p>Enter a channel ID or name</p> </td> 
   <td> <p>Choose how you want to select the channel where you want to create a message.</p> 
    <ul> 
     <li> <p><span class="bold">Enter manually</span> </p> <p>In the <span class="bold">Channel ID or name</span> field, enter or map the Channel ID or name of the channel where you want to post the message.</p> <p>Note: The Channel ID can be retrieved using the List Channels module.</p> </li> 
     <li> <p><span class="bold">Select from the list</span> </p> <p>Select the type of channel, then select the channel.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Channel type</td> 
   <td>Select the type of channel that contains the list of members you want to list.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Public / Private Channel</td> 
   <td>Select the channel that you want to list members of.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>Set the maximum number of members <em>Workfront Fusion</em> will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Set the Topic of a Channel

This action module changes the topic of a channel

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"> <p>Enter a channel ID or name</p> </td> 
    <td> <p>Choose how you want to select the channel that you want to change the topic for.</p> 
     <ul> 
      <li> <p><span class="bold">Enter manually</span> </p> <p>In the <span class="bold">Channel ID or name</span> field, enter or map the Channel ID or name of the channel where you want to post the message.</p> <p>Note: The Channel ID can be retrieved using the List Channels module.</p> </li> 
      <li> <p><span class="bold">Select from the list</span> </p> <p>Select the type of channel, then select the channel.</p> </li> 
     </ul> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader"> <p>Enter a channel ID or name</p> </td> 
   <td> <p>Choose how you want to select the channel that you want to change the topic for.</p> 
    <ul> 
     <li> <p><span class="bold">Enter manually</span> </p> <p>In the <span class="bold">Channel ID or name</span> field, enter or map the Channel ID or name of the channel where you want to post the message.</p> <p>Note: The Channel ID can be retrieved using the List Channels module.</p> </li> 
     <li> <p><span class="bold">Select from the list</span> </p> <p>Select the type of channel, then select the channel.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Channel type</td> 
   <td>Select the type of channel that you want to change the topic for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Public / Private / Multiple IM Channel / User</td> 
   <td>Select the channel or user that you want to change the topic for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Topic</td> 
   <td>Enter or map the new topic of the channel. This field does not support formatting or links.</td> 
  </tr> 
 </tbody> 
</table>

#### Set the Purpose of a Channel

This action module changes the purpose of a channel

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"> <p>Enter a channel ID or name</p> </td> 
    <td> <p>Choose how you want to select the channel where you want to create a message.</p> 
     <ul> 
      <li> <p><span class="bold">Enter manually</span> </p> <p>In the <span class="bold">Channel ID or name</span> field, enter or map the Channel ID or name of the channel where you want to post the message.</p> <p>Note: The Channel ID can be retrieved using the List Channels module.</p> </li> 
      <li> <p><span class="bold">Select from the list</span> </p> <p>Select the type of channel, then select the channel.</p> </li> 
     </ul> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader"> <p>Enter a channel ID or name</p> </td> 
   <td> <p>Choose how you want to select the channel where you want to create a message.</p> 
    <ul> 
     <li> <p><span class="bold">Enter manually</span> </p> <p>In the <span class="bold">Channel ID or name</span> field, enter or map the Channel ID or name of the channel where you want to post the message.</p> <p>Note: The Channel ID can be retrieved using the List Channels module.</p> </li> 
     <li> <p><span class="bold">Select from the list</span> </p> <p>Select the type of channel, then select the channel.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Channel type</td> 
   <td>Select the type of channel that you want to change the topic for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Public / Private / Multiple IM Channel / User</td> 
   <td>Select the channel or user that you want to change the topic for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Purpose</td> 
   <td>Enter or map the new purpose of the channel. This field does not support formatting or links.</td> 
  </tr> 
 </tbody> 
</table>

#### Join a Channel

This action module joins the user to a channel.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Channel ID</p> </td> 
   <td> <p>Enter or map the ID&nbsp;of the channel that you want to join.</p> <p>Note: The Channel ID can be retrieved using the List Channels module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Leave a Channel

This action module removes the user from a channel.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Channel ID</p> </td> 
   <td> <p>Enter or map the ID&nbsp;of the channel that you want to leave.</p> <p>Note: The Channel ID can be retrieved using the List Channels module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create a Channel

This action module creates a new channel.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Name</p> </td> 
   <td> <p>Enter or map a name for the new channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Is private</td> 
   <td>Enable this option to set the new channel as private.</td> 
  </tr> 
 </tbody> 
</table>

#### Archive a Channel

This action module creates a new channel.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Channel ID</p> </td> 
   <td> <p>Enter or map the ID&nbsp;of the channel that you want to archive.</p> <p>Note: The Channel ID can be retrieved using the List Channels module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Unarchive a Channel

This action module creates a new channel.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Channel ID</p> </td> 
   <td> <p>Enter or map the ID&nbsp;of the channel that you want to unarchive.</p> <p>Note: The Channel ID can be retrieved using the List Channels module.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Reactions

* [List reactions](#list3) 
* [Add a reaction](#add) 
* [Remove a reaction](#remove)

#### List reactions

This action module returns reactions that a user made.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>User</p> </td> 
   <td> <p>Select the user that made the reactions that you want to list.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of <em>reaction</em>s you want the module to <em>return</em> during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Add a reaction

This action module adds a reaction to an item.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Channel type</td> 
   <td>Select the type of channel that you want to add a reaction to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Public / Private / Multiple IM channel / User</td> 
   <td>Select the channel or user that you want to add a reaction to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Message ID</td> 
   <td> <p> Enter or map the time stamp of the message you want to add a reaction to.</p> <p>Note: The time stamp can be retrieved using another module, such as the Watch Private Channel Module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Reaction (emoji) name</td> 
   <td>Enter or map the name of the emoji that you want to use for a reaction. Example: <code>thumbsup</code>. </td> 
  </tr> 
 </tbody> 
</table>

#### Remove a reaction

This action module adds a reaction to an item.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Channel type</td> 
   <td>Select the type of channel that you want to remove a reaction from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Public / Private / Multiple IM channel / User</td> 
   <td>Select the channel or user that you want to add a reaction from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Message ID</td> 
   <td> <p> Enter or map the time stamp of the message you want to add a reaction to.</p> <p>Note: The time stamp can be retrieved using another module, such as the Watch Private Channel Module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Reaction (emoji) name</td> 
   <td>Enter or map the name of the emoji that you want to remove from the message. Example: <code>thumbsup</code>. </td> 
  </tr> 
 </tbody> 
</table>

### Stars

* [Add a star](#add2) 
* [Remove a star](#remove3)

#### Add a star

This action module makes a channel a starred channel.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Channel type</td> 
   <td>Select the type of channel that you want to add a star to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Public / Private / IM / Multiple IM channel</td> 
   <td>Select the channel or user that you want to add a star to.</td> 
  </tr> 
 </tbody> 
</table>

#### Remove a star

This action module removed the star from a starred channel.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Channel type</td> 
   <td>Select the type of channel that you want to add a star to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Public / Private / IM / Multiple IM channel</td> 
   <td>Select the channel or user that you want to add a star to.</td> 
  </tr> 
 </tbody> 
</table>

### Saved Items

* [Save an Item](#save) 
* [Remove Saved Item](#remove2)

#### Save an Item

This action module adds an item to saved items.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Message ID (Time stamp)</td> 
   <td> <p> Enter or map the time stamp of the message you want to save.</p> <p>Note: The time stamp can be retrieved using another module, such as the Watch Private Channel Module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">File ID</td> 
   <td> <p>Enter or map the file that you want to save.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Remove Saved Item

This action module adds an item to saved items.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Message ID (Time stamp)</td> 
   <td> <p> Enter or map the time stamp of the message you want to remove from saved items.</p> <p>Note: The time stamp can be retrieved using another module, such as the Watch Private Channel Module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">File ID</td> 
   <td> <p>Enter or map the file you want to remove from saved items.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Pins

* [Pin an Item](#pin) 
* [Unpin an Item](#unpin)

#### Pin an Item

This action module pins an item, such as a file or file comment, to a channel.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Channel type</td> 
   <td>Select the type of channel that you want to pin an item to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Public / Private / Multiple IM channel / User</td> 
   <td>Select the channel or user that you want to pin an item to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Message ID</td> 
   <td> <p> Enter or map the time stamp of the message you want to pin.</p> <p>Note: The time stamp can be retrieved using another module, such as the Watch Private Channel Module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Unpin an Item

This action module unpins an item from a channel. You can unpin files, file comments, channel messages, or group messages.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Channel type</td> 
   <td>Select the type of channel that you want to unpin an item from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Public / Private / Multiple IM channel / User</td> 
   <td>Select the channel or user that you want to unpin an item from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Message ID</td> 
   <td> <p> Enter or map the time stamp of the message you want to unpin.</p> <p>Note: The time stamp can be retrieved using another module, such as the Watch Private Channel Module.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Users

* [Watch Multiparty Direct Messages](#watch4) 
* [Search for User](#search) 
* [List Users](#list4) 
* [Get a User](#get5) 
* [Invite Users](#invite) 
* [Kick a User](#kick)

#### Watch Users

This trigger module starts the scenario when a new user is added to the Slack workspace.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>Set the maximum number of users <em>Workfront Fusion</em> will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Search for User

This action module retrieves details about a single user, by using their email address.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Email </p> </td> 
   <td> <p>Enter or map the email address of the user you want to retrieve details about.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Users

This action module returns a list of all users in a workspace.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Limit</p> </td> 
   <td> <p>Enter or map the maximum number of <em>user</em>s you want the module to <em>return</em> during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a User

This action module retrieves details about a member of a workspace.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>User ID</p> </td> 
   <td> <p>Enter or map the User ID&nbsp;of the user you want to retrieve details for.</p> <p>Note: The User ID can be retrieved using another module, such as the List Users module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Invite Users

This action module invites 1-30 users to a public or private channel.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Channel type</td> 
   <td>Select the type of channel that you want invite users to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Public / Private / Multiple IM channel / User</td> 
   <td>Select the channel or user that you want to invite users to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Users</td> 
   <td> <p>Select the users that you want to add to the channel.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Kick a User

This action module removes a user from a channel.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Channel type</td> 
   <td>Select the type of channel that you want remove a user from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Public / Private channel</td> 
   <td>Select the channel that you want to remove a user from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Users</td> 
   <td> <p>Select the user that you want to remove from the channel.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Reminders

* [List Reminders](#list6) 
* [Get a Reminder](#get6) 
* [Create a Reminder](#create4) 
* [Complete a Reminder](#complete) 
* [Delete a Reminder](#delete3)

#### List Reminders

This action module returns a list of all reminders created by or given to the currently authenticated user.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Limit</p> </td> 
   <td> <p>Enter or map the maximum number of <em>reminder</em>s you want the module to <em>return</em> during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a Reminder

This action module retrieves details about a specific reminder.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Reminder ID</p> </td> 
   <td> <p>Enter or map the Reminder ID&nbsp;of the reminder you want to retrieve details for.</p> <p>Note: The Reminder ID can be retrieved using another module, such as the List Reminders module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create a Reminder

This action module creates a reminder.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Text</td> 
   <td>Enter or map the content of the reminder</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Time</td> 
   <td> <p>Enter or map the date and time when this reminder should happen. Enter one of the following: </p> 
    <ul> 
     <li> <p>The Unix timestamp (up to five years from now)</p> </li> 
     <li> <p>The number of seconds until the reminder (if within 24 hours) </p> </li> 
     <li> <p>A natural language description (Examples: "in 15 minutes" or "every Thursday")</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>User </p> </td> 
   <td> <p>Select the user that receives the reminder.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Complete a Reminder

This action module completes a specific reminder.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Reminder ID</p> </td> 
   <td> <p>Enter or map the Reminder ID&nbsp;of the reminder you want to complete.</p> <p>Note: The Reminder ID can be retrieved using another module, such as the List Reminders module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a Reminder

This action module deletes a specific reminder.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Reminder ID</p> </td> 
   <td> <p>Enter or map the Reminder ID&nbsp;of the reminder you want to delete.</p> <p>Note: The Reminder ID can be retrieved using another module, such as the List Reminders module.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Events

#### New Event

This instant trigger starts a scenario when a new message or other event is created.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Webhook</p> </td> 
   <td> <p>Select the webhook you want to use.</p> <p>Or</p> <p>Create a new webhook.</p> 
    <ol> 
     <li value="1"> <p>Click <b>Add</b>.</p> </li> 
     <li value="2"> <p>Select the event type.</p> </li> 
     <li value="3"> <p>Select or add a connection. For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </li> 
     <li value="4"> <p>If prompted, select the channel that you want to watch.</p> </li> 
     <li value="5"> <p>Click <b>Save</b> to save the webhook and return to the module.</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### Profile

#### Set a status

This action module updates a user's current status.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Status text</p> </td> 
   <td> <p>Enter or map the status text. Consider the following:</p> 
    <ul> 
     <li> <p>You can enter up to 100 characters.</p> </li> 
     <li> <p>You can use markup or other formatting, such as user mentions.</p> </li> 
     <li> <p>You can include emojis in the status text by using the format <code>:emojiname:</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Status Emoji</td> 
   <td> <p>Enter or map the emoji that you want to use to represent your status. Use the format <code>:emojiname:</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Status expiration</td> 
   <td>Enter or map the date and time you want the status to expire. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Type coercion</a>.</td> 
  </tr> 
 </tbody> 
</table>

### Other

#### Make an API Call

This action module lets you make a custom authenticated call to the *Slack* API

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
without having to think through authentication
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  without having to think through authentication</MadCap:conditionalText>`. This way, you can create a data flow automation that can't be accomplished by the other *Slack* modules. 

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your <em>Slack</em> account to <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Enter a path relative to <code>https://slack.com/api/</code>. Example: <code>/users.identity</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p><em>Workfront Fusion</em> adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p>Add the query for the API call in the form of a standard JSON object.</p> <p>For example: <code>{“name”:“something-urgent”}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Base URL</td> 
   <td>Select the base URL that you want to use for the API call.</td> 
  </tr> 
 </tbody> 
</table>

## Terminology

The following terminology may be useful when configuring Slack modules:

* `DM`: Direct Message
* `IM`: Instant Message
* `Private Channel`: formerly Group
* `Direct Message`: formerly IM
* `Channel`: Conversation in the API documentation, channel in the Slack app.

