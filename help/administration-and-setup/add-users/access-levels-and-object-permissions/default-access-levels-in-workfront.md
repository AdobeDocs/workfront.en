---
filename: default-access-levels-in-workfront
user-type: administrator
content-type: reference
product-area: system-administration
keywords: access,model,funnel,diagram,levels,permissions
navigation-topic: access-levels
---



# Built-in access levels in *`Adobe Workfront`* {#built-in-access-levels-in-adobe-workfront}

All 6 of the built-in access levels are designed for a particular type of user:



*  System Administrator
*  Planner
*  Worker
*  Reviewer
*  Requestor
*  External User


For general information about these access levels, see [Access levels overview](access-levels-overview.md).


Depending on the access level, up to 3 settings are available for most of the *`Workfront`* object types:

If you need a custom Planner, Worker, Requester, or Reviewer access level, you can copy the built-in access level and determine the amount of access you want it to allow for the various *`Workfront`* object types. For information on creating a custom access level or modifying one of the built-in access levels, see [Create or modify custom access levels](create-modify-access-levels.md).


>[!IMPORTANT] {type="important"}
>
>We strongly recommend that you leave the built-in access levels unchanged so that you can refer to them after you set up your users.





## System Administrator access level {#system-administrator-access-level}

Attached to the *`Plan`* license, this built-in access level is designed for a user who is in charge of administering the *`Adobe Workfront`* system. You cannot modify this built-in access level.


Users with the System Administrator access level can do everything within *`Workfront`*. They can view and edit all *`Workfront`* objects and information entered in *`Workfront`* by all other users. 


They also have access to the complete Setup area, where they can change any setting at the system level. And they can access all areas in the `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Main Menu  <img src="assets/main-menu-icon.png"></MadCap:conditionalText>`.


For more information, see [Grant a user full administrative access](grant-a-user-full-administrative-access.md).


## Planner access level {#planner-access-level}

Also attached to the *`Plan`* license, this access level is designed for:



* Managers of groups, teams, projects, and resources
* Anyone who is responsible for planning, creating, and managing tasks, projects, portfolios, and programs
* Anyone who is responsible for assigning work (tasks and issues) to other users
* Users who build reports and who approve timesheets, work items, and documents
* Users who need access to all areas in the `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Main Menu  <img src="assets/main-menu-icon.png"></MadCap:conditionalText>`  



You can create a custom version of the *`Planner`* built-in access level and determine the amount of access it allows for the various *`Workfront`* object types. For more information, see [Built-in access levels in Adobe Workfront](#customiz) in this article.


The following are the highest access settings available for objects in the Planner access level:



## Worker access level {#worker-access-level}

Attached to the *`Work`* license, this built-in access level is designed for users who for perform the work in *`Workfront`*. They do not plan the work; they complete it.


Users with this access level:



* Are assigned to work items where they can contribute and log time
* Can approve work and documents, but not timesheets
* Can access and share reports
* Can communicate with other users in the system  
* Can access all the areas in the `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Main Menu  <img src="assets/main-menu-icon.png"></MadCap:conditionalText>`, but their `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> "Users"</MadCap:conditionalText>` area is named Teams. In the Teams area, users with this access level can view only teams that they belong to, along with the work assigned to those teams.

*  Have limited ability to create objects—they can’t create projects, portfolios, programs, or reports.


You can create a custom version of the *`Worker`* built-in access level and determine the amount of access it allows for the various *`Workfront`* object types. For more information, see [Built-in access levels in Adobe Workfront](#customiz) in this article.


The following are the highest access settings available for objects in the Worker access level:



## Reviewer access level {#reviewer-access-level}

Attached to the *`Review`* license, this access level is designed for executives who request work from other users and who review and approve work. These are not project owners or team members, but they need access to *`Workfront`* to see the work items that they oversee.


For example, a stakeholder with this access level could log in to *`Workfront`* to participate in an ongoing review of marketing materials, see work updates on work, and review documents, approvals, reports, and calendars.


Users with the Reviewer access level:



* Cannot be assigned work items or approve time sheets
* Can access requests and documents in the `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Main Menu  <img src="assets/main-menu-icon.png"></MadCap:conditionalText>`.
* Have limited ability to create objects—they can’t create projects, portfolios, programs, or reports.


You can create a custom version of the *`Reviewer`* built-in access level and determine the amount of access it allows for the various *`Workfront`* object types. For more information, see [Built-in access levels in Adobe Workfront](#customiz) in this article.


More limited for projects and tasks than the Worker access level, the following are the highest access settings available for objects in the Reviewer access level:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> object type</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">No access</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">View access</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Edit access</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Projects</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Tasks</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Issues</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Portfolios</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Programs</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓ (The default setting is No Access.)</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Reports (including dashboards and calendar reports)</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Filters, views, and groupings</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Documents</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Users</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Templates</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Financial data</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>✓ (The default setting is No Access. The View setting allows the user to view only the Finance <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      area
     </MadCap:conditionalText> <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      in
     </MadCap:conditionalText> Project Details.)</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Resource Management</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="mc-variable WFVariables.Scenario_Planner_-_feature_name variable varname">Scenario Planner</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">✓ (The default setting is No Access.)</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"><span class="mc-variable WFVariables.Workfront_Align_(Goals) variable varname">Workfront Goals</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">✓ (The default setting is No Access.)</td> 
  </tr> 
 </tbody> 
</table>



## Requestor access level {#requestor-access-level}

Attached to the *`Request`* license, this built-in access level is designed for users who make and receive simple work requests in *`Workfront`*. By default, they are limited to the Requests area.


For example, a user can log issues to your organization’s help desk request queue. 


Users with this built-in access level:



* Can make requests and update those requests
* Can upload and approve documents
* Can review the status of issues they have submitted
* Cannot be assigned to work items  
*  Can `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> access requests only from the Main Menu <img src="assets/main-menu-icon.png"></MadCap:conditionalText>`. For more information about request queues, see [Create a Request Queue](create-request-queue.md).


You can create a custom version of the *`Requester`* built-in access level and determine the amount of access it allows for the various *`Workfront`* object types. For more information, see [Built-in access levels in Adobe Workfront](#customiz) in this article.


The following are the highest access settings available for objects in the Requestor access level:



## External User access level {#external-user-access-level}

This access level is not attached to a paid *`Workfront`* license. It is the most restrictive access level, designed primarily for collaborators such as external consultants who don't log into *`Workfront`*, but need to review, download, or view documents occasionally.


*`Workfront`* users can assign tasks to external users even though external users can't log in to the system. But we advise against this because that work would remain unresolved in the system.


Users with the External User access level:



* Can view only documents and calendar reports that are shared with them
* See the users who share documents and calendar reports with them
* Approve the documents that are shared with them


You cannot modify this access level.


The following are the highest access settings available for objects in the External User access level.

