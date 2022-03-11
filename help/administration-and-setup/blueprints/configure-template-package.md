---
filename: configure-template-package
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Configure a blueprint
description: You can configure details of the project template or organizational structure before you install the blueprint.
---

# Configure a blueprint

You can configure details of the project template or organizational structure before you install the blueprint.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System administrator</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configure a project template blueprint

<ol> 
 <li value="1"> <p>Find the blueprint you want to use.</p> </li> 
 <li value="2"> <p>Click <span class="uitext">Install</span>, then choose an environment:<br></p> 
  <table> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><span class="uitext">Production</span> </td> 
     <td>Production is your live environment. </td> 
    </tr> 
    <tr> 
     <td><span class="uitext">Sandbox Preview</span> </td> 
     <td>The Sandbox Preview is a testing environment that serves as a replica of your live environment and is refreshed each weekend by Workfront. </td> 
    </tr> 
    <tr> 
     <td><span class="uitext">Sandbox 1 & 2</span> </td> 
     <td>The Custom Refresh Sandbox is a separate testing environment which is refreshed manually by you. There is an additional cost to obtain a Custom Refresh Sandbox.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="3">Continue with the following sections:</li> 
 <ul> 
  <li><a href="#template2" class="MCXref xref">Template preferences</a> </li> 
  <li><a href="#role" class="MCXref xref">Role mapping</a> </li> 
  <li><a href="#team" class="MCXref xref">Team mapping</a> </li> 
  <li><a href="#company" class="MCXref xref">Company mapping</a> </li> 
  <li><a href="#group" class="MCXref xref">Group mapping</a> </li> 
 </ul> 
</ol>

## Template preferences

Choose how you want to install the template.

