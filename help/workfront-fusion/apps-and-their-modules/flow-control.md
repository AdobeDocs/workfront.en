---
filename: flow-control
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
---



# Flow control {#flow-control}

When you are creating or editing a scenario, you can configure settings to control the way data flows through it.


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


## Repeater  {#repeater}

You can use a Repeater module to repeat a task a given number of times. A Repeater module generates bundles, one after another.


For example, you could use a Repeater module to send five emails with the subjects "Hello 1," "Hello 2," and so on, by connecting the `Email > Send me an email` module to the Repeater module.


To use a Repeater module:



1.  Click the Flow Control icon ![](assets/flow-control-icon.gif) at the bottom of the screen, then click `Repeater` in the menu that displays.
1.   Click the Repeater bundle, then click `Connect automatically` in the box that displays.
1.  In the Flow Control box that appears, type the number of repetitions (outputted bundles) you want in the `Repeats` box.


   In our email example, you would type 5.


   ![](assets/repeater-2-350x207.png)




   The value of the item increases in each repetition by this value specified in the `Step` field, which you can view by selecting `Show advanced settings`. This number is 1 by default.

1. Click `OK` to close the `Flow Control` box.

1. Click the app or service module connected to the Repeater module.
1.  In the box that appears, type the information that you want to repeat.


   In our email example, you would type Hello in the Subject box, then map 

   ```
   i
   ```

   from the repeater module.


   ![](assets/repeater-3-350x207.png)








>[!NOTE]
>
>The number of repeats is not determined by the value of >
>
>```>
>i
>```>
>
>, as it would be in a loop in programming. The module will repeat the number of times indicated in the Repeats field. The value >
>
>```>
>i
>```>
>
>changes with each iteration of the repeater module, and can be mapped to later modules. The example above maps the value of >
>
>```>
>i
>```>
>
>into the Hello message, resulting in messages that read "Hello 1," Hello 2," and so on.




## Iterator {#iterator}

An Iterator is a special type of module that converts an array into a series of bundles. Each array item will be a separate bundle in the Iterator module output. For more information, see [Iterator module](iterator-module.md).


## Array aggregator {#array-aggregator}

An array aggregator is a special type of module which allows to merge several bundles into one single bundle. For more information, see [Aggregator module](aggregator-module.md).


## Router {#router}

The Router module allows you to branch your flow into several routes and process the data within each route differently. Once a Router module receives a bundle, it forwards it to each connected route in the order the routes were attached to the Router module. For more information, see [Router module](router-module.md).
