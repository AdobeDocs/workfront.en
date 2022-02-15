---
filename: filter-parent-task-filter
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
---



# Filter: parent task filters {#filter-parent-task-filters}

You can apply the task filters below to display working tasks. Working tasks are tasks that can be worked independently and are not parent tasks to other tasks. In one example, a filter identifies children tasks that could be parents themselves. In this case, they are not working tasks.

` `**Tip: **`` 


*   If you consider adding more than one filter to a report, we recommend that you add all your filters using the report builder interface, and clicking Switch to Text Mode after all the other filter rules have been added. Then, you can add the code for the parent task filter as noted above.&nbsp;
*  We also recommend that you add a grouping for Project Name to make the report easier to read. For more information about adding groupings to your reports, see the article [Groupings overview in Adobe Workfront](groupings-overview.md). 





## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters, Views, Groupings</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


##  



## Display tasks with no children (they could have a parent) {#display-tasks-with-no-children-they-could-have-a-parent}

You can apply the following filter to a task report to display tasks with no children.&nbsp;They could have parents of their own and be children of other tasks. 



1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> From the  <span class="bold">Main Menu</span>  <img src="assets/main-menu-icon.png">, click  <span class="bold">Reports.</span></MadCap:conditionalText>` 
1. Click `New Report`.
1. Select a `Task Report`.
1. Click `Filters`.
1. Click `Add a Filter Rule`.
1. In the `Start typing field name ...` line, start typing `Number of Children`.

1.  Select `Equal (Case Sensitive)` for your modifier, then enter `0` for the number of children.  
   ![](assets/parent-task-filter-from-the-ui-350x76.png)




   Or


   Click  `Switch to Text Mode`, and in the&nbsp;text editing window, copy and paste the following text:&nbsp;




   ```
   numberOfChildren=0<br>numberOfChildren_Mod=eq
   ```



1.  Click `Save + Close`.


   This pulls a report for all tasks which are working tasks in your system. Some of these tasks could have a parent, but they are not parent tasks themselves. 





## Display tasks with parents (they could have children)  {#display-tasks-with-parents-they-could-have-children}

You can apply the following filter to a task report to display tasks with parents, meaning they are children tasks. However, these tasks could also have children of their own because the filter does not exclude their children. Children tasks that are also parents for other tasks are not considered working tasks. 



1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> From the  <span class="bold">Main Menu</span>  <img src="assets/main-menu-icon.png">, click  <span class="bold">Reports.</span></MadCap:conditionalText>` `<li>Click <span class="bold">New Report</span>.</li>` `<li>Select a <span class="bold">Task Report</span>.</li>` `<li>Click <span class="bold">Filters</span>.</li>` `<li>Click <span class="bold">Add a Filter Rule</span>.</li>` `<li>In the <span class="bold">Start typing field name ...</span> line, start typing <span class="bold">Parent ID</span>.</li>` `<li> <p>Select <span class="bold">Is Not Blank</span> for your modifier.</p> <p> <img src="assets/filter-parent-id-not-blank-350x100.png" style="width: 350;height: 100;"> <br> </p> <p>Or</p> <p>Click&nbsp;<span class="bold">Switch to Text Mode</span>, and in the&nbsp;text editing window, copy and paste the following text:&nbsp;</p> <p><code>parentID_Mod=notblank</code> </p> </li>` `<li> <p>Click <span class="bold">Save + Close</span>.</p> <p>This pulls a report for all tasks in your system that have parents and are children tasks of those parents. Some of these tasks could be a parent themselves. </p> </li>` 





## Display tasks with no children and no parents (standalone tasks)  {#display-tasks-with-no-children-and-no-parents-standalone-tasks}

You can apply the following filter to a task report to display standalone working tasks.&nbsp;These tasks don't have a parent and they have no children of their own. 



1.   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> From the  <span class="bold">Main Menu</span>  <img src="assets/main-menu-icon.png">, click  <span class="bold">Reports.</span></MadCap:conditionalText>` 
1.  Click `New Report`.
1.  Select a `Task Report`.
1.  Click `Filters`.
1.  Click `Add a Filter Rule` and in the `Start typing field name ...` line start typing `Number of Children` select `Equal (Case Sensitive)` for your modifier, then enter `0` for the number of children.
1.  Click `Add another Filter Rule` and in the `Start typing field name ...` line start typing `Parent ID`, then select `Is Blank`. 


   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)




   Or 


   Instead of steps 6-7, click  `Switch to Text Mode` and in the&nbsp;text editing window, copy and paste the following text:&nbsp;
   `<pre>numberOfChildren=0</pre>``<pre>numberOfChildren_Mod=eq</pre>``<pre>parentID_Mod=isblank</pre>` 

1.  Click `Save + Close`.


   This pulls a report for all tasks in your system that have no parents nor children. These are standalone working tasks. 



