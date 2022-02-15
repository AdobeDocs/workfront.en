---
filename: retry
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
---



# Retry {#retry}

In some cases it is useful to re-execute a failing module for a couple of times if there is a chance that the reason for the failure might pass over time.


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


## Workarounds to the Retry error handling directive {#workarounds-to-the-retry-error-handling-directive}

*`Adobe Workfront Fusion`* currently does not offer the Retry error handling directive, though two workarounds can be employed to mimic its functionality. For more information, see [Directives for error handling](directives-for-error-handling.md).


### Use the Break directive {#use-the-break-directive}




1. In the [Scenario settings panel](scenario-settings-panel.md), enable the `Allow storing of Incomplete Executions` option.

1. Attach an error handler route to the module, as described in [Error handling](error-handling.md).
1.  Link the Break directive to the error handler route (see [Directives for error handling](directives-for-error-handling.md)) and configure it.


   ![](assets/break-directive-350x241.png)







#### Drawbacks {#drawbacks}




* The minimum retry interval is one minute.
* If the module is processing multiple bundles and the processing of a bundle fails, the partial execution (only the bundle that caused the error) is moved to the [View and resolve incomplete executions](view-and-resolve-incomplete-executions.md) folder and scheduled for retries according to the Break directive settings. However, the current execution continues and the module continues to process the subsequent bundles. At least you can enable the "Sequential processing" option in the Scenario settings to prevent the scenario from executing again until the execution stored in the the Incomplete executions folder has been successfully resolved.




### Use the Repeater module {#use-the-repeater-module}




1. Employ the `Repeater` module and set its Repeats field to the maximum number of attempts.
1. Link the potentially failing module to the `Repeater` module.
1. Attach an error handler route to this module (see [Error handling](error-handling.md)).
1. Link the `Tools > Sleep` module to the error handler route and set its `Delay` field to the number of seconds between the attempts.

1. Link the `Ignore` directive after the `Tools > Sleep` module (see [Directives for error handling](directives-for-error-handling.md)).

1. Link the `Tools > Set variable` module after the the potentially failing module and configure it to store the module's result in a variable named, for example, 

   ```
   Result
   ```

   .

1. Link the `Array aggregator` module after the `Tools > Set` variable and choose the `Repeater` module in its Source Module field.

1. Link the `Tools > Get variable` module to the `Array aggregator` module and configure it to obtain the value of the 

   ```
   Result
   ```

   variable.

1. Insert the `Tools > Get` variable module between the `Repeater` module and the potentially failing module and configure it obtain the value of the 

   ```
   Result
   ```

   variable.

1. Insert a filter between this `Tools > Get` variable module and the potentially failing module to continue only if the 

   ```
   Result
   ```

   variable does not exist.




` `**Example: **`` Here is a sample scenario where the HTTP > Make a request module represents the potentially failing module:


![](assets/http-make-request-350x116.png)




If the result of the potentially failing module is too complex to be stored in a simple variable, you may employ a data store to store/retrieve the result. The data store would contain just one record. The record's key can be, for example, 

```
Result
```

.


For more information on data stores, see [Data Stores](data-stores.md)


#### Drawback {#drawback}

This workaround might appear a bit too complex and it is also more demanding in terms of operations.
