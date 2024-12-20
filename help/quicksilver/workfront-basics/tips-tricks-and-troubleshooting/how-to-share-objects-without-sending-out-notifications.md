---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: How to Share Objects Without Generating Notifications
description: Find out how you can share objects and prevent notifications from being send out about this change. This is particularly helpful when you share objects in bulk. 
author: Alina
feature: Get Started with Workfront
---

# How to share objects without generating notifications

<!--Audited: 12/2024-->

When you share an object in Adobe Workfront, the people you are sharing the object with receive an email notification about the sharing. 

Receiving an email notification when someone shares an object with you is important to be aware of this change. However, too many notifications might be too confusing for users. If you want to share a large number of objects with users at one time, temporarily disabling notifications will help avoid the confusion. 

People receive email notifications when the following settings are enabled at the same time: 

* One or both of the following Event Notifications are enabled at the system or group level: 

    * Object Share to User
    * Object Share to Team is enabled at the system or group level.
* One or both of the following email notifications are enabled in the user's profile:

    * Someone shares an object with me
    * Someone shares an object with my team 

If you need to share multiple objects with multiple people (in bulk), but you do not want them to receive email notifications about this change, do the following:

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

You must have the following to share objects:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New license: Standard</p> 
   Or
   <p>Current license: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View access or higher to the objects you want to share</p>
   <p>Edit access to users</p>
   <p><b>NOTE</b></p>
   <p> You must be a system or group administrator to check for the status of Event Notifications for the system or the group</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to the objects you want to share</p></td> 
  </tr> 
 </tbody> 
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Share objects without generating notifications
1. Ensure that the following **Event Notifications** are enabled at the system or group level: 

    * **Object Share to User**
    * **Object Share to Team is enabled at the system or group level**.

    For information, see [Configure event notifications for everyone in the system](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). 

    If these event notifications are not enabled, the notifications about sharing an object will not be sent to the users. If one or both are enabled, continue with the following steps. 

{{step-1-to-users}}

1. Select multiple users in the list, then click **Notifications** > **Miscellaneous**. 
1. Disable one or both of the following notifications (depending on which ones are enabled from the system or group level):

    * **Someone shares an object with me**
    * **Someone shares an object with my team**

    Ensure that all selected users have these notifications selected before you disable them. This way, you can re-enable them in bulk for all of them after you share the objects.

1. Click **Save Changes**.
1. Go to a list of objects that you want to share and select the objects, then click the **Share** icon at the top of the list. 

    For information about sharing a objects in bulk, see [Share an object](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md). 

1. Go back to the list of users for whom you disabled the notifications and select the same users.  
1. Select the same users in the list, then click **Notifications** > **Miscellaneous**. 
1. Enable one or both of the following notifications (depending on which ones are enabled from the system or group level):

    * **Someone shares an object with me**
    * **Someone shares an object with my team** 

1. Click **Save Changes**.

    The objects were shared with the selected users and none of them received any email notifications about this change.






