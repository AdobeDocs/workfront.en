---
product-area: projects;templates
navigation-topic: plan-a-project
title: Designate Resource Managers for a project or template
description: You can designate Resource Managers for a project to indicate who is responsible for managing resources on the project.
author: Alina
feature: Work Management
exl-id: ae2a89e7-8049-4ee6-9b28-ce247d3f2a6f
---
# Designate Resource Managers for a project or template

<!--
<p This article might have to be deleted when the Resource Manager field/ requirement will be forever removed from the system; right now it's still a requirement for Scheduler - January 2023/p>
-->

<!-- remove Prod and Prev references with Prod release - Jan 2023-->

You can designate Resource Managers for a project to indicate who is responsible for managing resources on the project. This is an informational field and it is not connected to any resource management tools. 

<!-- drafted for res scheduling deprecation blurb for preview release
Designating Resource Managers for a project is a prerequisite for using the Scheduling tools in Adobe Workfront, in the Production environment.
  
>[!CAUTION]  
>  
>  
> <span class="preview">Some of the information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span>  
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span>  
>  
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../../resource-mgmt/workload-balancer/workload-balancer.md).</span>  
>  
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

## Access requirements

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Templates</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project or template</p> 
   
   <p><b>NOTE</b>
   
   Users who are added as Resource Managers to a project or a template immediately gain Manage permissions on the project or the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Templates</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project or template</p> 
   
   <p><b>NOTE</b>
   
   Users who are added as Resource Managers to a project or a template immediately gain Manage permissions on the project or the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator.

## Considerations about Resource Managers

>[!NOTE]
>
>Resource Manager is not a job role; it is a field available on a project or a template that you can manually update.

* You can designate up to 30 users as Resource Managers for an individual project or template.

<!--
* In the Production environment,designating Resource Managers on projects is a prerequisite to allowing users to schedule resources for work on the project when using the Scheduling tools.

  For information about resource scheduling, see [Resource Scheduling](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md). 

  <span class="preview">Scheduling tools have been removed from the Preview environment.</span>

* Designating Resource Managers on projects is not a prerequisite to allowing users to schedule resources for work using the Workload Balancer.

  For information about the Workload Balancer, see [Workload Balancer overview](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

 -->

* You cannot designate teams or groups as resource managers. You can only designate users as resource managers.

* The users that you designate as Resource Mangers on a project or template do not automatically become part of the Project Team.

  For information about project teams, see [Manage the Project Team](../../../manage-work/projects/planning-a-project/manage-project-team.md).

* You can designate Resource Managers for projects or for project templates. When you designate Resource Managers on a project template, any users you designate as Resource Managers on the template automatically become Resource Managers on any projects that are created using that template.
* You can view the Resource Manager field in the following areas:

   * When editing a project, as described in this article.
   * When editing a template, as described in this article.
   * When building project or template reports. For information about building reports, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). 
   * When creating or customizing a project or template view for a list. For more information, see [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* You can quickly add or remove Resource Managers on multiple projects or templates by adding the Resource Manager field to a view of a list or a project and editing this field using in-line edit.

## Designate Resource Managers for a project

1. Do any of the following:

   *  To add Resource Managers to a single project, go to the project where you want to designate one or more resource managers, then click the **More menu** next to the project name, then **Edit .** 
   
   * To add Resource Managers to multiple projects simultaneously, navigate to a list of projects, select the projects where you want to designate one or more resource managers, then click **Edit**.

     Existing Resource Managers are not removed from the projects you are editing; any users you add in this way are added as Resources Managers on the project in addition to any existing Resource Managers.
   
   * To add Resource Managers to a new project, begin creating a new project.

     For information about creating a project, see [Create a project](../../../manage-work/projects/create-projects/create-project.md).

1. In the **Overview** section on the Edit Project dialog box, click in the **Resource Manager** field.
1. Begin typing the name of the user who you want to add as a resource manager for the project, then click the name when it appears in the list.

   Repeat this step to add multiple resource managers for the project.

1. Click **Save Changes**.

## Designate Resource Managers for a template

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront. 

1. Click **Templates**.

1. Do any of the following:

   * To add Resource Managers to a single template, go to the template where you want to designate one or more resource managers, then click the **More menu** next to the template name, then **Edit .** 
   
   * To add Resource Managers to multiple templates simultaneously, go to a list of templates and select the templates where you want to designate one or more Resource Managers, then click **Edit**.

     Existing Resource Managers are not removed from the templates you are editing; any users you add in this way are added as Resources Managers on the template in addition to any existing Resource Managers.

   * To add Resource Managers to a new template, click **New Template**,then click the **More menu** next to the template name, then **Edit .**

1. In the **Overview** section, click in the **Resource Manager** field.
1. Begin typing the name of the user who you want to add as a resource manager for the template, then click the name when it appears in the list.

   Repeat this step to add multiple resource managers to the template. 

1. Click **Save Changes**.
