---
filename: scenario-execution-flow
content-type: overview
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
---



# Scenario execution flow {#scenario-execution-flow}

This article explains how a scenario executes and how data flows through it. It also explains where you can find information about your processed data and how to read it.


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


## Scenario execution flow {#scenario-execution-flow-1}

After a scenario is set up correctly and activated, it executes according to its defined schedule.


As the scenario begins, the first module responds to an event it has been set to watch for. If it returns any bundles (data), they pass on to the next module and the scenario continues, passing the bundles through each successive module, one by one. 


If the bundles process correctly throughout all of the modules, the scenario is marked as a success in the scenario detail area, as explained in [Scenario detail](scenario-detail.md).



* For more information on setting up a scenario, see [Basic scenario settings](basic-scenario-settings.md).
* For more information on activating a scenario, see [Activate or deactivate a scenario](activate-or-inactivate-scenario.md).
* For more information on scheduling a scenario, see [Schedule a scenario](schedule-a-scenario.md).
* For more information on modules, see [Types of modules](module-types.md).



` `**Example: **`` In a scenario that downloads documents from *`Adobe Workfront`* and sends them to a folder in Dropbox, data would flow as follows.


The scenario's first step, performed by the first module, is to watch for bundles (documents). In this example, the module watches for bundles in *`Workfront`*. If it does not return a bundle, the scenario ends after the first module.


If a bundle is returned, the bundle passes through the rest of the scenario. In this example, the rest of the scenario consists of the second and last module, which uploads the bundle to the Dropbox folder.


![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)




If the first module returns multiple bundles, the first bundle is uploaded to Dropbox before the second bundle is uploaded. Then the second bundle uploads, then the third, and so on. 


## Information about processed bundles {#information-about-processed-bundles}

For each module, the bundle goes through a 4-step process before going on to the next module or reaching its final destination. The 4-step process is Initalization, Operation, Commit/Rollback, and Finalization. This is called transaction processing and it helps to explain how data was processed in a module.


Once a scenario run is complete, each module displays an icon showing the number of operations performed. You can click this icon to display the detailed information about the processed bundles, in the format described above. You can see which modules settings were used and which bundles were returned by which module.


![](assets/info-processed-bundles-350x397.png)




A module received input information such as:



* Converted image
* Selected folder where the image shall be uploaded to
* Original name of the Facebook image


After processing, the module returned this output information:



* Image ID assigned by Dropbox
* Full path where in Dropbox *`Workfront Fusion`* uploaded the file


The above information is captured for each bundle separately, as marked by the drop down boxes Operation 1 and Operation 2 in the image.


For more information on transaction processing see [Scenario execution, cycles, and phases](scenario-execution-cycles-phases.md).


## Error occurred while executing a scenario {#error-occurred-while-executing-a-scenario}

An error might occur during the scenario run. For example, if you delete the Dropbox folder that you have set as the target folder in the module setting, the scenario terminates with an error message. For more information about how to handle errors, see [Error processing](error-processing.md).
