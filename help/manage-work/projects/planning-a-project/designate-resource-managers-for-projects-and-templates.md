---
filename: designate-resource-managers-for-projects-and-templates
product-area: projects;templates
navigation-topic: plan-a-project
title: Designate Resource Managers for a project or template
description: You can designate up to 30 users as Resource Managers for an individual project or template. Designating Resource Managers for a project is a prerequisite for using the Scheduling tools in Adobe Workfront.
---

# Designate Resource Managers for a project or template

You can designate up to 30 users as Resource Managers for an individual project or template. Designating Resource Managers for a project is a prerequisite for using the Scheduling tools in&nbsp;*Adobe Workfront*.

>[!NOTE]
>
>We are no longer developing the Resource Scheduling tools and they will soon be removed from *Adobe Workfront*. We recommend that you use the *Workload Balancer* for scheduling your resources. 
>
>For information about scheduling resources using the new *Workload Balancer*, see the section [The Workload Balancer](../../../resource-mgmt/workload-balancer/workload-balancer.md).
>
>For more information about the timeline for removing the Resource Scheduling tools and replacing them with the *Workload Balancer*, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Templates</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project or template</p> <p>Users who are added as Resource&nbsp;Managers to a project or a template immediately gain Manage permissions on the project or the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Considerations about Resource Managers

>[!NOTE]
>
>Resource Manager is not a *Workfront* role; it is a field available on a project or a template that you can manually update.

* Designating Resource Managers on projects is a prerequisite to allowing users to schedule resources for work on the project when using the Scheduling tools.

  For information about resource scheduling, see&nbsp; [Resource Scheduling](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md)&nbsp;. 

* Designating Resource Managers on projects is not a prerequisite to allowing users to schedule resources for work using the *Workload Balancer*.

  For information about the *Workload Balancer*, see [Overview of the Workload Balancer](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

* You cannot designate teams or groups as resource managers. You can only designate users as resource managers.

* The users that you designate as Resource Mangers on a project or template do not automatically become part of the Project&nbsp;Team.

  For information about project teams, see [Manage the Project Team](../../../manage-work/projects/planning-a-project/manage-project-team.md).

* You can designate Resource Managers for projects or for project&nbsp;templates. When you designate Resource Managers on a project template, any users you designate as Resource Managers on the template automatically become Resource Managers on any projects that are created using that template.
* &nbsp;You can view the Resource Manager field in the following ways:

  * When building reports, as described in [Glossary of Adobe Workfront terminology](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).
  * When creating or customizing Views, as described in [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* You can add or remove Resource Managers by adding the Resource Manager field to a View, viewing it on a list of projects, and editing the Resource Manager field via in-line edit.

## Designate Resource Managers for a project

<ol> 
 <li value="1"> <p>Do any of the following:</p> 
  <ul> 
   <li>&nbsp; <draft-comment>
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       To add Resource Managers to a single project, go to the project where you want to designate one or more resource managers, then click the 
      <span class="bold">More menu <img src="assets/more-icon.png"></span> next to the project name, then 
      <span class="bold">Edit .</span> 
     </MadCap:conditionalText>
    </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      To add Resource Managers to a single project, go to the project where you want to designate one or more resource managers, then click the 
     <span class="bold">More menu <img src="assets/more-icon.png"></span> next to the project name, then 
     <span class="bold">Edit .</span> 
    </MadCap:conditionalText></li> 
   <li> <p>To add Resource Managers to multiple projects simultaneously, navigate to a list of projects, select the projects where you want to designate one or more resource managers, then click <span class="bold">Edit</span>.</p> <p>Existing Resource Managers are not removed from the projects you are editing; any users you add in this way are added as Resources Managers on the project in addition to any existing Resource Managers.</p> </li> 
   <li> <p> To add Resource Managers to a new project, begin creating a new project. </p> <p>For information about creating a project, see <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Create a project</a>.</p> </li> 
  </ul> </li> 
 <li value="2"> <p>In the <span class="bold">Overview</span> section on the Edit Project dialog box, click in the <span class="bold">Resource Manager</span> field.</p> </li> 
 <li value="3"> <p>Begin typing the name of the user who you want to add as a resource manager for the project, then click the name when it appears in the list.</p> <p>Repeat this step to add multiple resource managers for the project. Up to 30&nbsp;resource managers can be designated for a given project.</p> </li> 
 <li value="4">Click <span class="bold">Save Changes</span>.<br></li> 
</ol>

## Designate Resource Managers for a template

<ol> 
 <li value="1"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Click the 
    <span class="bold">Main Menu</span> icon 
    <img src="assets/main-menu-icon.png"> in the upper-right corner of 
    <em>Adobe Workfront</em>. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
   <span class="bold">Main Menu</span> icon 
   <img src="assets/main-menu-icon.png"> in the upper-right corner of 
   <em>Adobe Workfront</em>. 
  </MadCap:conditionalText></li> 
 <li value="2"> <p> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      Click&nbsp; 
     <span class="bold">Templates</span>. 
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Click&nbsp; 
    <span class="bold">Templates</span>. 
   </MadCap:conditionalText></p> <p> <br> </p> </li> 
 <li value="3">Do any of the following:<br> 
  <ul> 
   <li> <draft-comment>
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       To add Resource Managers to a single template, go to the template where you want to designate one or more resource managers, then click the 
      <span class="bold">More menu <img src="assets/more-icon.png"></span> next to the template name, then 
      <span class="bold">Edit .</span> 
     </MadCap:conditionalText>
    </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      To add Resource Managers to a single template, go to the template where you want to designate one or more resource managers, then click the 
     <span class="bold">More menu <img src="assets/more-icon.png"></span> next to the template name, then 
     <span class="bold">Edit .</span> 
    </MadCap:conditionalText></li> 
   <li><p>To add Resource Managers to multiple templates&nbsp;simultaneously, go to a list of templates and select the templates where you want to designate one or more&nbsp;Resource Managers, then click <span class="bold">Edit</span>.</p><p>Existing Resource Managers are not removed from the templates&nbsp;you are editing; any users you add in this way are added as Resources Managers on the template&nbsp;in addition to any existing Resource Managers.<br></p></li> 
   <li> <draft-comment>
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       To add Resource&nbsp;Managers to a new template, click&nbsp; 
      <span class="bold">New Template</span>,then click the 
      <span class="bold">More menu <img src="assets/more-icon.png"></span> next to the template name, then 
      <span class="bold">Edit .</span> 
     </MadCap:conditionalText>
    </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      To add Resource&nbsp;Managers to a new template, click&nbsp; 
     <span class="bold">New Template</span>,then click the 
     <span class="bold">More menu <img src="assets/more-icon.png"></span> next to the template name, then 
     <span class="bold">Edit .</span> 
    </MadCap:conditionalText></li> 
  </ul></li> 
 <li value="4"> <p>In the <span class="bold">Overview</span> section, click in the <span class="bold">Resource Manager</span> field.</p> </li> 
 <li value="5"> <p>Begin typing the name of the user who you want to add as a resource manager for the template, then click the name when it appears in the list.</p> <p>Repeat this step to add multiple resource managers to the template. Up to 30&nbsp;resource managers can be designated for a given template.&nbsp;</p> </li> 
 <li value="6">Click <span class="bold">Save Changes</span>.</li> 
</ol>

