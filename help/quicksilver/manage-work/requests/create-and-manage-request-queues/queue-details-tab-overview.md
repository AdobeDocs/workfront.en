---
filename: queue-details-tab-overview
content-type: overview
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Overview of the Queue Details tab in a project
description: You can set up a Request Queue where users can enter occasional requests that are not planned work on a project.
hidefromtoc: true
---

# Overview of the Queue Details tab in a project

Overview of the Queue Setup section You can set up a Request Queue where users can enter occasional&nbsp;requests that are not planned work on a project.

For more information about how to create a Request Queue, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

You can customize the Request Queue by editing the Queue Setup section of a project.&nbsp;

When adding or modifying features in the Queue Setup area, you&nbsp;impact all future issues and requests that are submitted to the project.&nbsp;

>[!IMPORTANT]
>
>The changes you make do&nbsp;not retroactively&nbsp;impact issues or requests&nbsp;already on the project.&nbsp;

To customize the Queue Setup section of a project, you can edit the following sections:

* Queue Details. For more information about understanding the information included in the Queue Details, see the section [Overview of the Queue Details section](#overview2) in this article.
* Routing Rules. For more information about setting up Routing Rules, see [Create Routing Rules](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).
* Queue Topics. For more information about setting up Queue Topics, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
* Topic Groups. For more information about setting up Topics Groups, see [Create Topic Groups](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

Overview of the Queue Details section You can use Queue Details to configure a project as a Request Queue. Use this&nbsp;section to manage what kind of information you collect from users on a request form and determine who can access that information.

When configuring the Queue Details &nbsp;section in a project, consider the following areas:

* [Queue Type](#understanding-queue-type) 
* [Queue Properties](#understanding-queue-properties) 
* [New Issue Fields](#understanding-new-issue-fields) 
* [Email Settings](#understanding-email-settings)

### Queue Type

**Publish as Help Request Queue:**

Selecting this field identifies this project as a Request Queue and all incoming issues are considered Requests. When this field is not selected, the project behaves like a standard project in Adobe Workfront and all incoming issues are added on the Issues tab of the project.

**Who can add requests to this Queue?**

This indicates who has access to the Request Queue.&nbsp;

* **Anyone** — Allows all active users with a license to submit requests to the queue. 
* **People with view access to this project** &nbsp;— Users with View rights to&nbsp;the project can submit a request to the queue. 
* **People in this project’s company** — Users in the same company as the project can submit requests. The company is shown in parentheses when this option has been selected and the company is associated with the project. 
* **People in this project’s group** — Users in the group selected on the project can submit requests. The group is shown in parentheses.

**Share with These Links:**

If the **Publish as Help Request Queue** option is selected, a **Direct Access URL** and **Embed Code** become available for the Request Queue. To use either option, a person must be a Workfront user.

The following options enable you to provide direct access to the Request Queue and Request Queue forms to users&nbsp;outside of Workfront.&nbsp;Users must already have access rights to the Request Queue in order to gain direct access. Using either option&nbsp;described here does&nbsp;not automatically grant access to users:

* **Direct Access URL:** When a user accesses this URL from&nbsp;a browser, the user is taken directly to the request queue within Workfront. Users must first log in to Workfront before gaining access to the request queue.  
  To provide users with a direct URL to a queue topic or topic group, Go to the request queue and select the queue topic&nbsp;or topic group&nbsp;that you want users to access. The URL in the browser updates accordingly. Copy the&nbsp;URL from the browser&nbsp;and distribute it to users.

* &nbsp;**Embed Code:**&nbsp;Use this HTML&nbsp;code to embed the request queue form as an iframe within any HTML&nbsp;page.  
  If users are not already authenticated to Workfront&nbsp;when they view the page where the code is embedded, the Workfront login dialog box is displayed. After users log in, the Request Queue form is displayed.

>[!NOTE]
>
>When displaying a Request Queue in an iframe, only the form is displayed. Navigation components and logos are not displayed.

In order for the request queue form to be displayed when using this&nbsp;embed code, you must enable the **Allow embedding of Workfront in an iframe** setting in your system setup. For more information about enabling embedding of Workfront in an iframe, see [Configure system security preferences](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).&nbsp;If this setting is not enabled, the iframe is displayed as blank.  
You can adjust various aspects of how the embedded&nbsp;form is displayed, as follows:

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Functionality</strong> </p> </th> 
   <th> <p><strong>Solution</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Adjust the size of the frame</p> </td> 
   <td> <p>Modify the "width" and "height" attributes.</p> <p>By default, the width is "500" and the height is "600"</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Direct users to a specific Queue Topic or Topic Group</p> </td> 
   <td> <p>Add the "path" parameter to the src URL. You can find the path parameter by navigating to the desired Queue Topic or Topic Group in the non-embedded form and inspecting the URL.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Show and allow users to change the pre-configured Topic Group drop-down list</p> </td> 
   <td> <p>Use&nbsp;the "path" parameter by adding the "showPreSelectedOptions=true" parameter to the src URL.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Detect when the form has been submitted</p> </td> 
   <td> <p>Add&nbsp;a "message" event listener to your web&nbsp;page's window to check if event.data.type is requestSubmitted. 'event.data.newIssueID' will be set to the ID of the created issue.</p> </td> 
  </tr> 
 </tbody> 
</table>

![](assets/queue-type-350x246.png)

### Queue Properties

Consider the following settings in the Queue&nbsp;Properties area:

**Request Types**

The following&nbsp;are the four global issue types in Workfront:

* Bug Report
* Change Order
* Issue
* Request

These types can&nbsp;only be renamed by a system administrator when issue statuses are created at the system level. Each type&nbsp;selected here will be available on the New Issue form&nbsp;and you can select more than one type. Using more than one type can help organize multiple&nbsp;requests coming in.

**Default Duration**

The default duration is the length of time it typically takes to complete an issue. This becomes the default for all incoming issues&nbsp;and can be modified manually.&nbsp;Duration is generally set in hours, days, or weeks. The Default Duration of an issue is the same as the Planned Hours on the issue. The Planned Completion Date of the issue calculates based on this field.

The default for the issue Duration is 1 day or 8 hours. If your Workfront administrator set the Typical Hours per&nbsp;Work Day as less than 8 hours, the Default Duration for issues is still 8 hours. For example, if the Typical Hours per Work Day is set to 7 hours, the Default Duration for issues is 1.14 Days or 8 hours. For more information about how to set up the system Typical Hours per Work Day, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

**People from the same company will inherit the same permissions for all requests.**

When selected, all requests submitted to the queue show for users in the same company. Users can view these requests in the All Requests section located within&nbsp;the Requests area. &nbsp;Activating or deactivating this feature impacts all future requests. It does not retroactively impact existing issues.

**When someone makes a request, automatically grant...**

Automatically grants the type of permission a user has&nbsp;when they submit a request to the queue. Setting permissions here saves time, rather than having to grant permissions for each individual incoming request. Choosing this option impacts all future requests, but does not retroactively impact existing requests.

**Default Approval**

When&nbsp;an organization uses approval processes with incoming work, the user can associate&nbsp;an approval process with the Request Queue. An approval process is automatically initiated with all incoming items. Approval processes must first be created by the system administrator in order for this field to display.

**Default Route**

It&nbsp;comes from Routing Rules that have already been setup on the project. Use this field to attach a Routing Rule or change the route when necessary. Choosing a Routing Rule here applies the same routing to all the issues submitted on this project. For information about creating Routing Rules, see [Create Routing Rules](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).  
![](assets/queue-properties-350x315.png)

### New Issue Fields

Predefined fields are available on the&nbsp;form. By default, Issue Name shows on all forms.

Consider the following fields in the New Issue Fields area:

**Show the following selected fields to all users**

Select fields from this area to choose what additional&nbsp;fields to display in your request queue.

**Show all selected and unselected fields to**

This field defines who sees the unselected as well as the selected fields from the above section on the New Issue form.

You can give the following sets of users access to view the fields you selected:

* **All Users (Plan Licenses)** - All users who have a Plan license can&nbsp;see the selected as well as the unselected fields.&nbsp; 
* **People with view access to this project (Plan License)** - Those users with a Plan license that also have View rights to this project can see the selected as well as the unselected fields. The rest of the users who can submit requests to this project can see just the selected fields. 
* **No Users** - No users can see the unselected fields. All users who can submit requests to this project can only see the fields selected.&nbsp;

**Custom****Forms**

The drop-down list for the custom&nbsp;forms displays all available custom forms for projects and issues.&nbsp; You must create a custom form before you can select it in this list. If there are no custom forms in Workfront, nothing displays in the drop-down list. To learn how to create custom forms, please refer to [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).  
![](assets/queueproperties-details2-350x174.png)

### Email Settings

You&nbsp;can allow issues to be added via email.&nbsp;This enables&nbsp;anyone with a valid Workfront account to send requests using email.

You can allow issues to be emailed into a Workfront project only if you designate the project as a Request Queue.

For more information about setting up an email account to allow users to send issues to a project in Workfront, see [Enable users to email an issue into a Request Queue project](enable-email-issues-into-projects.md).

To set up the email account associated with a Request Queue, specify the following information in the **Email Settings** area:

* **Allow Issues to be added via email:** Select this option to allow issues to be added via email.
* **POP username:** The full email address (including the domain name) where the POP account is created.&nbsp;For example,&nbsp; *workfront.market.research@gmail.com*.

  >[!IMPORTANT]
  >
  >
  >  
  >  
  >  * Do not use your personal email address as the POP username. Instead, create a new email address dedicated for only this purpose - to allow users to email issues to this account.&nbsp; 
  >  * It is very important that you are using a POP email account. No other email protocol is supported&nbsp;for this setup.
  >  
  >

* **POP password:** The password that corresponds with the user name that&nbsp;you created.
* **POP server:** The server of the third-party email service where the POP account lives.   
  For example, pop.gmail.com.

* **Enforce SSL/TLS:** Select this option if you want the connection to always be secure. Depending on the third-party email service that you are using, this might be a requirement.
* **Port Number:** If **Enforce SSL/TLS**&nbsp;is selected, specify 995 as the port number.

  If **Enforce SSL/TLS**&nbsp;is unselected, leave this field blank.

* Click **Test Configuration**&nbsp;and ensure that you get a message stating that the configuration was successful.  
  ![](assets/screen-shot-2013-08-22-at-9.56.10-am-350x408.png)

For more information about setting up the POP account, including specific information to the POP configuration settings, see [Enable users to email an issue into a Request Queue project](enable-email-issues-into-projects.md).
