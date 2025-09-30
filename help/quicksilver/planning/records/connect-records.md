---
title: Connect Records
description: After you create connections between record types, you can connect individual records to one another. You can display information from one record on another record when you connect them. 
recommendations: noDisplay, noCatalog
feature: Workfront Planning
role: User, Admin
author: Alina
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
---

# Connect records 

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

You can connect Adobe Workfront Planning records to one another or to objects from other applications. You can display information from one record on another record when you connect them. 

This article describes how you can connect records. For more general information about connecting records, see [Connected records overview](/help/quicksilver/planning/records/connected-records-overview.md). 

You must first connect two record types to each other, or a record type to an object type from another application. This creates connected record fields. You can then connect records to one another or records to other objects from other applications in the connected record fields. 

Connecting records is similar to connecting records to objects from another application. 

For information about connecting record types to one another or to object types from other applications, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 

For an example of connecting record types, see [Example of connecting record types and records](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

You can connect the following: 

* Adobe Workfront Planning records with each other
* Adobe Workfront Planning records with objects from other applications. 

  You can connect records with objects of the types listed below from the following applications:
  
  * Adobe Workfront

    * Projects
    * Portfolios
    * Programs
    * Companies
    * Groups

  * Adobe Experience Manager Assets

    * Image files
    * Folders

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

## Access requirements

+++ Expand to view access requirements.

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
   <li><p>Adobe Experience Manager Assets, if you want to connect AEM assets with Planning records<p>
   <p>You must have an Adobe Experience Manager Assets license and an integration between AEM Assets and Workfront.
    For information, see <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront for Experience Manager Assets and Assets Essentials: article index</a>. </p>
   </li>  
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
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
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
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning objects</p> 
   <p>View or higher permissions to the object types you want to link from Workfront.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Contribute or higher permissions to a workspace and record type to connect records </p>  
   <p>View or higher permissions to a workspace and record type to view all connections to objects and fields from other applications, regardless of your access in the other application. </p>
   <p>View or higher permissions to the objects you want to link from Workfront or Experience Manager Assets. </p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).   

+++

## Considerations for connecting records

* To connect records with other records or objects, you must have the following:

    * At least one workspace, record type, and record. 

        For more information, see the following articles:

        * [Create workspaces](/help/quicksilver/planning/architecture/create-workspaces.md)
        * [Create record types](/help/quicksilver/planning/architecture/create-record-types.md)
        * [Create records](/help/quicksilver/planning/records/create-records.md)

    * Connections between record types, or between record types and objects from other applications. For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

* You can connect one or several records or objects to each other. This depends on the connection type you selected when connecting the record or object types. For information, see [Connect record types overview](/help/quicksilver/planning/architecture/connect-record-types-overview.md). 

## Connect records from Workfront Planning

You can connect records from Workfront Planning in the following areas of a Planning record:

* The connected record fields in the table view.
* The record's preview box or page in the connected record fields on the Details tab.
* The record's preview box or page on the Connections tab.
* The record's page on a Connected records page tab. 

### Connect Workfront Planning records from the table view or the Details area of a record

{{step1-to-planning}}

1. Click the workspace whose records you want to connect. 

    The workspace opens and the record types display as cards.
1. Click the card of a record type to open the record type page. 
1. Click the name of a table view to open it. 
1. (Optional) Add records to the record type that you selected by adding a new row to the table. For information, see [Create records](/help/quicksilver/planning/records/create-records.md). 
1. (Conditional) After you connect the selected record type with another record type, go to the connected field of a record and click inside the field or click **Connect** to add record. 

    ![Connect other records in table view](assets/connect-other-records-smaller-box-in-table-view.png)

1. Do one of the following:

    * Click a connected record's name from the list to add it to the selected record. The record is added automatically.
    * Start typing the name of a record and click it when it displays in the list. The record is added automatically. 

    >[!TIP]
    >
    >If only the image of the record was selected to display when the record types were connected, only the thumbnail or the icon of the record displays in the connected field. For more information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 
    >
    
