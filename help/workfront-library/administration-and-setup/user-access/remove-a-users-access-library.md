---
filename: remove-a-users-access-library
product: workfront-library
product-area: documents;user-management;system-administration
navigation-topic: user-access
title: Remove a user's access to Workfront Library
description: As a Workfront Library administrator, you can remove a user's access to Workfront Library. When you remove a user from Workfront Library, only their access to Workfront Library is removed. Their Workfront account remains active. Any content that they owned in Workfront Library remains in Workfront Library.
---

# Remove a user's access to Workfront Library

As a Workfront Library administrator, you can remove a user's access to Workfront Library. When you remove a user from Workfront Library, only their access to Workfront Library is removed. Their Workfront account remains active. Any content that they owned in Workfront Library remains in Workfront Library.

If a Workfront system administrator deactivates a user in Workfront, they automatically lose access to Workfront Library.

>[!TIP]
>
>Before deleting or deactivating a user in Workfront or in Workfront Library, we recommend reassigning the content they own to another Workfront Library user. To access content owned by a deactivated user, users must have View or Manage access to the content. Only users with Manage access can make changes to content owned by a deactivated user.  
>For information on changing the ownership of content, see [Transfer ownership assets to another user](../../../workfront-library/administration-and-setup/manage-assets/transfer-ownership-to-others.md).

A user might have multiple access levels assigned to them. For example, a user can have individual access to Workfront Library and access from any job role, team, group, or company that they are members of. For information on the differences between individual and user grouping access, see [Overview of user access to Workfront Library](../../../workfront-library/administration-and-setup/user-access/user-access-overview.md).

>[!NOTE]
>
>To determine how a user has access to Workfront Library, you can open the Library menu and go to `Setup` > `Access` > `Users`. In the Users area, you see a list of users and the type of access they have is listed in the Access Sources column.  
>![](assets/access-sources-column-350x274.png)<![CDATA[		]]>

* [Remove a user's individual access](#remove2) 
* [Remove access for a user grouping](#remove3)

## Remove a user's individual access

Removing a user's individual access to Workfront Library does not affect any other access sources that the user has.

To remove individual access:

<ol> 
 <li value="1"> In Workfront, click the Main Menu icon , then select Library to open Workfront Library in a new browser tab. </li> 
 <li value="2"> <p>In the upper-left corner of Workfront Library, click the <span class="bold">Menu</span> icon.</p> <note type="note">
   To remove a user from a portal, click 
   <span class="bold">Portals</span> in the bottom-left panel.
  </note> </li> 
 <li value="3"> <p>In the left panel, click <span class="bold">Setup</span> > <span class="bold">Users</span>.</p> </li> 
 <li value="4"> <p>To locate the user you want to remove, click the <span class="bold">Search</span> icon in the top-right corner, then enter the user's name and hit Enter.</p> <p> <img src="assets/search-icon-for-users-350x144.png" style="width: 350;height: 144;"> </p> <p>Or</p> <p>Scroll down until you've located the user's name.</p> </li> 
 <li value="5"> <p>Next to the user's name, click the More menu, then select <span class="bold">Remove individual access</span>.</p> <p> <img src="assets/remove-individual-access-selection-350x173.png" style="width: 350;height: 173;"> </p> </li> 
 <li value="6"> <p>(Optional) If the user owns assets and doesn't have access through a user grouping, you must select what you would like to do with the assets:</p> 
  <ul> 
   <li>Transfer the assets to a different user</li> 
   <li>Delete the assets</li> 
   <li>Keep the assets without transfering them to a new owner</li> 
  </ul> <note type="note">
   If you choose to keep the assets assigned to the user that you're removing, you can transfer the assets later. If you select to transfer the assets now, you must select a new owner to assign them to. To learn more about transfering assets, see 
   <a href="../../../workfront-library/administration-and-setup/manage-assets/transfer-ownership-to-others.md" class="MCXref xref">Transfer ownership assets to another user</a>.
  </note> </li> 
 <li value="7"> <p>In the Remove individual access dialog, click <span class="bold">Remove user</span>.</p> <p>The user appears in the Deactivated users list.</p> <note type="note">
   If you want to restore access for an inactive user, you can locate them by clicking the Filter icon, then selecting 
   <span class="bold">Deactivated users</span> from the menu. After finding the Deactivated users list, you can select 
   <span class="bold">Restore user access</span> from the More Menu.
  </note> </li> 
</ol>

## Remove access for a user grouping

As a Workfront Library administrator, you can remove access to Workfront Library for an entire group of users based on their user groupings:

* Job role
* Team
* Group
* Company

Users who are members of the removed user grouping lose their access to Workfront Library and all the content shared with the grouping, unless they have individual access to Workfront Library or access through another user grouping in Workfront Library. For information on Workfront Library access levels and permissions, see [Overview of user access to Workfront Library](../../../workfront-library/administration-and-setup/user-access/user-access-overview.md)

>[!NOTE]
>
>If you don't want specific users to access Workfront Library through a job role, team, group, or company, you need to remove them from that specific user grouping in Workfront. To learn how to make these changes from the user profile, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).  
>Alternatively, you can remove them from a user grouping by modifying the job role, team, group, or company that they are a member of. To learn more, see:  
>
>* [Create and manage job roles](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)
>* [Edit team settings](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md)
>* [View and manage a group’s memberships](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md)
>* [Create and edit companies](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)
>

To remove access for a user grouping in Workfront Library:

<ol> 
 <li value="1"> In Workfront, click the Main Menu icon , then select Library to open Workfront Library in a new browser tab. </li> 
 <li value="2"> <p>In the upper-left corner of Workfront Library, click the <span class="bold">Menu</span> icon.</p> <note type="note">
   To remove a grouping from a portal, click 
   <span class="bold">Portals</span> in the bottom-left panel.
  </note> </li> 
 <li value="3"> <p>In the left panel, click <span class="bold">Setup</span>, then select the type of user grouping you want to remove access for:</p> 
  <ul> 
   <li><span class="bold">Job role</span> </li> 
   <li><span class="bold">Team</span> </li> 
   <li><span class="bold">Group</span> </li> 
   <li><span class="bold">Company</span> </li> 
  </ul> <p>A list of the user groupings for the selected type displays in Workfront Library.</p> </li> 
 <li value="4"> <p>Click the <span class="bold">More</span> menu inline with the user grouping that you want to remove.</p> <p> <img src="assets/remove-grouping-library-350x169.png" style="width: 350;height: 169;"> </p> </li> 
 <li value="5"> <p>Click <span class="bold">Remove</span>, then click <span class="bold">Remove</span> to confirm.</p> <p>The user grouping is removed from Workfront Library. Removing a user grouping from Workfront Library does not delete the user grouping in Workfront.<br></p> <note type="note">
   To transfer assets owned by members of the grouping, you must go to the Deactivated users list. To learn more about transfering assets, see 
   <a href="../../../workfront-library/administration-and-setup/manage-assets/transfer-ownership-to-others.md" class="MCXref xref">Transfer ownership assets to another user</a>.
  </note> </li> 
</ol>

