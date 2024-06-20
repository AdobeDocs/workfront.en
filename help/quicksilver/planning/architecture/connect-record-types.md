---
title: Connect record types
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Adobe Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
---
<!-----
title: Connect record types
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Adobe Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application.
hidefromtoc: yes
hide: yes
feature: Work management
role: User
author: Alina
--->

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->
<!--************ THIS MIGHT NO LONGER BE A 'RELATIONSHIP' TYPE FIELD, BECAUSE THEY WILL SHOW IT IN THE CONNECTION TAB*****************************-->


# Connect record types

{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

You can connect record types to one another or record types with object types from other applications. 

This article describes how you can connect two Workfront Planning record types a Workfront Planning record type with an object from another application. 

After you establish the connection between records or object types, you can connect individual records to one another, and display fields from the linked record or object types on a Workfront Planning record. 

For information about connecting a Workfront Planning record to an object from another application, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

For an example of connecting record types and records, see [Example of connecting record types and records](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md). 

<!--ensure this last linked article is right; the title and the link should have changed-->

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
   <p> Adobe Workfront</p> <p>To connect Adobe Workfront Planning record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
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
   <p>Current: Plan</p>
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

<!--Maybe enable this at GA - but planing is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>--> 


## Considerations about connecting record types

* You can connect the following entities in Adobe Workfront Planning:

    * Two record types

        The record types must belong to the same workspace. 
    * A record type and an object type from another application. 

* You can connect Workfront Planning record types with the following object types from the following applications:

    * Adobe Workfront:

        * Projects
        * Portfolios
        * Programs
        * Companies
        * Groups

    * Adobe Experience Manager Assets:

        * Images
        * Folders

        >[!IMPORTANT]
        >
        >You must have an Adobe Experience Manager Assets license, and your organization's instance of Workfront must be onboarded to the Adobe Business Platform or the Adobe Admin Console to connect Workfront Planning records to Adobe Experience Manager Assets.
        >
        >If you have questions about onboarding to the Adobe Admin Console, see the [Adobe Unified Experience FAQ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* After you create individual records for a record type, you can select the records you connect to from the linked record type field. For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

* After you connect a record type with another record type or with an object type from another application, the following scenarios exist: 
    
    * **When you connect two record types**: A linked record field is created on the record type you're connecting from. A similar linked record field is created on the record type you are connecting to. 

        For example, if you connect the "Campaign" record type with the "Product" record type, a linked record field that you name "Linked Product" is created on the Campaign record type and a linked record type automatically named "Campaign" is created on the Product record type. 

    * **When you connect a record type with an object type from another application**: 
    
        * A linked record field is created on the record type you're connecting from. No linked record field is automatically created on the other application's object type. 
        
        * A new Workfront Planning read-only record type is created for the other application's object only when actual objects are connected to Workfront Planning records.  

            For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

        * Planning records fields are not accessible from Workfront objects.
        * Planning record fields are accessible from Experience Manager assets when your Workfront administrator configures the metadata mapping through the integration between Workfront and Adobe Experience Manager Assets. For more information, see [Configure asset metadata mapping between Adobe Workfront and Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
    
    * **When you add linked (or lookup) fields of the record or object you connect to**: You can connect fields from the other application's object to the Workfront Planning record type. Linked fields are read-only and they automatically display information from connected records or objects when you connect the records or the objects. 

        For example, if you connect the "Campaign" record type with a Workfront project and you select to bring the Planned Completion Date field of the project to the Workfront Planning record, a linked field called Planned Completion Date (from Project) is automatically created for the campaign. You cannot manually edit this linked field. The Planned Completion Date (from Project) field displays the Planned Completion Date of the linked projects.  

        >[!IMPORTANT]
        >
        >    Everyone with View or higher permissions to the workspace can view the information in the linked fields, regardless of their permissions or access level in the application of the linked object types.

* Linked record fields are preceded by a relationship icon ![](assets/relationship-field-icon.png). 
    
    Linked fields are preceded by an icon that identifies the field type. For example, linked (or lookup) fields are preceded by icons that indicate that a field is a number, a paragraph, or a date. 


## Connect record types

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}} 

1. Click the workspace whose record types you want to connect, 

    Or

    From a workspace, expand the downward-pointing arrow to the right of an existing workspace name and select the workspace that you want to connect record types from.
1. Click the card of a record type to open the record type page. 
1. Click the **+** icon in the upper-right corner of the table view, then click the **New connection** tab.

    ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. In the **Record type** field, search for a record type, or select one of the following: 

    * Another record type from the section of the workspace you selected

        ![](assets/new-connection-tab-fields-with-another-record-selected.png)

        >[!TIP]
        >
        >Only record types from the workspace you selected are available to connect to. 
        > 
        >If you don't have other record types in the selected workspace, the workspace section does not display. 

    * A **Project, Portfolio, Program, Company**, or **Group** from the **Workfront Object Types** section.

        ![](assets/workfront-project-connection-selection.png)

    * **Experience Manager Assets** from the **Adobe Applications** section. 

        ![](assets/aem-assets-connection-selection.png)

1. Update the following information: 

    * **Name**: The name of connected field, as it will appear in the table view or the record page of the original record type. This creates the linked record column in the table view of the original record type or the linked record field for the original records. By default, the name of the field is the name of the record or object you connect to. 

    >[!TIP]
    >
    >You can have multiple connections to the same record or object type. If you do not edit the connected field name, Workfront adds a numeral after the name of the connected record, to indicate the number of connected record types by the same name. 

     * **Description**: Additional information about the connected record field. The description of a field displays when you hover over the field's column in a table. 
     * **Allow multiple records**: Select this option to indicate that you allow that users can add multiple records when the linked record type field displays on the original records. This is selected by default.
     * **Select lookup fields**: Select this option to add fields from the selected record type. The lookup fields are fields associated with the record or object type that you are linking to. Linking them displays information from the record or object you're linking to on the record you are liking from. This is selected by default. 

        >[!TIP]
        >
        > You cannot add the following field types as lookup fields:
        >
        >    * People
        >    * Created by
        >    * Last modified by
        >    * Workfront typeahead fields (including fields like Project Owner, or Project Sponsor)

1. (Conditional and optional) If you selected to connect a Workfront object, select a **Custom form** from the **Link only objects that match these criteria** section. Only objects that have the selected custom forms attached can be linked to the selected record type. You can select more than one form.  

    >[!NOTE]
    >
    > You must create custom forms in Workfront for the selected objects before they display in this list.

1. (Conditional) If you selected to connect to Experience Manager Assets, select a repository from the **Experience Manager repository** drop-down menu in the **Link assets from the following repository** section. This is a required field. Only repositories you have access to in Experience Manager Assets display in this field. 

    >[!NOTE]
    >
    >Your Workfront administrator can map Workfront Planning fields to Experience Manager Assets fields through the Metadata mapping in Workfront. For more information, see [Configure asset metadata mapping between Adobe Workfront and Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en). 

1. (Conditional) If you selected to connect to Experience Manager Assets or to a Workfront Planning record type, disable the **Title** toggle in the **Record appearance** area, if you don't want the title of connected records or assets to display in the linked field. When disabled, only records' thumbnails display in  the linked fields. Records without a thumbnail image display an image icon instead. The toggle is enabled by default. An example of how the connected records will display shows in the **Record appearance** area. 

    >[!TIP]
    >
    >    When you allow multiple records to be linked, displaying only the thumbnail might save space in smaller areas, like record views.
    >
    >The title of a record is the primary field of the record. For more information, see [Primary field overview](/help/quicksilver/planning/fields/primary-field-overview.md). 

1. Click **Create**.

1. (Conditional) If you selected the **Select lookup field** setting, the **Add lookup fields** box opens. 

    Click the **+** icon  to add fields from the **Unselected fields** area. 

    Or
  
    Click the **-** icon to remove fields from the **Selected fields** area

    ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

    The values for the connected fields populate automatically after you link records or objects. 

    >[!IMPORTANT]
    >
    >    Everyone with View or higher permissions to the workspace can view the information in the linked fields, regardless of their permissions or access level in the application of the linked object types.
    
    
1. (Optional) Click **Skip** to skip adding fields from the linked record or object type. The **Name** or the **Title** of the linked record is the only visible field in the table view of the record type you connect from. 

1. (Optional and conditional) If you select to link a number, currency, percentage, or date-type field, also select an aggregator value. The values for the linked fields display either separated by commas or as a aggregated value according to the aggregator you choose, when users select more than one linked record in the linked record field. 

    >[!IMPORTANT]
    >
    >    You must select an aggregator value when adding lookup date fields, if you want the fields to be available to add as Start and End Dates for the timeline and calendar views. For example, you can select the MAX or the MIN aggregator for a lookup date field. 

    ![](assets/aggregator-drop-down-for-number-linked-field.png)  

    >[!NOTE]
    >
    > Aggregators are not available when connecting record types to Experience Manager Assets.  

    Select from the following:

    * **None**: Displays the values that come from multiple records separated by commas. This is the default selection. 
    * **MAX**: Displays the highest value from all the values that come from multiple records selected in the linked record field. 
    * **MIN**: Displays the lowest value from all the values that come from multiple records selected in the linked record field. 
    * **SUM**:  Displays the total of all the values that come from multiple records selected in the linked record field.
    * **AVG**: Displays the average of all the values that come from multiple records selected in the linked record field.
    * **UNIQUE**: Removes duplicates from the lookup field values and only shows the unique values. This is not available for the following field types:
        * Paragraph
        * Checkbox
        * People

    >[!NOTE]
    >
    >For example, you can link the Product record (linked record) from the Campaign record (original record) and name it "Product field". You can also choose to link the Budget field of the Product record from the Campaign record and call it "Product Budget". If you allowed to select multiple records in the "Product field", you can select Product 1 with a Budget of $100,000 and Product 2 with a Budget of $110,000, and Product 3 with a Budget of $100,000. You can view the following Budget information in the linked field from the original record, depending on which aggregator you choose: 
    >
    >* **None**: $100,000, $110,000, $100,000
    >* **MAX**: $110,000
    >* **MIN**: $100,000
    >* **SUM**: $310,000
    >* **AVG**: $103,000.33 
    >* **UNIQUE**: $100,000 
    >

1. (Optional) Use the **search** icon ![](assets/search-icon.png) to search for a field.

1. Click **Add fields** to save your changes.

    The following items are added: 

    * A linked record field on the record type you are linking from. The linked record field will display individual records from the linked record type, after you manually add them. For information about adding records, see [Connect records](/help/quicksilver/planning/records/connect-records.md). The name of the linked record field is the name you selected in step 7. <!--accurate--> 
    
    * A linked (or lookup) field (or fields) that display information about the linked record or object types after you manually add the records or objects in the linked record field. Lookup fields are created only when the **Select lookup fields** setting is selected when creating the connection. Lookup fields are automatically named according to this pattern: 

        `<Name of the original field on the linked record> (from <Name of your linked field>)`

        For example, if you linked a Campaign record type with a Program record type and name the Program linked record field "Program information", then select to also display the Program's Budget field in the Campaign's table view, the linked field is automatically named `Budget (from Program information)` in the campaign's table view. 

    * When you link record types to one another, a linked record field is also added on the record type you are linking to. The name of the linked record field on the linked record type is the name of the record type that you link from. 
    
        For example, if you link the "Product" record type from the "Campaign" record type and you name the connected field of the Campaign "Linked Product", a "Campaign" linked record field is created for the Product record type. 

        >[!TIP]
        >
        > A linked record field  is not created for objects from another application to the record type you are linking from in Workfront Planning.

1. (Optional and conditional) From either the original record type or the linked record type table view, click the downward-pointing arrow in the header of the linked record fields, then click one of the following:

    * **Edit field**: You can update the **Name** and the **Description** information of the field. 
    * **Edit lookup fields**: Add or remove any of the linked record's fields. 

    ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

    To add or remove lookup fields, follow the directions in steps 10-14 above. <!--ensure these step numbers stay accurate--> 

    >[!NOTE]
    >
    > You cannot add lookup fields that belong to record types that you are linking from to object types from another application.  
    >
    > For example, you cannot add the lookup field of "Campaign Status" to a Workfront project you are linking to from the campaigns.
    
1. (Optional) Click the downward-pointing arrow in the header of a linked record field or the header of a lookup field from the record type you are linking from, then click **Delete**. 

    The record field or the lookup field are deleted. If you delete a record field, any lookup fields associated with the linked record are also deleted.
