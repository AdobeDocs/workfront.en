---
filename: project-owners-and-sponsors
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: Overview of project owners and sponsors
description: You can designate a Project Owner and a Project Sponsor for a project.
---

# Overview of project owners and sponsors

You can designate a Project&nbsp;Owner and a Project Sponsor for a project.

The Project Owner is the individual responsible for the completion of the project on time and on budget.

The Project Sponsor is an important stakeholder for the project that has resources invested in the project. The project's completion typically benefits the Project Sponsor.

For information about how to update the Project Owner or Sponsor for a project, see [Update project owners and sponsors](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md).

## Project owners

You can designate the manager of a project by specifying a Project Owner on a project or a template.&nbsp;

You can define only one Project Owner for a project.&nbsp;

The following are possible using the Project Owner field:&nbsp;

<ul> 
 <li> <p>You can designate only one user as the Project&nbsp;Owner. </p> </li> 
 <li>You can designate Project Owners as the hours approver for the project.</li> 
 <li> <p>You can designate the Project Owner as a generic approver when defining project, task, or issue approvals processes. For information about approvals, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md" class="MCXref xref" xrefformat="{para}">Edit an approval process</a>. </p> <note type="important"> 
   <p>When you assign an approval to the Project Owner and no one is designated as the owner of a project, the approval is reassigned to the main <em>Workfront administrator</em> as indicated in the Customer Info section in the Setup area. For information, see <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref" xrefformat="{para}">Configure basic information for your system</a>.</p> 
   <p>&nbsp;</p> 
   <p>&nbsp;</p> 
   <p> <br> </p> 
  </note> </li> 
 <li> <p>You can enable certain notifications that are delivered only to the Project Owner.</p> <p>For more information about email notifications, see the section <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify" class="MCXref xref" xrefformat="{para}">Configure event notifications for everyone in the system</a> in the article <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref" xrefformat="{para}">Configure event notifications for everyone in the system</a>.</p> </li> 
 <li> <p>You can display the Project Owner field in a report or list. </p> <p>You can also display the Project Owner field in a view, grouping, or prompt.</p> <p>For example, you can copy the following text mode expression into a filter to display projects owned by the logged in user:&nbsp;<code>ownerID=$$USER.ID</code>&nbsp;</p> <p>For more information about creating reports, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref" xrefformat="{para}">Create a custom report</a>.</p> </li> 
</ul>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Owner of a project</h2>
<ol>
<li value="1">Go to the project you want to update.</li>
<li value="2"> <draft-comment>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Click
<span class="bold">Project&nbsp;Details</span> in the left panel.
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Click
<span class="bold">Project&nbsp;Details</span> in the left panel.
</MadCap:conditionalText></li>
<li value="3"> <draft-comment>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Click&nbsp;the
<span class="bold">Edit</span> icon
<img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;
<span class="bold">Overview</span>.
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Click&nbsp;the
<span class="bold">Edit</span> icon
<img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;
<span class="bold">Overview</span>.
</MadCap:conditionalText> </li>
<li value="4"> <p>Specify the name of a user for the <span class="bold">Project Owner</span> field.</p> <p>Only active users can be specified as Project Owners.</p> </li>
<li value="5"> <draft-comment>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Click&nbsp;
<span class="bold">Save Changes</span>.
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Click&nbsp;
<span class="bold">Save Changes</span>.
</MadCap:conditionalText></li>
</ol>
</div>
-->

## Update the Project Owner of a project

<ol> 
 <li value="1">Go to the project you want to update.</li> 
 <li value="2"> <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click 
   <span class="bold">Project&nbsp;Details</span> in the left panel. 
  </MadCap:conditionalText></li> 
 <li value="3"> <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click&nbsp;the 
   <span class="bold">Edit</span> icon 
   <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;
   <span class="bold">Overview</span>. 
  </MadCap:conditionalText> </li> 
 <li value="4"> <p>Specify the name of a user for the <span class="bold">Project Owner</span> field.</p> <p>Only active users can be specified as Project Owners.</p> </li> 
 <li value="5"> <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click&nbsp;
   <span class="bold">Save Changes</span>. 
  </MadCap:conditionalText></li> 
</ol>

## Project sponsors

You can designate any user in the system as a Project Sponsor.&nbsp;The Project Sponsor is usually a manager, executive, or stakeholder who needs to know what is happening with the project.

Consider the following when assigning a Project Sponsor:

* The Project Sponsor does not&nbsp;gain&nbsp;any additional access to the project but is added to the email notifications of the project. For information about notifications, see the article [Configure event notifications for everyone in the system](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

<ul> 
 <li> <p>You can designate only one Project Sponsor.</p> </li> 
 <li> <p>You can designate the Project Sponsor as a generic approver when defining project, task, or issue approvals processes. For information about approvals, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md" class="MCXref xref" xrefformat="{para}">Edit an approval process</a>. </p> <note type="important">
   When you assign an approval to the Project Sponsor and no one is designated as the sponsor of a project, the approval is reassigned to the Project Owner. If no one is designated as the owner of the project, the approval is assigned to the 
   <em>Workfront administrator</em>. 
   <br>
  </note> </li> 
 <li> <p>You can display the Project&nbsp;Sponsor field in a report or list.</p> <p>You can also display the Project Sponsor field in a view, grouping, or prompt.</p> <p>For example, you can copy the following text mode expression into a filter to display projects sponsored by the logged in user:&nbsp;<code>sponsorID=$$USER.ID</code>&nbsp;</p> <p>For more information about creating reports, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref" xrefformat="{para}">Create a custom report</a>.</p> </li> 
</ul>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Sponsor of a project </h2>
<ol>
<li value="1">Go to the Project you want to update.</li>
<li value="2"> <draft-comment>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Click
<span class="bold">Project&nbsp;Details</span> in the left panel.
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Click
<span class="bold">Project&nbsp;Details</span> in the left panel.
</MadCap:conditionalText></li>
<li value="3"> <draft-comment>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Click&nbsp;the
<span class="bold">Edit</span> icon
<img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;
<span class="bold">Overview</span>.
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Click&nbsp;the
<span class="bold">Edit</span> icon
<img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;
<span class="bold">Overview</span>.
</MadCap:conditionalText> </li>
<li value="4"> <p>Specify the name of a user for the <span class="bold">Project Sponsor</span> field.</p> <p>Only active users can be specified as Project Sponsors.</p> </li>
<li value="5"> <draft-comment>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Click&nbsp;
<span class="bold">Save Changes</span>.
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Click&nbsp;
<span class="bold">Save Changes</span>.
</MadCap:conditionalText></li>
</ol>
</div>
-->

## Update the Project Sponsor of a project

<ol> 
 <li value="1">Go to the Project you want to update.</li> 
 <li value="2"> <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click 
   <span class="bold">Project&nbsp;Details</span> in the left panel. 
  </MadCap:conditionalText></li> 
 <li value="3"> <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click&nbsp;the 
   <span class="bold">Edit</span> icon 
   <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;
   <span class="bold">Overview</span>. 
  </MadCap:conditionalText> </li> 
 <li value="4"> <p>Specify the name of a user for the <span class="bold">Project Sponsor</span> field.</p> <p>Only active users can be specified as Project Sponsors.</p> </li> 
 <li value="5"> <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click&nbsp;
   <span class="bold">Save Changes</span>. 
  </MadCap:conditionalText></li> 
</ol>