1. (Conditional) If you selected One to many or One to one for the Connection type when you connected the record types, and you try connecting a record or an object that is already connected elsewhere, you will receive a warning that connecting it again will remove it from the original connection. Click **Connect** to allow the removal and connect the record, or **Cancel** to go back to the field and select another record.
1. (Optional) If you cannot find an object to connect, and you want to add it, click **+ Add** 
 
    Or

    Start typing a name for the object, then click **+ Add** to create and add it. 
    
    For more information, see the section "Create records as you connect them from other records" in the article [Create records](/help/quicksilver/planning/records/create-records.md).
    
    >[!TIP]
    >
    >    You can open a record's page and connect other records by doing the following in the table view:
    >1. Click the name of the record in the view.
    >1. Find the linked record field and double-click the field (if there are records already connected)
    >Or
    >Click **Connect records** (if the field is empty) to add records from the connected record or object type. 
    >
    >![Connect records from record page field](assets/connect-records-from-record-page-field.png)

1. (Optional) Click **See all** to display all records. 

1. (Conditional) If you clicked **See all** in the previous step, the **Connect objects** box displays. 

    ![Connected objects table for records](assets/connected-objects-table-for-records.png)

1. Start typing the name of a record in the search box, then select it when it displays in the list

    Or

    Select the name of one or multiple records in the box, then click **Connect objects**.

    The following are added:

    * The linked records display in the linked record field of the record that you selected in a previous step. 
    * The linked fields are populated with the information from the linked records, if you added linked lookup fields when you connected the record types. 
    
    Updating the linked records updates the linked fields for the records that you are linking from automatically. You cannot manually edit linked fields. 
        
      >[!TIP]
      >
      >* We use "linked fields" and "lookup fields" interchangeably. 
      >
      >* When you choose to connect multiple records when you connected the record types, the field values from the multiple objects are either displayed separated by commas or are aggregated according to the aggregator you chose when connecting the record types.
      >* You cannot add Workfront typeahead fields (including fields like Project Owner, or Project Sponsor) as lookup fields.
      >
      >* Workfront objects' date field information displays in 24 hour format in Workfront Planning, regardless of how it displays in Workfront. 
      >
      >   For example, if a project's Planned Start Date displays as 3:00 PM in Workfront, it will display as 15:00 in Workfront Planning in an imported lookup field.
    
1. (Optional) Close the record type page and go to the workspace you selected. 
1. Click the card for the record type that you linked to. 

    For example, if you connected the **Campaign** record with the Product record, click the **Product** card. 
  
    The record type card should open in the table view. If not, select a table view. 
  
    Notice that the **Campaign** linked record field displays the names of the campaigns you linked to products in the Product record type page. Updating the Campaign information automatically updates the Campaign linked record field for the Product record type.

### Connect Workfront Planning records to Workfront objects from the table view or the Details area of a record

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

After you create a connection between a record type and a Workfront object type, you can connect individual records to objects in Workfront. The Workfront fields you connected are automatically populated on the records you are linking the objects from.

>[!NOTE]
>
>You cannot connect Workfront object types with Workfront Planning record types from Workfront.


{{step1-to-planning}}

1. Click the workspace whose records you want to connect.

    The workspace opens and the record types display as cards.
1. Click the card of a record type to open the record type page. 
1. Select a **Table** view from the **View** drop-down menu.

1. Click **New record**  to add individual records to the record type that you selected. For information, see [Create records](/help/quicksilver/planning/records/create-records.md). 

1. (Conditional) After you connect the selected record type with a Workfront object type, go to the connected field on a record and either click the field, or click **Connect** to add Workfront objects. 

    ![Connect projects in table view](assets/connect-projects-smaller-box-in-table-view.png)

1. Do one of the following:

    * Click an object from the list to add it to the selected record. Objects are listed alphabetically. The object is added automatically.
    * Start typing the name of an object and click it when it displays in the list. The object is added automatically. 

    >[!TIP]
    >
    >You can open a record's page from the view, double-click the linked record field, or click **Connect** in the field to add objects from the connected object type.

1. (Optional) If you cannot find an object to connect, and you want to add it, click **+ Add** 
 
    Or

    Start typing a name for the object, then click **+ Add** to create and add a new project, portfolio, or program. 

    For information, see [Create Workfront objects from Workfront Planning](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)

1. (Optional) Click **See all** to display all objects you have at least permissions to view.

    If you clicked **See all** in the previous step, the **Connect objects** box displays. 

    ![Connect objects box to select projects](assets/connect-objects-box-to-select-projects.png)

