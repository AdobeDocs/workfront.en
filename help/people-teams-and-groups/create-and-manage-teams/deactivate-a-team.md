---
filename: deactivate-a-team
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Deactivate a team
description: You can deactivate teams you no longer use while retaining the associated historical data. Adobe Workfront administrators can reactivate a team at any time from the Teams area in Setup. If you deactivate a team, the team no longer displays in the following areas:
---

# Deactivate a team

You can deactivate teams you no longer use while retaining the associated historical data. *Adobe Workfront administrators* can reactivate a team at any time from the Teams area in Setup. If you deactivate a team, the team no longer displays in the following areas:

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
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan or license type you have, contact your *Workfront administrator*.

## Deactivate a team

Any work assigned to the team prior to deactivation remains assigned. We recommend reassigning work before you deactivate the team.

>[!TIP]
>
>You can create a report to filter for any tasks or issues where the deactivated team is still assigned.

When using request queues, if you deactivate a team assigned as the default team in a routing rule, the team remains and requests are still routed to the deactivated team. We recommend updating routing rules with active teams before you deactivate the team.

<ol> <draft-comment>
  <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Teams</span>.</p> </li>
 </draft-comment>
 <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Teams</span>.</p> </li> <draft-comment>
  <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click the <span class="bold">Switch team</span> icon, then either select a new team from the drop-down menu or search for a team in the search bar.</p> </li>
 </draft-comment>
 <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click the <span class="bold">Switch team</span> icon, then either select a new team from the drop-down menu or search for a team in the search bar.</p> </li> <draft-comment>
  <li value="3" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click the <span class="bold">More</span> menu, then select <span class="bold">Edit</span>.</p> <p> <img src="assets/edit-team-settings-350x205.png" style="width: 350;height: 205;"> </p> </li>
 </draft-comment>
 <li value="3" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click the <span class="bold">More</span> menu, then select <span class="bold">Edit</span>.</p> <p> <img src="assets/edit-team-settings-350x205.png" style="width: 350;height: 205;"> </p> </li> 
 <li value="4">Uncheck the <span class="uitext">Is Active</span> box.</li> 
 <li value="5"> <p>Click <span class="uitext">Save changes</span>.</p> </li> 
</ol>

## Known limitations

Deactivated teams display in the following areas:

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>The Owner field in <em>Workfront Goals</em>. This requires an additional license for <em>Adobe Workfront Goals</em>. For more information, see <a href="../../workfront-goals/goal-management/getting-started-with-wf-goals.md" class="MCXref xref">Get started with Adobe Workfront Goals</a>.</p> </li>
  -->

* The Owner field in *Workfront Goals*. This requires an additional license for *Adobe Workfront Goals*. For more information, see [Get started with Adobe Workfront Goals](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).

