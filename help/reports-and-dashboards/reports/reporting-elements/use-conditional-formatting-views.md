---
filename: use-conditional-formatting-views
product-area: reporting
navigation-topic: reporting-elements
---



# Use conditional formatting in Views {#use-conditional-formatting-in-views}

As you share your reports with other users in  *`Adobe Workfront`*, consider customizing the View of the reports, to make certain information easier to read, or just stand out.


You can customize the Details tab of your reports by adding special or conditional formatting to the view of your reports.


You must have Manage permissions to the report, to be able to edit it and add special formatting to the View.


For more information about creating reports, see the article [Create a custom report](create-custom-report.md).


By conditionally formatting columns in the View of the report, you can set up rules that affect the way the report is displayed. When those conditions or rules are met, the special formatting is applied.


For example, if the percent complete of a task&nbsp;is less than 20 percent, you can highlight the field by showing the percentage number in bold, red text, and a yellow background color.


With a conditionally formatted View,&nbsp;you can:



* Change the header of a column.
* You can change the value of a column to customized text or an image.
* Format the display of a field by changing the font type, color, alignment, or the color of the background.


The changes you make in the View of the report take effect only in the Details tab of the report. These changes do not affect the Summary, Matrix, or Chart tabs of the report.



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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Filters, Views, Groupings</p> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars to edit a view in a report</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions to a report to create or edit a view in a report</p> <p>Manage permissions to a view</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

You must create a report before you can add conditional formatting to it.


For information on creating a report, see [Create a report](create-report.md).


## Create a conditionally formatted View {#create-a-conditionally-formatted-view}




1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>,then click&nbsp; <span class="bold">Reports</span>.</MadCap:conditionalText>` 
1.  Click the name of a report where you want to create a conditionally-formatted view.


   Or


   Click  `Report Actions`, then click  `Edit`.

1. (Conditional) If you edited a report, select an existing column, or create a new column.  
1. Click `Advanced Options`.  

1.  Specify the following information:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Custom Column Label</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Specify a name for the column.</p> <p>If you are editing an existing column, specifying a name here changes the existing column name.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Field Format</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Choose&nbsp;the format in which the value in the column displays. Depending on what the column field is, this allows you to set how dates, numbers, or currency display.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Show this column when on a Dashboard</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Select this field if you want the column to display when the report is placed on a dashboard. The column always displays when you look at the report outside a dashboard.</td> 
  </tr> 
 </tbody> 
</table>


1.  Click `Add a Rule for this Column`.


   >[!NOTE]
   >
   >You cannot apply conditional formatting to a User Team ID field.



1. In the `When the:` section, set a condition statement for the column. For example: when the Task Percent Complete Equals (Case Sensitive) 50.
1.  In the `Show the field like this:`&nbsp;section specify what this field looks like when the condition defined above is met.  
   Specify the following information:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Text Color</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Select the color in which the&nbsp;text is displayed. There are 8 colors available.</p> <p>Note: If the field contains a hyperlink, the text color selections are not applied to this field.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Text Format</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Select whether to display text in bold or italic.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Text Alignment</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Select whether to&nbsp;align the text&nbsp;to the right, center, or the left within the column.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Background</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Select the color of the background for the text.&nbsp;There are 8 colors available.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Show Icon</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Select from one of 16 icons, if you want to display an icon instead of the actual value for this column.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Show Text</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select this option to display a custom label for this column, instead of its actual value. Specify the text to show instead of the value in the field provided.</p> <p>Important: Selecting <span class="bold">Show Text</span> disables the ability to inline edit the text in this column.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Apply to the entire row</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Select this option to apply settings to the entire row rather than applying settings to just the selected column.</td> 
  </tr> 
 </tbody> 
</table>


1. Click `Add Rule`.  
   You can add additional rules to the same column, or add rules to other columns.  
   Rules are applied in the order that they were created.  
   For example, you can first create a rule that states when the Project Status is Building, the&nbsp;text color is purple and bold. You then create a second rule that states when the Task Name is not blank, the text color is red and italicized, and the background color is green. In this example, the following occurs:  

    
    
    * Tasks whose Project Status is Building are displayed in purple and bold text. If the task name is not blank, tasks also have a green background.
    * Tasks whose Project Status is anything other than Building (and the Task Name is not blank)&nbsp;are displayed in a red and italicized text&nbsp;with a green background.
    
    

1. Click `Done`.
1. Click `Save + Close`.  
   On the report, users see changes to the format if the conditions specified have been met.  



