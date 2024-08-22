---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Configure a Blueprint
description: You can configure details of the project template or organizational structure before you install the blueprint.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: df10bc8f-b980-4c61-ae6d-bcea03103738
---
# Configure a blueprint

You can configure details of a blueprint before you install it. Project template and organizational structure blueprint types usually require some preferences to be set and some properties to be mapped. Other blueprint types may not require configuration and you will install them as-is. For more information about installation, see [Install a blueprint](/help/quicksilver/administration-and-setup/blueprints/blueprints-install.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>
   <p>New: Standard</p>
   <p>or</p>
   <p>Current: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td>You must be a [!DNL Workfront] administrator. </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configure a project template blueprint

1. Find the blueprint you want to use.
1. Click **[!UICONTROL Install]**, then choose an environment:

   <table style="table-layout:auto">
        <tr>
        <td><strong>Production</strong></td>
        <td>Production is your live environment.</td>
    </tr>
    <tr>
        <td><strong>Sandbox Preview</strong></td>
        <td>The Sandbox Preview is a testing environment that serves as a replica of your live environment and is refreshed each weekend by Workfront.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 &amp; 2</strong></td>
        <td>The Custom Refresh Sandbox is a separate testing environment which is refreshed manually by you. There is an additional cost to obtain the Custom Refresh Sandbox.</td>
    </tr>
   </table>

1. Continue with the following sections:

   * [[!UICONTROL Template preferences]](#template-preferences)
   * [[!UICONTROL Role mapping]](#role-mapping)
   * [[!UICONTROL Team mapping]](#team-mapping)
   * [[!UICONTROL Company mappin]g](#company-mapping)
   * [[!UICONTROL Group mapping]](#group-mapping)

## [!UICONTROL Template preferences] {#template-preferences}

Choose how you want to install the template.

You can also designate template ownership before you install the blueprint. You can make changes to these fields after the template is installed. For more information, see [Edit project templates](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

![[!UICONTROL Template Preferences] section](assets/Blueprints_TemplatePreferences.png)

1. In the [!UICONTROL Template Preferences] section, specify a new template name.
1. Specify the following:

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Template owner]<strong></td>
        <td>This person receives [!UICONTROL Manage] permissions on the template and will become the Project owner when the template is used to create a project.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Template sponsor]</strong></td>
        <td>This person is usually a manager, executive, or stakeholder who needs to know what is happening with the project. The Project Sponsor does not gain any additional access to the project but is added to the email notifications for the project.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Portfolio]</strong></td>
        <td>This is the portfolio the project will belong to when it's created.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Program]</strong></td>
        <td>This is the program the project will belong to when it's created.</td>
    </tr>
   </table>

1. Select whether the template is installed as active or inactive.
1. Select whether you want to use defined new issue preferences, if preferences are available.

   Click **[!UICONTROL See issue preferences]** to review the specific preferences that will install with the blueprint. Projects created from the imported template use these preferences for new issues added in the [!UICONTROL Issues] section.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Queue topic groups</strong></td> 
      <td> <p>Queue topic groups define the highest level of categories for the issues or requests. Users view topic groups as menu options when selecting where to submit requests. A topic group can contain multiple queue topics. For more information, see <a href="../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Create Topic Groups</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Queue topics</strong></td> 
      <td> <p>Queue topics work in conjunction with routing rules to assign issues or requests. They are the menu options that users select when entering an issue or request, after selecting a topic group. For more information, see <a href="../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Create Queue Topics</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Routing rules</strong></td> 
      <td>Routing rules send issues or requests to specific job roles , users, or teams. They can also send the requests to specific projects, other than the one associated with the request queue. For more information, see <a href="../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Create Routing Rules</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!INFO]
   >
   >**Example:** The new issue preferences in this blueprint provide four queue topics. The user selects one of these topics when creating an issue. (Because only one topic group exists, it is automatically applied and the user does not have to select it.) When the user completes and submits the issue, routing rules determine which job role or team it is assigned to.
   >![Sample new issue preferences](assets/Blueprints_IssuePrefsDetails.png)
   >![Queue topics for new issue](assets/blueprints-newissueqtopicsexample-350x204.png)
   >![Issue routed to job role](assets/Blueprints_ProjectShowsIssueAssignment.png)

   >[!TIP]
   >
   >* Using the issue preferences helps create consistency in the way that new issues or requests are captured on your projects.
   >* Setting these preferences does not automatically make the projects created from the template into request queues. For information about setting up a request queue, see [Create a Request Queue](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   >* Not all blueprints contain new issue preferences.


## [!UICONTROL Role mapping] {#role-mapping}

>[!NOTE]
>
>This section may not appear in some blueprints.

Some templates include prescribed job roles. Job roles help you assign the right people when the template is converted to a project. You can customize how roles are mapped before you install the blueprint. Click **[!UICONTROL See role descriptions]** to learn more about the roles available in the blueprint.

The blueprint searches by the role name to see if any existing roles match. The search is case sensitive, so names must be an exact match. If no existing roles match, you can have the blueprint create them for you.

![[!UICONTROL Role Mapping] section](assets/Blueprints_RoleMapping.png)

1. If a role exists, you can choose one of the following options:

   1. Create a new role with a different name, then type the name in the text box.
   1. Use existing role, then select a role in the selection box.
   1. Do not use mapped role. This option is not recommended because some tasks will not have roles assigned.

1. If a role does not exist, you can choose one of the following options:

   1. Create a new role. This option creates the role the blueprint recommends.
   1. Create a new role with a different name, then type the name in the text box.
   1. Use existing role, then select a role in the selection box.
   1. Do not use mapped role. This option is not recommended because some tasks will not have roles assigned.

>[!NOTE]
>
>The installation process does not apply roles to specific people. You should verify the people in those roles after installing the blueprint solution and assign people if necessary. For information, see [Actions to take after installing a blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

For more information about job roles in [!DNL Workfront], see [Create and manage job roles](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## [!UICONTROL Team mapping] {#team-mapping}

>[!NOTE]
>
>This section may not appear in some blueprints.

Some templates include prescribed teams. Work assigned to a team can be completed by any member of the team. You can customize how teams are mapped before you install the blueprint. Click **[!UICONTROL See team descriptions]** to learn more about the teams available in the blueprint.

The blueprint searches by the team name to see if any existing teams match. The search is case sensitive, so names must be an exact match. If no existing teams match, you can have the blueprint create them for you.

![[!UICONTROL Team Mapping] section](assets/Blueprints_TeamMapping.png)

1. If a team exists, you can choose one of the following options:

   1. Create a new team with a different name, then type the name in the text box.
   1. Use [!UICONTROL existing team], then select a team in the selection box.
   1. Do not use mapped team. This option is not recommended because some tasks will not have teams assigned.

1. If a team does not exist, you can choose one of the following options:

   1. Create a new team. This option creates the team the blueprint recommends.
   1. Create a new team with a different name, then type the name in the text box.
   1. Use [!UICONTROL existing team], then select a team in the selection box.
   1. Do not use mapped team. This option is not recommended because some tasks will not have teams assigned.

>[!NOTE]
>
>The installation process does not add people to the teams. You should verify the people on the teams after installing the blueprint solution and assign people if necessary. For information, see [Actions to take after installing a blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

For more information about how teams function in [!DNL Workfront], see [Create and manage teams](../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

## Company mapping {#company-mapping}

>[!NOTE]
>
>This section may not appear in some blueprints.

Some blueprints include prescribed companies. A company is an organizational unit that can represent your organization, a department within the organization, or a client you work with. You can customize how companies are mapped before you install the blueprint. Click **[!UICONTROL See company descriptions]** to learn more about the companies available in the blueprint.

The blueprint searches by the company name to see if any existing companies match. The search is case sensitive, so names must be an exact match. If no existing companies match, you can have the blueprint create them for you. The primary company in the blueprint is mapped to the primary company in your environment, even if they do not have the same name.

![[!UICONTROL Company Mapping] section](assets/Blueprints_CompanyMapping.png)

1. If a company exists, you can choose one of the following options:

   1. Create a new company with a different name, then type the name in the text box.
   1. Use existing company, then select a company in the selection box.\

      The primary company in the blueprint is mapped to the primary company in your environment, even if they do not have the same name.
   1. Do not use mapped company. This option is not recommended, because the company references in other objects will be empty.

1. If a company does not exist, you can choose one of the following options:

   1. Create a new company. This option creates the company the blueprint recommends.
   1. Create a new company with a different name, then type the name in the text box.
   1. Use existing company, then select a company in the selection box.
   1. Do not use mapped company. This option is not recommended, because the company references in other objects will be empty.

>[!NOTE]
>
>To configure the companies after installing the blueprint, see [Actions to take after installing a blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

For information about associating a template with a company, see [Edit project templates](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

For information about how companies function in [!DNL Workfront], see [Create and edit companies](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## [!UICONTROL Group mapping] {#group-mapping}

>[!NOTE]
>
>This section may not appear in some blueprints.

Some blueprints include prescribed groups. A group is a group of users that coincides with your departmental structure. Groups are similar to but distinct from teams and companies in Workfront. You can customize how groups are mapped before you install the blueprint. Click **[!UICONTROL See group descriptions]** to learn more about the groups available in the blueprint.

The blueprint searches by the group name to see if any existing groups match. The search is case sensitive, so names must be an exact match. If no existing groups match, you can have the blueprint create them for you.

![[!UICONTROL Group Mapping] section](assets/Blueprints_GroupMapping.png)

1. If a group exists, you can select **[!UICONTROL Remap Group]** and choose one of the following options:

   1. **[!UICONTROL Create a new group with a different name]**, then type the name to assign to this group. References to the group in the blueprint definition will be associated to this new group instead.
   1. **[!UICONTROL Replace with an existing group]**, then search for and select a group in the selection box.

      >[!NOTE]
      >
      >You cannot rename an existing group.

1. If a group does not exist, you can:

   1. Change the suggested group name by typing it in the text box.
   1. Select **[!UICONTROL Remap Group]** and choose [!UICONTROL Replace with an existing group], then search for and select a group in the selection box.
   1. Select **[!UICONTROL Remap Group]** and choose **[!UICONTROL Insert under an existing group]**, then search for and select a group in the selection box. This option creates a new subgroup under the existing group.

>[!NOTE]
>
>To configure the groups after installing the blueprint, see [Actions to take after installing a blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

For information about using groups in [!DNL Workfront], see [Groups overview](../../administration-and-setup/manage-groups/groups-overview/groups.md).
