---
filename: work-with-resource-pools
product-area: resource-management
navigation-topic: resource-planning
title: Resource pools overview in Adobe Workfront
description: As a resource manager, you can manage your resources by adding users to resource pools.
---

#  Resource pools overview in `Adobe Workfront`

As a resource manager, you can manage your resources by adding users to resource pools.

Efficient resource management cannot happen without populating your Resource Pools with users and attaching them to projects. This a prerequisite for using the Resource Planning functionality.

For more information about the prerequisites needed before you can start using Resource Planning, see the "Prerequisites for working in the `Resource Planner`" section in [Resource Planner overview](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

For information about creating and managing resource pools, see the following articles:

* [Create resource pools in Adobe Workfront](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md) 
* [Associate resource pools with projects and templates in Adobe Workfront](../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md) 
* [Associate resource pools with users in Adobe Workfront](../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md) 
* [Remove users from resource pools in Adobe Workfront](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md)

<!--
Access requirements You must have the following: Adobe Workfront plan* Pro and higher Adobe Workfront license* Plan Access level configurations* Edit access to Resource Management that includes access to Manage Resource Pools Edit access to Projects, Templates, and Users Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see Create or modify custom access levels. Object permissions Manage permissions for the projects, templates, and users you associate the Resource Pools with For information on requesting additional access, see Request access to objects in Adobe Workfront. *To find out what plan, license type, or access you have, contact your Workfront administrator.
-->

## Overview of Resource Pools

* A Resource Pool is a collection of users that are needed at the same time for the completion of a project.
* A Resource Pool can be shared across multiple projects, programs, or portfolios when it is associated with all the projects in the programs and portfolios. 
* You can either create a Resource Pool and populate it with existing users upon its creation, or you can create the Resource Pool and associate it with an existing user or with a new user as you are creating or editing the user. 
* After you populate your Resource Pools with users, you can associate them with projects and templates, and manage your user allocation to the projects more efficiently. 
* You can associate as many Resource Pools as needed with a project, template, or user.

## Criteria for associating users with a Resource Pool

There are several ways to structure your Resource Pools.

We recommend the following approaches:

* You can have all the users in the same Resource Pool belong to the same team.

  For example, if you want all the users of a Marketing team to be available for a project, you would want a Marketing Resource Pool where you would add all the users in that team. You can then associate the Marketing Resource Pool with the projects the members of that team are assigned to.

* You can have all the users in the same Resource Pool fulfill similar roles, especially if the roles are in high demand and must be budgeted separately.

  For example, you may have external resources that work as Consultants that you want to have available for a project from time to time. You can create a Resource Pool for Consultants that you can attach to your projects, where you can place both users that are internal or external Consultants.

* You can also create Resource Pools by department or cost center. 
* We do not recommend adding all users in the system to one Resource Pools if you have a large number of users, or if you manage resources for a large number of a projects at a time.

<!--
Create a Resource Pool Log in as a user who has access to edit Resource Pools. For more information, see Create a Resource Pool. Click the Main Menu icon in the upper-right corner of Adobe Workfront. Click Resourcing. Click Resource Pools in the left panel. Click New Resource Pool. Specify the following: Name This is the name of the Resource Pool. Description This is a brief description about this Resource Pool. For example, you can specify for what purpose it should be used. (Optional) Pool Members Add users to the Resource Pool individually. Or To add a large amount of users to the Resource Pool at one time, you can add one of the following entities associated with users. This adds those users to the Resource Pool: Teams: all members of the team are added to the Resource Pool. Groups: all members of the group are added to the Resource Pool. Roles: all users associated with that role are added to the Resource Pool. Companies: all users in the company are added to the Resource Pool. Tip: You can only add active users, teams, roles, or companies. Note: If a user becomes a member of a group, team, company or is associated with a job role after the group, team, company or job role have been added to the Resource Pool, the new member is not automatically added to the Resource Pool. If a user belongs to the team, group, company, and job role you are adding, at the same time, the user is added only once to the Resource Pool. Users who are deactivated after having been added to the Resource Pool appear dimmed in the list of users and are marked as being deactivated. (Optional) Use the Undo link to remove the users added through a group, team, company or job role. Note: There is no limit to how many users you can have in a Resource Pool. However, we recommend not adding too many users to a Resource Pool, as Resource Management could become a challenge otherwise. The list of users only shows the first 2,000 users in the Resource Pool, and they are listed alphabetically. (Optional) Use the Search option to find a user in the Resource Pool. Click Create.
-->

<!--
Remove users from a Resource Pool You can remove users from a Resource Pool when those users are no longer needed in that pool. To remove a user from a Resource Pool: Log in as a user who has access to edit Resource Pools. For more information, see the section Create a Resource Pool in this article. Click the Main Menu icon in the upper-right corner of Adobe Workfront. Click Resourcing. Click Resource Pools in the left panel. Select a Resource Pool and click Edit. Or Click the name of a Resource Pool. Start typing the name of a user that you want to remove in the Search in this Resource Pool field. Or Start typing the name of a company, job role, team, or group, if you want to remove all the users associated with those entities. Click the 'x' icon at the user level to remove a user from the Resource Pool. They are removed from all the lists they appear in. Or To remove all users associated with a job role, group, team, or company, click Remove at the job role, group, team level, or company level. This removes all the users associated with that job role, group, team, or company from the Resource Pool. Click Save.
-->

<!--
Associate Resource Pools with users You must have administrative rights to editing users in order to edit or create users. For more information about the access needed to edit or create users, see Grant access to users. Associate Resource Pools with one user Associate Resource Pools with users in bulk Associate Resource Pools with one user You can associate users with Resource Pools when you are creating your Resource Pools. For more information about creating a Resource Pool, see the section Create a Resource Pool in this article. If you create Resource Pools without populating them with users, you can later associate them with users as you are editing or creating new users. The Resource Pools must be created before you can associate them with a user. To associate Resource Pools with users: Click the Main Menu icon in the upper-right corner of Adobe Workfront. Click Users. Check the box next to the name of a user from the list, then click Edit. Click Resource Planning. Start typing the name of a Resource Pool that you want to associate with the user in the Resource Pools field, then select it from the list, when it appears. You can associate multiple Resource Pools with one user. Click Save Changes. For more information about editing users, see Edit a user's profile. For more information about creating new users, see Add users. Associate Resource Pools with users in bulk You can edit multiple users in bulk and associate the same Resource Pools with all of them at the same time. To associate Resource Pools with several users in bulk: Click the Main Menu icon in the upper-right corner of Adobe Workfront. Click Users. Select several users on the list, and click Edit. Click Resource Planning. Start typing the name of a Resource Pool that you want to associate with the users in the Resource Pools field, then select it from the list, when it appears. You can associate multiple Resource Pools with multiple users. Note: Only the Resource Pools that are common to all the users selected appear in this field. If the users selected have no shared Resource Pools, this field is empty. If this field is empty, the Resource Pools you specify here will overwrite their individual Resource Pools. Click Save Changes. For more information about how to edit users in bulk, see Edit user profiles in bulk.
-->

<!--
Associate resource pools with projects and templates After you create Resource Pools, you can associate them with projects or templates so you can later budget your resources on the projects. You must have the following rights to associate Resource Pools with Projects and Templates: You must have rights to Edit projects in your access level, as well as Manage permissions on the project in order to edit the project and associate it with Resource Pools. You must have rights to Edit templates in your access level, as well as Manage permissions on the template in order to edit the template and associate it with Resource Pools. We recommend that you create your Resource Pools in advance, associate them with projects, and budget your resources before the project starts. Associate Resource Pools with one project or template Associate Resource Pools with several projects or templates in bulk Associate Resource Pools with one project or template You can associate Resource Pools with a template in the same manner you associate Resource Pools with a project. To associate Resource Pools with a project: Go to a project and click the Edit icon in the upper-right corner. Click Settings. Start typing the name of a Resource Pool in the Resource Pools field, then select it from the list when it appears. You can associate multiple Resource Pools with one project or template. Click Save Changes. For more information about how to edit a project and associate it with Resource Pools, see Edit projects. For more information about how to edit a template and associate it with Resource Pools, see Edit project templates. Associate Resource Pools with several projects or templates in bulk You can edit multiple projects or templates in bulk and associate the same Resource Pools with all of them at the same time. You can associate Resource Pools with templates in the same manner you associate Resource Pools with projects. To associate Resource Pools with several projects in bulk: Go to a list of projects. Select multiple projects, then click Edit. Click Settings. Start typing the name of a Resource Pool in the Resource Pools field, then select it from the list when it appears. You can associate multiple Resource Pools with the projects or templates. Note: When you edit projects or templates in bulk, only the Resource Pools that are common to all the projects or templates selected appear in this field. If the projects selected have no shared Resource Pools, this field will be empty. The Resource Pools you specify here will overwrite the individual Resource Pools of the projects or templates. Click Save Changes. When your Resource Pools are associated with your projects or your templates, you can budget user allocations for your projects inside the Resource Planner. For more information about the Resource Planner, see Resource Planner overview. For more information about how to edit projects in bulk, see the "Edit projects in bulk" section in Edit projects. For more information about how to edit templates in bulk, see the "Edit templates in bulk" section in Edit project templates.
-->

