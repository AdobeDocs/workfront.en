---
filename: faq
content-type: faq
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
---



# *`Adobe Workfront Fusion`* FAQ {#adobe-workfront-fusion-faq}



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


## What is a scenario? {#what-is-a-scenario}



### Answer {#answer}

A scenario defines a sequence of steps to be executed by *`Adobe Workfront Fusion`*. For each scenario, you specify the data source, how the data is to be processed, and what data is to be used and what is to be ignored. *`Workfront Fusion`* lets you create as complex of scenarios as you need; even the most sophisticated scenarios are possible.


For more information, see [Create a practice integration scenario](create-a-practice-scenario.md).


## Can I use more than one module in a scenario? Or just a trigger and action? {#can-i-use-more-than-one-module-in-a-scenario-or-just-a-trigger-and-action}



### Answer {#answer-1}

You can use as many modules as you want in a scenario. You can create independent routes and specify which data should flow through them. You can also use results returned by individual actions and then pass them on to the next action.


## Can *`Workfront Fusion`* work with files? {#can-workfront-fusion-work-with-files}



### Answer {#answer-2}

Yes. Using *`Workfront Fusion`*, files can be received, saved, transformed, converted, encrypted, and so on. Moreover, *`Workfront Fusion`* provides a wide range of built-in features designed to enable users to work effectively and creatively with the data contained in the files.


For more information, see [About mapping files](about-mapping-files.md).


## What happens if I let *`Workfront Fusion`* process an email containing more than one attachment? {#what-happens-if-i-let-workfront-fusion-process-an-email-containing-more-than-one-attachment}



### Answer {#answer-3}

If you use the Email module Retrieve attachments, each attachment is sent individually through the rest of the modules in the scenario. Similar modules are also available in other apps that receive multiple files at once.


For more information, see [Email modules](email-modules.md).


## Some triggers allow scenarios to run instantly. What does "instantly" mean? {#some-triggers-allow-scenarios-to-run-instantly-what-does-instantly-mean}



### Answer {#answer-4}

Common scenarios are run at intervals according to the schedule you specify (for example, every hour, every 5 minutes, once a month, and the like). There are special triggers, called instant triggers (webhooks), that can start your scenario immediately after they receive data from a given service. Instant triggers can be extremely useful. We recommend to use them whenever possible. They help to reduce the number of operations. Received data is processed immediately without waiting for the next scheduled run. For example, the Google Sheets module Watch Changes starts a scenario immediately after a cell us updated.


## What are aggregators? {#what-are-aggregators}



### Answer {#answer-5}

An Aggregator merges data into one single collection. An example of this is files being compressed into a zip archive and sent as an email attachment.


For more information, see [Aggregator module](aggregator-module.md).


## What is an operation? {#what-is-an-operation}



### Answer {#answer-6}

An operation is any task performed by a module. An operation occurs, for example, every time a trigger runs and every time an action performs a task. 


## What is data transfer? {#what-is-data-transfer}



### Answer {#answer-7}

Data transfer refers to the amount of data transferred through your scenario. For example, suppose you have a scenario that retrieves a 100KB image from FTP and reduces its size to 50KB and saves both images to Dropbox. The amount of data used in this scenario is 150KB. 


## What is a connection? {#what-is-a-connection}



### Answer {#answer-8}

A connection is the link between your *`Workfront Fusion`* account and the third-party service you want to use. The connection can be easily created when editing a scenario. To add a connection, click the `Add` button in the module setting and follow the step-by-step instructions.


For more information, see [About connecting Adobe Workfront Fusion to an app or service](about-connecting-wf-fusion-to-app-or-service.md).
