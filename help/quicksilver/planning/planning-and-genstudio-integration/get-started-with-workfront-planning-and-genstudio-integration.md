---
title: Get Started with the Workfront Planning and GenStudio for Performance Marketing Integration
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products. Learn some of the basics about how you can streamline your workflows using this integration.
hide: yes
hidefromtoc: yes
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
---
# Get started with the Workfront Planning and GenStudio for Performance Marketing integration

<!--Better metadata, at publishing:
---
title: Get Started with the Workfront Planning and GenStudio for Performance Marketing Integration
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products. Learn some of the basics about how you can streamline your workflows using this integration.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

---
-->

<!--use this article to make this one similar to it: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-integrations/review-approval-integrations/wf-proof-and-genstudio-->


There is a native integration between Adobe GenStudio for Performance Marketing and Adobe Workfront Planning. The purpose of this integration is the prevent users from having to switch back and forth between the two applications to update identical or similar information. 

You can now update or create your campaigns in either GenStudio or Workfront Planning and continue working on them from either application. 

The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products.

With the integration between Workfront Planning and GenStudio for Performance Marketing, you can:

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* View the GenStudio workspace in Workfront Planning. 
* Modify your campaigns in GenStudio and have real-time updates of the same information in Workfront Planning. 
* Modify your campaigns in Workfront Planning and have real-time updates of the same information in GenStudio. 

## Access requirements

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
   <li><p> Adobe Workfront Planning<p></li>
   <p><li> Adobe GenStudio for Performance Marketing<p></li>
   </ul></td> 
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
   <td role="rowheader"><p>Adobe Workfront Planning package</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p> System administrator</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Contribute or higher permissions to a workspace and record type  </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Integration requirements

* Workfront and GenStudio for Performance Marketing must be enabled to the same organization. If your company has multiple Workfront instances, only one can be integrated with GenStudio for Performance Marketing. 

* The Workfront instance is part of the Adobe Unified Experience, including using the Identity Management System (IMS). 

    For information, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Users using both Planning and GenStufio can belong to only one Workfront instance within the IMS organization.

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->


## Considerations for managing a GenStudio workspace in Workfront Planning

* Your organization must purchase Adobe GenStudio for Performance Marketing before you can view a GenStudio workspace in Workfront Planning.

    For more information about GenStudio, see [Adobe GenStudio for Performance Marketing User Guide](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home). 

    For more information about the GenStudio and Workfront Planning integration, see [Get started with the Workfront Planning and GenStudio for Performance Marketing integration](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)

* Workfront users must have access to GenStudio to be able to see the GenStudio workspace in Workfront Planning. 


* The following sections describe what are some limitations for what you can and cannot manage in a GenStudio workspace from Workfront Planning. 

### The GenStudio workspace in Workfront Planning

* If your organization has multiple Workfront instances, only one instance of Workfront can display your GenStudio workspace.
* The GenStudio workspace displays a visual indicator that makes it clear that it is imported from GenStudio.

### Record types

* You cannot edit record types from GenStudio in Workfront Planning. 
* You cannot share record types from GenStudio with other users. Workfront administrators can view the GenStudio workspace in their Planning area. 
* Record types that are synced with GenStudio display a visual indicator that makes it clear that the record types is imported from GenStudio.

### Records

* You can add or delete records in GenStudio and they become visible in (or are removed from) Workfront Planning. 
    You can add or delete records in Workfront Planning and they become visible in (or are removed from) GenStudio. 
* You can add records from Workfront Planning in the following ways:

    * Manually, from scratch
    * By importing them using a CSV or Excel file

    For information, see [Create records](/help/quicksilver/planning/records/create-records.md). 
* You cannot create or delete Activation records from Workfront Planning. 

### Fields

* All record fields are imported from GenStudio and the field settings cannot be edited. 
* You can create fields for GenStudio record types in Workfront Planning only if you have system administrator access in GenStudio. 
* You can edit record information on all records in the GenStudio workspace in any of the visible fields from Workfront Planning. 

    For information, see [Edit records](/help/quicksilver/planning/records/edit-records.md). 
* You can hide fields in the table view of a GenStudio record type, but you cannot delete fields from Workfront Planning.

<!-- checking: 
I had this from Iskuhi, so not sure if you CAN create fields in Planning?? - only the newly added fiedsl can be changed or the reference fields. - from this: https://experience.adobe.com/?commentID=6848549f00000091e5f5a16636e381c0#/@adobeinternalworkfront/so:hub-Hub/workfront/project/67649bc00000545810daad1cd1fbb9cc/updates 
-->

<!--document who shows up in the Created by and Updated by fields - not clear, asking-->

### Views

* You can create views for GenStudio record types. You cannot edit views automatically imported from GenStudio, but you can change the view elements for the GenStudio table view. For example, you can modify the filters, sort, groupings, row colors and row height in the table view. 

    For information, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md). 

* You can share the view of a GenStudio record type in the following ways:

    * Copy the view link
    * Export the view to a file (available only for the table view)

### Connections

* You cannot connect other record or object types from GenStudio record types in Planning. 
* You can connect to GenStudio record types from other record types in Planning. 
