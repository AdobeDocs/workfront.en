---
filename: groups
title: Groups
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
---




# Groups {#groups}

As a `Workfront administrator`, you can create groups of users that coincide with your departmental structure. Groups are similar to, but distinct from teams and companies. 


You grant groups the access to the `Workfront` areas where they need to work and communicate. Each group can then keep their `Workfront` information such as users, templates, and custom forms, and projects separate from those of other departments. 


At least one `Group Administrator` is required for every group. For information about `Group Administrators`, see [Group Administrators](group-administrators.md).


For information about subgroups, see [Subgroups](subgroups.md).


## About using groups to organize users {#about-using-groups-to-organize-users}

As a `Workfront administrator` or `Group Administrator`, you can associate users to groups and subgroups. If you make a group public, users with a Planner license can associate users with it. For more information about Group Administrators and public groups, see [Create and manage groups](create-manage-groups.md).  



When you create a user, we recommend that you add that user to the appropriate Home Group and other groups that the user should work in. A user can have only one Home Group, but can be in multiple other groups. 


Being part of a group gives the user access to objects that are shared with the group and the subgroups. For example, if you share a project with a group, users in the group and the group's subgroups have access to it.


>[!TIP] {type="tip"}
>
>If departments in your organization often work together to manage projects and the resources on those projects, it might not be necessary to divide departments into many smaller groups. A few high level groups might work best. 


A group can have an unlimited number of users.


For more information about creating new users, see [Add users](_Add users.md).


## About granting a group access to objects {#about-granting-a-group-access-to-objects}

When you share an object with a group, all members of that group (including members of any subgroups) have access to the object. For more information about sharing in `Workfront`, see [Share Permissions on objects](sharing-permissions-on-objects.md).


## About associating a group with a project {#about-associating-a-group-with-a-project}

Groups can be associated with a project in order to indicate ownership of the project. This does not implicitly grant each member of the group rights to the project. In order to have rights to the project users must receive rights by sharing the project with them.  
For more information about sharing in `Workfront`, see [Share Permissions on objects](sharing-permissions-on-objects.md).


While users can be members of multiple groups, a project can have a single group associated with it. Users from other groups can still work on the same project, if the projects has been shared with them or their groups. The group associated with the project is usually either the group responsible for completing the project, or the group for whom the project is delivered.


For more information about associating a project with a group, see [Understand the project Overview area](understand-project-overview-area.md).
