

# View and manage a group’s details

The highlighted information on this page refers to functionality available only in the new Workfront experience beta. 
You can view and edit the Group Details page for a group or subgroup that you manage. This page includes a description of the group, the names of the Business Leader and group administrators, and an option that allows you to make the group and all of its subgroups public or private. 

For information about other ways you can manage a group, see [Create a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> <p>You must be a group administrator of the group or a Workfront administrator. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your Workfront administrator.

## View and manage a group’s details

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2"> <p>Click <span class="bold">Groups</span>.</p> <p>In the list of groups that displays, group administrators can see the groups they manage, as well as any subgroups of those groups. Adobe Workfront administrators can see all groups.</p> </li> 
 <li value="3">Click the name of the top-level group that you want to edit.</li> In the left menu, click Group Details, then do any of the following: Description You can type up to 512 characters. If the field is blank, click Add to type a description. Is Active WHEN UNDRAFTING AND LATER UNHIGHLIGHTING THIS, make sure to do the same to the blurb at the top of each of the 3 articles this snippet is in (Enabled by default) Makes the group active in your Workfront instance. In type-ahead fields like the one shown below, when regular users search for a group to attach it to an object or to share an object with it, only active groups display in the list. To streamline this for your users, you can disable the Is Active option for groups that are not currently in use. You can easily view, filter and group the Groups list based on active or inactive status using this field. For information about using views, filters, and groupings in lists, see Reporting elements: filters, views, and groupings. For information about inactive groups, see Inactive groups in this article. Group accessibility (Available only if you are viewing Details for a group, not a subgroup.) Enable or disable the option Make this group and subgroups private. For a public group, any user (in or out of the group) who has edit-user access can add the group to the profile of other users. They cannot do this for a private group. You can edit this option only on the top parent group in a hierarchy of groups that has more than one level. All subgroups of the parent group inherit its setting. Group stakeholders Group Administrators: Add or remove users with a Planner license as group administrators for the group. Begin typing the name of a user, then click the name when it appears in the drop-down menu. Business Leader: Do one of the following: If you have not yet assigned a Business Leader for the group, click Add, start typing the name of the user you want to assign, then click the person’s name when it appears. If the group already has a Business Leader and you want to change it, double-click the name of the existing Business Leader. Delete the name, start typing the name of the user you want to assign, then click the person’s name when it appears. Add custom form If your access level allows you to manage custom forms, add a custom form to the group. For more information, see Custom forms. 
</ol>

<!--
Inactive groups Consider the following about a group that you deactivate by disabling the Is Active option. For more about this option, see View and manage a group’s details in this article. If you copy an inactive group, the new group is also inactive. Deactivating a group also deactivates all subgroups below it. If you want to re-activate one of the subgroups, you must first move from underneath the inactive parent group, then select the Is Active option on its Details page. For instructions on moving a group, see Move a group. For instructions on selecting its Is Active option, see View and manage a group’s detailsin this article. Deactivating a group does not change the following: Any associations the group has to certain objects. The associated objects continue to function as they did before, without any changes. For example, if a project is associated with a group you deactivate, the project continues to use the group's preferences and statuses without any changes. Your ability to create a new object, such as an approval, team, or company, from within the group's page in setup. By default, the new object is associated with the inactive group. Your ability, as an administrator, to find the group in filters and reporting. You can also find it in group type-ahead fields where you might want to manage the group's settings in the Setup area. This includes the Preferences, Event Notifications, and System Licenses areas. For example, as shown below, if you go to Setup > Project Preference > Projects and clear the type-ahead field above the options there, you can still find an inactive group and configure its project preferences.
-->

