---
title: Field overview
description: You can add new fields in Adobe Maestro that reflect your organization's lifecycle. Fields are attributes of record types.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
---
# Field overview

<!--
title: Field overview
description: You can add new fields in Adobe Maestro that reflect your organization's lifecycle. Fields are attributes of record types. 
hidefromtoc: yes
author: Alina
feature: Work Management (***************WE NEED A NEW ONE HERE***********)
role: User, Admin
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

You can add new fields in Adobe Maestro that reflect your organization's lifecycle. Fields are attributes of record types. 


## Considerations about Maestro fields

* You can create fields only from the table view of a record type page. Fields display as columns in the table view. All fields associated with a record type also display in the Details page of each record of that type. 

    For information about managing table columns (or record fields), see [Manage the table view](../views/manage-the-table-view.md).

    For information about managing fields, also see the following articles: 

    * [Edit fields](../fields/edit-fields.md)
    * [Delete fields](../fields/delete-fields.md)
    
* The fields associated with a record type are available to be associated with all the records of that type. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Fields associated with a record type cannot be added to another record type. <!-- this will change when they open the Field library tab when creating a field-->

* You can create fields manually or automatically in the following ways:

    * Manually:

        * By adding columns in the table view of a record type page. The columns of the table are the fields associated with the record type. They are the same fields that display on a record's Details page. 
        
            You cannot create fields from the Details page of a record.
            
            This article describes how to manually create fields. 

        * By connecting record types. You can create linked record fields when you add a new connection between two Maestro record types, or a record type and an object types from other applications. 
        
           <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

           For more information about connecting Maestro record types, see [Connect record types](../architecture/connect-record-types.md).  

        * By importing record types using an Excel or CSV file. For more information, see [Create record types](../architecture/create-record-types.md). 

    * Automatically: 

        * By default every time you create a record type. 

            The following are standard fields created by default for each new operational record type:

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

            The following are the standard fields created by default for each new taxonomy record type:

            * Name <!--will more be added? If not, consider rephrasing this bullet-->

        * When you create a workspace from a template. Maestro creates fields for operational record types and taxonomies when you create a workspace from a template. For information, see [Create workspaces](../architecture/create-workspaces.md). 

* Maestro fields are not accessible from Workfront. 

* Workfront fields are accessible from Maestro only when you connect Maestro record types with Workfront object types and add linked or lookup fields from Workfront objects. For information, see [Connect record types](../architecture/connect-record-types.md).  

* You can view and update the settings for the fields that you or any other user created, if you have Manage permissions to the workspace that the field belongs to. 

* You can have up to 500 fields for one record type.

* Field names can have up to 250 characters.

* When deleting an operational record type, taxonomy, or workspace, all fields associated with them and the fields' values are also deleted and cannot be recovered. <!-- this might change with a possible recycle bin solution?!-->
