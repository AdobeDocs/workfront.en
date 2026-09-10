---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "View: List of Project Users with Job Roles"
description: You can apply this view in a project list or report to display a list of users that are associated with the project, as well as a list of the job roles they are performing on the project.
author: Courtney
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/rvhc2k8P5eA7X-b-x-kXgI4j4G5FR0J29PXIFSoRPj0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# View: list of project users with job roles

<!--Audited: 11/2024-->

You can apply this view in a project list or report to display a list of users that are associated with the project, as well as a list of the job roles they are performing on the project.

The information in this report can also be found in the  People area  of the project.

>[!TIP]
>
>If no job roles are listed for the users but you know that they are associated with job roles in their user profiles, this might mean they are assigned to tasks and issues but they might not be associated with a job role on the task or issue, or the users listed in the report are not the assignees on tasks and issues, but fulfill other roles on the project (for example, Owner or Sponsor.)

![project_with_user_and_role_information_report.png](assets/project-with-user-and-role-information-report-350x100.png)

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Contributor or Request to modify a view </p>
   <p>Standard or Plan to modify a report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a view</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++


## View a list of project users with job roles

1. Go to a list of projects.
1. From the **View** drop-down menu, select **New View**.
1. In the **Column Preview** area, eliminate all columns except for one.
1. Click the header of the remaining column, then click **Switch to Text Mode** > **Edit Text Mode**.
1. Remove the text you find in the **Edit Text Mode** box, and replace it with the following code:  

   ```
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.section=0
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=200
   column.1.displayname=Project Users
   column.1.listdelimiter=<br>
   column.1.listmethod=nested(projectUsers).lists
   column.1.textmode=true
   column.1.type=iterate
   column.1.valueexpression={user}.{name}
   column.1.valueformat=HTML
   column.2.displayname=Project Roles
   column.2.listdelimiter=<br>
   column.2.listmethod=nested(projectUserRoles).lists
   column.2.textmode=true
   column.2.type=iterate
   column.2.valueexpression={role}.{name}
   column.2.valueformat=HTML
   ```

1. Click **Done** > **Save View**.
