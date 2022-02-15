---
filename: aggregator-module
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
---



# Aggregator module {#aggregator-module}

An aggregator module is a type of module designed to merge several bundles of data into a single bundle. 


For more information about module types, see [Types of modules](module-types.md).


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


## Aggregator module {#aggregator-module-1}

When an aggregator module executes, it does the following:



* Accumulates all the bundles it receives during a single source module's operation.
* Outputs a single bundle with an array containing one item per each accumulated bundle. The content of the array's items depends on particular aggregator module and its setup.


The following image shows a typical setup of the aggregator module :


![](assets/array-aggregator-350x190.png)



<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Source Module</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The module from which the bundle aggregation will start. The source module is usually an iterator or a search module that outputs a series of bundles. When you setup the aggregator's source module (and close the aggregator's setup), the route between the source module and the aggregator module are wrapped in a grey area so that you can see clearly the start and the end of the aggregation. </p> <p>For more information on iterators, see <a href="iterator-module.md" class="MCXref xref">Iterator module</a></p> <p>For more information on search modules see search modules in <a href="module-types.md" class="MCXref xref">Types of modules</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Target structure type</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>(Applicable only for the Array aggregator module.) The target structure into which the data shall be aggregated. The default option, Custom, enables you to choose items that should be aggregated into the Array aggregator's output bundle's <code>Array </code>item:</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>Once you connect more modules after the Array aggregator module and get back to the module's setup, the Target structure type dropdown will contain all following modules and their fields that are of type Array of Collections, as shown in the Attachments field of the Slack &gt; Create a Message module:</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Aggregated fields</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Select the fields that you want to include in the aggregator module output.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Group by</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>The aggregator's output can be split into several groups with the help of the Group by field. The Group by field can contain a formula that is evaluated for each aggregator's input bundle. The aggregator then outputs one bundle per each distinct formula's value. Each bundle contains two items:</p> 
    <ul> 
     <li><code>Key </code>contains the distinct value.</li> 
     <li><code>Array </code>contains the aggregated data from the bundles for which the formula evaluated to the <code>Key </code>value.</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> <p>Stop processing after an empty aggregation</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>By default, the aggregator module outputs the result of the aggregation even in case no bundles reached the aggregator module (for example, because they have been all filtered out on their way). If the option Stop processing after an empty aggregation is enabled, the aggregator module will not produce any output bundle in this case and the flow will stop.</p> </td> 
  </tr> 
 </tbody> 
</table>



>[!NOTE]
>
>Bundles generated by modules between the source module and the aggregator module are not outputted by the aggregator module, so they are not accessible by the modules in the flow after the aggregator. If you need any data from a bundle outputted by a module between the source module and the aggregator module, make sure to include the given item in the aggregator module's setup (as in the Aggregated fields field in the setup of the Array aggregator module).



` `**Example: **`` Use Case: Zipping all email attachments and uploading the ZIP to Dropbox


The scenario below shows how to:



* Watch a mailbox for incoming emails: Email > Watch emails trigger will output a bundle with item 

  ```
  Attachments[]
  ```

  , which is an array containing all the email's attachments.
* Iterate the email's attachments: Email > Iterate attachments iterator takes the items from the 

  ```
  Attachments[]
  ```

  array one by one and sends them further as separate bundles.
* Aggregate the bundles outputted by the Email > Iterate attachments module: Archive > Create an archive aggregator accumulates all the bundles it receives and outputs a single bundle containing the ZIP file.
* Upload the resulting ZIP file to Dropbox: Dropbox > Upload a file obtains the ZIP file from the Archive > Create an archive module and uploads it to Dropbox.


![](assets/dropbox-archive-350x87.png)




Below is a sample setup of the Archive > Create an archive aggregator:


![](assets/archive-create-an-archive-350x484.png)


