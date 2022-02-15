---
filename: business-case-finances
content-type: overview
navigation-topic: business-case-and-scorecards
---



# Overview of Business Case financial fields  {#overview-of-business-case-financial-fields}

The Business Case sub-tab includes financial fields for the project.&nbsp;In order for some of the financial fields to have values, corresponding areas of the Business Case must be completed.&nbsp;&nbsp;


The following project financial fields display in the Business Case:

<table style="width: 649px;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');" border="1" cellspacing="15" cellpadding="1" class="TableStyle-TableStyle-HeaderRow"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 182px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th style="background-color: #d3d3d3;" scope="col" class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Name of Field</th> 
   <th style="background-color: #d3d3d3; width: 498px;" scope="col" class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Aligned&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Displays the alignment of the project according to its scorecard. A high percentage value indicates that the project is well-aligned with the purpose and goals of the organization. <br>For more information about using scorecards, see <a href="create-scorecard.md" class="MCXref xref">Create a scorecard </a>.</p> <p>This field displays in the Business Case Summary area.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Budgeted Cost</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The total cost estimated to be associated with the project when the project launches.</p> <p>The Budgeted Cost for the project is calculated by the following formula:<br></p> <p><code>Budgeted Cost =&nbsp;Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> uses the Budgeted Hours from the&nbsp;<span class="mc-variable WFVariables.Resource_Planner_tool variable varname">Resource Planner</span> to calculate the Budgeted Labor Cost.<br>For more information about calculating Budgeted Cost, see <a href="budgeted-cost.md" class="MCXref xref">Calculate Budgeted Cost</a>.&nbsp;</p> <p>This field displays in the Business Case Summary area.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Budgeted Expense Cost</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The budgeted cost of all the expenses on the project.&nbsp;</p> <p>This is calculated by the following formula:</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code><![CDATA[                        ]]></p> <p>For more information about calculating expenses, see <a href="manage-project-expenses.md" class="MCXref xref">Manage project expenses </a>.</p> <p>This field displays in the Expenses&nbsp;area.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Budgeted Labor Cost</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The cost associated with the resources assigned to complete the work on the project.</p> <p>The Budgeted Labor Cost for the project is calculated by the following formula:<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code><![CDATA[                            ]]><br></p> <p><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> uses the Budgeted Hours from the&nbsp;<span class="mc-variable WFVariables.Resource_Planner_tool variable varname">Resource Planner</span> to calculate the Budgeted Labor Cost.<br>For more information about calculating Budgeted Labor Cost, see <a href="budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>.</p> <p>This field displays in the Resource Budgeting area of the Business Case.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Expenses Planned Cost</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>This is the same as Budgeted Expense Cost.&nbsp;</p> <p>Note:  The Expenses Planned Cost is different than the Planned Cost for the Project. The Expenses Planned Cost is calculated the Planned Amount of the expenses on the project, whereas the Planned Cost is calculated using the Planned Hours on the project.&nbsp;</p> <p>This field displays in the Expenses&nbsp;area, for each expense.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Net Value</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This is the total expected value of the project after calculating its benefit and removing the costs.</p> <p>The Net Value for the project is calculated by the following formula:<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>. <br></p> <p>For more information about calculating Net Value, see <a href="calculate-net-value.md" class="MCXref xref">Calculate Net Value</a>.<br></p> <p>This field displays in the Business Case Summary area.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Planned Benefit</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">A manual estimate of the monetary benefit for your organization when this project is completed. It can be any amount of currency and it is specific to you and to each project you manage. The Planned Benefit cannot have a negative value. This field displays in the Business Case Summary area and it can be edited in the Project Info area of the Business Case. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Potential&nbsp;Cost of Risks</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>This is the Potential Cost of all the risks on the project. </p> <p>This is calculated using the following formula:</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code><![CDATA[                        ]]></p> <p>For more information about risks on the project, see&nbsp;<a href="create-edit-risks-on-projects.md" class="MCXref xref">Create and edit risks on projects</a>.</p> <p>This field displays in the Business Case Summary area.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Potential Risk</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>In the Business Case Summary, this is the amount of the cost of the all the risks if they should occur, based on their probability. For example, if a Risk has a Potential Cost of $100 and a Probability of occurring of 10%, the Potential&nbsp;Risk is $10. The Potential Risk in the Business Case Summary is calculated by the following formula:</p> <p><code>Potential&nbsp;Risk = SUM(Risk Potential Cost x Probability)</code> for all risks. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Risk Mitigation Cost</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The&nbsp;cost of the mitigation plan for the risks you are estimating might occur on the project.<br>For more information about risks on the project, see <a href="create-edit-risks-on-projects.md" class="MCXref xref">Create and edit risks on projects</a>.</p> <p>This field displays in the&nbsp;Risks area for each risk specified on the project.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Potential Cost for one Risk</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The estimated financial cost when the risks defined on the project would actually occur, regardless of their probability.&nbsp;</p> <p>This is a manually updated field which displays on each risk in the Risks area of the Business Case.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">Risks Total Potential Cost</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>This is the total estimated financial cost of all the risks defined on the project when they actually have occurred.&nbsp;</p> <p>This is calculated by the following formula:</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code><![CDATA[                        ]]></p> <p>It displays as a currency number next to the title of the Risks area of the Business Case.</p> </td> 
  </tr> 
 </tbody> 
</table>

