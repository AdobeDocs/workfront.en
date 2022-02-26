---
filename: give-users-access-portal
product: workfront-library
product-area: documents;user-management;system-administration
navigation-topic: user-access
title: Give users access to a Workfront Library portal
description: Before users can open a Workfront Library portal, they must be given access to the portal. As a user with Manage access or higher to a portal, you can grant users the following types of access to the portal.
---

# Give users access to a *Workfront Library* portal

Before users can open a *Workfront Library* portal, they must be given access to the portal. As a user with Manage access or higher to a portal, you can grant users the following types of access to the portal.

* `Individual`: Access that you grant to individual users
* `User grouping`: Access that users receive through their membership in a user grouping that you've added to the portal

When you add individual users and user groupings to a portal, you assign them an access level, which defines the activities that users can perform on content in the portal. For information on the permissions allowed for each access level, see [Permissions in Workfront Library](../../../workfront-library/administration-and-setup/user-access/permissions-in-workfront-library.md).

For information on setting up a portal, see [Set up a portal in Workfront Library](../../../workfront-library/administration-and-setup/workfront-library-setup/set-up-a-portal-in-library.md).

## Add users to a portal

<ol> 
 <li value="1"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In <em>Workfront</em>, click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png">, then select <span class="bold">Library</span> to open <em>Workfront Library</em> in a new browser tab.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In <em>Workfront</em>, click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png">, then select <span class="bold">Library</span> to open <em>Workfront Library</em> in a new browser tab.</p> </li> 
 <li value="2"> <p>In the upper-left corner of <em>Workfront Library</em>, click the <span class="bold">Menu</span> icon.</p> </li> 
 <li value="3"> <p>In the left panel, click <span class="bold">Portals</span>.</p> <p> <img src="assets/portals-red-square-350x224.png" style="width: 350;height: 224;"> </p> </li> 
 <li value="4"> <p>Select the portal to which you want to add users.</p> <p>The portal opens.</p> </li> 
 <li value="5"> <p>Click the <span class="bold">Menu</span> icon in the upper-left corner of the portal, then click <span class="bold">Setup</span> > <span class="bold">Users</span>.</p> </li> 
 <li value="6"> <p>Click <span class="bold">Add</span>.</p> </li> 
 <li value="7"> <p>In the <span class="bold">Search</span> box, begin typing the name of the user to whom you want to give access, then select the user's name when it displays in the dropdown menu.</p> </li> 
 <li value="8"> <p>Repeat step 7 until you have selected all the users you want to add.</p> <p>Users are automatically assigned Viewer access to the portal.</p> </li> 
 <li value="9">(Optional) Assign a different access level to the users.
  <ol>
   <li value="1"><p>Select the user or users for whom you want to change access, then click <span class="bold">Edit</span>.</p><p>The Edit Access dialog box opens.</p><p><img src="assets/editaccess-324x214.png" style="width: 324;height: 214;"></p></li>
   <li value="2"><p>In the <span class="bold">Access Level</span> drop-down menu, select the desired access level.</p></li>
  </ol></li> 
 <li value="10"> <p>Click <span class="bold">Save.</span></p> <p>The users are added to the portal.</p> <p><em>Workfront Library</em> sends the users an email with a link to the portal. </p> </li> 
</ol>

## Add user groupings to a portal

Users can inherit access to a portal through a *Workfront* user grouping that you've added to the portal.

You can add the following *Workfront* user groupings to a portal:

* Job roles
* Teams
* Groups
* Companies

When you add a user grouping, all members of that grouping are given access to the portal.

Any user grouping that you add to the portal must first exist and be populated with users in *Workfront*.

<ol> 
 <li value="1"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In <em>Workfront</em>, click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png">, then select <span class="bold">Library</span> to open <em>Workfront Library</em> in a new browser tab.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In <em>Workfront</em>, click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png">, then select <span class="bold">Library</span> to open <em>Workfront Library</em> in a new browser tab.</p> </li> 
 <li value="2"> <p>In the upper-left corner of <em>Workfront Library</em>, click the <span class="bold">Menu</span> icon.</p> </li> 
 <li value="3"> <p>In the left panel, click <span class="bold">Portals</span>.</p> <p> <img src="assets/portals-red-square-350x224.png" style="width: 350;height: 224;"> </p> </li> 
 <li value="4"> <p>Select the portal to which you want to add a user grouping.</p> <p>The portal opens.</p> </li> 
 <li value="5"> <p>Click the <span class="bold">Menu</span> icon in the upper-left corner of the portal, then click <span class="bold">Setup</span>. </p> </li> 
 <li value="6">Click the type of user grouping you want to give access to, then click <span class="bold">Add</span>.</li> 
 <li value="7"> <p>In the <span class="bold">Search</span> box, begin typing the name of the user grouping you want to add and select the grouping name when it displays in the drop-down menu.</p> <p> The user grouping now has access to the portal and is automatically assigned Viewer access. All members of the grouping receive an email inviting them to see the content shared with them through the portal.</p> </li> 
 <li value="8">(Optional) Assign a different access level to the user grouping.
  <ol>
   <li value="1">Select the user grouping that you want to change access to, then click <span class="bold">Edit</span>.</li>
   <li value="2">In the <span class="bold">Access Level</span> dropdown menu, select the desired access level.</li>
   <li value="3">Click <span class="bold">Save</span>.</li>
  </ol></li> 
 <li value="9"> <p>(Optional) To view who is in a user grouping, select the desired grouping, then click the arrow next to the grouping's name.</p> </li> 
</ol>

