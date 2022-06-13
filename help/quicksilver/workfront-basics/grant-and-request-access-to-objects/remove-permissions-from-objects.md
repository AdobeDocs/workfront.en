---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: Remove permissions from objects
description: You can remove other users' permissions on objects that you have access to Share. Removing permissions from objects is identical for all objects that can be shared.
feature: Get Started with Workfront
---

# Remove permissions from objects

You can remove other users' permissions on objects that you have access to Share. Removing permissions from objects is identical for all objects that can be shared.&nbsp;

Similar considerations as for sharing objects apply for removing permissions from objects.&nbsp;For more information, see the section [Considerations about sharing objects](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider) in the article [Overview of sharing permissions on objects](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

## Access requirements

You must have the following to share objects:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you want to share</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to the objects you want to share</p> <p>Manage permissions to remove inherited permissions on objects</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Remove entities from the sharing list of an object {#remove-entities-from-the-sharing-list-of-an-object}

You can remove entities (users, job roles, teams, groups, companies) from the sharing list of an object.&nbsp;This removes their permissions to the object.

1. Go to the object you want to share.

   For information about which objects can be shared, see [Overview of sharing permissions on objects](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Click the **More** icon ![](assets/more-icon.png)next to the object name, then click&nbsp;**Sharing** or**Share.**

   ![](assets/share-a-document-350x160.png)

1. Click the **x** next to the name of a user, team, group, company, job role to remove them in the object access box.

   ![](assets/remove-permissions-on-project-nwe-350x479.png)

1. In the `<User Name>`'s Workfront access will be removed from this drop-down menu, select whether you want their access to be removed just from the object you have selected, or from all children objects associated with it.  
   The following scenarios exist:

   * If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they were previously granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.&nbsp;
   * If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they were previously given individual permission on each child object.&nbsp;

1. Click **Save**.

## Remove permissions from several objects in bulk

You can remove entities (users, job roles, teams, groups, companies) from several objects at a time when you bulk select them in a list.&nbsp;

>[!NOTE]
>
>You cannot view what access entities have for all the objects selected when you select them in bulk. You must know which entity you want to remove from the sharing of the objects selected before removing their permissions.

1. Go to the list of objects that you want to share.

   For information about which objects can be shared, see [Overview of sharing permissions on objects](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Select several objects in the list, then click the **Share** icon ![](assets/share-icon.png)at the top of the list. 
1. Type the name of the user, role, team, group, or company for which you want to remove the access in the **Edit `<Object Name>` access to** field. 
1. From the access drop-down menu, select **No Access**.

   ![](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. In the `<User Name>`'s Workfront access will be removed from this drop-down menu, select whether you want their access to be removed just from the objects that you have selected, or from all other children objects associated with it.  
   The following scenarios exist:

   * If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they were previously granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.&nbsp;
   * If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they were previously given individual permission on each child object.

   **Example:** Select whether to remove permissions to just the tasks you selected in a list, or to the issues and documents attached to the tasks as well.

   ![](assets/remove-permissions-bulk-drop-down-for-attached-objects-nwe-350x96.png)

1. (Optional) To change permissions in bulk for several objects, select another level of sharing for the selected entity.

   For example, if they have Manage permissions, select Contribute or View instead. 

1. Click **Save**.

## Remove inherited permissions

Inherited permissions can be removed from objects allowing for owners to specifically&nbsp;identify who will get access to children objects regardless of the access of a user to a parent object.

>[!IMPORTANT]
>
>Only users with Manage permission are able to remove inherited permissions.

To remove inherited permissions:

1. Go to an object to which you have Manage permissions. For example, go to a task.   
1. Go to the object access box as described in the [Remove entities from the sharing list of an object](#remove-entities-from-the-sharing-list-of-an-object) section in this article.
1. Select the **x**&nbsp;next to **Inherited Permission**&nbsp;on the sharing box to remove&nbsp;anyone listed there.

   ![](assets/remove-inherited-permissions-on-project-nwe-350x475.png)

   This ensures that no one who is granted permissions to the parent object (for example, the project) has permissions to this task by default. You must list&nbsp; individual entities in the sharing list of the task to grant permissions on the task.

   >[!TIP]
   >
   >You cannot remove individual entities from the Inherited Permissions list. You can only disable the Inherited Permissions for all entities listed.

1. Click **Save**.&nbsp;

## Make an object private

If you have shared an object system-wide, or you have shared it with external uses by making it public, you can make it private again by removing the system-wide or public permissions.&nbsp;

For more information about making an object available system-wide, or publicly, see [Share an object](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

To make an object private:

1. Go to the object you want to make private.  
   For example, navigate to a report.
1. Click **Report Actions**, then **Sharing**.

   ![](assets/report-permissions-make-private-nwe-350x477.png)

1. Click **Remove public access** to remove the access of external users to viewing the report.
1. Click **Remove system-wide access** to stop sharing it with all Workfront users.&nbsp;
1. Click **Save**.

