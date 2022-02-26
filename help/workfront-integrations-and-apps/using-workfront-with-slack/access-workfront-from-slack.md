---
filename: access-workfront-from-slack
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Access Adobe Workfront from Slack
description: Integrating Adobe Workfront with Slack allows you to access Workfront from Slack, or perform certain actions in Workfront using a slash command. The integration can be used from any Slack environment, including the Slack mobile app.
---

# Access *Adobe Workfront* from Slack

Integrating *Adobe Workfront* with Slack allows you to access *Workfront* from Slack, or perform certain actions in *Workfront* using a slash command. The integration can be used from any Slack environment, including the Slack mobile app.

You or your Slack administrator must install the *Workfront* app in your Slack instance before you can use *Workfront* from Slack. For more information, see [Configure Adobe Workfront for Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## About slash commands

When using Slack, you type messages inside of a message field. When you start your message with a slash, it becomes a command and it behaves differently than a simple message. The command tells Slack to perform an action.

You can access your *Workfront* instance from Slack by typing a slash command in any Slack channel.

Remember the following when using a slash command in Slack to access *Workfront*:

* Slash commands are case sensitive. 
* The commands for *Workfront*are only visible to you, regardless of which channel you are typing them in.
* The command should always start with the following:  
  <pre>/workfront</pre> Or&nbsp; <pre>/wf </pre> followed by a space and the name of an action you want to perform in *Workfront*.  
  This indicates that your command is meant for the *Workfront* app. The commands for *Workfront* work only when you have already configured the *Workfront* app with your Slack instance.

For a list of all the commands you can run from Slack for *Workfront*, see [Access Workfront from a slash command in Slack](#access-workfront-from-slash-command).

## Log in to *Workfront* from Slack

When you type any command in the message field in Slack, you will be asked to log in to *Workfront* first.   
For a complete list of *Workfront* commands from Slack, see&nbsp;the [Access Workfront from a slash command in Slack](#access-workfront-from-slash-command) section in this article.&nbsp;

To log in to *Workfront* from Slack:

<ol> 
 <li value="1">Log in to your Slack instance.</li> 
 <li value="2">From any channel, type one of the following commands:<br><pre>/workfront log in</pre> Or<br><pre>/wf log in</pre></li> 
 <li value="3">Click the <em>Workfront</em> <span class="bold">Log In</span> link displayed in the response.<br>A new tab opens with fields for <em>Workfront</em> credentials.</li> 
 <li value="4"> <p>Follow the prompts to log in to <em>Workfront</em> using Enhanced Authentication, OAuth 2.0, or your Security Assertion Markup Language (SAML) URL.</p> <note type="note"> 
   <ul> 
    <li>When you are prompted to enter the <em>host</em> of your <em>Workfront</em> account, type it using this format: <em>yourCompany'sDomain.my.workfront.com</em>. Your company's domain is usually the name of your company.</li> 
    <li>Enhanced Authentication is not available until a <em>Workfront administrator</em> enables it for this integration. </li> 
   </ul> 
  </note> <p>The configuration page for <em>Workfront</em> notifications in Slack opens.</p> </li> 
 <li value="5">(Optional) Disable any <em>Workfront</em> notifications that you do not want to receive in Slack.<br>For information about configuring <em>Workfront</em> settings for Slack, see the <a href="#configuring-preferences" class="MCXref xref">Configure settings</a> section in this article</li> 
 <li value="6">Navigate back to your Slack channel.<br>You are logged in to <em>Workfront</em> from your Slack instance.&nbsp;</li> 
</ol>

## Access *Workfront* from Slack

* [About slash commands](#access-workfront-with-a-slash-command) 
* [Access Workfront from a shared link in Slack](#access-workfront-from-shared-link)

## Access *Workfront* from a slash command in Slack

<ol> 
 <li value="1"> Log in to your Slack instance and log in to <em>Workfront</em> from Slack.<br>For more information about logging in to <em>Workfront</em> from Slack, see <a href="#logging-in-to-workfront" class="MCXref xref">Log in to Workfront from Slack</a></li> 
 <li value="2">From any channel, start typing the following command in the message field:&nbsp;<br><pre>/workfront help</pre> Or&nbsp;<br><pre>/wf help</pre></li> 
 <li value="3"> Select from the following commands:&nbsp; 
  <ul>
   <li><pre>/wf home</pre><p>Displays buttons from which you can access lists of your tasks, issues, and approvals. Clicking one of the buttons displays the first 20 items of each list in Slack.</p><p><img src="assets/slack-home-buttons-350x80.png" style="width: 350;height: 80;"></p><p>For more information about managing <em>Workfront</em> work items from Slack, see <a href="../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md" class="MCXref xref">Manage your work and approvals from Slack </a>.</p></li>
   <li><p><code>/wf add task <TaskName></code></p><p>Include the name of the task as it will appear in the <em>Workfront</em> interface.</p><p>Adds a task to <em>Workfront</em>.<br>For more information about adding tasks to <em>Workfront</em> from Slack, see the "Creating Tasks from Slack" section in <a href="../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md" class="MCXref xref">Create tasks and issues from Slack</a>.</p></li>
   <li><p><code> /wf add issue <Issue Name></code></p><p> Include the name of the issue as it will appear in the <em>Workfront</em> interface.<br>Adds an issue to <em>Workfront</em><br>For more information about adding issues to <em>Workfront</em> from Slack, see the "Creating Issues from Slack" section in <a href="../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md" class="MCXref xref">Create tasks and issues from Slack</a>.</p></li>
   <li><p><code>/wf favorites</code></p><p> Displays the list of your <em>Workfront</em> Favorites.<br>For more information about accessing your Favorites from Slack, see the <a href="../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites">Accessing Your Favorites List from Slack</a> section in the <a href="../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md">Accessing Your Favorites and Recent Items from Slack</a> article.</p></li>
   <li><p><code>/wf recent </code></p><p>Displays the list of your most recently accessed items in <em>Workfront</em>.<br>For more information about accessing your Recent Items from Slack, see the <a href="../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items">Accessing Your Recent Items List from Slack</a> section in the <a href="../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md" class="MCXref xref">Access your favorites and recent items from Slack</a> article. </p></li>
  </ul>
  <ul>
   <li><p> /<code>wf tasks</code></p><p>Displays a list of your tasks.</p><p>For more information about managing your tasks from Slack, see the "Managing Your Tasks from Slack" section in <a href="../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md">Managing Your Work and Approvals from Slack</a>.<br></p></li>
   <li><p><code> /wf issues</code></p><p>Displays a list of your issues.</p><p>For more information about managing your issues from Slack, see the "Managing Your Issues from Slack" section in <a href="../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md">Managing Your Work and Approvals from Slack</a>.</p></li>
  </ul>
  <ul>
   <li><pre>/wf approvals</pre> Displays your <em>Workfront</em> approvals.<br>For more information about managing your approvals from Slack, see the "Managing Your Approvals from Slack" section in <a href="../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md" class="MCXref xref">Manage your work and approvals from Slack </a>.<br></li>
   <li><p><code>/wf search <keyword></code> (include keyword)</p> Search for a specific keyword. You can search for the following types objects: 
    <ul>
     <li> Project </li>
     <li> Task&nbsp; </li>
     <li> Issue </li>
     <li> Report </li>
     <li> People </li>
     <li> Template </li>
     <li> Document </li>
     <li> Portfolio </li>
     <li> Program </li>
     <li> Dashboard </li>
     <li> Company </li>
     <li> Note &nbsp;<br>For more information about searching in Slack, see <a href="../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md" class="MCXref xref">Search for Adobe Workfront items from Slack</a>.</li>
    </ul></li>
   <li><pre>/wf log in</pre> Logs you in to <em>Workfront</em> from Slack.&nbsp; </li>
   <li><pre>/wf log out </pre> Logs you out of <em>Workfront</em> from Slack. You remain logged in to <em>Workfront</em> if you have a separate <em>Workfront</em> instance open in another browser tab on in another application.&nbsp; </li>
   <li><pre>/wf settings</pre> Gives you access to configuring your <em>Workfront</em> settings in Slack.<br>For information about configuring <em>Workfront</em> settings in Slack, see <a href="#configuring-preferences" class="MCXref xref">Configure settings</a>.</li>
   <li><pre>/wf help</pre> Displays a complete list of commands for <em>Workfront</em>.&nbsp; </li>
   <li><em> Visit <em>Workfront</em> Help:&nbsp; </em> Opens the Slack section on the <em>Workfront</em> Help Site in a new browser tab.&nbsp; </li>
  </ul></li> 
 <li value="4"> (Optional) To delete the message of any command, mouse over the upper-right corner of the Slack message containing the command and click<span class="bold">&nbsp;Show message actions</span>, then click <span class="bold">Delete message</span>. </li> 
 <li value="5"> (Optional and conditional) Click <span class="bold">Delete</span> to confirm you want to delete this message.&nbsp; </li> 
</ol>

### Access *Workfront* from a shared link in Slack

You can access *Workfront* objects from a link to those objects that is shared with you in Slack.&nbsp;

For more information about accessing *Workfront* from a shared link, see [Access Adobe Workfront objects from a shared link in Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## Configure settings

<ol> 
 <li value="1">Inside a Slack message field, type the following command:<br><pre>/workfront settings</pre> Or<br><pre>/wf settings</pre><p><img src="assets/slack-configuring-settings-350x302.png" style="width: 350;height: 302;"></p><br>All settings are enabled by default.</li> 
 <li value="2">Deselect from the following options, to disable your settings for <em>Workfront</em>: 
  <ul>
   <li>In the <span class="bold">General Settings</span> area, disable the <span class="bold">When pasting a <em>Workfront</em> URL in a Slack channel, show additional description, due date, or requestor name.&nbsp;</span>setting if you do not want Slack to add additional information about your <em>Workfront</em> objects when you share a URL to the object in Slack.</li>
   <li>In the <span class="bold">Notifications Settings</span> area, disable notifications that you want to stop receiving from <em>Workfront</em>.<br>For information about receiving <em>Workfront</em> notifications in Slack, see <a href="../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md" class="MCXref xref">Receive Adobe Workfront notifications in Slack </a>.</li>
  </ul></li> 
</ol>

## Log out of *Workfront* from Slack&nbsp;

1. Inside a Slack message field, type the following command:  
   <pre>/workfront log out</pre> Or  
   <pre>/wf log out</pre>  
   You receive a confirmation that you have been logged out of *Workfront*.  
   You remain logged in to *Workfront* if you have a separate *Workfront* instance open in another browser tab on in another application.&nbsp;

