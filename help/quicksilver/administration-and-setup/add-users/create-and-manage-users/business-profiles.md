---
title: Business Profiles Overview
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: add-users-to-workfront
description: Business profiles are an enhanced permission model that allows customers such as agencies to efficiently manage user access and ensure precise control over permissions at the group level. In a business profile, users have distinct permissions to group-specific objects. Additional objects can also be shared directly with the business profile.
author: Becky
feature: System Setup and Administration
role: Admin
---
# Business profiles overview

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for specific customers.</span>

Business profiles are an enhanced permission model that allows customers such as agencies to efficiently manage user access and ensure precise control over permissions at the group level. In a business profile, users have distinct permissions to group-specific objects. Additional objects can also be shared directly with the business profile.

A business profile for a user is similar to that user having a specific role in a group, such as a financial controller or project manager, and receiving the permissions that go along with that role for the specified group. The business profile can be temporary, allowing the permissions for a period of time that is set to expire, and maintaining data restrictions for the group or agency.

The Workfront system administrator:

* Creates the access levels and defines restricted fields as needed
* Updates the user profile with the group and the access level for that group (this is the business profile)
* Defines effective dates for the business profile as needed
* Assigns layout templates to the access levels

Any user who has access to share objects can share them with the business profile, and all users with the profile will see the object.

## Business profile example

>[!BEGINSHADEBOX]

Sam needs different access to projects for Agency A and Agency B. Both agencies are set up as groups in Workfront. (For information about groups, see Groups overview.)

For Agency A, Sam is acting as a financial controller and needs access to see all of the financial fields on their projects. For Agency B, Sam is acting as a project manager and needs to manage the tasks and issues, but should not be able to view the financial information.

The Workfront system administrator creates new access levels called Financial Controller and Project Manager. These access levels are given the correct access for financial data. Then the administrator opens Sam's user profile and selects "Agency A" as the group with the access level "Financial Controller" to create the first business profile, and "Agency B" as the group with the access level "Project Manager" to create the second business profile.

Once the business profiles are set up, when Sam goes to the list of projects, all of the projects for Agency A and Agency B will appear (along with any other projects that Sam has created or been given permissions to). The financial fields on Agency A's projects are visible to Sam in both the list view and the project details, but the financial fields on Agency B's projects are hidden. The field names appear but the field data is blank.

If other users at either agency share projects with the "Financial Controller – Agency A" or "Project Manager – Agency B" business profiles, then those projects are visible to Sam. The financial fields on Agency B's projects will always remain hidden because that is defined in the access level.

>[!ENDSHADEBOX]

## How business profiles are defined

The Adobe Workfront system administrator is responsible for defining all the areas of a business profile.

### Create access level

The Workfront system administrator creates the access level with the necessary access and defines any restricted fields as needed.

For more information, see [Create and modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### Add business profile to user

The Workfront system administrator adds the business profile to a user profile by selecting a group and access level. The combination of the two creates the business profile. Each group can only be used in one business profile per user. <!--how does this combine with more than one access level per group. As far as I can see a business profile is one level and one group-->

The business profile can have more than one access level per group. The level with the highest access takes precedence.

The administrator can assign effective dates to a business profile, so that the user's access will expire on a future date. The start and end dates indicate when the user begins and ends holding the profile in that group. Using effective dates to end the access instead of deleting the profile allows the profile to be activated again in the future.

Multiple business profiles are allowed for one user.

<!--image?-->

For more information, see [Edit a user's profile](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). <!--may be separate article now since it's not in the profile-->

### Assign layout templates to access level

The Workfront system administrator can optionally assign a layout template to the access level, to ensure that users with the related business profile see relevant information and actions based on their role within the system.

For more information, see [Assign users to a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

## How business profiles work

When a business profile is added to a user, the permissions in the combination of the group and the access level determine what the user will see in Workfront.

### Workfront layout

When the group in the business profile is associated to a project, the layout template for the access level in the business profile is applied. All users with the business profile will see the menu items, Home page, and other layout elements included in the template. The business profile layout template takes precedence over a layout template assigned to the user.

If the business profile has multiple access levels with the same group, the layout templates for both access levels are combined. All available layout elements are displayed. If a menu item is displayed in one template but hidden in another, it will be displayed. Only items that are hidden in all templates for the business profile are hidden.

For situations where the same items are displayed in multiple layout templates but the order of the items is different (such as the left navigation or pins), then the order from the template of the access level listed first in the business profile is used.

### Projects and other shared objects

When a project is associated to a group, a user with a business profile for that group can view the project. The visibility of fields in the project is based on the access level in the business profile. If multiple access levels are assigned to the group in the user's business profile, then the level with highest permissions applies.
 
For example, a user has two business profiles: the first provides financial controller access for a group (to see finance fields) and the second provides project manager access under a different group (where finance fields should not be viewed).

The user would see projects for both groups in the list of all projects. In both the list view and the project details, the user would see financial data only for the first group. The finance fields on the second group's projects would be blank.

Any user with access to share objects can share those objects with a business profile. All users assigned to the profile will have the specified permissions to the object. However, if access is restricted in the access level assigned by the administrator in the business profile, the access level takes precedence over permissions given in sharing. For example, if the access level does not allow creating tasks, then the user can't add tasks to a project, even if they are given Manage permissions to a project when it is shared with the business profile.

If a user is assigned a business profile after an object has already been shared with the profile, the user will see the object with the specified access.

When a business profile has multiple access levels, the level with the highest amount of access takes precedence.
 
For information on sharing, see [Share an object](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

For information about how access levels and permissions work together, see [Access levels overview](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

## Considerations about business profiles

* A user does not have to be a member of a group to be assigned a business profile for that group.
* The access level on the business profile can only upgrade a user's "base" access level. The business profile cannot take away the base access level permissions.
* In object lists and reports, the user has all of the permissions that are available to them from all of their assigned business profiles across the groups merged with their base access level. In other pages, the user has the base access level permissions.
* When a group is deleted from Workfront, all assigned business profiles for that group are removed from the associated users.
* If an access level is part of a business profile and you delete the access level, you are prompted to choose a new access level to use instead.
* Updates to business profiles are tracked in the Workfront audit logs. For more information, see Audit logs overview.
 
