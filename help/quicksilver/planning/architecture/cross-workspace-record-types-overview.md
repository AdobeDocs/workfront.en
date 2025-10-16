---
title: Cross-workspace Record Type Overview
description: Global record types can be added to multiple workspaces from a central or primary workspace in Adobe Workfront Planning.
hidefromtoc: yes
hide: yes
exl-id: aeedd871-dcd3-4fb3-bfc5-99db3e7c9296
---
<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Cross-workspace record type overview

{{planning-important-intro}}

You can enable cross-workspace capabilities for a record type in Adobe Workfront Planning. A cross-workspace record type can be referenced or accessible from more than one workspace. 

>[!IMPORTANT]
>
>There are enhanced Workfront package requirements to be able to enable cross-workspace capabilities for record types in your system. For information, see [Adobe Workfront Planning access overview](/help/quicksilver/planning/access/access-overview.md). 


The following are cross-workspace capabilities of record types:

* **Global record types**: Users can add global record types to other workspaces they manage.

* **Connectable record types**: Users can connect to this record type from other workspaces. 

This article gives you an overview of cross-workspace record types. For information about defining a record type's cross-workspace capabilities, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md). 

## Overview of global record types

Global record types can be added to multiple workspaces from a central or primary workspace in Workfront Planning. 

When implementing Workfront Planning for a multi-team organization with common workflows, you might need to define a cohesive structure and metadata for key record types (like Campaigns or Deliverables) that can be added to each team's workspaces to capture and manage their work. 

Also, you might need each team's work to roll up to a central level. 

In such a workflow, you can ensure that teams capture their work consistently while unlocking cross-team visibility, without the need to add everything to one workspace, or everyone in the organization to every workspace. You can use global record types to achieve this. 

To use global record types, do the following: 

1. From a workspace you manage, configure a record type to be global. 

    A workspace manager can give permissions to users with a Standard license, or teams, groups, roles, and companies to add a chosen record type to a workspaces they manage.

    The original record type will exist in its original workspace but will be made visible in other workspaces. 

    For information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md). 
1. Add a record type to a secondary workspace from an existing one that has been configured as a global record type.

    The record type will exist in the following workspaces: 

    * Its original workspace where it was designated as a global record type.
    * A secondary workspace. 

    For information, see [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

    The following sections describe considerations about global record types and how they function in either their original or secondary workspaces. 

### Considerations about the global record types in their original workspace

The record type configured to be global has the following properties:

* All its information (appearance, original fields) can only be edited in the original workspace. 

* You can perform the following actions on the global record type from its original workspace:

    * Edit it 
        
        Editing a global record type includes editing its appearance, cross-workspace capabilities, and all the fields created in the original workspace.
    * Create and manage request forms
    * Create and manage automations

* You can delete a global record type only if it has not been added to a secondary workspace. You must first remove it (by deleting it) from the secondary workspaces before you can delete it from the original workspace.

    For more information, see [Delete record types](/help/quicksilver/planning/architecture/delete-record-types.md).
* The records that you add to a global record type are visible only to users who have View permissions to the workspace where they were added. 
* The records that you add from a secondary workspace roll up and display in the original workspace. All members of the original workspace gain View permissions to them.
* When the original global record type is added to multiple secondary workspaces the following scenarios exist: 

    * Members of the original workspace automatically gain View permissions to all records added from any workspace, even if they are  not members of those workspaces.
    * Secondary workspace members can view only records from workspaces where they are a member. 
* The connected record types of a global record type will become available for connection from the workspaces where this record type is added. 

    For example, if you have a Campaign global record type that has a connection with a Regions record type, and you add the Campaign record type to a secondary workspace, Regions will become cross-workspace connectable from the secondary workspace. The secondary workspace members can now create campaigns and link them to regions.

* Fields created for a global record type from the original workspace are visible from all workspaces where the record type is added. You can edit field settings only from the original workspace. The settings of the fields created in the original workspace are read-only in the secondary workspaces for all members, regardless of their permissions on the secondary workspace. Secondary workspace managers cannot modify the field settings for fields configured in the original workspace. Only yhe workspace managers of the original workspace can modify field settings in the original workspace.  

### Considerations about global record types in a secondary workspace

* Secondary workspace contributors gain Contribute permission to the global record type in their team's workspace. They can add and manage records in it from the secondary workspace.

* Secondary workspace viewers gain View permission to the global record type in their team's workspace. They cannot add and manage records in it.  

* Secondary workspace managers can perform the following additional actions on the record type added from a global record type in a secondary workspace:

    * Delete it. 

        Deleting the record type from a secondary workspace only removes it from the secondary workspace. The records and fields added to it from the secondary workspace are also deleted. This does not delete the record type from its original workspace or from any other secondary workspaces where it has been added. 

        For more information, see [Delete record types](/help/quicksilver/planning/architecture/delete-record-types.md).
        
    <!--These two capabilities will come later - and edit some of the bullets below after these capabilities are released:
    * Add new fields
        Fields added to a global record from a secondary workspace are visible only from the secondary workspace. 
    * Share it
    * Add request forms to it
    * Add automations to it-->

* No user can perform the following actions on the record type added from a global record type in a secondary workspace:

    * Edit it

        You cannot edit its appearance, cross-workspace capabilities, or the fields added from the original workspace. 
    * Create and manage request forms
    * Create and manage automations

* Records added in a secondary workspace are visible from the following workspaces, only if you have View or higher permissions to these workspaces: 

    * The secondary workspace where they are added. 
    * The global record type's original workspace.
    * All other workspaces where the global workspace is added.

* The following scenarios exist for records created in secondary workspaces: 

    * If you have Manage permissions on the original workspace, and no permissions on a secondary workspaces, you can view records added from the secondary workspaces in the original workspace, but you cannot manage them from the original workspace. 
    * If you have Manage permissions on the secondary workspace, you can manage the records from both the global record type's original workspace and from the secondary workspace where they were added. 
    * You can view the records in additional secondary workspaces where the global record type is added only if you have View permissions to those workspaces. 

### Access to the connections of a global record type

Record types connected to the global record type in the original workspace become visible from other workspaces where the global record type is added and they are available for connections from the secondary workspaces where the global record type is added. 

### API access of a global record type

When adding records to a global record type from a secondary workspace using the Workfront Planning API, the system checks if the user has access to create records in the original workspace of the global record type. 

The following cases exist: 

* If the user has access, the record is created in the global record types's original workspace. 

* If the user doesn't have access, the user gets an error that they don't have access to the global record type's original workspace and they need to provide the workspace ID where they have access to create records.

## Overview of connectable record types

You can connect to a record type that has been defined as connectable from any workspace that you manage.  

Your teams might need their records linked to record types from other workspaces or view information captured on records that belong to records in other workspaces. You can achieve this configuration by designating a record type as connectable.  

To use connectable record types, do the following: 

1. Configure a record type to be connectable in a specific workspace. 

    A workspace manager can select what workspaces a designated record type is available to connect to. 

    The original record type will exist in its original workspace and it can be accessible to connect to from another workspace. 

    For information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md). 
1. Connect to a record type designated as connectable from another workspace you manage. 

    For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).
