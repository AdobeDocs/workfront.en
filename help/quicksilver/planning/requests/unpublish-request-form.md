---
title: Unpublish a Request Form in Adobe Workfront Planning
description: You can unpublish a request form if it is no longer needed or relevant. By unpublishing, you remove everyone's permissions to access the form.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: df8c4926-e258-49c0-ab9d-563ccaf7a6aa
---
# Unpublish a request form in Adobe Workfront Planning


<!--take Preview and Production references at Production time-->

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

You can unpublish a request form if it is no longer needed or relevant. By unpublishing, you remove everyone's permissions to access the form. 

You can also change the entities you share a request form with, if you want to keep it available to a smaller group of people. 

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront packages</p></td> 
   <td> 
<ul><li><p>Any Workfront package</p></li>
And
<li><p>Any Planning package</p></li></ul>
Or
<ul><li><p>Any Workflow package</p></li>
And
<li><p>Any Planning package</p></li></ul>
   </td> </tr>

  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table> 

For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Change the sharing of a request form

If you share a request for publicly, with everyone including users from outside your organization, you might consider restricting this access to certain users who either view or manage the workspace the form is associated with. 

To change the sharing of a request form: 

{{step1-to-planning}}
  
1. Click the workspace where you want to add records.

    The workspace opens and the record types display as cards.

1. Click a record type card. For information about creating a record type, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 

    The record type page opens in the view that you last accessed. By default, a record type page opens in the table view. 

1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name in the page header, then click **Manage request forms**.

   All request forms associated with the record type display in a table view. 
1. Hover over the name of a request form, then click the **More** menu ![More menu](assets/more-menu.png) to the right of its name, then click **Share**. 
1. Update the sharing choices by selecting one of the following: 

   * Anyone with view or higher access to the workspace
   * Anyone with contribute or higher access to the workspace
   * Anyone with the link

   For more information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md). 
1. (Optional) Click **Copy link**, if you changed the sharing of the request form and you want to share it to the new group of people with a new link. 

## Unpublish a request form for a record type

When a request form becomes irrelevant and you don't want anyone to access it any longer, you can unpublish it. 

{{step1-to-planning}}
  
1. Click the workspace where you want to add records.

    The workspace opens and the record types display as cards.

1. Click a record type card. For information about creating a record type, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 

    The record type page opens in the view that you last accessed. By default, a record type page opens in the table view. 

1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name in the page header, then click **Manage request forms**.

   All request forms associated with the record type display in a table view. 
1. Hover over the name of a request form, then click the **More** menu ![More menu](assets/more-menu.png) to the right of its name, then click **Unpublish**

Or

Click the name of the request form to open it, then click **Unpublish** in the upper-right corner of the request form.

   ![Unpublish button highlighted](assets/unpublish-button-highlighted.png)

   A confirmation displays at the bottom of the screen notifying you that the form was unpublished. 

   The **Unpublish** link or button changes to **Publish**. 

1. (Conditional) Click **Save**, if you unpublished the form after opening it. 

   Users can no longer access the request form from a link or from the request queue in the Requests area of Workfront. 
    
   Any records previously added using the request form remain on the record type page. 

   Any requests previously added remain in the Requests area of Workfront, on the Planning tab.
