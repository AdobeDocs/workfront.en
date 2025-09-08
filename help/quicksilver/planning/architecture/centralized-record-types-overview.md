---
title: Centralized Record Types Overview
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

# Centralized record types overview

Centralized record types can be added to multiple workspaces from a central or primary workspace in Adobe Workfront Planning. 

## Overview of centralized record types

When implementing Workfront Planning for a multi-team organization with common workflows, you might need to define a cohesive structure and metadata for key record types (like Campaigns or Deliverables) that can be added to each team's workspaces to capture and manage their work. 

Also, you might need each team's work to roll up to a central level. 

In such a workflow, you can ensure that teams capture their work consistently while unlocking cross-team visibility, without the need to add everything to one workspace, or everyone in the organization to every workspace. You can use centralized record types to achieve this. 

To use centralized record types, do the following: 

1. Configure a record type to be centralized in a specific workspace. 

    A workspace manager can select users with a Standard license, teams, groups, roles, or companies to add a chosen record type to a workspaces they manage.

    The original record type will exist in its original workspace but will be made visible from all other workspaces. 

    For information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md). 
1. Add an existing record type from an existing one that has been configured as a centralized one to a team's workspace. 

    The record type will exist in the following workspaces: 

    * Its original workspace where it was designated as a centralized record type.
    * The team's workspace. 

    For information, see [Add existing record types](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).

    The following sections describe considerations about centralized record types in either their original workspaces or after they are added to a team's workspaces.     

## Considerations about the centralized record types in their original workspace

The record type configured to be centralized has the following properties:

* All its information can only be edited in the original workspace. 

* You can perform the following actions on the centralized record type from a centralized record type's original workspace:

    * Edit it 
        
        Editing a centralized record type includes editing its appearance, cross-workspace capabilities, and all the fields created in the original workspace.
    * Create request forms
    * Manage request forms

* You can only delete a centralized record type only if  it has not been added to a team workspace. After it is added to a team's workspace, trying to delete it from the original workspace will generate an error.

    This is done so that the centralized record type can remain in the workspaces where it's already been added. 
* The records that you add to a centralized record type are visible only to users who have View permissions to its original workspace. 
* The records that you add from the team's workspace roll up and display in the original workspace. All members of the original workspace gain View permissions to it.

* The connected record types of a centralized record type will become available for connection from the workspaces where this record type is added. 

* Fields created for a centralized record type from the original workspace are visible from all workspaces where the record type is added. 

## Considerations about centralized record types after adding them to a team's workspace

* Team workspace contributors gain Contribute permission to the centralized record type in the team workspace. They can add and manage records in it.

* Team workspace viewers gain View permission to the centralized record type in the team workspace. They cannot add and manage records it in. 

* Team workspace managers can perform the following actions on the record type added from a centralized record type in a team's workspace:

    * Add new fields

        Fields added to a centralized record from a team workspace are visible only from the team's workspace. 
    * Share it
    * Delete it. 

        Deleting the record type from a team's workspace only removes it from the team's workspace. The records added to it from the team's workspace are also deleted. This does not delete the record type from its original workspace or from any other team workspaces where it has been added. 
        
        This is done so that it's possible to keep the already added centralized record type in workspaces that are already using it.

* You cannot perform the following actions on the record type added from a centralized record type in a team's workspace:

    * Edit it

        You cannot edit its appearance, cross-workspace capabilities, or the fields imported from the original workspace.
    * Create request forms
    * Manage request forms

* Records added in a team's workspaces are visible from the following workspaces, if you have View or higher permissions to these workspaces: 

    * The team's workspace where they are added. 
    * The centralized record type's original workspace.
    * All other workspaces where the centralized workspace is added.

* The following scenarios exist for records created in teams' workspaces: 

    * If you have Manage permissions on the original workspace, and no permissions on the teams' workspaces, you can view records added from the team's workspaces in the original workspace, but you cannot manage them from the original workspace. 
    * If you have Manage permissions on the team's workspace, you can manage the records in the centralized record type's original workspace or from the workspace where they were added. 
    
        You can view the records in additional team workspaces where the centralized record type is added only if you have View permissions to those workspaces. 

## Access to connections

Record types connected to the centralized record type in the original workspace become visible for team workspaces where the centralized record type is added. 

## API behavior

When adding records to a centralized record type from a team workspace using the Workfront Planning API, the system checks if the user has access to create records in the original workspace of the centralized record type. 

The following cases exist: 

* If the user has access, the record is created in the centralized record types's original workspace. 

* If the user doesn't have access, the user gets an error that they don't have access to the centralized record type's original workspace and they need to provide the workspace ID where they have access to create records.