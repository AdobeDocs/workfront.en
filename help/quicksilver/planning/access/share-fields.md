---
title: Share Workfront Planning Fields
description: You can share the field of a Workfront Planning record with others to ensure collaboration when using Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
---

# Share Workfront Planning fields

{{planning-important-intro}}

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


You can share the field of a Workfront Planning record with others to ensure collaboration when using Adobe Workfront Planning.

Field sharing lets workspace administrators control access to an individual field. Each field in a record type has its own sharing dialog where access can be set to No Access, View field values, or Manage field values.

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->



 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront or Workflow with a Planning package</p> 
Or
<p>Any Workfront Planning as a standalone product package</p> 
 </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Any</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Planning license</p></td> 
   <td><p>Any</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>You must add both a Workflow and a Planning license type to the access level when you have both a Workflow and a Planning package</p>   
</td> 
  </tr>  
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td><p>Manage permissions to a field to change values for the field</p>  
   <p>Contribute or higher permissions to a record type to inherit Manage permissions to the field</p>  
   </td> 
  </tr>
</tbody> 
</table> 

 For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerations about sharing fields

* You can share fields with users, job roles, groups, teams, or companies. 
* You can only share fields from the table view of a record type. 
* You cannot share the following types of fields:

    * System fields (for example, Created By, Record ID)
    * Primary fields 
    * Lookup fields. They always inherit the permissions of their source object fields. 
* Access to a field comes from combining the following settings:

    * **Inherited permissions**: By default, a field inherits the same access someone has on the record type. You can turn off Inherited permissions and give users a lower access to the field than they have for the record type. 
    * The **Everyone with access to the record type can view** or **Only invited people can access** selection. You can either allow everyone with permissions to the workspace to view the field or give permissions only to individual entities. 

    If multiple rules apply to the same person, they receive the highest permission available to them from one of the rules.
   
* To make a field view-only for everyone in a workspace, ensure the following setup exists: 

   * Turn off inherited permissions
   * Keep the **Everyone with access to the record type can view** setting
   * Do not add any individual entities. 

* Depending on the record type permissions, users can receive the following field permissions:

    * View record type permissions give a user permissions to view field values
    * Contribute or Manage record type permissions give a user permissions to manage field values

* Only workspace owners and managers can adjust field permissions. Workspace managers always retain Manage access to all fields and this cannot be lowered.
* Field sharing controls access to values, not field settings. Only workspace managers can change a field's configuration. 
* Adding someone to a field's sharing list does not grant them workspace or record-type access. If they lack that access, a warning icon indicates the permission will only take effect once they're added to the record type.
* Fields with restricted permissions are enforced everywhere where the field displays. This includes all the views, record details pages, request forms, connections and lookup fields, Canvas dashboards, the API, and MCP tools. 
* Public views remain fully visible and read-only to anyone that can access them. 
<!--Not sure if this is right - right now, it allows me to duplicate with the values in the new record - checking with Lilit: * When you duplicate a record, the restricted values are not copied to the new records.-->
* Restricted field value changes are not recorded in the History of a record. 
* Permission changes for fields don't trigger notifications.
* For global record types, field permissions apply across all secondary workspaces and can't be adjusted locally.

<!--
From Claude: 
Additional permissions for fields - maybe add this to the Overview article for all of the sharing?? - help/quicksilver/planning/access/sharing-permissions-overview.md 

Here's how record type / workspace access maps to field-level access in the document:

Field permission levels (only two, plus none):

No Access – field is completely hidden
View field values – can see the value, can't edit
Manage field values – can view and edit

Default inheritance from record type role

Record type / workspace access    Default field permission
View    View field values
Contribute    Manage field values
Manage (workspace manager)    Manage field values (locked — cannot be reduced)

So by default, a field simply mirrors whatever role someone has on the record type — Viewers get read-only, Contributors and Managers get edit rights. Workspace managers are a special case: whenever they're added to a field's sharing list, "Manage field values" is pre-selected and the "View field values" option is disabled, since their edit access can never be taken away.

Wildcard (fallback) setting
Separate from inheritance, each field has a wildcard default:

Everyone in the workspace can view (default)
Only invited people can access

