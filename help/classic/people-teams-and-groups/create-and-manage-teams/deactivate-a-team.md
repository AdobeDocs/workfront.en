---
filename: deactivate-a-team
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Deactivate a team
description: You can deactivate teams you no longer use while retaining the associated historical data. Adobe Workfront administrators can reactivate a team at any time from the Teams area in Setup. If you deactivate a team, the team no longer displays in the following areas - EDIT ME.
---

# Deactivate a team

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

You can deactivate teams you no longer use while retaining the associated historical data. Adobe Workfront administrators can reactivate a team at any time from the Teams area in Setup. If you deactivate a team, the team no longer displays in the following areas:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Typeahead fields in custom forms</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Sharing dialog for objects</p> </li> 
     <li> <p>User Profile*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Main selection drop-down menu in the Teams area</p> </li> 
     <li> <p>Assignments typeahead</p> </li> 
     <li> <p>Add to Kanban board dialog in a project</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Deactivated teams don't appear when you search for a team, but will still display in Home Team and Other Teams if the user was assigned to the team prior to deactivation.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan or license type you have, contact your Workfront administrator.

## Deactivate a team

Any work assigned to the team prior to deactivation remains assigned. We recommend reassigning work before you deactivate the team.

>[!TIP]
>
>You can create a report to filter for any tasks or issues where the deactivated team is still assigned.

When using request queues, if you deactivate a team assigned as the default team in a routing rule, the team remains and requests are still routed to the deactivated team. We recommend updating routing rules with active teams before you deactivate the team.

1. Click ```People``` in the Global Navigation Bar.
1. Click the ```Teams``` tab, then in the drop-down list,&nbsp;select the team that you want to edit.
1. Uncheck the ```Is Active``` box.
1. Click ```Save changes```.

## Known limitations

Deactivated teams display in the following areas:

* The Assignments field in Home

