---
filename: create-an-agile-team
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
---



# Create an agile team {#create-an-agile-team}

*`Adobe Workfront`* enables agile teams to complete work in an incremental, organized way.


Any user in the organization can see the agile team and view all agile components for the team, including the backlog, iterations, story board, and individual stories. However, only members of the team with Edit access to work can make changes to work assigned to the team.


*`Workfront`* supports the following agile methodologies:



* `Scrum`: Teams have a backlog of work that needs to be done. When the team is ready to work on a specific chunk of work, the work is moved from the backlog to an iteration. For more detailed information about managing a Scrum team, see [Scrum in an agile team](_scrum-in-an-agile-team.md).

* `Kanban:` Teams move work in&nbsp;the Kanban view across predetermined&nbsp;statuses. Default statuses are: backlog, in-process, and done. For more detailed information about managing a Kanban&nbsp;team, see [Kanban in an agile team](_using-kanban-in-an-agile-team.md).





## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 </col> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 </col> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> to create a new agile team; <span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> or higher to convert a team to an agile team</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan or license type you have, contact your *`Workfront administrator`*.


## Decide on an agile methodology {#decide-on-an-agile-methodology}

You can use either a Scrum or Kanban agile methodology for your agile team. Each methodology provides various benefits. The way your agile team works determines the agile methodology you choose to use.


Both Scrum and Kanban agile methodologies in *`Workfront`* allow you to move stories across a story board to indicate a status change and progress of the story.


Scrum and Kanban agile methodologies in *`Workfront`* differ in the following ways:


### Benefits of using Kanban in *`Workfront`* {#benefits-of-using-kanban-in-workfront}

The Kanban agile methodology in *`Workfront`* enables you to more easily move stories across an agile story board while limiting the amount of work in progress. There are no start and end dates when using the Kanban agile methodology.


The following functionality supports this methodology:



* Display the backlog on the Kanban agile story board.  
  For more information, see [Add the backlog to the Kanban board](view-the-backlog-on-the-kanban-board.md).

* Configure items on the backlog to be automatically added to the Kanban agile story board when other items are moved to a status that equates with Complete.  
  For more information, see the section [Configure stories to be automatically added from the backlog](configure-kanban.md#configur5) in the article [Configure Kanban](configure-kanban.md).

* Configure a Work In Progress (WIP) limit to be displayed on the Kanban agile story board.  
  For more information, see [Manage the work in progress (WIP) limit on the Kanban board](work-in-progress-limit-on-the-kanban-board.md).





### Benefits of using Scrum in *`Workfront`* {#benefits-of-using-scrum-in-workfront}

The Scrum agile methodology in *`Workfront`* enables you to add a set of stories to an agile iteration and create a story board for that iteration. The iteration is based on the start and end dates that you define.


The following functionality supports this methodology:



* Include issues on the Scrum story board
* Include issues on the backlog&nbsp;of an agile team
* Subtasks can be displayed on the Scrum story board
* View a burndown chart to see progress against stories during the iteration  
  For more information, see [Agile burndown chart overview](burndown-chart-overview.md).





## Create a new agile team {#create-a-new-agile-team}




1.  Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*.
1.  Click the `Switch Teams` icon ![Switch team icon](assets/switch-team-icon.png), then click `Create New Team`.


   ![Select Create new team.](assets/create-new-team-350x198.png)



1.  Specify the following information on the New Team dialog:

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Team Name</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Type a name for the new agile team.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">This is an Agile Team</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Select this option to configure this new team to be an agile team.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Group</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Begin typing the name of a group to add to the team, then select the name when it appears in the drop-down list.</p> <p>Note: When a team is assigned to a group or subgroup, any <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> of that group or subgroup can manage the team without being a member of it. <span class="mc-variable WFVariables.AdminGroupInitCapPlur variable varname">Group administrators</span> can go to the Teams area from the Main Menu and click the Switch Teams arrow <img src="assets/switch-team-icon.png" alt="Switch team icon"> to list all of the teams that are assigned to the groups that they manage.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Team Members</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Begin typing the name of a user to be on the team, then select the name when it appears in the drop-down list.<br>Repeat this process to add multiple users to the team.<br>Because users can be on more than one team, they can be on both agile and non-agile teams.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"><span class="bold">Description</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Type a description for the team.</td> 
  </tr> 
 </tbody> 
</table>


1.  Click `Create`.


   For information on configuring an Agile team, see the following articles:

    
    
    * [Configure Kanban](configure-kanban.md) 
    * [Configure Scrum](configure-scrum.md) 
    
    





## Convert an existing team into an agile team {#convert-an-existing-team-into-an-agile-team}

You can&nbsp;convert an existing team to be&nbsp;an agile team:



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*.

1. Click the `Switch team` icon ![Switch team icon](assets/switch-team-icon.png), then either select a new team from the drop-down menu or search for a team in the search bar.

1. Select the team that you want to convert to an agile team.
1. Click the `More` menu, then select `Edit`.  
   Only team members with either a Plan or Work license see this option.  
   ![](assets/edit-team-settings-350x205.png)


1. In the `Agile` section, select  `This is an Agile Team`.

1. In the `Methodology` section, select whether the team will be using a  `Scrum` or  `Kanban`&nbsp;agile methodology.  

1.  Click  `Save Changes.`


   For information on configuring an Agile team, see the following articles:

    
    
    * [Configure Kanban](configure-kanban.md) 
    * [Configure Scrum](configure-scrum.md) 
    
    



