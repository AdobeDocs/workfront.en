---
filename: filter-same-name-statuses-from-different-groups
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
---



# Filter: display items by same-name statuses when the statuses are associated with different groups {#filter-display-items-by-same-name-statuses-when-the-statuses-are-associated-with-different-groups}

You can have a task status assigned to Group A named *New Status* with the 3-letter key *NST*. You may have another task status assigned to Group B also named *New Status* with the 3-letter key *NES.* Although the names for the 2 statuses can be identical, the 3-letter code is always unique.  
For more information about group statuses, see [Create or edit a group status](create-or-edit-a-group-status.md).


Using the filter builder, you cannot identify between the 2 statuses that have the same name. You must use Text&nbsp;Mode to distinguish between the 2 statuses.



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


## Display items by same-name statuses when the statuses are associated with different groups  
{#display-items-by-same-name-statuses-when-the-statuses-are-associated-with-different-groups}




1. Go to the filter you want to customize for a list of tasks, for example.  
   This works the same for projects and issues as well.
1.  Click `Add a Filter Rule` for the `Status` field of the object of your list.  
   For example, in a task report, add `Status Equal *New Status*`, if you want to display only tasks which are in a status of `New Status`.


   >[!TIP] {type="tip"}
   >
   >Notice that you have only one option for a status named New Status.



1. Click `Switch to Text Mode`.  
   The following code should display:  
   `<pre xml:space="preserve">status=NST<br>status_Mod=in </pre>`

   >[!NOTE]
   >
   >Only one status displays here. The status line displays one of the 3-letter keys for one of the statuses.



1. Add the following 2 lines of code to add the status that is missing from the filter:  
   `<pre>OR:1:status=NES<br>OR:1:status_Mod=in</pre>`

1.  Click  `Done`, then `Save Filter`.


   The list displays both tasks with a status of "New Status" from Group A and with a status of "New Status"&nbsp;from Group B.