1. Start typing the name of a Workfront object in the search box, then select it when it displays in the list

    Or

    Select the name of one or multiple objects in the box, then click **Connect objects**. 

    >[!IMPORTANT]
    >
    >* You can only add Workfront objects you have access to view. 
    >
    >* Once you add Workfront objects, everyone with View or higher permissions to the workspace can view the Workfront objects and their field information, regardless of their permissions or access in Workfront.

    The following are added: 

    * The selected Workfront objects are added to the linked record field. 
    * If you added them when you connected the record type with Workfront, the linked fields (or the lookup fields) of the Workfront objects are automatically populated with information from Workfront.

    For more information about connecting record types with objects from another application, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).
     
1. (Optional) Click the name of a Workfront object connected to a Workfront Planning record either in the linked field of a table view or from the linked field in the record page.

    This opens the Workfront object in Workfront, if you have at least View permissions to the object. 

   >[!TIP]
   >
   >* When you choose to connect multiple records when connecting the record types, the values of the lookup fields are either displayed separated by commas or are aggregated according to the aggregator you chose.
   >
   >* A linked record field is not created for the linked Workfront objects in Workfront.

1. (Optional) From the table view of the record type, hover over the column header of the linked Workfront object, and click the drop-down menu, then click **Edit lookup fields**.

1. Add Workfront object fields from the **Unselected fields** area

    Or

    Remove Workfront object fields fro the **Selected fields** area. 

    This adds or removes linked fields from the Workfront Planning records. The information associated with the removed fields remains in Workfront. 


### Connect Workfront Planning records to Adobe Experience Manager objects from the table view or the Details area of a record

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

