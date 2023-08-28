---
title: Example of connecting record types and records
description: This article describes an example of creating a connection between an Adobe Maestro record type and a Workfront project, as well as a connection between a Maestro record and a project. 
hidefromtoc: yes
hide: yes
---

# Example of connecting record types and records

<!---------------------------THIS SECTION MUST BE REDONE WITH THE NEW UI ----------->

This article describes an example of creating a connection between an Adobe Maestro record type and a Workfront project, as well as a connection between a Maestro record and a project.

For example, you have a record type named Campaign as your original record type. 

You also have another record type called Product, which has a currency field called Budget. 

You want to create a field on the record type of Campaign where you can show the values of the Budget field on the record type Product. 

To do this:

1. Open the table view for the Campaign record type. 
1. Click the **+** icon in the upper-right corner of the table view to add a new field, then click **New connection**. 
1. Add the following information, for example:

    * **Name**: Product information. This is the name of the linked record field. 
    * **Description**: This is the Product that I want my Campaigns associated with. 
    *** Linked record type**: Product
    * * **Allow multiple records**: If you leave this option selected, this allows users to select multiple records when the linked record type field (Product information) displays on the original records (Campaigns).
1. From the list of fields associated with the **Product** record type, select the **Budget** field. This creates a field called **Budget (from Product information)**, which is the name of the linked field. 

    >[!TIP]
    >
    >    If you want to view the Budget of all selected products as one total number, select **SUM** in the drop-down menu to the right of the field name. When users select multiple products in the **Product information** linked record field, the **Budget (from Product information)** field adds all their Budget values together and displays the total. <!-- check the shot below - added a bug with a couple of UI changes here-->
    > If you select **None**, instead of **SUM**, the individual budgets will display separated by commas.

    ![](assets/example-of-relationship-field-product-information-budget-with-sum.png)

    This generates the following fields: 
    
    * In the Campaign record table view and in the Details page of a campaign: 

        * **Product information** (the linked record field): This will display the name or names of the Products. 
        * **Budget (from Product information)** (the linked field): This will display the Budgets of the Products selected in the Product information field. 

    * In the Product record table view and in the Details page of a product: 

        * **Campaign**: This indicates that the Product record type is linked from the Campaign record type.

        ![](assets/example-campaign-information-relationship-fields-from-product-record-table.png)

    >[!TIP]
    >
    >    Relationship-type fields are preceded by the relationship icon ![](assets/relationship-field-icon.png). 

1. To populate the **Product information** field, from the **Campaign** record type table view, create a campaign by adding a new row in the table. 
1. Click the **+** icon inside the  **Product information** column of the new campaign. The **Connect objects** box displays. The name of the record type that you are linking to (Product) displays in the upper-left corner of the box.

    ![](assets/connect-objects-box-to-select-other-maestro-records-example-for-product-record.png)

1. Select the Product records you want to connect with the Campaign records, then click **Connect objects**.

    The following columns are populated in the Campaign record type table: 
    * The Product information field populates for the Campaign record with the selected Products. 
    * The Budget (from Product information) field populates with the Budget value for each selected Product. 

    ![](assets/example-product-information-and-budget-relationship-fields-for-campaign-record-table.png)

    >[!TIP]
    >
    >When you do not select an aggregator for the multiple values, all values display separated by commas. 

1. To populate the **Campaign** field from the **Product** table view, repeat steps 5-7 starting from the Product record type table view and selecting campaign information. <!--ensure the step numbers remain correct--> 





    
## Connect record types with Workfront projects