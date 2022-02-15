---
filename: share-a-task
title: Share a task
product-area: projects
navigation-topic: grant-and-request-access-to-objects
---



# Share a task in  *`Adobe Workfront`* {#share-a-task-in-adobe-workfront}

Your *`Adobe Workfront administrator`* can grant you access to view or edit tasks when they assign access levels. For more information about granting access to tasks, see [Grant access to tasks](grant-access-tasks.md).


Along with the access level that users are granted, you can also grant them permissions to View, Contribute, or Manage specific tasks that you have access to share.


Permissions are specific to one item in *`Workfront`* and define what actions one can take on that item.  



## Considerations when sharing a task {#considerations-when-sharing-a-task}

In addition to the considerations below, also see [Overview of sharing permissions on objects in Adobe Workfront](sharing-permissions-on-objects-overview.md).



* The creator of a task has Manage permissions to it, by default.
* You can share tasks individually, or you can share several of them at a time, in bulk.  
  Sharing tasks is identical to sharing other objects. For more information about sharing items in *`Workfront`*, see [Share an object in Adobe Workfront](share-an-object.md). 

*  You can grant the following permissions to a task:&nbsp; 
    
    
    * View
    * Manage
    * Contribute  
      ![](assets/screen-shot-2014-05-30-at-11.37.24-am-175x192.png) ![](assets/screen-shot-2014-01-23-at-1.12.40-pm-154x258.png) ![](assets/screen-shot-2014-01-22-at-10.53.00-am-182x252.png)  
    
    
    
*  When you share a task, users inherit the same permissions on all the children objects associated with the task, by default. For example, they inherit the same permissions on the children tasks, issues, and documents attached to the task.   
  For more information about the hierarchy of objects in *`Workfront`*, see&nbsp; [Understand objects in Adobe Workfront](understand-objects.md).


  The *`Workfront administrator`* can specify whether documents should inherit permissions from higher objects in the user's access level. For more information about restricting inherited permissions on documents, see [Create or modify custom access levels](create-modify-access-levels.md).

* You can remove inherited permissions from a task.  
  For more information about removing inherited permissions from objects, see&nbsp; [Remove permissions from objects in Adobe Workfront](remove-permissions-from-objects.md). 





## Ways to share a task {#ways-to-share-a-task}

You can share a task in the following ways:



*  Manually, either individually or in bulk. Manually sharing tasks is similar to sharing any other object in *`Workfront`*. 


  For more information about sharing objects in *`Workfront`*, see&nbsp; [Share an object in Adobe Workfront](share-an-object.md). 






*  Automatically, by doing the following:

    
    
    *  Specify the permissions on any of the parent objects of the task: project, program, or portfolio. Tasks inherit the permissions from their parent objects. For information about viewing inherited permissions on objects, see [View inherited permissions on objects in Adobe Workfront](view-inherited-permissions-on-objects.md). 
    *  Add entities to Project Sharing on a template used to create the project the task is on. For information about sharing projects from templates, see [Share a template overview](share-a-template.md). 
    
    

    
    
    *  Specify the permissions on all tasks in a project when you edit the project.&nbsp;For information about managing the access to tasks on the project based on a user's permissions to the project, see the [](edit-projects.md#access) section in the article [Edit projects](edit-projects.md). 
    
    


  >[!TIP] {type="tip"}
  >
  >If you don't specify what task permissions you want users to have when they are assigned to the tasks on the project, they receive the same permissions they have on the project, by default. 







## Task permissions {#task-permissions}

The following table displays what permissions you can grant users when allowing them to View, Contribute, or Manage a task:

<table border="2" cellspacing="15" cellpadding="1" style="mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;width: 100%;" class="TableStyle-TableStyle-HeaderRow"> 
 <col style="width: 150px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 150px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 150px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 150px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="bold">Action</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="bold">Manage</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"><span class="bold">Contribute</span> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"><span class="bold">View</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Add Task(s)</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Add Predecessors</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Add Issue(s)</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Delete Task</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>General Task edit<br></p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Change Task Status</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Edit Task Constraint</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">View Task</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Add Document(s)</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Copy Task*</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Move Task*</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Log Hours</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Modify Planned Dates</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Accept Assignment</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Make an Assignment</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Attach Custom Form</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Edit Custom Fields</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Create an Approval Process</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Approve A Task</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Edit Finance*</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Add/Edit Expenses</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">View Finance</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Updates/Comments</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Share</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">Share System-wide</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;Controlled by access level and the permissions on the project.
