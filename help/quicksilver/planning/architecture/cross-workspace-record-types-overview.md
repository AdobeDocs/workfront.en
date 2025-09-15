---
title: Cross-workspace Record Types Overview
description: Centralized record types can be added to multiple workspaces from a central or primary workspace in Adobe Workfront Planning. 
hidefromtoc: yes
hide: yes
---
<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Cross-workspace record types overview

In Adobe Workfront Planning, you can enable cross-workspace capabilities for a record type that allows you to reference a record type in more than one workspace. 

The following are cross-workspace capabilities of record types:

* You can designate a record type as centralized. Users can add centralized record types to other workspaces they can manage. 

    >[!IMPORTANT]
    >
    >You must have a Workfront Planning Plus package, in addition to a Workfront package to use centralized record types.
    >
    >For more information about what is included in each Workfront Planning package, contact your Workfront account manager.

* You can designate a record type as connectable. Users can connect to this record type from other workspaces. 

This article gives you an overview of cross-workspace record types. For information about defining a record type's cross-workspace capabilities, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md). 


## Overview of centralized record types

Centralized record types can be added to multiple workspaces from a central or primary workspace in Adobe Workfront Planning. 

When implementing Workfront Planning for a multi-team organization with common workflows, you might need to define a cohesive structure and metadata for key record types (like Campaigns or Deliverables) that can be added to each team's workspaces to capture and manage their work. 

Also, you might need each team's work to roll up to a central level. 

In such a workflow, you can ensure that teams capture their work consistently while unlocking cross-team visibility, without the need to add everything to one workspace, or everyone in the organization to every workspace. You can use centralized record types to achieve this. 

To use centralized record types, do the following: 

1. Configure a record type to be centralized in a specific workspace. 

    A workspace manager can select users with a Standard license, teams, groups, roles, or companies to add a chosen record type to a workspaces they manage.

    The original record type will exist in its original workspace but will be made visible from all other workspaces. 

    For information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md). 
1. Add a record type from an existing one that has been configured as a centralized record type to a secondary workspace. 

    The record type will exist in the following workspaces: 

    * Its original workspace where it was designated as a centralized record type.
    * A secondary workspace. 

    For information, see [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

    The following sections describe considerations about centralized record types and how they function in either their original or secondary workspaces. 

### Considerations about the centralized record types in their original workspace

The record type configured to be centralized has the following properties:

* All its information can only be edited in the original workspace. 

* You can perform the following actions on the centralized record type from a centralized record type's original workspace:

    * Edit it 
        
        Editing a centralized record type includes editing its appearance, cross-workspace capabilities, and all the fields created in the original workspace.
    * Create request forms
    * Manage request forms

* You can only delete a centralized record type only if it has not been added to a secondary workspace. After it is added to another workspace, trying to delete it from the original workspace will generate an error.

    This is done so that the centralized record type can remain in the workspaces where it's already been added. 
* The records that you add to a centralized record type are visible only to users who have View permissions to the workspace where they were added. 
* The records that you add from a secondary workspace roll up and display in the original workspace. All members of the original workspace gain View permissions to it.

* The connected record types of a centralized record type will become available for connection from the workspaces where this record type is added. 

    For example, if you have a Campaign record type that has a connection with Regions record type, and you add the Campaign record type to a secondary workspace, Regions will become cross-workspace connectable for the secondary workspace. The secondary workspace members can now create campaigns and link them to regions.

* Fields created for a centralized record type from the original workspace are visible from all workspaces where the record type is added. Fields from an original workspace are read-only in the secondary workspaces. 

### Considerations about centralized record types after adding them to a secondary workspace

* Secondary workspace contributors gain Contribute permission to the centralized record type in their team's workspace. They can add and manage records in it.

* Secondary workspace viewers gain View permission to the centralized record type in their team's workspace. They cannot add and manage records it in. 

* Secondary workspace managers can perform the following actions on the record type added from a centralized record type in a secondary workspace:

    * Delete it. 

        Deleting the record type from a secondary workspace only removes it from the secondary workspace. The records added to it from the secondary workspace are also deleted. This does not delete the record type from its original workspace or from any other secondary workspaces where it has been added. 
        
    <!--These two capabilities will come later:
    * Add new fields
        Fields added to a centralized record from a secondary workspace are visible only from the secondary workspace. 
    * Share it-->

* You cannot perform the following actions on the record type added from a centralized record type in a secondary workspace:

    * Edit it

        You cannot edit its appearance, cross-workspace capabilities, or the fields added from the original workspace.
    * Create and manage request forms
    * Crate and manage request forms

* Records added in a secondary workspaces are visible from the following workspaces, if you have View or higher permissions to these workspaces: 

    * The secondary workspace where they are added. 
    * The centralized record type's original workspace.
    * All other workspaces where the centralized workspace is added.

* The following scenarios exist for records created in teams' workspaces: 

    * If you have Manage permissions on the original workspace, and no permissions on a secondary workspaces, you can view records added from the secondary workspaces in the original workspace, but you cannot manage them from the original workspace. 
    * If you have Manage permissions on the secondary workspace, you can manage the records in the centralized record type's original workspace or from the workspace where they were added. 
    
        You can view the records in additional secondary workspaces where the centralized record type is added only if you have View permissions to those workspaces. 

### Access to the connections of a centralized record type

Record types connected to the centralized record type in the original workspace become visible from other workspaces where the centralized record type is added. 

### API access of a centralized record type

When adding records to a centralized record type from a secondary workspace using the Workfront Planning API, the system checks if the user has access to create records in the original workspace of the centralized record type. 

The following cases exist: 

* If the user has access, the record is created in the centralized record types's original workspace. 

* If the user doesn't have access, the user gets an error that they don't have access to the centralized record type's original workspace and they need to provide the workspace ID where they have access to create records.

## Overview of connectable record types

You can connect to a record type that has been defined as connectable from any workspace that you manage.  

Your teams might need their records linked to record types from other workspaces or view information captured on records that belong to records in other workspaces. You can achieve this configuration by designating a record type as connectable.  

To use connectable record types, do the following: 

1. Configure a record type to be connectable in a specific workspace. 

    A workspace manager can select select what workspaces a designated record type is available to connect to. 

    The original record type will exist in its original workspace and it will be added as a connected record type to another workspace. 

    For information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md). 
1. Connect to a record type designated as connectable from another workspace you manage. 

    For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

    The following sections describe considerations about centralized record types and how they function in either their original or secondary workspaces. 