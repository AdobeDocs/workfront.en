---
title: Share Record Types
description: You can share a record type with others to ensure collaboration when using Adobe Workfront Planning.
hide: yes
hidefromtoc: yes
exl-id: bf49db73-09f1-417e-836b-16c6062740d4
---
<!-- add these to metadata on release:

author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog-->

# Share record types

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

You can share a record type with others to ensure collaboration when working with records in Adobe Workfront Planning. 

>[!IMPORTANT]
>
>* Granting permissions to a workspace gives users the same permissions to the record types in the workspace, by default. 
>* Additionally, you can adjust permissions on individual record types.
>* However, you cannot grant people higher permissions to a record type than the permissions they have to the workspace.
>* People with Manage permission to the workspace always keep their Manage access to all record types in the workspace. Their permissions cannot be lowered on record types, even when Inherited permissions are turned off.
> 
> For more information, see the [Considerations when sharing record types](#considerations-when-sharing-record-types) section in this article. 

## Access requirements

+++ Expand to view access requirements. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

You must have the following access to perform the steps in this article:  

 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning.</p> 
<p>Your organization must be onboarded to the Adobe Unified Experience for users to be able to request and grant permissions to a view from a permission request. </p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  <p>Manage permissions to a record type</p>  
   <p>Only users with Manage permissions to a workspace can share Manage permissions to a record type</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerations when sharing record types

* For general information about sharing objects in Workfront Planning, also see [Overview of sharing permissions in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md). 

* Currently you can achieve the following when you share record types:
   * Give people View permissions to a workspace, when you share a record type with them for the first time and they don't have any permissions to the workspace. 
   
      This also gives them View permissions to all record types in the workspace.

      As you give them permissions to the record type, there is an indication in the sharing box that they are also added to the workspace.
   * Make the record type view-only for everyone in the workspace (except for workspace managers), when you turn off Inherited permissions. 
   
      People with Manage permissions to the workspace always have Manage permissions on the record types, even when you turn off Inherited permissions on the record type.
   <!-- checking with Lilit - this doesn't make much sense: * Add people with Contribute permission to the workspace, who will retain Contribute permission to the record type. This way, only the selected people can manage records in the record type, while others can only view them. -->
   * Lower people's permission to a record type. You cannot increase someone's permission to a record type from what they have on the workspace. 
   
      For example, if someone has Contribute permission to the workspace, you can change their permission to a specific record type to View. However, if they have View permission to the workspace, you cannot grant them Contribute permission to any record type. 

* It's not possible to remove access to a record type for people in the workspace. Everyone always has at least View permission.

* You can share a record type internally with the following entities: 

    * Workfront users, groups, teams, companies, and job roles
* You cannot share record types externally, with users outside of Workfront.
* To give a user that does not have workspace permissions higher than View permissions to a record type, you must first share the workspace with them with a higher permission than View.   

## Share permissions to a record type

You can adjust permissions to individual record types of a workspace if you have Manage permission to the workspace. 

{{step1-to-planning}}

1. Open the workspace whose record types you want to share, then click a record type card. 

   This opens the record type page.

1. From the tab of any view, click **Share** in the upper-right corner of the record type. 

   The **Share** box opens.

   ![Permissions for record types with inherited permissions on](assets/permissions-for-record-types-with-inherited-permissions-on.png)

1. (Optional) In the **Who has access** area, select from the following options: <!--the Only invited people is supposed to be removed - rewrite this - according to Vahan-->

   * **Only invited people can access**: You must specify users, groups, team, company, or job roles that you want to share the view with. 
   * **Everyone in the workspace can view**: All users that have View or higher permissions to the workspace can access the view. This is the default option. <!--rewrite this based on what Lilit says in the proof: At this point, once the inherited permissions are disabled, everyone in the workspace except workspace managers will have View permission to the record type because the "Everyone in the workspace can view"  setting cannot be changed. -->

1. (Optional) Expand the **Inherited permissions** option to view users, teams, groups, companies, or job roles that inherit permissions from the workspace.

   >[!TIP]
   >
   >You cannot remove individual entities from the Inherited permissions list.
 

1. (Optional and conditional) If you want to share the record type with specific entities and give them a different access to the record type than they already have for the workspace, do the following:

1. **Turn off** Inherited permissions.

   >[!TIP]
   >
   >Workspace managers continue to have Manage permissions to the record type.

   1. In the **Grant access to this record type** field, add the users, teams, groups, companies, or job roles that you want to grant a different permission level to.
   1. Choose a permission level. 


   >[!IMPORTANT]
   >
   >* You can never give users greater permissions on a record type than they have on a workspace.
   >* You cannot give users a lesser permission than Manage to a record type, if they have Manage permissions to the workspace. 
   >* You can give users a lesser permission to the record type if they have Contribute permissions to the workspace. 
   > For more information, see [Overview of sharing permissions in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md). 

1. To give users who do not have permissions to the workspace access to view record type, in the **Grant access to this view** field, start typing the name of a user, a group, team, company, or job role, then click it when it displays in the list. 

   The entity you selected is added to the record type and to the workspace with **View** permissions. 

   System administrators always receive Manage permissions to record types shared with them, and there is an indication that a user is a System administrator.

1. Click **Copy link** to copy a link to the record type to your clipboard. 
1. Click **Save**.

   The record type is now shared with other users. 

1. Share the copied link with others. Users who receive the link must be active users and log in to Workfront to be able to access the record type page and display it in the selected view. 

<!-- This is not working yet: *************************** edit this before publishing, because this was not tested with record types - this section came from sharing views *******************: 

## Grant permissions to a record type from a permission request

Users who access a link to a record type to which they do not have permissions can request permissions to the record type. All users with Manage permissions to the view receive the permission request and can grant or deny the permissions. 

1. (Conditional) If you are are the manager of a view, you might receive a request from another user to access the view in the following areas:
   
   * An in-app notification
      ![In-app notification for access request for view](assets/in-app-notification-for-access-request-for-view.png)
   * An email notification
      ![In-app notification for access request for view](assets/in-app-notification-for-access-request-for-view.png)
1. (Conditional) From the notification area in Workfront, click the in-app notification
   Or
   From the email notification, click **View all notifications**, then click the notification in the list.

   The **Pending access requests** box displays. 

      ![Notifications list approval box](assets/notifications-list-approval-box.png)
1. (Optional) For the user whose permissions you want to approve, select one of the following options from the drop-down menu to the right of the user's name: 
   * **View**
   * **Manage**
1. Select the user for whom you want to approve or deny the permission, then click **Approve all** or **Deny all**. 
1. Click the left-pointing arrow to the left of **Pending access requests**, then click **Save**.

   If you approved the request, the users are added to the sharing box of the view. The user requesting the permission receives an email confirmation that their request was approved. <!--will they also get an in-app notification??-->

## Remove permissions to a record type

<!-- take this section out - this is what Lilit said: Because of "Everyone in the workspace can view" wildcard, currently it's not possible to entirely remove access to a record type. Let's take out this section. -->

{{step1-to-planning}}

1. Open the workspace whose record types you want to stop sharing, then click a record type card. This opens the record type page.

1. From the tab of any view, click **Share** in the upper-right corner of the record type. 

   The **Share** box opens.
1. Find the user, group, team, company, or job role that whose permissions you want to remove, expand the permissions drop-down menu to the right of their name, then click **Remove**. <!--check the screen shot below - the UI text for View might not be accurate-->

    ![Remove option on record type sharing drop-down](assets/remove-option-on-record-type-sharing-drop-down.png)

1. Click **Save**.

   People no longer have access to the record type. They could still have permissions to the workspace, unless you also remove them from workspace permissions. 
   
   There is no notification for the users that have been removed from accessing the view that they no longer have this access.
