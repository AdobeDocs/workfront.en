---
title: Share Planning requests
description: You can share a Workfront Planning request with others after it's been submitted. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
# Share Planning requests

<!--add to TOC, and miniTOC-->

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

After a Planning request is submitted, you can control who sees it, who can work on it, and what actions each person or team is allowed to take. This keeps the right people focused on the right requests — and ensures they can take only the actions appropriate to their role.

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront or Workflow with a Planning package</p> 
Or
<p>Any Workfront Planning when purchased as a standalone product</p> 
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
   <td>   <p>View or higher permissions to a workspace and record type, if you are a Workfront user</p>  </td> 
  </tr>  
</tbody> 
</table> 

For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerations when sharing requests

* You can grant the following permissions to users to a request: 

    * View: Users can only see the request.
    * Contribute: Users can view, edit, and comment on the request.
    * Manage: Users can view, edit, comment on, and delete the request.

* Requesters are automatically granted Manage access to the requests they submit, unless an admin has configured a different default.
    
    For information, see [Create request form](/help/quicksilver/planning/requests/create-request-form.md). 

* Workfront administrators can access and manage all requests.
* Users with Manage access to a record type inherit Manage access to that record type's intake form and to every request submitted through it.
* Anyone with permissions to a request can share the request with the same permission level or lower a lower level than their own. 

    Users with Contribute permissions cannot give anyone else Manage permissions to the request. 

* Different people and teams can hold different levels of access on the same request.
* Permissions could be assigned through multiple entities. If a user has Contribute permissions to a request but their group or job role has View permissions, they retain the highest level of permissions which is Contribute. 
* Requests inherit permissions from the workspace and the record type. You cannot remove or edit Inherited permissions for Planning requests.

## Share a request

Ensure you are using the new request experience.

1. {{step1-to-requests}}
1. Find a Planning request and click it to open it. 
1. Click **Share**. 

    The **Share** box opens for the selected request.

    ![Requests sharing box](assets/requests-sharing-box.png)

1. In the **Grant access to this request field**, start typing the name of a user, team, role, group or company and click it when it displays on the list. 

    Only active entities display in the list. 
1. From the drop-down menu to the right of each entity's name, select one of the following permissions levels:

    * Manage
    * Contribute
    * View
1. (Optional) For each permission level, click the granular permission icon and select or deselect any granular permissions, like **Edit**, **Comment**, **Share**, or **Delete**. 

    ![Granular permissions on requests](assets/granular-permissions-on-requests.png)
1. (Optional) Expand the Inherited permissions line to view who gains permissions from the workspace and the record type.

    >[!TIP]
    >
    >You cannot remove or edit Inherited permissions for Planning requests.

1. Click **Save**.


    The request is shared with the entities you selected. 


