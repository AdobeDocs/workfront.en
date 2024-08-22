---
title: Field overview
description: You can add new fields in Adobe Workfront Planning that reflect your organization's lifecycle. Fields are attributes of record types.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
---
# Field overview

<!--
title: Field overview
description: You can add new fields in Adobe Workfront Planning that reflect your organization's lifecycle. Fields are attributes of record types. 
hidefromtoc: yes
author: Alina
feature: Work Management (***************WE NEED A NEW ONE HERE***********)
role: User, Admin
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

You can add new fields in Adobe Workfront Planning that reflect your organization's lifecycle. Fields are attributes of record types. 


## Considerations about Adobe Workfront Planning fields

* You can create fields only from the table view of a record type page. Fields display as columns in the table view. All fields associated with a record type also display in the record page. 

    For information about managing table columns (or record fields), see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).

    For information about managing fields, also see the following articles: 

    * [Edit field settings](/help/quicksilver/planning/fields/edit-fields.md)
    * [Delete fields](/help/quicksilver/planning/fields/delete-fields.md)
    
* The fields associated with a record type are available to be associated with all the records of that type. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Fields associated with a record type cannot be added to another record type. <!-- this will change when they open the Field library tab when creating a field-->

* You can create fields manually or automatically in the following ways:

    * Manually:

        * By adding columns in the table view of a record type page. The columns of the table are the fields associated with the record type. They are the same fields that display on a record's page. 
        
            You cannot create fields from the record's page.  

        * By connecting record types. You can create linked record fields when you add a new connection between two record types, or a record type and an object types from other applications. 
        
           <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

           For more information about connecting record types, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).  

        <!--* By importing record types using an Excel or CSV file. For more information, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). -->

    * Automatically: 

        The following are standard fields created by default for each new record type:

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

        Workfront Planning creates fields for record types when you create a workspace from a template. For information, see [Create workspaces](/help/quicksilver/planning/architecture/create-workspaces.md). 

* Workfront Planning fields are not accessible from Workfront. 

* Workfront fields are accessible from Workfront Planning only when you connect record types with Workfront object types and add linked or lookup fields from Workfront objects. For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).  

* You can view and update the settings for the fields that you or any other user created, if you have Manage permissions to the workspace that the field belongs to. 

* You can have up to 500 fields for one record type.

* Field names can have up to 250 characters.

* When deleting a record type or workspace, all fields associated with them and the fields' values are also deleted and cannot be recovered. <!-- this might change with a possible recycle bin solution?!-->
