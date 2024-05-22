---
title: Manage records in the Planning section of Adobe Workfront objects
description: You can display the records connected to Adobe Workfront objects in the Planning section of a Workfront object, in the left panel.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
---
<!--add this to the main TOC and the mini TOC-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--add also Group and Company when they are available-->


# Manage records in the Planning section of Adobe Workfront objects

{{maestro-important-intro}}

You can display the records connected to Adobe Workfront objects in the Planning section of a Workfront object, in the left panel.

The Planning section is available for the following Workfront objects:

* Project
* Portfolio
* Program
<!--* Group
* Company-->

## Access requirements

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
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Workfront Planning beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>View or higher access to Projects, Programs, and Portfolios</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>In Workfront, View or higher permissions to a project, portfolio, or program</a> </p> 
   <p>In Workfront Planning, View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all Workfront Planning workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in the Main Menu and the Planning section in the left panel to your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

## Considerations about the Planning section of Workfront objects

* First, you must connect record types to Workfront object types, and records to Workfront objects to view them in Workfront. 

   For information, see the following articles:

   * [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Connect records](/help/quicksilver/planning/records/connect-records.md)
* You can view the Planning section in a Workfront object, even when there are no records associated with the Workfront object.  
* You can connect Planning records with Workfront objects from Workfront, in the Planning section.

## Manage records in the Planning section

{{step1-to-maestro}}

   The last accessed workspace opens by default. 

1. Click the card of a record type that is connected to a Workfront project, portfolio, or program. 
1. Choose a table view from the **View** drop-down menu.
1. (Conditional) Go to the connected record field in the table and add a Workfront object, then click the name of the Workfront object in the field. For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 
  The objects's page opens in Workfront Planning. 
1. Click **Go to source**, in the upper-right corner of the screen. 

   The object's page opens in Workfront. 
1. Click **Planning** in the left panel. 

      >[!NOTE]
      >
      >   Your Workfront or group administrator must add the Planning section to your layout template before it displays for a Worfront project, portfolio, or program. 

   The Planning section displays with the following information: 
   
   * The connected records display on individual cards that contain the following information:
      * Name of the record
      * The record thumbnail
      * The name of the connected record field as it displays in Workfront Planning. 
   * Records display under their respective workspace. 

   ![](assets/planning-section-on-project.png)

1. Click a record card to display more information about the record. The record preview box displays.
1. (Optional) Start modifying fields in the record's preview box. Your changes are saved automatically. 
1. (Optional) Click the **Open in a new tab** icon ![](assets/open-details-in-a-new-tab-icon.png) in the upper-right corner of the preview box to open the record's details page. 
1. Hover over a record card, then click the disconnect record icon **-**, then click **Disconnect**. 
   The following things occur: 
   * The record is no longer connected to the Workfront object. 
   * The Workfront object is also removed from the record's connected field from Workfront Planning. 
   * The values for the Workfront fields connected to the Planning record are also deleted.
1. Click **Connect** to connect more records. 

   <!--checking with the team on the below note - not sure if if should stay Manage or Contribute - Lilit said Contribute??-->

   >[!NOTE]
   >
   >   The Connect button displays only for the workspaces where you have Contribute permissions. 

1. Click the records you want to connect. The following things occur:

   * The records are immediately connected to the Workfront object and they display in the Planning section. 
   * The Workfront object is added to the Workfront Planning record's connected field. 
   * The values for the Workfront fields connected to the Planning record are populated in Workfront Planning. 

<!--add more steps here for what happens after clicking Connect-->


