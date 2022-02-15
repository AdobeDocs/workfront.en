---
filename: sharing-permissions-on-objects-overview
content-type: overview
navigation-topic: grant-and-request-access-to-objects
---



# Overview of sharing permissions on objects in *`Adobe Workfront`* {#overview-of-sharing-permissions-on-objects-in-adobe-workfront}

The highlighted information on this page refers to functionality available only in the new Workfront experience beta. 


You do not have to be an *`Adobe Workfront administrator`* to share permissions on objects that you have access to, but permissions on objects work within the access levels set by the *`Workfront administrator`*. 


For more information about access levels and permissions, see [How access levels and permissions work together](how-access-levels-permissions-work-together.md). 


You can share or remove permissions to an object you created or an object that was shared with you. When you are not the creator of the object, you must have Share access on the object that you want to share in your access level in addition to Share permissions on the object. For information about access levels, see [Access levels overview](access-levels-overview.md). 


>[!NOTE]
>
>A *`Workfront administrator`* can add or remove permissions to any items in the system, for all users, without being the owner of those items.




## Objects that you can share in *`Workfront`* {#objects-that-you-can-share-in-workfront}

You can share the following objects in  *`Workfront`* with other users:



* `Projects`: For more information, see [Share a project in Adobe Workfront](share-a-project.md).

* `Templates`: For more information, see [Share project templates](share-project-template.md).

* `Portfolios`: For more information, see [Share a portfolio in Adobe Workfront](share-a-portfolio..md).

* `Programs`: For information, see [Share a program in Adobe Workfront](share-a-program.md) .

* `Tasks`: For information, see [Share a task in Adobe Workfront](share-a-task.md).

* `Issues`: For information, see [Share an issue in Adobe Workfront](share-an-issue.md).

* `Documents`: For information, see [Share a document in Adobe Workfront](document-permissions.md).

* **Folders**: For information, see [Share a document folder](share-a-document-folder.md).

* **Proofs**: For information, see [Share a Proof in Workfront Proof](share-proof.md). 

* `Reports, dashboards, and calendars`: For information, see [Share reports, dashboards, and calendars in Adobe Workfront](permissions-reports-dashboards-calendars.md).&nbsp;Additionally, see the following articles:
    
    
    * [Share a report in Adobe Workfront](share-report.md)
    * [Share a dashboard in Adobe Workfront](share-dashboard.md)
    * [Share a calendar report](share-a-calendar-report.md)
    
    

* **Filters, views, and groupings**: For information, see [Share a filter, view, or grouping in Adobe Workfront](share-filter-view-grouping.md). 

*  ` `Plans`: For information, see [Share a plan in the Adobe Workfront Scenario Planner](share-a-plan.md).` 


  `This requires an additional license.` 

*  **Goals**: For information, see [Share a goal in Adobe Workfront Goals](share-a-goal.md). 


  This requires an additional license.





## Considerations about sharing objects {#considerations-about-sharing-objects}




*   You can share only the same level or a lower level of permissions you have on the object.


  For example, if you have Contribute permissions on the object, you cannot grant another user Manage permissions on that object.

*  You cannot share an object with a permission level higher than the access level of a user.&nbsp;For example, if a user has View access to Projects in their access level, you cannot give them Manage permissions on a project. 
*  A user with permissions to at least View an object can share that object with someone else.
*  You can share objects with active users, job roles, teams, groups, or companies.


  >[!NOTE]
  >
  >`You can share a plan or a goal only with other active users` `.` `This requires additional licenses.`
  >
  >
  >`For more information see:` 
  >
  >    
  >    
  >    *  [Share a plan in the Adobe Workfront Scenario Planner](share-a-plan.md) 
  >    *  [Share a goal in Adobe Workfront Goals](share-a-goal.md) 
  >    
  >    








## Share limitations {#share-limitations}


You can share an object with up to 100 entities (users, teams, groups, job roles, companies). We recommend that you share objects with groups, teams, or companies rather than with individual users, to avoid this limitation.&nbsp;


## Share permissions for objects {#share-permissions-for-objects}


