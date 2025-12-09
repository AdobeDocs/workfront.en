---
title: Hierarchy and Breadcrumb Overview
description: You can create multiple workspace hierarchies between the record types in a workspace.
hide: yes
hidefromtoc: yes
---
<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Hierarchy and Breadcrumb Overview
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---
-->

# Hierarchy and breadcrumb overview

As a workspace manager, you can define flexible but structured hierarchies between record types and and other object types in Adobe Workfront Planning. 

Hierarchies are connections between record types. You can have up to 4 record and object types connected in one hierarchy. 

For information about creating hierarchies, see [Create workspace hierarchies](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md). 

The following are benefits of using hierarchies in your workspaces: 

* To organize work in a way that reflects how your teams actually plan, operate, and deliver. 
* For users to understand where they are, how record types connect, and how strategy flows into execution by referring to a set of breadcrumbs that indicate their place in the system. 
* To offer a better navigation, and create clarity and continuity across all workflows. 
* To define flows that fit how your organization works, supporting both flexibility and consistency across all stages of work.

## Considerations when working with hierarchies

* As a workspace manager, you can create multiple hierarchies for one workspace.
* If a connection between the selected record types already exists, the system reuses the existing connection.
* If no connection exists, Workfront will automatically create one as part of the hierarchy setup.
* The following are rules for hierarchy setup:
    * A record type can only have one parent record type in a given workspace. 
    
        For example, a Tactic record type cannot have both a Campaign and a Goal record type as a parent in the same workspace. 
    * A record can be connected to multiple parent records of the same type, when you connect one to many or many to many record types.
        For example, Tactic A can belong to both Campaign X and Campaign Y. 
    * A record type can connect to multiple children  record types. 
        
        For example, a Campaign record type can be the parent to multiple other record types, like Tactics, Tests, and other record types.
    * Hierarchies can include both Planning record types and Workfront object types.

        For example, you can have a Campaign record type with Planning Tactics and Workfront Projects as the children. 

        <!--asking if ONLY projects are supported here in slack; if yes, make a note to say that only Projects are supported; also add a note about AEM -->
    * Global record types may appear in multiple workspaces inside multiple hierarchies. <!--not sure if this AFTER they were added to another workspace; right now, I can see only the current workspace when building one??-->
    * Workfront object types can also appear in multiple hierarchies and across different workspaces.
    * Global record types cannot be part of hierarchies in different workspace. 

        For example, if a Campaign is a global record type and part of a hierarchy in Workspace 1, it can be added as an existing record type to Workspace 2 but cannot be part of a hierarchy there. <!--verifying that this is not connectable RT and it is about global ones - checking in slack-->
    * The record types with connections that do not create a corresponding field on their linked record types can also be part of hierarchies. New connections that are created during hierarch setup will always create a corresponding field on the linked record types, by default.

## Considerations when viewing breadcrumbs

When you create hierarchies between record types, they generate breadcrumbs for records that belong to those record types. 

For example, if you create a hierarchy and connect Campaigns with Tactics with Programs and then Projects, when you navigate to a record of any of the types connected in the hierarchy, you can view where in the hierarchy the record is placed. 

Consider the following: 

* If a record type is part of multiple hierarchies in multiple workspaces, you can switch between hierarchies from the record's breadcrumb on the record's page.
* Breadcrumbs work across Workfront and Planning. 

    For example, when looking at a project which is connected to Planning campaigns and tactics, and also to Workfront portfolios and programs, you can switch between both the Planning and the Workfront hierarchies from the breadcrumb. 

    For more information, see [Create workspace hierarchies](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).


