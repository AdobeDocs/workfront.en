---
filename: copy-modules-or-scenarios
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
---



# Copy modules or scenarios {#copy-modules-or-scenarios}




You can copy modules, groups of modules, or entire scenarios in *`Adobe Workfront Fusion`*. This ability allows you to reuse scenarios or parts of scenarios without having to build them again


## Access requirements {#access-requirements}

You must have the following access to use the functionality in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> license**</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFFusionIntegration variable varname">Workfront Fusion for Work Automation and Integration</span> </p> <p data-mc-conditions="SnippetConditions.HIDE"><span class="mc-variable WFVariables.WFFusionAutomation variable varname">Workfront Fusion for Work Automation</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Your organization must purchase <span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> as well as <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

You must add modules to a scenario before you can copy them. 


## Copy a module or a group of modules {#copy-a-module-or-a-group-of-modules}

When you copy a module, the copy retains all of the field values and settings of the original module. 


You can paste the module or modules into another area of the same scenario, or into a different scenario.


Consider the following when pasting modules into a different scenario.



*  Any field values that pull information from another module that you did not copy can no longer access that information. You must set these fields to pull information from the new scenario.
*  If you paste the modules into a scenario owned by another team or organization, all connections must be updated to connections owned by the group or organization that owns the new scenario.




### Copy modules {#copy-modules}

Copying a group of modules is similar to copying a single module. 



1.  Right-click on the module that you want to copy.


   >[!NOTE]
   >
   >You can select more than one module by holding shift and clicking on the modules that you want to copy. Copying a group of modules also copies any connecting lines, filters, or routing logic between them.



1.  Select **Copy module**.
1.  Move the cursor to the area of the scenario where you want the copy of the scenario.
1.  Right click, and select **Paste**.
1.  Connect the pasted modules to the scenario by dragging them to the appropriate location in the scenario.


   You can also use keyboard shortcuts to copy and paste.





## Copy a scenario by cloning {#copy-a-scenario-by-cloning}

Cloning a scenario creates a copy of the scenario, which you can then edit.



1.  Open the scenario detail page:

    
    
    1.  Click the `Scenario` tab in the left panel, then click a scenario you would like details on.
    
    
       Or
    
    
       If you are working on the scenario in the [Scenario editor](scenario-editor.md), click the left arrow ![](assets/exit-editing-arrow.png) near the upper-left corner of the window.
    
    
    

1.  Right click **Options** at the upper-right of the page.
1.  Select **Clone**.
1.  (Optional) Enter a name for the new scenario.
1.  (Optional) Enable **Keep the states of any new modules the same as those being duplicated** to ensure that the copied scenario also includes information about the most recent records processed by the original scenario.
1.  Click **Save** to create the scenario.




## Copy a scenario by using blueprints {#copy-a-scenario-by-using-blueprints}

Scenario blueprints represent the arrangement, mapping, and field values of a given scenario at a given point in time. You can export a scenario blueprint into a JSON file on your computer, then import it when creating a new scenario. Scenarios imported from a scenario blueprint can be edited.


A scenario blueprint represents the entire scenario. If you want to copy only certain modules from a scenario, see [Copy a module or a group of modules](#copy) in this article.


>[!NOTE]
>
>For information on blueprints in the context of *`Adobe Workfront`*, see [Blueprints overview](blueprints-overview.md).




### Export a scenario blueprint {#export-a-scenario-blueprint}




1.  In the scenario, click the **More** menu in the scenario settings area.
1.  Click Export Blueprint.


   A JSON file is created and downloads to your computer. You can locate this file in your Downloads folder.





### Import a blueprint {#import-a-blueprint}



>[!IMPORTANT] {type="important"}
>
>If you import a blueprint to an existing scenario, the scenario blueprint replaces the existing scenario. You cannot append a blueprint onto an existing scenario.





1.  Begin creating a new scenario.
1.  In the scenario, click the **More** menu in the scenario settings area.
1.  Click **Import Blueprint**.
1.  In the dialog that appears, click **Browse**
1.  Navigate to the blueprint you want to import, and click **Open**.
1.  Click **Save**.


   A JSON file is created and downloads to your computer. You can locate this file in your Downloads folder.





## Copy and reuse scenarios by using templates {#copy-and-reuse-scenarios-by-using-templates}

You can create templates as a starting point for your *`Workfront Fusion`* scenarios. When you create a scenario from a template, you can modify the scenario without modifying the template. Field values are not saved in templates.


For more information on creating and using templates, see [Scenario Templates](_fusion-templates.md).
