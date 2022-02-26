

# View and manage a group’s details

The highlighted information on this page refers to functionality available only in the new Workfront experience beta.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You can view and edit the Group Details page for a group or subgroup that you manage. This page includes a description of the group, the names of the Business Leader and <em>group administrators</em>, and an option that allows you to make the group and all of its subgroups public or private.</p>
-->

You can view and edit the Group Details page for a group or subgroup that you manage. This page includes a description of the group, the names of the Business Leader and *group administrators*, and an option that allows you to make the group and all of its subgroups public or private.

For information about other ways you can manage a group, see [Create a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> <p>You must be a <em>group administrator</em> of the group<draft-comment>
      <MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
       s
      </MadCap:conditionalText>
     </draft-comment><MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
      s
     </MadCap:conditionalText> or a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your *Workfront administrator*.

## View and manage a group’s details

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2"> <p>Click <span class="bold">Groups</span>.</p> <p>In the list of groups that displays, <em>group administrators</em> can see the groups they manage, as well as any subgroups of those groups. <em>Adobe Workfront administrators</em> can see all groups.</p> </li> 
 <li value="3">Click the name of the top-level group that you want to edit.</li> <draft-comment>
  <li value="4" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>In the left menu, click <span class="bold">Group Details</span>, then do any of the following:</p> 
   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td> <p>You can type up to 512 characters.</p> <p>If the field is blank, click <span class="bold">Add</span> to type a description.</p> </td> 
     </tr> <draft-comment>
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader"><span class="preview">Is Active</span> </td> 
       <td> 
        <div class="preview"> <draft-comment>
          <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> WHEN UNDRAFTING AND LATER UNHIGHLIGHTING THIS, make sure to do the same to the blurb at the top of each of the 3 articles this snippet is in</p>
         </draft-comment>
         <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> WHEN UNDRAFTING AND LATER UNHIGHLIGHTING THIS, make sure to do the same to the blurb at the top of each of the 3 articles this snippet is in</p> 
         <p>(Enabled by default) Makes the group active in your <em>Workfront</em> instance.</p> 
         <p>In type-ahead fields like the one shown below, when regular users search for a group to attach it to an object or to share an object with it, only active groups display in the list.</p> 
         <p> <img src="assets/group-type-aheads.jpg"> </p> 
         <p>To streamline this for your users, you can disable the Is Active option for groups that are not currently in use.</p> 
         <p>You can easily view, filter and group the Groups list based on active or inactive status using this field. For information about using views, filters, and groupings in lists, see <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Reporting elements: filters, views, and groupings</a>.</p> 
         <p>For information about inactive groups, see <a href="#inactive" class="MCXref xref">Inactive groups</a> in this article.</p> 
        </div> </td> 
      </tr>
     </draft-comment>
     <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
      <td role="rowheader"><span class="preview">Is Active</span> </td> 
      <td> 
       <div class="preview"> 
        <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> WHEN UNDRAFTING AND LATER UNHIGHLIGHTING THIS, make sure to do the same to the blurb at the top of each of the 3 articles this snippet is in</p> 
        <p>(Enabled by default) Makes the group active in your <em>Workfront</em> instance.</p> 
        <p>In type-ahead fields like the one shown below, when regular users search for a group to attach it to an object or to share an object with it, only active groups display in the list.</p> 
        <p> <img src="assets/group-type-aheads.jpg"> </p> 
        <p>To streamline this for your users, you can disable the Is Active option for groups that are not currently in use.</p> 
        <p>You can easily view, filter and group the Groups list based on active or inactive status using this field. For information about using views, filters, and groupings in lists, see <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Reporting elements: filters, views, and groupings</a>.</p> 
        <p>For information about inactive groups, see <a href="#inactive" class="MCXref xref">Inactive groups</a> in this article.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Group accessibility</td> 
      <td> <p>(Available only if you are viewing Details for a group, not a subgroup.) Enable or disable the option <span class="bold">Make this group and subgroups private</span>.</p> <p>For a public group, any user (in or out of the group) who has edit-user access can add the group to the profile of other users. They cannot do this for a private group.</p> <p>You can edit this option only on the top parent group in a hierarchy of groups that has more than one level. All subgroups of the parent group inherit its setting.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Group stakeholders</td> 
      <td> 
       <ul> 
        <li><span class="bold">Group Administrators</span>: Add or remove users with a Planner license as <em>group administrators</em> for the group. Begin typing the name of a user, then click the name when it appears in the drop-down menu.</li> 
        <li><span class="bold">Business Leader</span>: Do one of the following:
         <ul>
          <li>If you have not yet assigned a Business Leader for the group, click <span class="bold">Add</span>, start typing the name of the user you want to assign, then click the person’s name when it appears.</li>
          <li>If the group already has a Business Leader and you want to change it, double-click the name of the existing Business Leader. Delete the name, start typing the name of the user you want to assign, then click the person’s name when it appears.</li>
         </ul></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Add custom form</td> 
      <td>If your access level allows you to manage custom forms, add a custom form to the group. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Custom forms</a>.</td> 
     </tr> 
    </tbody> 
   </table> </li>
 </draft-comment>
 <li value="4" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>In the left menu, click <span class="bold">Group Details</span>, then do any of the following:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Description</td> 
     <td> <p>You can type up to 512 characters.</p> <p>If the field is blank, click <span class="bold">Add</span> to type a description.</p> </td> 
    </tr> 
    <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
     <td role="rowheader"><span class="preview">Is Active</span> </td> 
     <td> 
      <div class="preview"> 
       <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> WHEN UNDRAFTING AND LATER UNHIGHLIGHTING THIS, make sure to do the same to the blurb at the top of each of the 3 articles this snippet is in</p> 
       <p>(Enabled by default) Makes the group active in your <em>Workfront</em> instance.</p> 
       <p>In type-ahead fields like the one shown below, when regular users search for a group to attach it to an object or to share an object with it, only active groups display in the list.</p> 
       <p> <img src="assets/group-type-aheads.jpg"> </p> 
       <p>To streamline this for your users, you can disable the Is Active option for groups that are not currently in use.</p> 
       <p>You can easily view, filter and group the Groups list based on active or inactive status using this field. For information about using views, filters, and groupings in lists, see <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Reporting elements: filters, views, and groupings</a>.</p> 
       <p>For information about inactive groups, see <a href="#inactive" class="MCXref xref">Inactive groups</a> in this article.</p> 
      </div> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Group accessibility</td> 
     <td> <p>(Available only if you are viewing Details for a group, not a subgroup.) Enable or disable the option <span class="bold">Make this group and subgroups private</span>.</p> <p>For a public group, any user (in or out of the group) who has edit-user access can add the group to the profile of other users. They cannot do this for a private group.</p> <p>You can edit this option only on the top parent group in a hierarchy of groups that has more than one level. All subgroups of the parent group inherit its setting.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Group stakeholders</td> 
     <td> 
      <ul> 
       <li><span class="bold">Group Administrators</span>: Add or remove users with a Planner license as <em>group administrators</em> for the group. Begin typing the name of a user, then click the name when it appears in the drop-down menu.</li> 
       <li><span class="bold">Business Leader</span>: Do one of the following:
        <ul>
         <li>If you have not yet assigned a Business Leader for the group, click <span class="bold">Add</span>, start typing the name of the user you want to assign, then click the person’s name when it appears.</li>
         <li>If the group already has a Business Leader and you want to change it, double-click the name of the existing Business Leader. Delete the name, start typing the name of the user you want to assign, then click the person’s name when it appears.</li>
        </ul></li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Add custom form</td> 
     <td>If your access level allows you to manage custom forms, add a custom form to the group. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Custom forms</a>.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2><a name="Inactive"></a>Inactive groups</h2>
<p>Consider the following about a group that you deactivate by disabling the Is Active option. For more about this option, see <a href="#view" class="MCXref xref">View and manage a group’s details</a> in this article.</p>
<ul>
<li> <p>If you copy an inactive group, the new group is also inactive.</p> </li>
<li> <p>Deactivating a group also deactivates all subgroups below it.</p> <p>If you want to re-activate one of the subgroups, you must first move from underneath the inactive parent group, then select the Is Active option on its Details page.</p> <p>For instructions on moving a group, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md" class="MCXref xref">Move a group</a>.</p> <p>For instructions on selecting its Is Active option, see <a href="#view" class="MCXref xref">View and manage a group’s details</a>in this article.</p> </li>
<li> <p>Deactivating a group does not change the following:</p>
<ul>
<li> <p>Any associations the group has to certain objects.</p> <p>The associated objects continue to function as they did before, without any changes.</p> <p>For example, if a project is associated with a group you deactivate, the project continues to use the group's preferences and statuses without any changes.</p> </li>
<li> <p>Your ability to create a new object, such as an approval, team, or company, from within the group's page in setup. By default, the new object is associated with the inactive group.</p> </li>
<li> <p>Your ability, as an administrator, to find the group in filters and reporting.</p> <p>You can also find it in group type-ahead fields where you might want to manage the group's settings in the Setup area. This includes the Preferences, Event Notifications, and System Licenses areas.</p> <p>For example, as shown below, if you go to Setup&nbsp;>&nbsp;Project Preference&nbsp;>&nbsp;Projects and clear the type-ahead field above the options there, you can still find an inactive group and configure its project preferences.</p> <p> <img src="assets/group-typeahead-preferences-350x215.jpg" style="width: 350;height: 215;"> </p> </li>
</ul> </li>
</ul>
</div>
-->

## Inactive groups

Consider the following about a group that you deactivate by disabling the Is Active option. For more about this option, see [View and manage a group’s details](#view) in this article.

<ul> 
 <li> <p>If you copy an inactive group, the new group is also inactive.</p> </li> 
 <li> <p>Deactivating a group also deactivates all subgroups below it.</p> <p>If you want to re-activate one of the subgroups, you must first move from underneath the inactive parent group, then select the Is Active option on its Details page.</p> <p>For instructions on moving a group, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md" class="MCXref xref">Move a group</a>.</p> <p>For instructions on selecting its Is Active option, see <a href="#view" class="MCXref xref">View and manage a group’s details</a>in this article.</p> </li> 
 <li> <p>Deactivating a group does not change the following:</p> 
  <ul> 
   <li> <p>Any associations the group has to certain objects.</p> <p>The associated objects continue to function as they did before, without any changes.</p> <p>For example, if a project is associated with a group you deactivate, the project continues to use the group's preferences and statuses without any changes.</p> </li> 
   <li> <p>Your ability to create a new object, such as an approval, team, or company, from within the group's page in setup. By default, the new object is associated with the inactive group.</p> </li> 
   <li> <p>Your ability, as an administrator, to find the group in filters and reporting.</p> <p>You can also find it in group type-ahead fields where you might want to manage the group's settings in the Setup area. This includes the Preferences, Event Notifications, and System Licenses areas.</p> <p>For example, as shown below, if you go to Setup&nbsp;>&nbsp;Project Preference&nbsp;>&nbsp;Projects and clear the type-ahead field above the options there, you can still find an inactive group and configure its project preferences.</p> <p> <img src="assets/group-typeahead-preferences-350x215.jpg" style="width: 350;height: 215;"> </p> </li> 
  </ul> </li> 
</ul>

