---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Resource Planner Display Limitations
description: To improve performance, Adobe Workfront is limiting the amount of information you can display as well as the amount of information you can export from the Resource Planner.
author: Lisa
feature: Resource Management
exl-id: 12f56f11-59fb-4318-b43a-5ac695ca1e7e
---
# Resource Planner display limitations

To improve performance, Adobe Workfront is limiting the amount of information you can display as well as the amount of information you can export from the Resource Planner.

When you approach this limit, Workfront displays a warning message to let you know you have reached that limit.

If the information you expect to see in the Resource Planner does not display, it is possible that you are trying to display too much information and some data has not been displayed due to this limitation.

We recommend the following for optimal performance in displaying and exporting the Resource Planner:

* Use filters to reduce the amount of information you display in the Resource Planner and view only information that is pertinent to you.
* Use all your exporting options to reduce the amount of information you export at one time and to ensure you export only pertinent information.  
  For more information about using filters and exporting options in the Resource Planner, see [Filter information in the Resource Planner](../../resource-mgmt/resource-planning/filter-resource-planner.md).

  For information about exporting information from the Resource Planner, see [Export information from the Resource Planner](../../resource-mgmt/resource-planning/export-resource-planner.md).

The amount of information that you can display or export depends on which view you apply and what environment you use to access the Resource Planner.

## Limitations in the Project View

Consider the following when applying the Project view to the Resource Planner:

* You can only see projects you have access to manage. 
* You can expand each project to view roles associated with it, and each role to view the users associated with it.

  You can view up to 300 projects, when you scroll to the bottom of the list, unless there are more than 30,000 rows of projects, roles, and users. Then, you receive a warning message that you have reached the 30,000 row limit. 

* You can view three or four time periods at a time, depending on the size of your screen.

Consider the following when exporting information from the Project view of the Resource Planner, after you have applied all the appropriate filters and export options:

* When you select to export everything ( projects, roles, and users) in the Resource Planner, all the objects that match your criteria appear in the exported file whether you have scrolled to the bottom of the list to display them or not.
* Rows without allocation information are included in the exported file.

* You can export up to 30,000 rows.

## Limitations in the Role View

Consider the following when applying the Role view to the Resource Planner, after you have applied all the appropriate filters:

* You can see only roles that are associated with projects that you can manage.

* You can see up to 300 roles when you scroll to the bottom of the list, unless there are more than 30,000 rows of roles, projects, and users. Then, you receive a warning message that you have reached the 30,000 row limit for what you can view on the screen.
* You can expand each role to display a list of projects, and every project to display a list of users that can fulfill those roles on the projects.

  20 projects display by default and you can use the Load More option to display additional projects, or scroll under each project to load more users.

* You can view three or four time periods, depending on the size of your screen.

Consider the following when exporting information from the Role view of the Resource Planner, after you have applied all the appropriate filters and export options:

* When you select to export everything (roles, projects, and users) in the Resource Planner, all the objects that match your criteria appear in the exported file whether you have scrolled to the bottom of the list to display them or not.
* Rows without allocation information are included in the exported file.
* You can export up to 30,000 rows.

## Limitations in the User View

Consider the following when applying the User view to the Resource Planner:

* You can display all users that meet the following criteria:

   * You have access to view
   * Are active
   * Have logged in at least once.

* You can expand each user to display the projects associated with it, and each project to display roles associated with it.  
  The first 50 projects and roles display by default, and you can use the Load More option to display additional projects or roles.

  >[!NOTE]
  >
  >If you have filtered the list of users by projects, only the users associated with the filtered projects can be expanded and also display hour information

* You can see up to 2,000 users in the web interface. Workfront displays a warning message when you reach this limit.
* You can view three or four time periods, depending on the size of your screen.

Consider the following when exporting information from the User view of the Resource Planner, after you have applied all the appropriate filters and export options:

* When you select to export everything ( users, roles, and projects) in the Resource Planner all the roles, projects and users are included in the exported file, whether they are expanded or not in the web interface.

* You can export up to 30,000 rows that contain users, as well as the projects and roles listed underneath, whether you have scrolled to the bottom of the list to display them or not. All the users, projects, and roles are included in the exported file, whether they are expanded or not in the web interface. 
* Rows without allocation information are included in the exported file.
