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

When implementing Workfront Planning for a multi-team organization with common workflows, you might need to  define a cohesive structure and metadata for key record types (like Campaigns or Deliverables) that can be added to each team's workspaces to capture and manage their work. 

Also, you might need each team's work to roll up to a central, more global level. 

In this workflow, you can ensure that teams capture their work consistently while unlocking cross-team visibility, without the need to add everyone in the organization to one workspace. 

To use centralized record types, do the following: 

1. Configure a record type to be centralized. 

    For information,, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md). 
1. Add an existing record type from a centralized one. 

    For information, see [Add existing record types](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).




· A new setting "Allow adding the record type in other workspaces" is available in Advanced Settings for record types.

· If enabled, the workspace manager can select users with Standard license, teams, groups, roles, or companies who can add the record type in the workspaces they manage.

· The workspace manager who is editing the setting will be automatically added to the selected users list by default

o The workspace manager can remove his own name after adding at least 1 other entity

o There needs to be at least 1 user/team/... selected to save the setting

o Once the record type is added in at least 1 other workspace, all selected users can be removed

§ This is done so that it's possible to prevent adding the global record type in new workspaces but keep it in workspaces that are already using it.

· In phase 1, all records from the connected record types are automatically shared with any workspace where the record type has been added.

· Once the record type is enabled as cross-workspace, a system-generated "Workspace" field is added to the record type

o It shows the workspace from where each record has been created.

o This field is read-only and cannot be deleted.

o It can be hidden from view fields.

o The workspace field can be used for filtering, grouping, and sorting, as well as in any view settings, like other fields.


Cross-Workspace Record Types in Local Workspaces

· When trying to add a new record type to their workspace, local workspace managers see an option to select from the list of global record types that are available for them

· When they select one of the global record types, it's immediately added to the workspace

· It's possible to move the global record type into any section and position within the local workspace


Permissions to the global record type in local workspaces

Within local workspaces the members gain following access to the global record type:

· In Phase 1, local workspace managers gain Contribute permission. This means:

o Local workspace managers can:

§ Add the global record type

§ Add/edit/delete any records in the global record type, regardless of which workspace the record was added from.

§ Delete the global record type from their local workspace

o Local workspace managers cannot:

§ Add, edit, delete fields

§ Update the record type appearance and label

§ See advanced settings for the record type

§ Manage automations

§ Manage request forms

§ Adjust the record type sharing for their workspace's scope

§ Disable the global record type setting in advanced settings.

· Local workspace contributors gain Contribute permission to the global record type and can add and manage records in it

· Local workspace viewers gain View permission to the global record type

· As soon as a record is added to the global record type from any of the local workspaces, the Workspace field shows that workspace name

o For now it's not possible to edit and change the workspace field

· Records added to local workspaces are all rolled up and displayed in the primary workspace, and all members of the primary workspace gain view access to it.

· Records added in local workspaces are not displayed in other local workspaces using the same global record type and their members don't get access to the records.



Access to Connections:

· MVP scope

o The record types connected to the global record type will become visible for local workspaces where the global record type is added so that they can use the connection fields to tag


API behavior

If the user tries to create records in a global record type via API without providing the workspace ID, the system checks if the user has access to create records in the primary workspace (where global record type is created)

· If yes, the record is created in the primary workspace

· If no, the user gets a validation error that he does not have access to the primary workspace and needs to provide the workspace ID where he has access to create.