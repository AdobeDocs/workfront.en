---
filename: manage-subgroups
user-type: administrator
product-area: system-administration;user-management
keywords: manage,subgroup,edit
navigation-topic: create-and-manage-subgroups
title: Manage a subgroup
description: As an group administrator of a subgroup, you can create, move, view, edit, copy, rename, export, and delete the subgroup.
---

# Manage a subgroup

As an *group administrator* of a subgroup, you can create, 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
move,
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> move, </MadCap:conditionalText>`view, edit, copy, rename, export, and delete the subgroup.

If there are any groups above your group, their administrators can also do these things for your group. The same is true for *Workfront administrators* (for any group).

For more information about subgroups, see [Subgroups overview](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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
   <td> <p><em>Plan</em> </p> <p>You must be a <em>group administrator</em> of the group or a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your *Workfront administrator*.

## Create, 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
move,
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> move, </MadCap:conditionalText>`view, edit, copy, rename, export, or delete a subgroup

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2"> <p>In the left panel, click <span class="bold">Groups</span> <img src="assets/groups-icon.png">.</p> <p>In the list of groups that displays, <em>group administrators</em> can see the groups they manage, as well as any subgroups of those groups. <em>Adobe Workfront administrators</em> can see all groups.</p> </li> <draft-comment>
  <li value="3" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click the name of the group that contains the subgroup you want to work on.</p> <draft-comment>
    <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Or</p>
   </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Or</p> <draft-comment>
    <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">If you are moving one or more subgroups, click the name of the destination group (you will specify which subgroups you want to move in a later step).</p>
   </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">If you are moving one or more subgroups, click the name of the destination group (you will specify which subgroups you want to move in a later step).</p> </li>
 </draft-comment>
 <li value="3" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click the name of the group that contains the subgroup you want to work on.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Or</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">If you are moving one or more subgroups, click the name of the destination group (you will specify which subgroups you want to move in a later step).</p> </li> <draft-comment>
  <li value="4" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>In the left menu, click <span class="bold">Subgroups</span>.</p> </li>
 </draft-comment>
 <li value="4" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>In the left menu, click <span class="bold">Subgroups</span>.</p> </li> 
</ol>

