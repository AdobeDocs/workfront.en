---
filename: error-handling
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
---



# Error handling {#error-handling}

When errors occur during the execution of a scenario, it's usually because a service is unavailable due to a failure, a service responds with unexpected data, or the validation of input data fails.


>[!NOTE]
>
>If a module throws an error during the scenario execution and there is no error handling route attached to the module, a default error handling logic is executed as described in [Error processing](error-processing.md).


By adding an error handler route to a module, you can replace the default error handling logic with your own. *`Adobe Workfront Fusion`* offers 5 different directives, any of which can be inserted at the end of your error handler routes. For more information, see [Directives for error handling](directives-for-error-handling.md).


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


## Error handler route {#error-handler-route}

To add an error handler route to a module, (we will call it Module X), right click the module and select `Add error handler`:


![](assets/error-handler-route.png)




The module shows a list of Directives as well as the apps being used in your scenario. If Module X is the last module in your route, you need to choose one of the directives. Or you can go on to add one or more modules to your route. In this case, the Ignore directive is applied by default to Module X and, in the event of an error, the subsequent modules on that route are processed.


![](assets/directives-350x426.png)




As you can see below, if an error occurs while executing the Create a folder module, the Ignore directive will be applied automatically and the scenario will move to the next module on the error handler route if the filter "Data Error Takes Place" returns one or more bundles.


However, if there is no error, the scenario will move to the List all files in a folder module on the regular route.


![](assets/if-there-is-no-error-350x234.png)




Also, to differentiate an error handler route from a regular route, the former is composed of transparent circles as shown above.


## Error handling directives {#error-handling-directives}

The directives are briefly explained below. For more information, see [Directives for error handling](directives-for-error-handling.md).


There are a total of five directives which can be grouped into the following categories based on whether a scenario execution should continue or not:


The following directives ensure that a scenario execution continues:



* Resume allows you to specify a substitute output for the module with the error and the scenario execution status is marked as success
* Ignore simply ignores the error and the scenario execution status is marked as success
* Break stores the input to the queue of incomplete executions and the scenario execution status is marked as warning. For more information, see [View and resolve incomplete executions](view-and-resolve-incomplete-executions.md).


On the other hand, if a scenario execution should be stopped, you must use one of the following directives:



* Rollback stops the scenario execution immediately and marks its status as error
* Commit stops the scenario execution immediately and marks its status as success




## Additional Resources {#additional-resources}




* [Directives for error handling](directives-for-error-handling.md) 
* [Advanced error handling](advanced-error-handling.md) (includes the set up of the Dropbox Scenario referenced above)


