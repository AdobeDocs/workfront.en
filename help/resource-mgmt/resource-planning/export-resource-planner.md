---
filename: export-resource-planner
product-area: resource-management
navigation-topic: resource-planning
---



# Export information from the *`Resource Planner`*  {#export-information-from-the-resource-planner}

You can export information from any view of the *`Resource Planner`* to an Excel (.xlsx) file which is saved on your computer. 


>[!IMPORTANT] {type="important"}
>
>There are limitations in what information displays and what information you can export from the *`Resource Planner`*. For information on these limitations, see [Resource Planner display limitations](resource-planner-display-limitations.md)





## Access requirements {#access-requirements}

You must have the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> and higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Review variable varname">Review</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>View or higher access to&nbsp;Projects, Users, and Resource Management</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>View permissions or higher for projects</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Export information from the *`Resource Planner`*<![CDATA[		]]> {#export-information-from-the-resource-planner-1}




1. <![CDATA[				]]><![CDATA[			]]>`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span>. </MadCap:conditionalText>`
1. <![CDATA[			]]> `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click  <span class="bold">Resourcing</span>. The  <span class="bold">Planner</span> displays by default.</MadCap:conditionalText>`
1.  Select the view for the `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Planner</MadCap:conditionalText>`. You can select one of the following options: 
    
    
    *  View by User 
    *  View by Project 
    *  View by Role 
    
    

1.   Click `Export`. 
   The Export Options dialog box displays. `  
   ![](assets/rp-export-options-box-350x421.png)

   `  

1.  Specify the following information:  
   `Start Date`: The start date of your export. The exported file contains allocation and availability information starting with the first day of the week which contains the day you specify here.   
   `Number of Periods`: The number of time periods you want to include in your file. The default is 4 periods.  
   `Type`: The type of time periods by which you want to display the information in the exported file (weeks, months, or quarters.)   
   The following are the maximum time periods that you can export: 
    
    
    *  52 weeks 
    *  36 months 
    *  12 quarters
    
    
   `Select to Export`: Depending on which view you selected, you can select to export the availability and budgeting information for either all the objects listed on the screen or for specific ones.
   You can select to export the following information:
    
    
    * In the Project View, select to export:    
        
        
        * `<li>Projects</li>``<li>Projects and Roles</li>``<li>Everything (this is the default option)</li>`
        
        
        
    * In the User View, select to export:    
        
        
        * `<li>Users</li>``<li>Users and Projects</li>``<li>Everything (this is the default option)</li>`
        
        
        
    * In the Role View, select to export:    
        
        
        * Roles
        * Roles and Projects
        * Everything (this is the default option)
        
        
    
    
   `Data Formatting`: Depending on how you want your Excel file to be displayed, select the following options:
    
    
    * `Raw`: Select to display the availability and allocation information ungrouped by the objects it belongs to in the Excel file. (this is the default option)
    * `Grouped`: Select to display the availability and allocation information grouped by the objects it belongs to. This displays the exported information as it appears on the screen.
    
    
   A sample of how the information looks in the exported file is shown in the Export Options dialog box.

1.  Click `Export`to export the information from the *`Resource Planner`*.  
   Only the information that you saved is exported.  

1.  (Conditional) If you have unsaved Budgeted Hours in the Role or Project views, click `Save and Continue.`  
   An Excel (.xlsx) file is downloaded to your computer.  
   Exporting from the *`Resource Planner`* is unavailable while the file is prepared for downloading.  
   (Conditional) If you export a large amount of data, you receive an email with a link where you can download the file.  
   ![RP_eamil_with_exported_planner_attached.png](assets/rp-eamil-with-exported-planner-attached-350x116.png)


1. (Conditional) When you receive the email with the exported file, click `Download` to download the file.  
   This takes you back to *`Workfront`* where you can download the file.   
   You must be logged into *`Workfront`* for the download to complete.  
   If you do not download the file when it is delivered, the Download link remains active for 7 days after you initiate the export.



