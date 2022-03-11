---
filename: workfront-add-on-for-jira-beta
content-type: reference
navigation-topic: betas
title: Workfront Add-On for Jira Beta
description: As a Jira system administrator, you will soon be able to download and configure the Workfront add-on for Jira. This will allow you to integrate the two applications.
---

# `Workfront` Add-On for Jira Beta

As a Jira system administrator, you will soon be able to download and configure the `Workfront` add-on for Jira. This will allow you to integrate the two applications.&nbsp;

When you configure the `Workfront` add-on for Jira, you can specify triggers that will create Jira issues when certain criteria for creating items are met in `Workfront`. The items users create in `Workfront` are then linked to issues in Jira. As items update in one application, they become updated in the other application, based on the setup criteria you select in your configuration.&nbsp;

This way, the project managers can continue to work in `Workfront`, while the development users can continue working in Jira. Both entities are able to update just the item in their own environment and both of them see the updates from the other entity on their respective items.

This new functionality has not been generally&nbsp;released yet, but you can participate in our limited beta program to test it.&nbsp;

>[!NOTE]
>
>This beta program has only been made available for the On-Demand version of Jira. The current beta integration is not supported for the On-Premise version of Jira.

If you would like to be part of this beta program and have this functionality enabled in your `Workfront` app on your Jira environment, see [Uploading the Workfront Beta Add-On for Jira](#signing-up-for-the-android-requests-beta).

## Uploading the `Workfront` Beta Add-On for Jira&nbsp;

To join our beta testing and experience the new features:&nbsp;

<ol> 
 <li value="1">Log into Jira as a system administrator.</li> 
 <li value="2">Click <span class="bold">Settings</span> in the main Jira menu.</li> 
 <li value="3">Click <span class="bold">Add-ons</span>, then <span class="bold">Manage add-ons</span>.</li> 
 <li value="4">Click <span class="bold">Settings</span>.<br><img src="assets/second-settings-for-jira-wf-beta-add-on-350x137.png" alt="Second_settings_for_Jira_WF_beta_add-on.png" style="width: 350;height: 137;"></li> 
 <li value="5">Ensure that the&nbsp;<span class="bold">Enable private listings</span> field is enabled.<br><img src="assets/jira-wf--ensure-private-listings-field-enabled-350x147.png" alt="Jira_WF__ensure_private_listings_field_enabled.png" style="width: 350;height: 147;"></li> 
 <li value="6">Click <span class="bold">Apply</span>, then click <span class="bold">Upload add-on</span>.<br><img src="assets/jira-wf--upload-addon-for-beta-button.png" alt="Jira_WF__Upload_addon_for_beta_button.png"></li> 
 <li value="7">Copy the following URL and paste it in the field displayed:<br><a href="https://jira.workfront.com/atlassian-connect.json" data-saferedirecturl="https://www.google.com/url?hl=en&q=https://jira.workfront.com/atlassian-connect.json&source=gmail&ust=1517061032882000&usg=AFQjCNEFSllaLEOzoRTvc_QLSJ5jf_YuSg">https://jira.workfront.<wbr>com/atlassian-connect.json</a></li> 
 <li value="8">Click <span class="bold">Upload</span>.<br>The <span>Workfront</span> beta add-on is now available in the list of add-ons in Jira.<br>You can now start configuring your <span>Workfront</span> to Jira integration.&nbsp;</li> 
</ol>

## Configuring the `Workfront` Beta Add-On for Jira

<ol> 
 <li value="1">Log into Jira as a system administrator.</li> 
 <li value="2">Click <span class="bold">Settings</span> in the main Jira menu.</li> 
 <li value="3">Click <span class="bold">Add-ons</span>, then <span class="bold">Manage add-ons</span>.</li> 
 <li value="4">Expand the <span class="bold"><span>Workfront</span></span> add-on.</li> 
 <li value="5">Click <span class="bold">Configure</span>.</li> 
 <li value="6">Specify your <span>Workfront</span> credentials and domain information.<br><note type="note">
    You must log in to 
   <span>Workfront</span> as a system administrator to continue configuring the integration. We recommend that you create a system administrator account designated for the 
   <span>Workfront</span> to Jira integration and not use an existing account which might be connected to another user.&nbsp;
  </note><br><img src="assets/jira-wf-login-from-jira-focused-350x291.png" alt="Jira_WF_Login_from_Jira_focused.png" style="width: 350;height: 291;"></li> 
 <li value="7">Select the <span class="bold">Triggers</span> tab to configure the automatic creation of Jira items as new <span>Workfront</span> items are created.&nbsp;Creating an item in <span>Workfront</span> and assigning it to a specific entity can automatically create an item in Jira. The two items become linked.<br>Specify the following: 
  <ul>
   <li><span class="bold"><span>Workfront</span> team/user/role</span>: Specify which team, user, or role the item in <span>Workfront</span> must be assigned to in order to trigger the automatic creation of a Jira item.</li>
   <li>The <span class="bold">Jira project</span> on which you want to add the new item in Jira.</li>
   <li>The <span class="bold">Issue type</span> of the newly created item in Jira.&nbsp;</li>
  </ul></li> 
 <li value="8">Click <span class="bold">Save</span>.</li> 
 <li value="9">Select the <span class="bold">Setup</span> tab to configure which fields to synchronize between the linked Jira and <span>Workfront</span> items.<br>Consider specifying the following: 
  <ul>
   <li><span class="bold">Synchronize from <span>Workfront</span> to Jira</span>:<br>
    <ul>
     <li><span class="bold">Name</span></li>
     <li><span class="bold">Description</span></li>
     <li><span class="bold">Documents</span></li>
     <li><span class="bold">Planned Completion Date</span></li>
    </ul></li>
   <li><span class="bold">Synchronize from Jira to <span>Workfront</span></span>: 
    <ul>
     <li><span class="bold">Status</span></li>
     <li><span class="bold">Assignee</span>: When you assign an item in Jira to a user who does not have a <span>Workfront</span> account, the integration creates a new user in <span>Workfront</span>. This user does not occupy a <span>Workfront</span> license.</li>
     <li><span class="bold">Attachments</span></li>
    </ul></li>
   <li><span class="bold">Other</span>: Specify how you want the updates of the following fields to be recorded in the two applications: 
    <ul>
     <li>Custom Data</li>
     <li>Priority</li>
     <li>Due Date changes</li>
    </ul></li>
  </ul></li> 
 <li value="10">Click <span class="bold">Save</span>.&nbsp;</li> 
 <li value="11">(Optional) View the <span class="bold">Activity Log</span> tab for any errors that might occur as you are working with the integrated features.&nbsp;</li> 
</ol>

>[!NOTE]
>
>After you complete the configuration, anyone who can create items in `Workfront` can trigger the automatic creation of linked items in Jira, every time the triggers match those you specified. `Workfront` users will not need a Jira license to trigger the creation of items in Jira. Also, any Jira user can immediately start working on items automatically created from `Workfront` and their updates on these items will transfer to the `Workfront` items without them needing a license for `Workfront`.&nbsp;

For more information about configuring the `Workfront` add-on for Jira and updating items, see [Adobe Workfront for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/workfront-for-jira.md).

To see a demonstration of how to use the `Workfront` add-on for Jira, see the following video:

`<iframe class="mt-media" src="assets/252893646?title=0&byline=0&portrait=0" width="640px" height="360px" frameborder="0" allowfullscreen></iframe>`

## Testing the `Workfront` Beta Add-On for Jira

Depending on how you have configured your integration, and after watching the video, we would like you to test the following features:

* Add comments in Jira and `Workfront` to items.
* Change the Name or Description of an item in `Workfront` and notice the changes in the linked item in Jira.
* Change the Status or Assignee of an item in Jira and notice the changes in the linked item in `Workfront`.
* Review the `Workfront` right panel in Jira and notice the information included there
* Attach a Custom Form to the `Workfront` item and change its Priority then notice the changes, if any, in the `Workfront` right panel in Jira.

* Attach documents to both Jira and `Workfront` items.
* Log time on Jira items.
* Review the tabs available for your items in Jira and the Updates tab in `Workfront` and notice any changes or logs.
* Review the Activity Log at the system level in Jira and notice any errors that might have occurred.&nbsp;

We would like you to answer the following questions as you are testing the new functionality:&nbsp;

* Usefulness: Is automatically creating Jira tickets out of `Workfront` tasks and issues and keeping them synchronized helping you to get things done faster and more efficiently?
* Use cases: Why would you want to create Jira issues when you are creating `Workfront` tasks or issues and link them? Outline your main scenarios when being able to have this type of link can really help you.  
  Consider the following:&nbsp;

  * Triggers: Are assignment-based triggers enough, or would you like to have more trigger types, for example, triggers based on status changes in `Workfront`?
  * Working with documents: Attach files both to `Workfront` and Jira items which are linked, and notice how the synchronization of documents occurs between `Workfront` and Jira.
  
  * Comments: Are you satisfied with how Jira comments are displayed in `Workfront`, and how `Workfront` comments are displayed in Jira? What would you like to see improved?
  
  * Logging time: Does logging hours from the right panel work as expected? Is it intuitive enough? How can we improve the time tracking?

* Relevancy: Is the ability to link items between the two application relevant to you and the workflows in your organization? Is the `Workfront` information shown in Jira sufficient? What else would you like to synchronize between the two platforms?
* Convenience: Is the new ability to have work items linked between Jira and `Workfront` convenient for your developers and project managers?
* Issues: What errors or issues have you encountered when using the `Workfront` add-on for Jira? Was the interface clear enough and intuitive to allow you to navigate and use it freely and easily?
* Improvements: Tell us what you would like to see improved or added to the add-on.
* Satisfaction: On a scale from 1 to 5, with 5 being the most satisfied, how satisfied are you with the new `Workfront` add-on for Jira?

## Sending Feedback to Product&nbsp;Management

To submit feedback about your experience with the `Workfront` add-on for Jira do one of the following:

Submit feedback to Product Management:&nbsp;

1. Navigate to an item in Jira that is linked to an item in `Workfront`.&nbsp;
1. On the `Workfront` panel, click  `Submit Feedback`.

1. Complete the short survey and submit it.  
   The survey is submitted to the Product Management team.&nbsp;

Or:

1. Send an email with your feedback to *haykfalakyan@workfront.com*.