The following table illustrates the permission settings you can select from when sharing an object. Not all objects have all these settings available. You can grant another entity permissions to View or Manage an object. If you are sharing a project, task, or issue, you can also grant permissions to Contribute to it.

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">View</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>You can perform the following actions on the object:</p> 
    <ul> 
     <li>View the object</li> 
     <li>Add documents to the object</li> 
     <li>View Finance information about the object</li> 
     <li> <p>Share the object<br></p> <p>When you share the object, you can grant other users the same permission level you have only on the object, not a higher level.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Contribute</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>You can perform the following actions on the object:</p> 
    <ul> 
     <li>View it</li> 
     <li>All the actions included with the View permission.</li> 
     <li>Add Expenses to it</li> 
     <li>Add issues to it (if it is a task or a project)</li> 
     <li>Add tasks to it (if it is a project)</li> 
     <li>Edit Custom Forms on it</li> 
     <li>Log Hours on the object</li> 
     <li>Make assignments in it</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Manage</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>You can perform the following actions on the object:</p> 
    <ul> 
     <li>View it</li> 
     <li>All the actions included with the View and Contribute permissions</li> 
     <li>Delete it</li> 
     <li>Manage Finance information in it</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Make this public to external users</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Anyone without a <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> account can view the object by clicking a link to it. This is not available for all objects.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Make this visible system-wide</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>The object can be found in searches and viewed by anyone with a <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> account.</p> </td> 
  </tr> 
 </tbody> 
</table>



##  



## Understand inherited permissions and the hierarchy of objects {#understand-inherited-permissions-and-the-hierarchy-of-objects}




* [Permissions inherited from parent objects](#inherited-permissions-from-higher-ranking-objects) 
* [Permissions acquired through organizational memberships](#permissions-acquired-via-memberships)&nbsp;




### Permissions inherited from parent objects {#permissions-inherited-from-parent-objects}

Permissions in *`Workfront`* are inherited hierarchically. This means that if you are granting permissions to a user on a parent object, they gain the same permissions on the children objects associated with it by default.


For example, if you give a user Contribute permissions to a project, the user has Contribute permissions to all tasks and issues (child objects) associated with that project.


Continuing with the example above, you cannot restrict permissions to child objects. If you do not want the user to have Contribute permissions to child objects associated with the project, you must manually remove the Inherited Permissions from the objects and then adjust the permissions for the individual user, including any Advanced Settings.&nbsp;


For more information about the hierarchy and interdependency of objects in *`Workfront`*, see the section [Interdependency and hierarchy of objects](understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) in the article [Understand objects in Adobe Workfront](understand-objects.md).


>[!NOTE]
>
>Your *`Workfront administrator`* can disable inherited permissions for documents in your access level.&nbsp;For more information about disabling inherited permissions for documents in the access level, see [Create or modify custom access levels](create-modify-access-levels.md).




### Permissions acquired through organizational memberships&nbsp; {#permissions-acquired-through-organizational-memberships}

If you grant Manage permissions to a Group of users on an object, and you grant View permissions to an individual user in that Group on the same object, the user has the highest level of permissions (Manage) granted through the Group membership on the object.&nbsp;


If you want to grant lower permissions to a user who is already part of an organizational unit (Group, Team, Job Role, or Company) with a higher permission level, you must remove the permissions from the organizational unit, and add users individually with a lower level of permissions.&nbsp;&nbsp;


## Share an object {#share-an-object}

For information about how to share objects, see [Share an object in Adobe Workfront](share-an-object.md). 


## Remove permissions from objects {#remove-permissions-from-objects}

For information about how to remove permissions from objects, see [Remove permissions from objects in Adobe Workfront](remove-permissions-from-objects.md). 


## Request permissions to objects {#request-permissions-to-objects}

When someone sends you a link to an object which you do not have permissions to View, or when you have lower permissions on an object and you want to request a higher level of permissions, you can request permissions on the object.&nbsp;


You can request access to an object from anyone who has Share permission to the object.&nbsp;


For more information about requesting permissions to objects, see [Request access to objects in Adobe Workfront](request-access.md).
