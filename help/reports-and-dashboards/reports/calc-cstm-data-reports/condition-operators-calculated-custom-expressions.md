---
filename: condition-operators-calculated-custom-expressions
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
---



# Condition operators in calculated custom expressions {#condition-operators-in-calculated-custom-expressions}

You can use condition operators or modifiers when building calculated custom data in *`Adobe Workfront`* when using text mode.


For information about using text mode in  *`Workfront`*, see [Text Mode overview](understand-text-mode.md). 


Condition operators or modifiers help build a condition statement by connecting existing *`Workfront`* fields in statements and generating a new field. The most common use of condition operators is to build the condition of an "IF" statement. 


You can use "IF" statements in *`Workfront`* to compare, format, and string together fields of data for both reporting and custom data purposes. 


You can build "IF" statements for the following *`Workfront`* elements: 



* Views
* Groupings
* Calculated custom fields


For more information about building "IF" statements, see ["IF" statements overview](if-statements-overview.md).


The examples in this guide illustrate the use of condition operators in calculated custom fields. You can also use them in calculated custom columns or groupings as well, when following the correct syntax for calculated custom fields in reports. 


For information about the difference in syntax between the calculated custom fields and calculated custom data in reports, see [Calculated custom fields vs. calculated columns](calculated-custom-fields-calculated-columns.md).


Refer to the API Explorer to find the fields you want to reference in your calculated custom expressions. For information about the API Explorer, see [API Explorer](api-explorer.md).


You can use the following condition modifiers in *`Workfront`*:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Condition modifier</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Condition modifier syntax</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Condition modifier definition</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Equal</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">= </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Use this modifier to indicate that the condition is fulfilled when the first field of your statement is equal to the second field.</p> <p>For example, use the following statement in a calculated custom field to build an "IF" statement that compares the Planned Completion Date to the Projected Completion Date of a task: </p><pre>IF(Projected Completion Date=Planned Completion Date,"On Track","Off Track")</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Greater than </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&gt; </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Use this modifier to indicate that the condition is fulfilled when the first field of your statement is greater than the second field. <p>For example, use the following statement in a calculated custom field to build an "IF" statement that compares the Planned Completion Date to the Projected Completion Date of a task: </p><pre>IF(Projected Completion Date&gt;Planned Completion Date,"Late","")</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Greater than or equal to </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&gt;= </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Use this modifier to indicate that the condition is fulfilled when the first field of your statement is either greater than or equal to the second field. <p>For example, use the following statement in a calculated custom field to build an "IF" statement that compares the Planned Completion Date to the Projected Completion Date of a task: </p><pre>IF(Projected Completion Date&gt;=Planned Completion Date,"Late","Early")</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Lesser than </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&lt; </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Use this modifier to indicate that the condition is fulfilled when&nbsp; the first field of your statement is lesser than the second field. <p>For example, use the following statement in a calculated custom field to build an "IF" statement that compares the Planned Completion Date to the Projected Completion Date of a task: </p><pre>IF(Projected Completion Date&lt;Planned Completion Date,"Early","")</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Lesser than or equal to </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&lt;= </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Use this modifier to indicate that the condition is fulfilled when&nbsp; the first field of your statement is lesser than or equal to the second field. <p>For example, use the following statement in a calculated custom field to build an "IF" statement that compares the Planned Completion Date to the Projected Completion Date of a task: </p><pre>IF(Projected Completion Date&lt;=Planned Completion Date,"Early","Late")</pre></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Does not </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">! </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Add this operator in front of any of the above operators to negate the operator. </p> <p>For example: </p> 
    <ul> 
     <li>Equals: = </li> 
     <li>Does not equal: != </li> 
    </ul> <p>Adding this operator in front of the following data expressions adds a negative statement to expressions: </p> 
    <ul> 
     <li>CONTAINS </li> 
     <li>IN </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>For information about these data expressions and for a complete list, see <a href="calculated-data-expressions.md" class="MCXref xref">Calculated data expressions</a>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Or </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">|| </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Use this modifier to indicate that the condition is fulfilled when the expression&nbsp; finds either the first or the second value of your statement. </p> <p>For example, use the following statement in a calculated custom field to build an "IF" statement that marks projects in either the Current or Planning statuses as "Active": </p><pre>IF(Status="PLN"||Status="CUR","Active","Not Active")</pre> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">&nbsp;And </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">&amp;&amp; </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Use this modifier to indicate that the condition is fulfilled when the expression&nbsp; finds an item that fulfills two conditions at the same time. </p> <p>For example, use the following statement in a calculated custom field to build an "IF" statement that finds projects that are in Current status and have a Condition of At Risk and marks them as "Mediation Needed." </p><pre>IF(Status="CUR"&amp;&amp;Condition="AR","Mediation Needed","")</pre> </td> 
  </tr> 
 </tbody> 
</table>

