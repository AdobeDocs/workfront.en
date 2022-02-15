---
filename: iterator-module
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
---



# Iterator module {#iterator-module}

An iterator module is a special type of module that converts an array into a series of bundles. Each array item is outputted as a separate bundle.


For more information, see [Types of modules](module-types.md) and [Map an array](map-an-array.md).


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


## Iterator module configuration {#iterator-module-configuration}

You set up an iterator module the same you set up any other module. The Array field contains the array to be convertedor split into separate bundles.


![](assets/set-up-iterator-350x190.jpg)




For more information, see [Configure a module's settings](configure-a-modules-settings.md).

` `**Examples: **`` 


*  The below scenario shows how to retrieve emails with attachments and save the attachments as single files in a selected Dropbox folder.


  Emails can contain an array of attachments. The iterator module inserted after the first module will enable you to handle each attachment separately. The iterator module splits the array of attachments into single bundles. Each bundle, with one attachment, is then saved one at a time in a selected Dropbox folder. The iterator module set-up is shown above: the Array field should contain the 

  ```
  Attachments[]
  ```

  array.


  ![](assets/attachments-array-350x154.jpg)








*  For your convenience, many *`Workfront Fusion`* apps offer specialized iterator modules with a simplified setup. For example, the Email app contains the special iterator module Email > Iterate attachments that will produce the same results as the general It


  ![](assets/specialized-iterators-350x135.jpg)







## Troubleshooting: Mapping panel does not display mappable items under iterator module {#troubleshooting-mapping-panel-does-not-display-mappable-items-under-iterator-module}

When an iterator module does not have an information about the structure of the array's items, the mapping panel in the modules following the iterator module display only 2 items under the iterator module :

```
Total number of bundles
```

and 

```
Bundle order position
```

:


![](assets/mapping-panel-doesnt-display-350x147.png)




This because each module is responsible for providing information about items it outputs so that these items can be properly displayed in the mapping panel in the subsequent modules. However, several modules might be unable to provide this information in some cases; for example, JSON > Parse JSON or Webhooks > Custom Webhook modules with missing Data structure.


The solution is to manually execute the scenario to make the module learn about the items it outputs so it can provide the information to the following modules.


For example, if you have a JSON > Parse JSON module without a Data structure as below:


![](assets/json-parse-json-350x285.png)




And then if you connect an iterator module to it, you will not be able to map the output of the module to the Array field in the setup panel of the iterator module :


![](assets/connect-iterator-module-350x146.png)




To resolve this, manually start the scenario in the scenario editor. You can un-link the modules after the JSON > Parse JSON module to prevent the flow from proceeding further. Or you can right-click the JSON > Parse JSON module and choose `Run this module only` from the context menu to execute only the JSON > Parse JSON module.


When the JSON > Parse JSON executes, it learns about the items that it outputs and provides this information to all the subsequent modules, including the iterator module. The mapping panel in the Iterator's setup then displays the items:


![](assets/mapping-panel-displays-items-350x131.png)




Moreover, the mapping panel in the modules that are connected after the iterator module display the items contained in the array's items:


![](assets/items-contained-in-array-350x156.png)




If you cannot see some items in a module's mapping panel, run the scenario once so all the modules can learn about the items they output and provide this information to the following modules.
