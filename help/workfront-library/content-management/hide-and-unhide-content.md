---
filename: hide-and-unhide-content
product: workfront-library
product-area: documents
navigation-topic: content-management
title: Hide and unhide content in Workfront Library
description: You can limit who has access to content in Workfront Library by hiding it. To use the Hide feature you must have Manage permission to the content you want to hide.
---

# Hide and unhide content in Workfront Library

You can limit who has access to content in Workfront Library by hiding it. To use the Hide feature you must have Manage permission to the content you want to hide.

## Understand hidden content

When you hide content, it becomes hidden from you and from all users who have permissions to it, including external users and portal users. You cannot hide content from specific users.

Hidden content remains in Workfront Library but is not visible in Workfront Library or in any collections and portals to which the content has been added. However, users with Manage permission to hidden content can activate the Show Hidden filter, which allows them to view hidden items. For information on using the Show Hidden filter, see [Filter for hidden content in Workfront Library](../../workfront-library/content-management/filters/filter-hidden-content.md).

You can share folders and collections that contain hidden content with another user. Depending on a user's permissions level, the user might not be able to view the shared hidden content. Consider the following access scenarios:

| User access level to Workfront Library |Permission to hidden content |User's access to shared hidden content |
|---|---|---|
| Viewer |View |User is notified of the content, but does not have access to it. No thumbnail of the content displays in the user's Library area. |
| Manager or higher |View |User is notified of the content, and a thumbnail of the content displays in the user's Library area. The user can open and download the content, and add it to folders and collections. |
| Manager or higher |Manage |User has full access to the content. |

For more information on user access, see [Overview of user access to Workfront Library](../../workfront-library/administration-and-setup/user-access/user-access-overview.md).

Hidden content is labeled in the title bar as "hidden."

Thumbnails of hidden content display the crossed-out eye icon.

When you unhide content, it becomes visible to all users who had access to it prior to it being hidden.

>[!NOTE]
>
>Inactive items migrated from Workfront DAM to Workfront Library are automatically hidden.

## Hide content

<ol> 
 <li value="1"> In Workfront, click the Main Menu icon , then select Library to open Workfront Library in a new browser tab. </li> 
 <li value="2"> <p>In the upper-left corner of Workfront Library, click the <span class="bold">Menu</span> icon <img src="assets/library-menu-icon.png">.</p> </li> 
 <li value="3"> <p>Select the area where item you want to hide is located.</p> <p>You can choose Library, My Content , or Collections.</p> <p> <img src="assets/library-left-panel---new-350x217.png" style="width: 350;height: 217;"> </p> </li> 
 <li value="4"> <p>(Conditional) If you are in the list view, click the <span class="bold">Show grid view</span> icon <img src="assets/grid-view-icon.png"> to switch to the grid view.</p> </li> 
 <li value="5">Navigate to the item.</li> 
 <li value="6"> <p>Hover over the item, click the <span class="bold">More</span> icon in the upper-right corner of the thumbnail, then select <span class="bold">Hide</span> in the drop-down menu.</p> <p>The content thumbnail disappears from view. </p> </li> 
</ol>

## Unhide hidden content

<ol> In Workfront, click the Main Menu icon , then select Library to open Workfront Library in a new browser tab. 
 <li value="1"> <p>(Conditional) If you haven't enabled the Show Hidden filter, click the <span class="bold">Filter</span> icon <img src="assets/library-filter-icon.png">in the upper-right corner, then enable the <span class="bold">Show Hidden</span> toggle at the bottom of the filter list.</p> <note type="tip">
   Depending on the view you have activated, the name displayed on the Content View drop-down menu could be either Name or Last Modified.
  </note> </li> 
 <li value="2"> <p>In the upper-left corner of Workfront Library, click the <span class="bold">Menu</span> icon <img src="assets/library-menu-icon.png">.</p> </li> 
 <li value="3"> <p>Select the area where item you want to unhide is located.</p> <p>You can choose Library, My Content , or Collections.</p> <p> <img src="assets/library-left-panel---new-350x217.png" style="width: 350;height: 217;"> </p> </li> 
 <li value="4"> <p>(Conditional) If you are in the list view, click the <span class="bold">Show grid view</span> icon <img src="assets/grid-view-icon.png"> to switch to the grid view.</p> </li> 
 <li value="5">Navigate to the item.</li> 
 <li value="6"> <p>Hover over the item, click the <span class="bold">More</span> icon in the upper-right corner of the thumbnail, then select <span class="bold">Unhide</span> in the drop-down menu.</p> <p>The content is now visible to Workfront Library and portal users who had access to the content prior to it being hid. Any content links shared with external users are restored.</p> </li> 
</ol>