How the final permission is calculated

If inherited permissions are enabled: a person's access = the highest of (inherited from record type, wildcard, individually granted permission).
If inherited permissions are disabled: a person's access = the highest of (wildcard, individually granted permission) — record type role no longer factors in.
If inheritance is disabled, wildcard is "Only invited people can access," and the person isn't individually added → they get No Access.

Other permission notes

Individually granting access to someone doesn't grant them workspace/record-type access — it just sits inactive (with a warning icon) until they're separately added to the workspace.
For Global Record Types, field permissions are set once and apply to all secondary workspaces; secondary/team workspace managers cannot override them locally.

-->

## Share fields

As a workspace manager, you can adjust permissions to individual fields.

{{step1-to-planning}}

1. Open the workspace, then the record type whose fields you want to share.

1. From the table view, hover over the name of a field's column header, click the **More** menu ![More menu](assets/more-menu.png), then click **Share field**.

   The **Share** box opens.

1. (Optional) In the **Grant access** area, the **Everyone with access to the record type can view** option is selected by default. All users that have **View** or higher permissions to the workspace and record type have the same permissions to the field.

1. (Optional) Click the avatars of users under the **Inherited permissions from** option to view users, teams, groups, companies, or job roles that inherit permissions from the workspace. 

   The user's permissions to the record type displays when you expand the inherited permissions.

   >[!TIP]
   >
   >You cannot remove individual entities from the inherited permissions list. The users from teams, groups, companies or job roles are listed instead of the entities they were associated with when the workspace and the record type was shared with them.

1. (Optional and conditional) If you want to share the field with specific entities and give them a different access to the field than they already have for the record type, do the following:

   1. Deselect the **Turned on** option from **Inherited permissions**. It is selected by default.

      The option changes to **Turned off**.

      >[!TIP]
      >
      >Workspace managers continue to have Manage permissions to the record type and the field.

   1. (Optional) Click the **Everyone with access to the record type can view** dropdown menu and select **Only invited people can access**. 

      >[!IMPORTANT]
      >
      >This change together with turning off **Inherited permissions** removes the access for all the people who can view the record type and only give access to designated people. Workspace managers and administrators will always have access to all the fields. 


   1. In the **Grant access** box, add the users, teams, groups, companies, or job roles that you want to grant a different permission level to than they have for the workspace or the record type.

      When you share a field with a user, their primary job role and their email also display in the field. You must have the View Contact Info setting enabled for the Users object in your access level to be able to view the user's email.

   1. Choose one of the following permission levels:

      * View field values
      * Manage field values

      >[!IMPORTANT]
      >
      ><!-- * If users have Contribute or Manage permissions to the workspace and the record type, you can give them Manage permissions to the field. The View permission is dimmed.-->
      >* You cannot give users a lesser permission to the field if they have Contribute or higher to the record type.
      >
      >* You cannot grant permissions to users who are not in the workspace. Users who do not have permissions to the workspace and record type cannot access any of the fields. They will be able to access the fields when they get permissions to the workspace and record types. 

1. Click **Save**.

   The field is now shared with other users.

    <!--
    Not possible for fields: 
    The users you shared the field with receive both an in-app and email notification about having been given permissions to the field.
    For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md).
    -->  

## Remove permissions to a field

You can remove users' permissions from a field. However, they will retain at least View permissions to the workspace and record type which also gives them at least View permissions to the field.

You must remove their access from the workspace if you want them to have no permissions to the record types or fields in the workspace.

You cannot remove a user from Inherited permissions.

{{step1-to-planning}}

1. Open the workspace whose fields you want to stop sharing, then click a record type card. This opens the record type page.
1. From the table view, hover over the name of a field's column header, click the **More** menu ![More menu](assets/more-menu.png), then click **Share field**.

   The **Share** box opens.
1. Find the user, group, team, company, or job role that whose permissions you want to remove, expand the permissions drop-down menu to the right of their name, then click **Remove**.

1. Click **Save**.

   People no longer have the indicated permissions to the field. However, they still have permissions to the record type and the workspace, unless you also remove them from those permissions.

   There is no notification for the users that have been removed from accessing the field that they no longer have these permissions.
