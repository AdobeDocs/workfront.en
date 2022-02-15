---
filename: manage-work-and-team-requests-home
product-area: projects;agile-and-teams
navigation-topic: use-the-home-area
---



# Manage work and team requests in the Home area {#manage-work-and-team-requests-in-the-home-area}

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.


When work tasks and issues&nbsp;are assigned to you, they are listed on the Work List in the Home area. You can view, reassign, reply to, work on, or remove a request. Work requests in the Home area are not limited to issues associated with request queues.


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Tasks and Issues</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Contribute permissions or higher to the tasks and issues you need to work on</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## View a work request {#view-a-work-request}

Work requests that are assigned to you are displayed in the left panel in Home. You can configure which requests are displayed in Home using the filter at the top of the Work List.



1.  Click the `Main Menu` ![](assets/main-menu-icon.png) in the upper-right corner, then click  `Home`. 
1.  Click the `Filter` drop-down menu.


   ![](assets/displaying-work-items-filter-350x348.png)



1.  Click either or both of the following options:


   `Ready to Start:` Only tasks and issues that are ready to start are displayed. Both of the following statements must be true:

    
    
    *  The tasks and their parents have no predecessors or task constraints preventing them from being worked on.
    *  The Planned Start Date of the tasks or issues is in the past or up to two weeks in the future.
    
    
   **Not Ready**: Only tasks and issues that are not yet ready to start are displayed. Either one of the following statements must be true:

    
    
    *  The tasks and their parents might have predecessors or task constraints that prevent them from being worked on.
    *  The tasks or issues have a Planned Start Date that is more than two weeks in the future.
    
    





## Access a team request {#access-a-team-request}

You can access a request assigned to your team directly from the Home area. For more information about team requests, see [Team requests overview](team-requests-overview.md).



1.  Click the `Main Menu` ![](assets/main-menu-icon.png) in the upper-right corner, then click  `Home`. 
1.  In the `Work List`area, go to the  `Team Requests`grouping.  
   If there are no requests assigned to your team, the grouping does not appear.  



   ![](assets/team-requests-expanded-home-group-by-drop-down-nwe-350x540.png)



1. Click the team name.  
   The `Team Requests` `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> section</MadCap:conditionalText>` displays and shows all requests assigned to your team. For more information about working with team requests, see [Manage work and team requests](manage-work-and-team-requests.md).





## Reassign a request {#reassign-a-request}




1.  Click the `Main Menu` ![](assets/main-menu-icon.png) in the upper-right corner, then click  `Home`. 
1. In the `Work List` area, select the request you want to reassign.  

1.  Click on the `Assignments` widget and remove yourself from the request, then type the name of the user you want to reassign the request to. 


   >[!TIP] {type="tip"}
   >
   >If the work request is still in the Ready to Start or Not Ready state, you can use the `Reassign` button in the `More` menu in the Work List.  
   >![Reassign button](assets/reassign-in-left-panel-350x204.png)  




1. If a task's status is changed to New or In Progress after it was completed, you must reassign a user in order for the task to reappear in the Home Work List.




## Reply to a request {#reply-to-a-request}

You can reply to a request to further clarify the request or to propose a new date.



1.  Click the `Main Menu` ![](assets/main-menu-icon.png) in the upper-right corner, then click  `Home`. 
1. In the `Work List` area, select the request you want to reply to.
1.  Locate the individual who assigned the request to you.


   You can find this information on the Updates tab of the task. Make sure the option to `Show System Updates` is enabled.

1. Click `Start new update` and begin typing your reply.
1.  Enter the name of the recipient in the `Notify` box, then click `Update`.


   >[!TIP] {type="tip"}
   >
   >If the work request is still in the Ready to Start or Not Ready state, you can use the `Reply` button in the `More` menu in the Work List.  
   >![Reply button](assets/reassign-in-left-panel-350x204.png)   >
   >








## Work on a request {#work-on-a-request}

When you click the Work On It button, you are indicating to the user who submitted the request and to any other user who might be assigned to the request that you are going to start working on the request. For more information about working on requests, see&nbsp; [Manage work and team requests](manage-work-and-team-requests.md).



1.  Click the `Main Menu` ![](assets/main-menu-icon.png) in the upper-right corner, then click  `Home`. 
1. In the `Work List` area, select the request you want to work on, then click `Work On It`.  
   Information about the issue is displayed in the right panel.





## Remove a request {#remove-a-request}

If you decide that you should not be working on the request, you can either convert the task or issue back to a request or remove it from your list.



1.  Click the `Main Menu` ![](assets/main-menu-icon.png) in the upper-right corner, then click  `Home`. 
1. In the `Work List`, point to the item waiting to be worked on.
1. Click the Assignments widget and remove yourself. This removes the work item from your Work List. If the request is not assigned to anyone else or to another team or job role, the request is&nbsp;left unassigned.


