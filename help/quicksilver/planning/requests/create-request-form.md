---
title: Create a request form in Adobe Workfront Planning
description: After selecting a record type in Adobe Workfront Planning area, you can create a request form associated with that record type and share a link to it with other internal or external users. 
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
---
# Create a request form in Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

After selecting a record type in Adobe Workfront Planning area, you can create a request form and associat it with that record type. You can then share a link to it with other internal or external users. <!--double-check on the external part of it-->

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

You must have the following to be able to access Workfront Planning: 

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
   <td role="rowheader"><p>Adobe Workfront Planning plan*</p></td>
   <td>
<p>Any </p>   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning.</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>

  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Standard</p>
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
   <td>
   <ul>
   <li><p>Manage permissions to a workspace</p></li>
    <li><p>System Administrators can manage workspaces they did not create. </p></li>
    </ul>
   <p>For information about sharing permissions for Workfront Planning objects, see  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Overview of sharing permissions in Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p>  
</td>
  </tr>
 </tbody>
</table>

*For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).  

+++

## Create a request form for a record type

{{step1-to-planning}}
  
1. Click the workspace where you want to add records.

    The workspace opens and the record types display as cards.

1. Click a record type card. For information about creating a record type, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 

    The record type page opens in the view that you last accessed. By default, a record type page opens in the table view. 

1. Click the **More** menu ![](assets/more-menu.png) to the right of the record type name in the page header, then click **Create request form**.
1. Update the name of the request form. By default, the name of the form is **Untitled request form**. <!--check this; you logged a bug to rename it to this but was it fixed?--> 
1. (Optional) Add a **Description** for the request form. 

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Click **Create**. The request form for the selected record type opens. 

   The request form contains the following information, by default:

   * **Default section**: This is the default section break that Workfront applies to the request form. The Default section cannot be renamed or removed. 
   * **Subject** field: The field which will identify the request in Workfront. This capability is not yet available. 
   * All the fields associated with the record type. 

   The fields contained in the request form will be visible to everyone submitting a request to this record type. 

1. (Optional) Remove the **Subject** field, as this is not visible in Workfront Planning. <!--remove this step when we connect intake with the Requests area in Workfront-->
1. Hover over any fields on the form that you want to remove. They are added to the **Fields** tab on the left side of the form. 
1. Click on any field, then use the controls on the right side of the form to define any of the following information about the fields:

   * **Label**: this is the name of the field as it will appear on the request form. This does not change the name of the record field.
   * **Instructions**: Add more information about the field.
   * **Make a required field**: When selected, the field must have a value. Otherwise, the form cannot be submitted. 
   * **Add logic**: Define what conditions must be met in order for the field to display or be hidden.

1. Click the Content elements tab on the right side of the form, and add any of the following elements:

   * Descriptive text
   * Section Break 

   For more information about building a custom form, see [Design a form with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). 





