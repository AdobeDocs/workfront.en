---
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: Overview of project owners and sponsors
description: You can designate a Project Owner and a Project Sponsor for a project. 
author: Alina
feature: Work Management
exl-id: e3e8be3f-105f-4702-8c93-ae8092f5d5d3
---
# Overview of project owners and sponsors

<!-- Audited: 1/2024 -->

You can designate a Project Owner and a Project Sponsor for a project.

The Project Owner is the individual responsible for the completion of the project on time and on budget.

The Project Sponsor is an important stakeholder for the project that has resources invested in the project. The project's completion typically benefits the Project Sponsor.

For information about how to update the Project Owner or Sponsor for a project, see [Update project owners and sponsors](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md).

## Project owners

You can designate the manager of a project by specifying a Project Owner on a project or a template.

You can define only one Project Owner for a project.

The following are possible using the Project Owner field:

* You can designate only one user as the Project Owner. 
* You can designate Project Owners as the hours approver for the project.
* You can designate the Project Owner as a generic approver when defining project, task, or issue approvals processes. For information about approvals, see [Edit an approval process](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

  >[!IMPORTANT]
  >
  >When you assign an approval to the Project Owner and no one is designated as the owner of a project, the approval is reassigned to the main Workfront administrator as indicated in the Customer Info section in the Setup area. For information, see [Configure basic information for your system](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
  >
 

* You can enable certain notifications that are delivered only to the Project Owner.

  For more information about email notifications, see the section [Configure event notifications for everyone in the system](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify) in the article [Configure event notifications for everyone in the system](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* You can display the Project Owner field in a report or list.

  You can also display the Project Owner field in a view, grouping, or prompt.

  For example, you can copy the following text mode expression into a filter to display projects owned by the logged in user:&nbsp;

  ```
  ownerID=$$USER.ID
  ```

 For more information about creating reports, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Owner of a project</h2>
<p>(NOTE:&nbsp;drafted and moved to its own article)</p>
<ol>
<li value="1">Go to the project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Owner</strong> field.</p> <p>Only active users can be specified as Project Owners.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Project sponsors

You can designate any user in the system as a Project Sponsor. The Project Sponsor is usually a manager, executive, or stakeholder who needs to know what is happening with the project.

Consider the following when assigning a Project Sponsor:

* The Project Sponsor does not gain any additional access to the project but is added to the email notifications of the project. For information about notifications, see the article [Configure event notifications for everyone in the system](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* You can designate only one Project Sponsor.
* You can designate the Project Sponsor as a generic approver when defining project, task, or issue approvals processes. For information about approvals, see [Edit an approval process](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

  >[!IMPORTANT]
  >
  >When you assign an approval to the Project Sponsor and no one is designated as the sponsor of a project, the approval is reassigned to the Project Owner. If no one is designated as the owner of the project, the approval is assigned to the Workfront administrator.

* You can display the Project Sponsor field in a report or list.

  You can also display the Project Sponsor field in a view, grouping, or prompt.

  For example, you can copy the following text mode expression into a filter to display projects sponsored by the logged in user:

  ```
  sponsorID=$$USER.ID
  ```

  &nbsp;

  For more information about creating reports, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Sponsor of a project </h2>
<p>(NOTE: drafted and moved to its own article) </p>
<ol>
<li value="1">Go to the Project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Sponsor</strong> field.</p> <p>Only active users can be specified as Project Sponsors.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->
