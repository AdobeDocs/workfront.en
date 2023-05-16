---
title: Create fields for Maestro records
description: You must create record types before you can create fields to associate with them.
hidefromtoc: yes
hide: yes
---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!--Should the structure of this article be like this one: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-forms/custom-form-builder/use-the-custom-form-builder/add-a-custom-field-to-a-custom-form.html?lang=en ??-->

<!--will this cover adding fields in a table?! or just custom fields?! -->

# Create fields for Maestro records

In Adobe Maestro, you can create custom fields for each kind of operational record type or taxonomy. 

You must create record types before you can create fields to associate with them. For information, see [Create operational record types](../maestro/create-operational-record-types.md). 

## Access requirements

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any</p>
<!--the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Any</p> 
  <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Product</p></td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see the "Enable Maestro for the users in your Workfront instance" section in the article <a href="../maestro/maestro-overview.md">Adobe Maestro overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>*If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).


## Considerations about Maestro fields

* The fields associated with a record type are available to be associated with all the records of that type. 

* Maestro creates a set of fields by default every time you create a record type. The following are standard fields created by default for each new record type:

    * Name
    * Description
    * Start Date
    * End Date
    * Status. The default values for record statuses are:
        * Development
        * Planned
        * Active
        * Completed
        * On Hold

    You can add more values or rename the existing ones. 

* You can view and update all the fields that any other user added to any record type. <!--this will change with access/ permissions-->
* You can create custom fields or automatically add them by doing one of the following:
    * Linking to another record type and accessing their fields
    * Importing record types from other applications and accessing their fields
    <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->
* You cannot have more than 500 fields for one record type.
* Field names can have up to 250 characters.
* Fields associated with a record type cannot be added to another record type. <!-- this will change when they open the Field library tab when creating a field-->
* You can create fields on the record type page, in the Table view. The columns of the table are record fields. They are the same fields that display on a record's Details page. 
* When deleting a record type, taxonomy, or workspace, all fields associated with them are also deleted and cannot be recovered. 


## Create fields from scratch (#create-fields-from-scratch) <!--in a table (not sure if this can be done elsewhere?!-->

1. Click the **Main Menu** icon ![](assets/main-menu-workfront.png) in the upper-right corner of Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> then click **Maestro** ![](assets/maestro-icon.png).

    The last-accessed workspace should open by default. 

1. (Optional) Expand the downward-pointing arrow to the right of an existing workspace name and select the workspace that you want to create records for.
1. Click the record type you want to create fields for. 

    All records associated with the record type display in the table view, by default. 
