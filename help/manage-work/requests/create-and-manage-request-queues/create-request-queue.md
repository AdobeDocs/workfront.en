---
filename: create-request-queue
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Create a Request Queue
description: You can set up a Request Queue where users can enter occasional requests that are not planned work on a project. For example, a help desk request queue can be set up to capture all user requests that come to an IT department.
---

# Create a Request Queue

You can set up a Request Queue where users can enter occasional requests that are not planned work on a project. For example, a help desk request queue can be set up to capture all user requests that come to an IT department.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*

## Request queues overview

You set up a request queue as a project. When you designate the project as a Request Queue, the queue becomes accessible from the Requests area of *Adobe Workfront*. When you customize the Request Queue you are also customizing the form users fill out when they submit the requests.

This article describes how to create a request queue from an existing project. However, to build consistency for your request intake process or to add multiple layers to it for reporting purposes and better management, you can also configure additional building blocks of a request queue which are described in the following table. 

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Queue Details</td> 
   <td> <p>You must set up a project as a request queue in the Queue&nbsp;Details area.&nbsp;This step is mandatory. </p> <p>For more information, see the <a href="#creating-a-request-queue" class="MCXref xref">Create a Request Queue</a> section in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Topic Groups</td> 
   <td> <p>They are additional menus that classify requests based on common features. For example, for an IT Request Queue, you might want to have "On-site" and "Remote" topic groups. </p> <p>For more information, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Create Topic Groups</a>. </p> <p>This is optional.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Queue Topics</td> 
   <td> <p>They are additional menus that classify requests that belong to the same Topic&nbsp;Group based on common features. A&nbsp;topic group can contain several queue topics. </p> <p>For example, the "On-site" topic group for the IT&nbsp;Request Queue may contain the "Hardware", "Software" and "Network" queue topics. </p> <p>For more information, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Create Queue Topics</a>. </p> <p>This is optional.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Routing Rules</td> 
   <td> <p>They allow you to route each request to a user, job role, team, or to a project. </p> <p>For more information, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Create Routing Rules</a>. </p> <p>This is optional.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Create a Request Queue

When you set up a project as a Request Queue, the project status must be Current in order to display in the Requests area of *Workfront*.

To create a Request Queue:

<ol> 
 <li value="1"> <p>Go to the project that you want to set up as a Request Queue.</p> </li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional)&nbsp;Click <span class="bold">Project Details</span> in the left panel and add a <span class="bold">Description</span> to the project in the <span class="bold">Overview</span> area. This information displays on all new requests.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional)&nbsp;Click <span class="bold">Project Details</span> in the left panel and add a <span class="bold">Description</span> to the project in the <span class="bold">Overview</span> area. This information displays on all new requests.</p> </li> 
 <li value="3"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Queue Details</span> in the left panel. You might need to click <span class="bold">Show More</span>, then <span class="bold">Queue Details</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Queue Details</span> in the left panel. You might need to click <span class="bold">Show More</span>, then <span class="bold">Queue Details</span>.</p> <p>This opens the Queue Details <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      section 
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     section 
   </MadCap:conditionalText>. </p> </li> 
 <li value="4"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Specify the following information:</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Specify the following information:</p> 
  <ul> 
   <li><span class="bold">Publish as Help Request Queue:</span> Select this option to identify this project as a request queue. All incoming issues are considered Requests.<br>When this option is not selected, the project behaves like a standard project in <em>Workfront</em> and all incoming issues are issues.</li> 
   <li> <p><span class="bold">Who can add requests to this queue:</span> Select which users have access to add requests to this queue. You can allow the following groups of people to see the Request Queue in their Requests area of the Global Navigation Bar: </p> 
    <table cellspacing="0"> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td role="rowheader">Anyone </td> 
       <td>Any <em>Workfront</em> user with an active account can view this request queue and add requests to it</td> 
      </tr> 
      <tr> 
       <td role="rowheader">People with view access to this project</td> 
       <td>Users with View permissions to the project can view and add requests to this queue</td> 
      </tr> 
      <tr> 
       <td role="rowheader">People in this project's company</td> 
       <td>Users who belong to the company associated with this project can view and add requests to this queue. If there is a company associated with the project, the name of the company is listed in parentheses after this setting. </td> 
      </tr> 
      <tr> 
       <td role="rowheader">People in this project's group</td> 
       <td>Users who belong to the group associated with this project can view and add requests to this queue. If there is a group associated with the project, the name of the group is listed in parentheses after this setting. </td> 
      </tr> 
     </tbody> 
    </table> </li> 
   <li> <p><span class="bold">Share with these links:</span> The following options enable you to provide direct access to the Request Queue and the forms associated with it to users outside of <em>Workfront</em> or to <em>Workfront</em> users using an external page. For information about embedding a request queue in a dashboard as an external page, see <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md" class="MCXref xref">Embed a request queue in a dashboard</a>. </p> <p>Users must already have access rights to the Request Queue in order to gain direct access. Using either option described here does not automatically grant access to users. </p> <note type="tip">
     Users must first log in to 
     <em>Workfront</em> before gaining access to the request queue when they access the Request Queue page from another application.
    </note> 
    <ul> 
     <li> <p><span class="bold"> Direct Access URL:</span> When a user accesses this URL from a browser, the user is taken directly to the New Request <draft-comment>
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
          section 
        </MadCap:conditionalText>
       </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
         section 
       </MadCap:conditionalText>in the Requests area and this request is selected by default for them. </p> <draft-comment>
       <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png" style="width: 350;height: 118;"> </p>
      </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png" style="width: 350;height: 118;"> </p> <note type="note">
       You can display a Request Queue in a dashboard as an external page. In this case, the request queue is preselected, but you can select any other request queue from the Request&nbsp;Type field. users can change the Request&nbsp;Type. Navigation components of the Requests also display.
      </note> </li> 
     <li> <p> <span class="bold">Embed Code:</span> Use this HTML code to embed the request queue form as an iframe within any HTML page.<br>If users are not already authenticated to <em>Workfront</em> when they view the page where the code is embedded, the <em>Workfront</em> login dialog box is displayed. After users log in, the Request Queue form is displayed. </p> <draft-comment>
       <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png" style="width: 350;height: 210;"> </p>
      </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png" style="width: 350;height: 210;"> </p> <note type="note">
       When displaying a Request Queue in an iframe, only the request form displays, the request name is preselected and dimmed. User cannot change the Request type. Navigation components of the Requests area do not display. 
      </note> <p>In order for the request queue form to be displayed when using this embed code, you must enable the "Allow embedding of <em>Workfront</em> in an iframe" setting in your system setup. For more information about enabling embedding of <em>Workfront</em> in an iframe, see <a href="../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md" class="MCXref xref">Configure system security preferences</a>. If this setting is not enabled, the iframe is displayed as blank.</p> <p>You can adjust various aspects of how the embedded form is displayed, as follows:</p> 
      <table border="1" cellspacing="15"> 
       <col> 
       <col> 
       <thead> 
        <tr> 
         <th> <p><span class="bold">Functionality</span> </p> </th> 
         <th> <p><span class="bold">Solution</span> </p> </th> 
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
         <td> <p>Use the "path" parameter by adding the <code>showPreSelectedOptions=true</code> parameter to the <code>src URL</code>.</p> </td> 
        </tr> 
        <tr> 
         <td> <p>Detect when the form has been submitted</p> </td> 
         <td> <p>Add a "message" event listener to your web page's window and checking if <code>event.data.type</code> is <code>requestSubmitted</code>. <code>event.data.newIssueID</code> will be set to the ID of the created issue.</p> </td> 
        </tr> 
       </tbody> 
      </table> </li> 
    </ul> </li> 
  </ul> 
  <ul> 
   <li> <p><span class="bold">Request Types:</span> Select from the default options below. </p> <p>The <em>Workfront administrator</em> can rename the default request types. For more information about renaming the request types, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">Customize default issue types</a>.</p> 
    <ul> 
     <li>Change order</li> 
     <li>Issue</li> 
     <li>Requests</li> 
     <li> <p>Risk</p> <p>This is a required field and you must select at least one option. </p> </li> 
    </ul> <note type="note">
     Request&nbsp;Types display as a selection in the Requests area only if the Request Type is selected in both the Queue Details and the Queue Topic pages. For information about setting up the Queue Details area of a project, see 
     <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Create Queue Topics</a>. 
    </note> <p>Each type selected here will be available on the form (you can select more than one). Selecting more than one type can help organize multiple requests coming in.<br>For example, if you are using the form on a request queue for an IT project, the following request types can come in to the queue: hardware, software, bug fixes, and issues.<br></p> </li> 
   <li><span class="bold">Default Duration:</span> The default duration is the length of time it typically takes to complete an issue. This becomes the default for all incoming issues and can be modified manually. Duration is generally set in hours, days, or weeks. The Default Duration of an issue is the same as the Planned Hours on the issue. The Planned Completion Date of the issue calculates based on this field.<br>The default for the issue Duration is 1 day or 8 hours. If your <em>Workfront administrator</em> set the Typical Hours per Work Day as less than 8 hours, the Default Duration for issues is still 8 hours. For example, if the Typical Hours per Work Day is set to 7 hours, the Default Duration for issues is 1.14 Days or 8 hours. For more information about how to set up the system Typical Hours per Work Day, see the "Timeline Calculations" section in the article <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</li> 
   <li><span class="bold">People from the same company will inherit the same permissions for all requests.:</span> When selected, all requests submitted to the queue are visible for users in the same company. Users can view these requests in the All Requests <draft-comment>
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       section 
     </MadCap:conditionalText>
    </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      section 
    </MadCap:conditionalText>, located within the Requests area. At the time that this setting is enabled or disabled, it impacts all future requests; it does not retroactively impact information. </li> 
   <li> <p><span class="bold">When someone makes a request, automatically grant:</span> When a user makes a request to the request queue, the user is automatically granted the level of permission that you choose to that request. Select from the following permissions levels:<br><span class="bold">- View</span><br><span class="bold">- Contribute</span><br><span class="bold">- Manage</span></p> <p>For information about the <em>Workfront</em> permissions model, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects in Adobe Workfront</a>. <br>Setting permissions here saves time, rather than having to grant permissions for each individual incoming request. Choosing this option impacts all future requests, but does not retroactively impact existing requests. </p> </li> 
   <li> <p><span class="bold">Default Approval</span>: Associate an approval process with this request queue. Only Issue Approval Processes are visible in this drop-down menu. All issues submitted to this queue will be associated with this approval process. Your <em>Workfront administrator</em> must define system-level approval processes before you can associate them with request queues. <span> Users with administrative access to Approval processes can also create group-specific approval processes.</span> </p> <note type="important">
     If the group of the project changes, the group-specific approval process attached to existing issues becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see 
     <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">How group and approval process changes affect assigned approval processes</a>.
    </note> <p>If you have multiple queue topics associated with a request queue, we recommend that you associate approval processes with the queue topics instead. For more information about creating queue topics, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Create Queue Topics</a>. </p> 
    <div> 
     <p>Consider the following when adding approval processes to request queues: </p> 
     <ul style="list-style-type: circle;"> 
      <li>Only active approval processes display in the list. </li> 
      <li> <p>System-wide and group-specific approval processes display in the list. An approval process associated with a group other than that of the project does not display in the list.</p> </li> 
     </ul> 
    </div> </li> 
   <li><span class="bold">Default Route</span>: Associate a Routing Rule with this request queue. Use Routing Rules to automatically assign new issues submitted to a Request Queue to the correct resource (user, job role, or team), and to the correct project. All issues submitted to this queue will be associated with this Routing Rule. You must configure Routing Rules before you can associate them with request queue.<br>If you have multiple queue topics associated with a request queue, we recommend that you associate routing rules with the queue topics instead. For more information about creating routing rules, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Create Routing Rules</a>.</li> 
   <li> <p><span class="bold">New Issue Fields:</span> In the Show the following selected fields to all users section, select any fields that you want to be visible to all users who submit a request to the project or add an issue to the project or the tasks. </p> <note type="tip">
     New Issue Fields selected in the Queue&nbsp;Details section are also associated with any new issue added to the project or to the tasks in the Issues 
     <draft-comment>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
        section 
      </MadCap:conditionalText>
     </draft-comment>
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       section 
     </MadCap:conditionalText>.
    </note> <draft-comment>
     <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span>W</span><span><span data-mc-edit-date="2021-04-07T15:35:49.1747020-04:00" data-mc-editor="alinawilson" data-mc-comment="drafted and stays yellow and QS and will replace the first sentence with 21.2 preview" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-07T15:35:35.9979889-04:00">hen</span><span> you enable any of the Assigned to,&nbsp;Job Role, or the Team fields, they are always renamed to Assignments in the request form, but you can only specify the type of assignment selected here.</span></span> </p>
    </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span>W</span><span><span data-mc-edit-date="2021-04-07T15:35:49.1747020-04:00" data-mc-editor="alinawilson" data-mc-comment="drafted and stays yellow and QS and will replace the first sentence with 21.2 preview" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-07T15:35:35.9979889-04:00">hen</span><span> you enable any of the Assigned to,&nbsp;Job Role, or the Team fields, they are always renamed to Assignments in the request form, but you can only specify the type of assignment selected here.</span></span> </p> <draft-comment>
     <p class="example" data-mc-autonum="<b>Example: </b>" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span class="autonumber"><span><b>Example: </b></span></span><span>If you selected Assigned To in the Queue Details area, you can enter only users in the Assignments field on the request form. In this case, you cannot enter job roles or a team.</span> </p>
    </draft-comment><p class="example" data-mc-autonum="<b>Example: </b>" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span class="autonumber"><span><b>Example: </b></span></span><span>If you selected Assigned To in the Queue Details area, you can enter only users in the Assignments field on the request form. In this case, you cannot enter job roles or a team.</span> </p> </li> <draft-comment>
    <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p><span><b>Documents</b>: If you select to display the Documents section in the new request form, select where the document uploading section should be positioned. Select from the following:</span> </p> 
     <table cellspacing="0"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">After custom forms</td> 
        <td><span>The Documents section displays at the bottom of the request form.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Before custom forms</td> 
        <td> <p><span>The Documents section displays between the <em>Workfront</em> fields and the custom fields of the request form.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table> <p> <img src="assets/nwe-new-issue-fields-area-with-documents-350x167.png" style="width: 350;height: 167;"> </p> </li>
   </draft-comment>
   <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p><span><b>Documents</b>: If you select to display the Documents section in the new request form, select where the document uploading section should be positioned. Select from the following:</span> </p> 
    <table cellspacing="0"> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td role="rowheader">After custom forms</td> 
       <td><span>The Documents section displays at the bottom of the request form.</span> </td> 
      </tr> 
      <tr> 
       <td role="rowheader">Before custom forms</td> 
       <td> <p><span>The Documents section displays between the <em>Workfront</em> fields and the custom fields of the request form.</span> </p> </td> 
      </tr> 
     </tbody> 
    </table> <p> <img src="assets/nwe-new-issue-fields-area-with-documents-350x167.png" style="width: 350;height: 167;"> </p> </li> 
   <li> <p><span class="bold">Show all selected and unselected fields to:</span> Select which users you want to see all the fields on the form. The following options control the access to the fields on the form.</p> 
    <table cellspacing="0"> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td role="rowheader">All Users (Plan Licenses)</td> 
       <td>All users who have a Plan license can see the selected as well as the unselected fields.</td> 
      </tr> 
      <tr> 
       <td role="rowheader">People with view access to this project (Plan License)</td> 
       <td>Those users with a Plan license that also have View rights to this project can see the selected as well as the unselected fields. The rest of the users who can submit requests to this project can see just the selected fields.</td> 
      </tr> 
      <tr> 
       <td role="rowheader">No Users</td> 
       <td>No users can see the unselected fields. All users who can submit requests to this project can only see the fields selected. </td> 
      </tr> 
     </tbody> 
    </table> </li> 
   <li> <p><span class="bold">Custom Forms</span>: Select a custom form to associate with the Request Queue. Only Issue Custom Forms are available to select from this drop-down menu. All issues submitted to the Request Queue will have the selected forms associated with them.<br>If you have multiple Queue Topics associated with a Request Queue, we recommend that you associate custom forms with the Queue Topics instead. For more information about creating sub-sections for the Request Queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Create Queue Topics</a>.</p> <p>If you have multiple custom forms associated with the Request Queue, drag and drop the forms to sort them in the desired order, in the <span class="bold">Reorder Forms</span> section.</p> <note type="tip">
     Custom forms added to the Queue&nbsp;Details section are also associated with any new issue added to the project or the tasks in the Issues 
     <draft-comment>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
        section. 
      </MadCap:conditionalText>
     </draft-comment>
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       section. 
     </MadCap:conditionalText>
    </note> </li> 
   <li><span class="bold">Allow Issues to be added via email:</span> Select this option to allow requests to be submitted via email.<br>For more information, see <a href="../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md" class="MCXref xref">Enable users to email an issue into a Request Queue project</a>. </li> 
  </ul> </li> 
 <li value="5">Click <span class="bold">Save</span>.<br>Your project has now been configured to be a Request Queue and users can now add requests to it. </li> 
 <li value="6"> <p>(Optional) To enhance the Request Queue functionality, build additional sub-sections for your queue, as well as rules to route the incoming requests to the correct team, assignee or project. </p> <p>For information about creating sub-sections for the Request Queue, see the articles <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Create Queue Topics</a> and <a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Create Topic Groups</a>.<br>For information about routing the requests to the appropriate assignee, team, and appropriate project, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Create Routing Rules</a>.</p> </li> 
</ol>