<ol data-mc-continue="true"> 
 <li value="5"> <p>Do any of the following:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Create a new subgroup</td> 
     <td> <draft-comment>
       <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">If you want to create the new subgroup one level down from the group you are viewing, click <span class="bold">Add subgroup</span>.</p>
      </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">If you want to create the new subgroup one level down from the group you are viewing, click <span class="bold">Add subgroup</span>.</p> <draft-comment>
       <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Or, if you want to create the new subgroup beneath another subgroup in the list, select that subgroup, then click <span class="bold">Add s</span><span class="bold">ubgroup</span>.</p>
      </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Or, if you want to create the new subgroup beneath another subgroup in the list, select that subgroup, then click <span class="bold">Add s</span><span class="bold">ubgroup</span>.</p> <p>For information about the options you can use to configure the subgroup, see the table in <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">Create a subgroup</a>.</p> <p>A group hierarchy cannot exceed 15 levels, but a single level can have an unlimited number of parallel groups.</p> </td> 
    </tr> <draft-comment>
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Move a subgroup </td> 
      <td> <p>You can move existing subgroups under another group you administer.</p> <p>A group hierarchy cannot exceed 15 levels, but a single level can have an unlimited number of parallel groups.</p> 
       <ol> 
        <li value="1"> <p>(Optional) Select a subgroup to make it the destination group.</p> <p>If you skip this step, the group you selected in step 3 is the destination group.</p> </li> 
        <li value="2">Click <span class="bold">Add Subgroup</span> > <span class="bold">Existing Group</span>.</li> 
        <li value="3"> <p>In the <span class="bold">Existing Group</span> box that appears, start typing the name of a subgroup you want to move.</p> <p>The results that display do not contain groups above the destination group.</p> <p>You can make sure you are selecting the right group by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.<draft-comment>
           <MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
             Depending on the details configured for the group, you might also see its Business Leader and description.
           </MadCap:conditionalText>
          </draft-comment><MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
            Depending on the details configured for the group, you might also see its Business Leader and description.
          </MadCap:conditionalText></p> </li> 
        <li value="4"> <p>Click the name of the subgroup you want to move when you see it display in the list.</p> </li> 
        <li value="5"> <p>Repeat Steps c-d for any other subgroups you want to move to the destination group</p> </li> 
        <li value="6">Click <span class="bold">Save</span>.</li> 
       </ol> </td> 
     </tr>
    </draft-comment>
    <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
     <td role="rowheader">Move a subgroup </td> 
     <td> <p>You can move existing subgroups under another group you administer.</p> <p>A group hierarchy cannot exceed 15 levels, but a single level can have an unlimited number of parallel groups.</p> 
      <ol> 
       <li value="1"> <p>(Optional) Select a subgroup to make it the destination group.</p> <p>If you skip this step, the group you selected in step 3 is the destination group.</p> </li> 
       <li value="2">Click <span class="bold">Add Subgroup</span> > <span class="bold">Existing Group</span>.</li> 
       <li value="3"> <p>In the <span class="bold">Existing Group</span> box that appears, start typing the name of a subgroup you want to move.</p> <p>The results that display do not contain groups above the destination group.</p> <p>You can make sure you are selecting the right group by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
           Depending on the details configured for the group, you might also see its Business Leader and description.
         </MadCap:conditionalText></p> </li> 
       <li value="4"> <p>Click the name of the subgroup you want to move when you see it display in the list.</p> </li> 
       <li value="5"> <p>Repeat Steps c-d for any other subgroups you want to move to the destination group</p> </li> 
       <li value="6">Click <span class="bold">Save</span>.</li> 
      </ol> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Edit a subgroup</td> 
     <td> <p>Select the subgroup you want to edit, then click <draft-comment>
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
         the Edit icon 
         <draft-comment>
          <img src="assets/edit-icon.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
         </draft-comment>
         <img src="assets/edit-icon.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
        </MadCap:conditionalText>
       </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
        the Edit icon 
        <img src="assets/edit-icon.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       </MadCap:conditionalText>.</p> <p>For information about the options you can use to configure the subgroup, see the table in <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Export one or more subgroups</td> 
     <td> 
      <ol> 
       <li value="1">Select the subgroup or subgroups you want to export.</li> 
       <li value="2">Click the Export icon <img src="assets/export.png">, then select the file format you want.</li> 
      </ol> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Copy a subgroup to create a new top-level group</td> 
     <td> <p>(Available only for <em>Workfront administrators</em>.) When you copy a subgroup, it becomes a parent group. All group members and subgroups are copied with it. The groups members retain any assignments they had in the original group.</p> <p>For more information about copying a subgroup, see <a href="#copying" class="MCXref xref">Copying a subgroup</a> in this article.</p> 
      <ol> 
       <li value="1">Select a subgroup, then click <draft-comment>
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
          the Copy icon 
          <img src="assets/copy-icon.png">
         </MadCap:conditionalText>
        </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
         the Copy icon 
         <img src="assets/copy-icon.png">
        </MadCap:conditionalText> to create a new top-level group based on the selected group.</li> 
       <li value="2"> <p>Configure the new group’s settings.</p> <p>For help with these settings, see the table in the section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Create a top-level group by copying an existing group or subgroup</a> in the article <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Create a top-level group by copying an existing group or subgroup</a>.</p> </li> 
      </ol> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Delete a subgroup</td> 
     <td> <note type="important">
       When you delete a group or subgroup, you need to preserve the users, work items, and any subgroups that are currently assigned to it. To help you make sure they are preserved, a prompt requires you to reassign the group’s objects to a different group in the step below.
      </note> 
      <ol> 
       <li value="1">Select the subgroup, then click <draft-comment>
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
          the Delete icon 
          <img src="assets/delete.png">
         </MadCap:conditionalText>
        </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
         the Delete icon 
         <img src="assets/delete.png">
        </MadCap:conditionalText>.</li> 
       <li value="2">In the <span class="bold">Delete Group</span> box that appears, starting typing and then select the name of the group where you want to move the members, work items, and subgroups of the group you are deleting.</li> 
       <li value="3">Click <span class="bold">Delete Them</span>.</li> 
      </ol> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

` `**Tip: **`` When you are managing a group that contains subgroups, it’s helpful to be able to identify and filter data about the entire group and all of its subgroups. You can do this by using the Top Parent ID field in a report or list.

For example, imagine that you manage a large Marketing department and you want a list of all of the projects that the entire department is working on.

In *Workfront*, this Marketing department is represented by a group called Marketing, with 3 subgroups called Field Marketing, Product Marketing, and Digital Marketing. To list the projects that belong to the entire Marketing department (all 4 groups), you could create a Filter for the Projects area with the following Filter Rule:

```
Group: Top Parent ID > Equal > Marketing
```

You can also use the Top Parent Name field to identify data associated with a top-level group, but only in Views, not in Filters or Groupings.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h2>View and manage a group’s subgroup members</h2>
<p>When you are viewing the main page of a group you administer, you can view and manage all of the users in the group’s subgroups. For instructions, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md" class="MCXref xref">View and manage subgroup members</a>.</p>
</div>
-->

## View and manage a group’s subgroup members

When you are viewing the main page of a group you administer, you can view and manage all of the users in the group’s subgroups. For instructions, see [View and manage subgroup members](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Copying a subgroup

Consider the following when you copy a subgroup.

* If a subgroup you copy has its own subgroups, they are included in the copy and their names are formatted as follows:

  *Original subgroup name* (Copy)

* Any subgroup that belongs to a public group is also public, so any user with edit-user access, in or out of the group, can add users to the subgroup.