1. Click the **+** icon to the upper-right corner of the table view to add new fields.
1. In the **New field** tab, select from the following field types: 

    * [Number](#number) 
    * [Percentage](#percentage)
    * [Currency](#currency)
    * [Single-line text](#single-line-text)
    * [Paragraph](#paragraph)
    * [Single-select](#single-select)
    * [Multi-select](#multi-select) 
    * [Date](#date)
    * [Relationship](#relationship)
1. Continue with adding each field, as described in the sections below. 

### Number {#number}

You can use number fields to capture information in a number format. 

1. Start creating a field as described in the section [Create fields from scratch](#create-fields-from-scratch) in this article, then select the **Number** field type.

    ![](assets/number-field-type.png)
1. Add the following information:

    * **Name**: The name of the field type, as it will appear in a table or the Details page of the record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
    * **Description**: Additional information about the field.
    * **Precision**: The number of decimals that you want to record for the field. You can display up to 6 decimals.
    * **Allow negative numbers**: Select this option if you want to allow negative numbers in this field. This option is deselected by default.
1. Click **Create**.

    The new number field is added as a column to the record type and its values can be associated with records. The field also displays on the Details page of a record.  

### Percentage {#percentage}

You can use number fields to capture information in a percentage format. 

1. Start creating a field as described in the section [Create fields from scratch](#create-fields-from-scratch) in this article, then select the **Percentage** field type.

    ![](assets/percentage-field-type.png)

1. Add the following information:
     * **Name**: The name of the field type, as it will appear in a table or the Details page of the record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
     * **Description**: Additional information about the field.
    * **Precision**: The number of decimals that you want to record for the field. You can display up to 6 decimals.
    * **Allow negative numbers**: Select this option if you want to allow negative percentage values in this field. This option is deselected by default.
1. Click **Create**. 

    The new percentage field is added as a column to the record type and its values can be associated with records. The field also displays on the Details page of a record. 

### Currency {#currency}

You can use number fields to capture information in a currency format. 

1. Start creating a field as described in the section [Create fields from scratch](#create-fields-from-scratch) in this article, then select the **Currency** field type.

    ![](assets/currency-field-type.png)

1. Add the following information:
     * **Name**: The name of the field type, as it will appear in a table or the Details page of the record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
     * **Description**: Additional information about the field.
     * **Currency**: The type of currency you want to display in this field.
      * **Precision**: The number of decimals that you want to record for the field. You can display up to 6 decimals.
    * **Allow negative numbers**: Select this option if you want to allow negative currency values in this field. This option is deselected by default.
1. Click **Create**. 

    The new currency field is added as a column to the record type and its values can be associated with records. The field also displays on the Details page of a record. 

### Single-line text {#single-line-text}

You can use the single-line text field to capture limited alphanumeric information like Owner, Stakeholder, Team, or Organizational unit.

1. Start creating a field as described in the section [Create fields from scratch](#create-fields-from-scratch) in this article, then select the **Single-line text** field type.

    ![](assets/single-line-text-field-type.png) 

1. Add the following information:
     * **Name**: The name of the field type, as it will appear in a table or the Details page of the record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
     * **Description**: Additional information about the field.
1. Click **Create**. 

    The new single-line field is added as a column to the record type and its values can be associated with records. The field also displays on the Details page of a record. 

### Paragraph {#paragraph}

You can use a paragraph field to capture additional lenghty alphanumeric information, similar to the Description field. 

1. Start creating a field as described in the section [Create fields from scratch](#create-fields-from-scratch) in this article, then select the **Paragraph** field type.

    ![](assets/paragraph-field-type.png)
 

1. Add the following information:
     * **Name**: The name of the field type, as it will appear in a table or the Details page of the record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
     * **Description**: Additional information about the field.
1. Click **Create**. 

    The new paragraph field is added as a column to the record type and its values can be associated with records. The field also displays on the Details page of a record. 

### Single-select {#single-select}

You can use a single-select field to capture additional information in any format by selecting one option from a drop-down menu. 

1. Start creating a field as described in the section [Create fields from scratch](#create-fields-from-scratch) in this article, then select the **Single-select** field type.

    ![](assets/single-select-field-type.png)
 

1. Add the following information:
     * **Name**: The name of the field type, as it will appear in a table or the Details page of the record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
     * **Description**: Additional information about the field.
     * **Choices**: The options  available to select from the drop-down menu after the field is saved. You can have both numbers and letters for the name of each choice. Manually drag and drop each choice in the desired order, or select the **Sort choices A-Z** option if you want the choices to be automatically listed in alphabetical order.
1. Click **Add choice** to add as many choices or options as needed.      
1. Click the **x** icon to the right of a choice to remove it.
1. Click the color swatch to the left of a choice to expand the color selector and customize the color of each option. 
1. Click **Create**. 

### Multi-select {#multi-select}

You can use a multi-select field to capture additional information in any format by selecting more than option from a drop-down menu. 

1. Start creating a field as described in the section [Create fields from scratch](#create-fields-from-scratch) in this article, then select the **Multi-select** field type.

    ![](assets/multi-select-field-type.png)
 

1. Add the following information:
     * **Name**: The name of the field type, as it will appear in a table or the Details page of the record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
     * **Description**: Additional information about the field.
     * **Choices**: The options  available to select from the drop-down menu after the field is saved. You can have both numbers and letters for the name of each choice. Manually drag and drop each choice in the desired order, or select the **Sort choices A-Z** option if you want the choices to be automatically listed in alphabetical order.
1. Click **Add choice** to add as many choices or options as needed.      
1. Click the **x** icon to the right of a choice to remove it.
1. Click the color swatch to the left of a choice to expand the color selector and customize the color of each option. 
1. Click **Create**. 


### Date {#date}

You can use a date field to capture additional information in date and time format. 

1. Start creating a field as described in the section [Create fields from scratch](#create-fields-from-scratch) in this article, then select the **Date** field type.

    ![](assets/date-field-type.png)
 

1. Add the following information:
     * **Name**: The name of the field type, as it will appear in a table or the Details page of the record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
     * **Description**: Additional information about the field.
     * **Date format**: The type of date format you want to display in this field.
        
        Select from the following formats:
        * **Locale**: Matches the locale of your browser.
        * **Standard**: 05/16/2023
        * **Friendly**: May 16, 2023
        * **European**: 16/05/2023
        * **ISO**: 2023-05-16
    * Include a time field: Select this option if you want to inclue a time stamp. Select from the following options:
        * **24hr**: 18:00
        * **12hr**: 6:00 PM

        This is deselected by default.

### Relationship {#relationship}

You can use a relationship field to link record types to one another. By doing this, you can display fields from the linked record on another record. 

1. Start creating a field as described in the section [Create fields from scratch](#create-fields-from-scratch) in this article, then select the **Relationship** field type.

    ![](assets/relationship-field-type.png)

1. Add the following information:
     * **Name**: The name of the field type, as it will appear in a table or the Details page of the record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->

    >[!TIP]
    >
    >We recommend that you include the name of the record you are linking to in this name, if you need to have an indication what record the new field is coming from. 

     * **Description**: Additional information about the field.
     * **Find a record type**: The field you want to link to. 
     * **Allow multiple records**: <!--asking Lusine and Lilit in common slack what this field should show/ do--> This is selected by default. 

1. (Optional) Select the fields you want to display as linked fields from the list of the linked record. Use the **search** icon ![](assets/search-icon.png) to search for a field. If you don't select any of the fields, the name of the linked record is the only visible field in the table and the Details page of the record.

1. Click **Create**.

    The following fields (or columns) are added to the records in the table view:
        
    * The linked record field with the name you selected in step 2. <!--ensure this stays accurate--> For example, if you linked to a record type called "Audience" and its field called "Background", you might name the linked field "Audience Background."
    * The field from the linked record which is named according to this pattern: 

        `The name of the original field on the linked record (from The name of your linked field)`

        In our example, the second field is named "Background (from Audience Background)


## Create fields by linking record types

## Create fields by importing record types from other applications