You can also designate template ownership before you install the blueprint. You can make changes to these fields after the template is installed. For more information, see [Edit project templates](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

![Template Preferences section](assets/blueprints-templatepreferences-350x147.png)

<ol> 
 <li value="1"> <p>In the <span class="uitext">Install Preferences section</span>, specify a new template name.</p> </li> 
 <li value="2"> <p>Specify the following:<br></p> 
  <table> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><span class="uitext">Template owner</span> </td> 
     <td>This person receives Manage permissions on the template and will become the Project owner when the template is used to create a project.</td> 
    </tr> 
    <tr> 
     <td><span class="uitext">Template sponsor</span> </td> 
     <td>This person is usually a manager, executive, or stakeholder who needs to know what is happening with the project. The Project Sponsor does not gain any additional access to the project but is added to the email notifications for the project.</td> 
    </tr> 
    <tr> 
     <td><span class="uitext">Portfolio</span> </td> 
     <td>This is the portfolio the project will belong to when it's created.</td> 
    </tr> 
    <tr> 
     <td><span class="uitext">Program</span> </td> 
     <td>This is the program the project will belong to when it's created.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="3"> <p>Select whether the template is installed as active or inactive.</p> </li> 
 <li value="4"> <p>Select whether you want to use defined new issue preferences, if preferences are available.</p> <p> Click <span class="bold">See issue preferences</span> to review the specific preferences that will install with the blueprint. Projects created from the imported template use these preferences for new issues added in the Issues section.</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Queue topic groups</td> 
     <td> <p>Queue topic groups define the highest level of categories for the issues or requests. Users view topic groups as menu options when selecting where to submit requests. A topic group can contain multiple queue topics. For more information, see <a href="../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Create Topic Groups</a>. </p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Queue topics </td> 
     <td> <p>Queue topics work in conjunction with routing rules to assign issues or requests. They are the menu options that users select when entering an issue or request, after selecting a topic group. For more information, see <a href="../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Create Queue Topics</a>. </p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Routing rules </td> 
     <td>Routing rules send issues or requests to specific job roles , users, or teams. They can also send the requests to specific projects, other than the one associated with the request queue. For more information, see <a href="../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Create Routing Rules</a>. </td> 
    </tr> 
   </tbody> 
  </table> 
  <div class="example" data-mc-autonum="<b>Example: </b>">
   <span class="autonumber"><span><b>Example: </b></span></span> 
   <p>The new issue preferences in this blueprint provide four queue topics. The user selects one of these topics when creating an issue. (Because only one topic group exists, it is automatically applied and the user does not have to select it.) When the user completes and submits the issue, routing rules determine which job role or team it is assigned to.</p> 
   <p> <img src="assets/blueprints-issueprefsdetails-350x202.png" alt="Sample new issue preferences" style="width: 350;height: 202;"> </p> 
   <p> <img src="assets/blueprints-newissueqtopicsexample-350x204.png" style="width: 350;height: 204;" alt="Queue topics for new issue"> </p> 
   <p> <img src="assets/blueprints-projectshowsissueassignment-350x71.png" alt="Issue routed to job role" style="width: 350;height: 71;"> </p> 
  </div> 
  <div class="tips" data-mc-autonum="<b>Tips: </b>">
   <span class="autonumber"><span><b>Tips: </b></span></span> 
   <ul> 
    <li>Using the issue preferences helps create consistency in the way that new issues or requests are captured on your projects.</li> 
    <li>Setting these preferences does not automatically make the projects created from the template into request queues. For information about setting up a request queue, see <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>.</li> 
    <li>Not all blueprints contain new issue preferences.</li> 
   </ul> 
  </div> </li> 
</ol>

## Role mapping

>[!NOTE]
>
>This section may not appear in some blueprints.

Some templates include prescribed job roles. Job roles help you assign the right people when the template is converted to a project. You can customize how roles are mapped before you install the blueprint. Click `See role descriptions` to learn more about the roles available in the blueprint.

The blueprint searches by the role name to see if any existing roles match. The search is case sensitive, so names must be an exact match. If no existing roles match, you can have the blueprint create them for you.

![Role Mapping section](assets/blueprints-rolemapping-350x123.png)

1. If a role exists, you can choose one of the following options:

  1. `Create a new role with a different name`, then type the name in the text box.
  1. `Use existing role`, then select a role in the selection box.
  1. `Do not use mapped role`. This option is not recommended because some tasks will not have roles assigned.

1. If a role does not exist, you can choose one of the following options:

  1. `Create a new role`. This option creates the role the blueprint recommends.
  1. `Create a new role with a different name`, then type the name in the text box.
  1. `Use existing role`, then select a role in the selection box.
  1. `Do not use mapped role`. This option is not recommended because some tasks will not have roles assigned.

>[!NOTE]
>
>The installation process does not apply roles to specific people. You should verify the people in those roles after installing the blueprint solution and assign people if necessary. For information, see [Actions to take after installing a blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

For more information about job roles in Workfront, see [Create and manage job roles](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## Team mapping

>[!NOTE]
>
>This section may not appear in some blueprints.

Some templates include prescribed teams. Work assigned to a team can be completed by any member of the team. You can customize how teams are mapped before you install the blueprint. Click `See team descriptions` to learn more about the teams available in the blueprint.

The blueprint searches by the team name to see if any existing teams match. The search is case sensitive, so names must be an exact match. If no existing teams match, you can have the blueprint create them for you.

![Team Mapping section](assets/blueprints-teammapping-350x121.png)

1. If a team exists, you can choose one of the following options:

  1. `Create a new team with a different name`, then type the name in the text box.
  1. `Use existing team`, then select a team in the selection box.
  1. `Do not use mapped team`. This option is not recommended because some tasks will not have teams assigned.

1. If a team does not exist, you can choose one of the following options:

  1. `Create a new team`. This option creates the team the blueprint recommends.
  1. `Create a new team with a different name`, then type the name in the text box.
  1. `Use existing team`, then select a team in the selection box.
  1. `Do not use mapped team`. This option is not recommended because some tasks will not have teams assigned.

>[!NOTE]
>
>The installation process does not add people to the teams. You should verify the people on the teams after installing the blueprint solution and assign people if necessary. For information, see [Actions to take after installing a blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

For more information about how teams function in Workfront, see [Create and manage teams](../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

## Company mapping

>[!NOTE]
>
>This section may not appear in some blueprints.

Some blueprints include prescribed companies. A company is an organizational unit that can represent your organization, a department within the organization, or a client you work with. You can customize how companies are mapped before you install the blueprint. Click `See company descriptions` to learn more about the companies available in the blueprint.

The blueprint searches by the company name to see if any existing companies match. The search is case sensitive, so names must be an exact match. If no existing companies match, you can have the blueprint create them for you. The primary company in the blueprint is mapped to the primary company in your environment, even if they do not have the same name.

![Company Mapping section](assets/blueprints-companymapping-350x101.png)

1. If a company exists, you can choose one of the following options:

  1. `Create a new company with a different name`, then type the name in the text box.
  1. `Use existing company`, then select a company in the selection box.  
     The primary company in the blueprint is mapped to the primary company in your environment, even if they do not have the same name.
  1. `Do not use mapped company`. This option is not recommended, because the company references in other objects will be empty.

1. If a company does not exist, you can choose one of the following options:

  1. `Create a new company`. This option creates the company the blueprint recommends.
  1. `Create a new company with a different name`, then type the name in the text box.
  1. `Use existing company`, then select a company in the selection box.
  1. `Do not use mapped company`. This option is not recommended, because the company references in other objects will be empty.

>[!NOTE]
>
>To configure the companies after installing the blueprint, see [Actions to take after installing a blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

For information about associating a template with a company, see [Edit project templates](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

For information about how companies function in Workfront, see [Create and edit companies](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Group mapping

>[!NOTE]
>
>This section may not appear in some blueprints.

Some blueprints include prescribed groups. A group is a group of users that coincides with your departmental structure. Groups are similar to but distinct from teams and companies in Workfront. You can customize how groups are mapped before you install the blueprint. Click `See group descriptions` to learn more about the groups available in the blueprint.

The blueprint searches by the group name to see if any existing groups match. The search is case sensitive, so names must be an exact match. If no existing groups match, you can have the blueprint create them for you.

![Group Mapping section](assets/blueprints-groupmapping-350x225.png)

<ol> 
 <li value="1"> <p>If a group exists, you can select <span class="bold">Remap Group</span> and choose one of the following options:</p> 
  <ol> 
   <li value="1"> <p><span class="bold">Create a new group with a different name</span>, then type the name to assign to this group. References to the group in the blueprint definition will be associated to this new group instead.</p> </li> 
   <li value="2"> <p><span class="bold">Replace with an existing group</span>, then search for and select a group in the selection box.</p> <note type="note">
     You cannot rename an existing group.
    </note> </li> 
  </ol> </li> 
 <li value="2"> <p>If a group does not exist, you can:</p> 
  <ol> 
   <li value="1"> <p>Change the suggested group name by typing it in the text box.</p> </li> 
   <li value="2"> <p>Select <span class="bold">Remap Group</span> and choose <span class="uitext">Replace with an existing group</span>, then search for and select a group in the selection box.</p> </li> 
   <li value="3"> <p>Select <span class="bold">Remap Group</span> and choose <span class="bold">Insert under an existing group</span>, then search for and select a group in the selection box. This option creates a new subgroup under the existing group.</p> </li> 
  </ol> </li> 
</ol>

>[!NOTE]
>
>To configure the groups after installing the blueprint, see [Actions to take after installing a blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

For information about using groups in Workfront, see [Groups overview](../../administration-and-setup/manage-groups/groups-overview/groups.md).