>[!IMPORTANT]
>
>You must have an Adobe Experience Manager Assets license, and your organization's instance of Workfront must be onboarded to the Adobe Business Platform or the Adobe Admin Console to be able to connect Workfront Planning records to Adobe Experience Manager Assets.
>
>If you have questions about onboarding to the Adobe Admin Console, see the [Adobe Unified Experience FAQ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

After you create a connection between a record type and Adobe Experience Manager Assets, you can connect individual records to Experience Manager assets. The asset fields you connected from Experience Manager Assets when you created the connection automatically populate on the record type you linked from.

>[!NOTE]
>
>Planning records and their fields are accessible from Experience Manager Assets when your Workfront administrator configures the metadata mapping through the integration between Workfront and Adobe Experience Manager Assets. For more information, see [Configure asset metadata mapping between Adobe Workfront and Experience Manager Assets](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).

To connect records with Experience Manager assets: 

{{step1-to-planning}}

1. Click the workspace whose records you want to connect. 

    The workspace opens and the record types display.
1. Click the card of a record type to open the record type page. 
1. Select a **Table** view from the **View** drop-down menu in the upper-right corner of the record type page.

1. (Optional) Click **New record** to add new records to the record type that you selected. For information, see [Create records](/help/quicksilver/planning/records/create-records.md). 
1. (Conditional) After you connect the selected record type with Experience Manager Assets, go to the connected field on a record and either click the field, or click **Connect** to add Experience Manager assets to the record, then click the **+** icon. 

    >[!TIP]
    >
    >  You can add click the **+** icon in the linked object field in the record page to connect assets to the record.

    The **Select Assets** box displays. <!--we might change this to Connect assets-->

    ![Select assets box for AEM record connections](assets/select-assets-box-for-aem-record-connections.png)

1. Click to select some of the following types of assets:

    * Images
    * Folders

    You can select multiple assets. 

    >[!IMPORTANT]
    >
    > You can connect only assets you have access to view in Experience Manager. Once connected, all Workfront Planning users can view the assets in Workfront Planning, regardless of their access in Experience Manager Assets. 

1. Click **Select**. <!-- we might change this to Connect-->

    The following are added: 

    * The selected Experience Manager assets are added to the linked record field. 
    * The linked fields (or lookup fields) populate with information from the Experience Manager connected assets. 
    
      Any existing information from the fields of the Experience Manager assets displays in the linked or lookup fields automatically. 

      >[!TIP]
      >
      >* When you select to connect multiple records when connecting the record types, the values of the multiple objects display either separated by commas or aggregated according to the aggregator you choose.
      >
      >* A linked record field to the Workfront Planning linked records is not created for the linked Experience Manager assets in the Experience Manager Assets application. 
     
1. (Optional) Go to the record type you linked to Experience Manager Assets from and click the name of an asset in the linked record field. The Experience Manager details of the asset display in a pop-up window. 

    ![Asset pop-up window with AEM details and thumbnail](assets/asset-pop-up-window-with-aem-details-and-thumbnail.png)

    The following fields display for an image file:

    * A thumbnail of the image
    * The image file name
    * Dimensions
    * Size
    * Description
    * The file path in Experience Manager
    * The asset type
    * Date created
    * Date modified 

1. (Optional) To open the Experience Manager assets record page in Experience Manager, go to the record type page of the record you are linking from, click the name of an asset in the linked record field to open the pop-up window, then click the **Open in AEM** icon ![Open asset in AEM icon](assets/open-asset-icon.png) to open the asset. 

   This opens the Experience Manager asset in Adobe Experience Manager Assets.  

1. (Optional) From the table view of the record type, hover over the column header of the linked Experience Manager asset, and click the drop-down menu, then click **Edit lookup fields**.

1. Add Experience Manager Assets object fields from the **Unselected fields** area

    Or

    Remove Workfront object fields fro the **Selected fields** area. 

    This adds or removes linked fields from the records. The information associated with the removed fields remains in Adobe Experience Assets.

### Connect Workfront Planning records with other records or objects from the Connections tab of the record page

1. Go to any view of a record type that has been connected to other Planning record types or object types from other applications. 
1. Follow the steps described in the previous subsections to find a record in the view that you want to connect with other records or objects. 
1. Click the name of a record. 

    The preview page opens. 
1. (Optional) Click the **Open in new tab** icon ![Open details in a new tab icon](assets/open-details-in-a-new-tab-icon.png) to open the record's page. 
1. Click the **Connections** tab in the record's preview or page. 

    ![Connections tab on record in Workfront Planning](assets/connections-tab-on-record-in-workfront-planning.png)

    All record or object types that are linked to the selected record type display as sections. Connected records or objects display under their record or object type names on cards. 

    >[!TIP]
    >
    >    Only connected records that have individual records connected display by default.

1. (Optional) Click **Show all connections** to show all connected record types, including the ones without connected records. 

1. (Optional) Click the downward-pointing arrow to the left of a section to collapse it. 

1. (Conditional) Click **Connect** to add more records or objects of the same type. 
1. (Optional) If you cannot find a record or an object to connect, and you want to add it, click **+ Add** 
 
    Or

    Start typing a name for the object, then click **+ Add** to create and add it to the record. 
    
    For more information, see the section "Create records as you connect them from other records" in the article [Create records](/help/quicksilver/planning/records/create-records.md).
1. Follow the steps described in the previous sections to connect records from Workfront Planning or objects from Workfront or Experience Manager Assets. 
    The records and objects are added immediately.
1. (Optional) Hover over the connected card of a record or object, then click the **Disconnect record** icon ![Disconnect record](assets/disconnect-icon-with-tooltip.png)  to disconnect it from the selected record. 

    ![Disconnect record icon with tooltip on connections tab](assets/disconnect-record-icon-with-tooltip-on-connections-tab.png)

    The record is immediately disconnected from all areas of Workfront Planning or from other applications where it might show as connected. Any lookup field values are also removed. 

### Connect records from the Connected records page of a record 

1. Go to any view of a record type that has been connected to other Planning record types or object types from other applications. 
1. Follow the steps described in the previous subsections to find a record in the view that you want to connect with other records or objects. 
1. Click the name of a record. 

    The preview page opens. 
1. Click the **Open in new tab** icon ![Open details in a new tab icon](assets/open-details-in-a-new-tab-icon.png) to open the record's page. 
1. Click an existing Connected records page tab in the record's page. You must first create a Connected records page. 

    A connected record type page displays in the table view.
    
    All connected records of one type display in the table.  
1. Click **Connect**, <span class="preview">**Connect records**, or **New row**</span> to add or remove records.

    ![Connect button highlighted in connected record details tab](assets/connect-button-highlighted-in-connected-record-details-tab.png)

    For information, see [Manage the record page layout](/help/quicksilver/planning/records/manage-the-record-page.md).
1. (Optional) If you cannot find a connected record, click **+ Add** to create and connect them. 

## Connect records from Workfront objects

You must have the following to connect Workfront Planning records from Workfront objects: 

* Connections between record types and Workfront object types that are established in Workfront Planning.
* Your Workfront or group administrator must add any of the following to a Workfront object type:

    * The Planning section to the Workfront projects, portfolios, and programs in your Layout Template. 

    * The Planning connections custom field to a custom form for one of the following objects:

        * Project
        * Portfolio
        * Program
        * Group
        * Company

    For more information, see [Manage record connections from Workfront objects](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
