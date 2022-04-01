

# View and manage a group’s details

You can view and manage the main details for a group you administer. These include the group’s name, description, Business Leader, and group administrators. You can also make the group and all of its subgroups public or private.

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

## View and manage a group’s details {#view-and-manage-a-group-s-details}

1. Click **Setup** near the upper-right corner of Adobe Workfront on the Global Navigation Bar.
1. Click **Groups**.

   In the list of groups that displays, group administrators can see the groups they manage, as well as any subgroups of those groups. Adobe Workfront administrators can see all groups.

1. Click the name of the top-level group that you want to edit.
1. In the box that displays, make any of the following changes:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Group Name</td> 
      <td>Change the name of the group.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Type a description for the group. You can type up to 512 characters.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Make this group and its subgroups public</td> 
      <td> <p>(Available only if you are viewing Details for a top-level group, not a subgroup.) Enable this option to allow users in the group with edit-user access (who are not administrators of the group) to add this group and its subgroups to the user profile of other users.</p> <p>For a public group, any user (in or out of the group) who has edit-user access can add the group to the profile of other users. They cannot do this for a private group.</p> <p>You can edit this option only on the top parent group in a hierarchy of groups that has more than one level. All subgroups of the parent group inherit its setting.</p> <p>Note:  
        <ul> 
         <li>You can’t make a subgroup public by itself, but you can make it’s top-level parent group public, which also makes all of the parent’s subgroups public.</li> 
         <li>A subgroup that belongs to a public group is public by default, so any user with edit-user access can add the subgroup to other users, as well.</li> 
        </ul> </p> <p>If you need information about the access needed to edit users, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>. For information about editing users, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Business Leader </td> 
      <td> <p>You can assign one user as a Business Leader for a group that you manage. A Business Leader is someone who makes business decisions for the group. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Business Leader overview</a><span>.</span></p> <p>If the person is not already a member of the group, adding their name to this field also adds them to the group.</p> <p>Note:  
        <ul> 
         <li>Before you can remove the Business Leader from a group, you must remove their name from the Business Leader field.</li> 
         <li>If you remove the name from the Business Leader field, that user remains a member of the group unless you remove them from it. For instructions on removing someone from a group, see the section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">Manage a group’s memberships</a> in the article <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">Manage a group</a>.</li> 
        </ul> </p> <p>For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Business Leader overview</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Group Members and Group Administrators</td> 
      <td> 
       <ul> 
        <li> <p>Group members: To add users and groups to the group, start typing the name of an existing user or group you want to add, then select the name when it appears.</p> <p>The users and groups that you add have access to all objects shared with the group.</p> </li> 
        <li> <p>Group administrators: You can assign a group member as an administrator for the group using the drop-down menu to the right of the user’s name.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">A top-level group must have at least 1 group administrator.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Search people and groups in the list</td> 
      <td> If you need to find a user or group already assigned to this group, you can type their name here and select it when it appears.</td> 
     </tr> 
    </tbody> 
   </table>

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2><a name="Inactive"></a>Inactive groups</h2>
<p>Consider the following about a group that you deactivate by disabling the Is Active option explained in the section <a href="#view-and-manage-a-group-s-details" class="MCXref xref">View and manage a group’s details</a> in this article.</p>
<ul>
<li> <p>Deactivating a group also deactivates all subgroups below it.</p> <p>For information about re-activating a subgroup in this situation, see <a href="#about-reactivating-a-subgroup-below-an-inactive-parent-group" class="MCXref xref">About reactivating a subgroup below an inactive parent group</a> in this article.</p> </li>
<li> <p>When you go to the Groups area in Setup, you can see only active groups in the list because Active is the default filter <img src="assets/filter-nwepng.png"> for it. If you want to see all of the groups you manage, including the inactive ones, you can use the All filter.</p> <p>For more information about filters in lists, see <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filters overview in Adobe Workfront</a>.</p> </li>
<li> <p>Deactivating a group does not change the following:</p>
<ul>
<li> <p>The group's associations to objects. Associated objects continue to function as they did before, without any changes.</p> <p>For example, if a project is associated with a group you deactivate, the project continues to use the group's preferences and statuses without any changes.</p> </li>
<li> <p>Your ability to create a new object, such as an approval, team, or company, from within the group's page in setup. By default, the new object is associated with the inactive group.</p> </li>
<li> <p>Your ability, as an administrator, to find the group in filters and reporting.</p> <p>You can also find it in group type-ahead fields where you might want to manage the group's settings in the Setup area. This includes the Preferences, Event Notifications, and System Licenses areas.</p> <p>For example, if you go to Setup > Project Preference > Projects and clear the type-ahead field above the options there, you can still find an inactive group and configure its project preferences.</p> </li>
</ul> </li>
</ul>
<h2 id="about-reactivating-a-subgroup-below-an-inactive-parent-group"><a name="Reactiva"></a>About reactivating a subgroup below an inactive parent group</h2>
<p>Deactivating a group also deactivates all subgroups below it. If you need to reactivate one of the subgroups under an inactive group, you can do one of two things:</p>
<ul>
<li> <p>Move the subgroup under an active group. Then enable the Is Active option for the moved group, as explained in the section <a href="#view-and-manage-a-group-s-details" class="MCXref xref">View and manage a group’s details</a> in this article.</p> <p>For instructions on moving a group, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md" class="MCXref xref">Move a group</a>.</p> </li>
<li> <p>Remove the subgroup from its parent group (which makes the subgroup a top-level group). Then enable the Is Active option for the moved group, as explained in the section <a href="#view-and-manage-a-group-s-details" class="MCXref xref">View and manage a group’s details</a> in this article.</p> <p>For instructions on removing a subgroup from its parent group, see the section <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make" class="MCXref xref">Remove a subgroup from its parent group and make it a top-level group</a> in the article <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md" class="MCXref xref">Manage a subgroup</a>.</p> </li>
</ul>
</div>
-->

