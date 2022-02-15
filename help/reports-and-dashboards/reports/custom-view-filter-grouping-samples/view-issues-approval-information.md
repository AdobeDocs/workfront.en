---
filename: view-issues-approval-information
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
---



# View: issues with approval information {#view-issues-with-approval-information}

The following issue view shows the approval process, step, names of the approvers, and the status of the issue before the approval was granted. Some of these fields are not accessible through the standard interface builder.


![custom_issue_view_with_approval_info.png](assets/custom-issue-view-with-approval-info-350x46.png)





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


## View issues with approval information {#view-issues-with-approval-information-1}




1. Go to a list of issues.
1. From the `View` drop-down menu, select `New View`.

1. In the `Column Preview` area, eliminate all columns except for one.
1. Click the header of the remaining column, then click `Switch to Text Mode`.
1. Mouse over the text mode area, and click `Click to edit text`.
1. Remove the text you find in the `Text Mode` box, and replace it with the following code:  
   `<pre style="font-style: normal;"><em>column.0.descriptionkey=name</em><br><em>column.0.link.linkproperty.0.name=ID</em><br><em>column.0.link.linkproperty.0.valuefield=ID</em><br><em>column.0.link.linkproperty.0.valueformat=int</em><br><em>column.0.link.lookup=link.view</em><br><em>column.0.link.valuefield=objCode</em><br><em>column.0.link.valueformat=val</em><br><em>column.0.linkedname=direct</em><br><em>column.0.listsort=string(name)</em><br><em>column.0.namekey=name.abbr</em><br><em>column.0.querysort=name</em><br><em>column.0.shortview=false</em><br><em>column.0.stretch=40</em><br><em>column.0.valuefield=name</em><br><em>column.0.valueformat=HTML</em><br><em>column.0.width=220</em><br><em>column.1.descriptionkey=assignedto</em><br><em>column.1.linkedname=assignedTo</em><br><em>column.1.listsort=nested(assignedTo).string(name)</em><br><em>column.1.namekey=assignedto</em><br><em>column.1.querysort=assignedTo:name</em><br><em>column.1.shortview=true</em><br><em>column.1.stretch=0</em><br><em>column.1.valuefield=assignedTo:name</em><br><em>column.1.valueformat=HTML</em><br><em>column.1.width=150</em><br><em>column.2.descriptionkey=role</em><br><em>column.2.linkedname=role</em><br><em>column.2.listsort=nested(role).string(name)</em><br><em>column.2.namekey=role</em><br><em>column.2.querysort=role:name</em><br><em>column.2.shortview=false</em><br><em>column.2.stretch=25</em><br><em>column.2.valuefield=role:name</em><br><em>column.2.valueformat=HTML</em><br><em>column.2.width=150</em><br><em>column.3.description=Approval Process Name</em><br><em>column.3.linkedname=direct</em><br><em>column.3.listsort=string(name)</em><br><em>column.3.name=Approval Process Name</em><br><em>column.3.querysort=name</em><br><em>column.3.shortview=false</em><br><em>column.3.stretch=35</em><br><em>column.3.valuefield=approvalProcess:name</em><br><em>column.3.valueformat=HTML</em><br><em>column.3.width=220</em><br><em>column.4.description=Approval Step Name</em><br><em>column.4.linkedname=direct</em><br><em>column.4.listsort=string(name)</em><br><em>column.4.name=Approval Step Name</em><br><em>column.4.querysort=name</em><br><em>column.4.shortview=false</em><br><em>column.4.stretch=0</em><br><em>column.4.valuefield=currentApprovalStep:name</em><br><em>column.4.valueformat=HTML</em><br><em>column.4.width=220</em><br>column.5.description=Previous Status<br><em>column.5.linkedname=direct</em><br><em>column.5.listsort=string(name)</em><br><em>column.5.name=Previous Status</em><br><em>column.5.querysort=name</em><br><em>column.5.shortview=false</em><br><em>column.5.stretch=0</em><br><em>column.5.valuefield=previousStatus</em><br><em>column.5.valueformat=HTML</em><br><em>column.5.width=220</em><br><em>column.6.linkedname=direct</em><br><em>column.6.listsort=HTML(approversString)</em><br><em>column.6.namekey=approver.plural.abbr</em><br><em>column.6.querysort=approversString</em><br><em>column.6.shortview=false</em><br><em>column.6.stretch=0</em><br><em>column.6.valuefield=approversString</em><br><em>column.6.valueformat=HTML</em><br><em>column.6.viewalias=approver.plural</em><br><em>column.6.width=200</em><br></pre>`

1. Click `Save View`.


