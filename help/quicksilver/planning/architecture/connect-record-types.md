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

{{maestro-important-intro}}

You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. 

You can connect record types to one another or record types with object types from other applications. 

By doing this, you can display fields from the linked record or object type on a Workfront Planning record.  

This article describes how you can connect two record types in Workfront Planning or a record type with an object from another application. 

After you establish the connection between records or object types, you can connect individual records to one another. 

For information about connecting a Workfront Planning record to an object from another application, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

For an example of connecting record types, see [Example of connecting record types and records](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md). 

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
<p>Your organization must be enrolled in the Adobe Workfront Planning closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
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


<!--Maybe enable this at GA - but planing is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>--> 


## Considerations about connecting record types

* You can connect the following entities in Adobe Workfront Planning:

    * Two record types

        The record types must belong to the same workspace. 
    * A record type and an object type from another application. 

* You can connect the following object types from the following applications with Workfront Planning record types:

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

    * **When you connect a record type with an object type from another application**: A linked record field is created on the record type you're connecting from. No linked record field is automatically created on the other application's object type. 
        
        A new Workfront Planning read-only record type is created for the other application's object only when actual objects are connected to Workfront Planning records. 
    
        For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 
    
    * **When you add lookup fields of the record or object you connect to**: You can connect fields from the other application's object to the Workfront Planning record type. These are linked or lookup fields. Linked fields automatically display information from connected records or objects when you connect the records or the objects. The linked lookup fields are always read-only and populate automatically with the values of the connected records or objects. 

        For example, if you connect the "Campaign" record type with a Workfront project and you select to bring the Planned Completion Date field of the project to the Workfront Planning record, a linked field called Planned Completion Date (from Project) is automatically created for the campaign. You cannot manually edit this linked field. The Planned Completion Date (from Project) field displays the Planned Completion Date of the linked projects.  

        >[!IMPORTANT]
        >
        >    Everyone with View or higher permissions to the workspace can view the information in the linked fields, regardless of their permissions or access level in the application of the linked object types.

* Linked record fields are preceded by a relationship icon ![](assets/relationship-field-icon.png). 
    
    Linked fields are preceded by an icon that identifies the field type. For example, icons that indicate that a field is a number, a paragraph, or a date. 

## Connect record types

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-maestro}}

   The last-accessed workspace should open by default. 

1. (Optional) Expand the downward-pointing arrow to the right of an existing workspace name and select the workspace that you want to connect record types from.
1. Click the card of a record type to open the record type page. 
1. Click the **+** icon in the upper-right corner of the table view, then click the **New connection** tab.

    ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. In the **Record type** field, search for a record type, or select one of the following: 

    * Another record type from the section of the workspace you selected

        >[!TIP]
        >
        >Only record types from the workspace you selected are available to connect to. 
        > 
        >If you don't have other record types in the selected workspace, the workspace section does not display. 

    * A **Project, Portfolio, Program, Company**, or **Group** from the **Workfront Object Types** section.
    * **Experience Manager Assets** from the **Adobe Applications** section. 

    ![](assets/new-connection-tab-fields-with-another-record-selected.png)


1. Update the following information: 

    * **Name**: The name of connected field, as it will appear in the table view or the record page of the original record type. This creates the linked record column in the table view of the original record type or the linked record field for the original records. 

    >[!TIP]
    >
    >We recommend that you include the name of the record you are linking to in the name of the connected record field to capture what record type the new field is coming from. The name of the linked record is not visible in the new linked record field or its linked fields. 

     * **Description**: Additional information about the connected record field. The description of a field displays when you hover over the field's column in a table. 
     * **Allow multiple records**: Select this option to indicate that you allow that users can add multiple records when the linked record type field displays on the original records. This is selected by default.
     * **Select lookup fields**: Select this option to add fields from the selected record type. The lookup fields are fields associated with the record or object type that you are linking to. Linking them displays information from the record or object you're linking to on the record you are liking from. This is selected by default. 

1. (Conditional and optional) If you selected to connect a Workfront object, select a **Custom form** from the **Link only objects that match these criteria** section. Only objects that have the selected custom forms attached can be linked to the selected record type. You can select more than one form. 

    ![](assets/workfront-project-connection-selection.png)

    >[!NOTE]
    >
    > You must create custom forms in Workfront for the selected objects before they display in this list.

1. (Conditional) If you selected to connect to Experience Manager Assets, select a repository from the **Experience Manager repository** drop-down menu in the **Link assets from the following repository** section. This is a required field. Only repositories you have access to in Experience Manager Assets display in this field. 

    <!--replace the screen shot below when they fix the permissions info icon bug-->
    
    ![](assets/aem-assets-connection-selection.png)

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
    
    
1. (Optional) Click **Skip** and don't add any fields from the linked record or object. The **Name** of the linked record is the only visible field in the original record's table view. 

1. (Optional and conditional) If you select to link a number, currency, percentage, or date-type field, also select an aggregator value. The values for the linked fields display either separated by commas or as a aggregated value according to the aggregator you choose, when users select more than one linked record in the linked record field. 

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

    >[!NOTE]
    >
    >For example, you can link the Product record (linked record) from the Campaign record (original record) and name it "Product field". You can also choose to link the Budget field of the Product record from the Campaign record and call it "Product Budget". If you allowed to select multiple records in the "Product field", you can select Product 1 with a Budget of $120,000 and Product 2 with a Budget of $100,000. You can view the following Budget information in the linked field from the original record, depending on which aggregator you choose: 
    >
    >* **None**: $120,000, $100,000
    >* **MAX**: $120,000
    >* **MIN**: $100,000
    >* **SUM**: $220,000
    >* **AVG**: $110,000  
    >

1. (Optional) Use the **search** icon ![](assets/search-icon.png) to search for a field.

1. Click **Add fields** to save your changes.

    The following items are added: 

    * A linked record field on the record type you are linking from. The linked record field will display individual records from the linked record type, after you manually add them. For information about adding records, see [Connect records](/help/quicksilver/planning/records/connect-records.md). The name of the linked record field is the name you selected in step 6. <!--accurate--> 
    
    * A linked field (or fields) that display information from the fields of the linked record or object types after you manually add the records or objects in the linked record field. The linked fields are created only when the **Select lookup fields** setting is selected when creating the connection. The linked fields are automatically named according to this pattern: 

        `<Name of the original field on the linked record> (from <Name of your linked field>)`

        For example, if you linked a Campaign record type with a Program record type and name the Program linked record field "Program information", then select to also display the Program's Budget field in the Campaign's table view, the linked field is automatically named `Budget (from Program information)` in the campaign's table view. 

    * When you link record types to one another, a linked record field is also added on the record type you are linking to. The name of the linked record field on the linked record type is the name of the record type that you link from. 
    
        For example, if you link the "Product" record type from the "Campaign" record type and you name the connected field of the Campaign "Linked Product", a "Campaign" linked record field is created for the Product record type. 

        >[!TIP]
        >
        > A linked record field  is not created for objects from another application to the record type you are linking from in Workfront Planning.

1. (Optional and conditional) From either the original record type or the linked record type table view, click the downward-pointing arrow in the header of the linked record fields, then click one of the following:

    * **Edit field**: You can only update the **Name** and the **Description** information of the field. 
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
