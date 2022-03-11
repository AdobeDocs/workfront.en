---
filename: share-an-asset-with-users
product: workfront-library
product-area: documents;user-management
navigation-topic: content-management
title: Share a Workfront Library item with other users
description: If you have Manage permission to a Workfront Library item, you can share it with other users and organizational units in Workfront Library and with external users.
---

# Share a `Workfront Library` item with other users

## Understand sharing items

If you have Manage permission to a `Workfront Library` item, you can share it with other users and organizational units in `Workfront Library` and with external users.

You can share the following `Workfront Library` items:

* [Content](#share) 
* [Folder](#folder) 
* [Collection](#collecti)

When you share a `Workfront Library` item with internal users, `Workfront` informs them of the shared item through an in-app notification.

You can share an item with an external user by emailing them a link to the item, which allows them download the item. External users do not need a Workfront login to access items you share with them.

Items that have been shared with internal users display the Shared icon.

### Content

When you share content that has multiple versions, you share a content package that contains all the versions. Users with View permission to the shared content can view only the active (or current) version of the asset, while users with Manage permission can view and download the active version, as well as older versions of content. For information on content versioning, see [Overview of content versioning in Workfront Library](../../workfront-library/content-management/content-versioning/content-versioning-overview.md).

### Folder

When you share a folder with another user, that user automatically inherits access to all the assets and sub-folders within the folder. For example, if you grant a user Manage permission to a folder, then that user has Manage permission to all the items contained within the folder and any of its sub-folders. For more information about folders, see [Overview of folders in Workfront Library](../../workfront-library/content-management/folders/folders-overview-library.md).

### Collection

When you share a collection with another user, that user automatically inherits access to all the assets, folders, and sub-folders contained within the collection. For example, if you grant a user Manage permission to a collection, then that user has Manage permission to all the items contained within the collection. For more information on collections, see [Edit a Workfront Library collection](../../workfront-library/content-management/collections/edit-a-collection.md).

## Specify users' permissions for shared items

When you share an item with other users, you give them access and permissions that allow them to use and manage that item. For more information on access and permissions, see [Permissions in Workfront Library](../../workfront-library/administration-and-setup/user-access/permissions-in-workfront-library.md).

You cannot give a user permissions to an item that exceeds their `Workfront Library` access level. For example, if a user has Viewer access to `Workfront Library`, that user cannot be given Manage permissions to an item. For more information on access levels, see [Overview of user access to Workfront Library](../../workfront-library/administration-and-setup/user-access/user-access-overview.md).

## Share a `Workfront Library` item

<ol> 
 <li value="1"> In Workfront, click the Main Menu icon , then select Library to open Workfront Library in a new browser tab. </li> 
 <li value="2"> <p>In the upper-left corner of <span>Workfront Library</span>, click the <span class="bold">Menu</span> icon <img src="assets/library-menu-icon.png">.</p> </li> 
 <li value="3"> <p>Select the area where the item you want to share is located.</p> <p>You can choose Library, My Content , or Collections.</p> <p> <img src="assets/library-left-panel---new-350x217.png" style="width: 350;height: 217;"> </p> </li> 
 <li value="4"> <p>(Conditional) If you are in the list view, click the <span class="bold">Show grid view</span> icon <img src="assets/grid-view-icon.png"> to switch to the grid view.</p> </li> 
 <li value="5">Navigate to the item and hover, then click the <span class="bold">More</span> icon in the upper-right corner.</li> 
 <li value="6"> <p>Select <span class="bold">Share</span> in the drop-down menu.</p> <p>The Share dialog displays.</p> <p>The Share dialog shows only the <span>Workfront Library</span> users and organizational units that you have shared the item with. </p> <note type="note">
    The Share dialog shows only the 
   <span>Workfront Library</span> users and organizational units that you have shared the item with. 
  </note> </li> 
 <li value="7"> <p>In the <span class="bold">Give access to</span> box, begin typing the name of the <span>Workfront Library</span> user or organizational unit that you want to share the item with, then click the name when it displays in the drop-down list. </p> <p>The user displays in the list and is, by default, given View permission to the item.</p> <note type="tip">
   If a user has a Manager or higher access level to 
   <span>Workfront Library</span>, you can choose to increase their permission level to Manage. 
  </note> </li> 
 <li value="8"> <p>(Optional) To change a user's permissions to the shared content, click the permissions level drop-down menu arrow, then select the desired permission.</p> <p> <img src="assets/sharechangeaccess-350x118.png" style="width: 350;height: 118;"> </p> <p>If a user with whom you want to share the content does not have an permissions level drop-down menu arrow, then you cannot increase their permissions. For more information on access to shared items, see <a href="#specifyi" class="MCXref xref">Specify users' permissions for shared items</a>.</p> </li> 
 <li value="9"> <p>(Optional) To share the item with an external user:</p> 
  <ol> 
   <li value="1">Enable <span class="bold">Make this public to external users</span>.</li> 
   <li value="2">Click <span class="bold">Copy Link</span>.</li> 
   <li value="3">Paste the link in a third-party tool such as a chat or email application, then distribute to the user.</li> 
  </ol> </li> 
 <li value="10">Click <span class="bold">Save</span>.</li> 
</ol>

