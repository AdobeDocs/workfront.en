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

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

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
* Access to a field comes from combining the following settings:

    * **Inherited permissions**: By default, a field inherits the same access someone has on the record type (View record type permissions give a user permissions to view field values; Contribute or Manage record type permissions give a user permissions to manage field values). You can turn off Inherited permissions and give users a lower access to the field than they have for the record type. 
    * The **Everyone in the workspace can view** or **Only invited people can access** selection. You can either allow everyone with permissions to the workspace to view the field or give permissions only to individual entities. 

    If multiple rules apply to the same person, they receive the highest permission available to them from one of the rules.

* Only workspace owners and managers can adjust field permissions; workspace managers always retain Manage access to all fields and this cannot be lowered.
* Field sharing controls access to values, not field settings. Only workspace managers can change a field's configuration. 
* Adding someone to a field's sharing list does not grant them workspace or record-type access. If they lack that access, a warning icon indicates the permission will only take effect once they're added to the record type.
* System fields (for example, Created By, Record ID) and primary fields cannot have restricted sharing.
* Restricted fields are enforced everywhere where the field displays. This includes all the views, record details pages, request forms, connections and lookup fields, Canvas dashboards, the API, and MCP tools. 
* Lookup fields inherit the permissions of their source field.
* Public views remain fully visible and read-only to anyone that can access them. 
* When you duplicate a record, the restricted values are not copied to the new records.
* Restricted field value changes are not recorded in the History of a record. 
* Permission changes for fields don't trigger notifications.
* For global record types, field permissions apply across all secondary workspaces and can't be adjusted locally.


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

## Share fields

