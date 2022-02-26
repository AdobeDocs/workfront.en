---
filename: create-a-practice-scenario-2
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Get started creating a scenario: Exercise 2
description: 
---

# Get started creating a scenario: Exercise 2

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">&nbsp;</p>
-->

&nbsp;

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">--------------------</p>
-->

--------------------

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">We will create a scenario that creates a new project in <em>Adobe Workfront Fusion</em> for every sales opportunity that is closed in Salesforce.</p>
-->

We will create a scenario that creates a new project in *Adobe Workfront Fusion* for every sales opportunity that is closed in Salesforce.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">RESHOOT - this is alloy</p>
-->

RESHOOT - this is alloy

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <span class="bold">Type</span> box, select <span class="bold">Opportunity</span> to specify the type of information the module will be looking for.</p>
   -->

   In the `Type` box, select `Opportunity` to specify the type of information the module will be looking for.

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <span class="bold">Maximum count of records</span> box, type the number of opportunities you want the module to watch to see if they close.</p>
   -->

   In the `Maximum count of records` box, type the number of opportunities you want the module to watch to see if they close.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">We'll type 10 for this example.</p>
   -->

   We'll type 10 for this example.

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <span class="bold">Watch</span> box, select an option to indicate whether you want the module to watch <span class="bold">Only new records</span> or <span class="bold">New records and all changes</span>.</p>
   -->

   In the `Watch` box, select an option to indicate whether you want the module to watch `Only new records` or `New records and all changes`.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Let's select <span class="bold">New records and all changes</span>.</p>
   -->

   Let's select `New records and all changes`.

   <!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <span class="bold">OK</span>.</li>
   -->

1. Click `OK`.
1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <span class="bold">Choose where to start</span> box, specify where you want the module to start its processing.</p>
   -->

   In the `Choose where to start` box, specify where you want the module to start its processing.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Let's select <span class="bold">Records from after a specific date</span>, then select a date about 6 months ago.</p>
   -->

   Let's select `Records from after a specific date`, then select a date about 6 months ago.

   <!--
   <li value="6" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <span class="bold">OK</span>.</li>
   -->

1. Click `OK`.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Mapping is the process of assigning a module's outputs, structured into items, to the module's input fields. You can learn a lot about mapping items between modules in the following articles:</p>
-->

Mapping is the process of assigning a module's outputs, structured into items, to the module's input fields. You can learn a lot about mapping items between modules in the following articles:

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about trigger modules, see <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref" xrefformat="{para}">Types of modules</a>.</li>
  -->

* For more information about trigger modules, see [Types of modules](../../workfront-fusion/modules/module-types.md).

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about connecting <em>Workfront Fusion</em> to an app, see <a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref" xrefformat="{para}">About connecting Adobe Workfront Fusion to an app or service</a>.</li>
  -->

* For more information about connecting *Workfront Fusion* to an app, see [About connecting Adobe Workfront Fusion to an app or service](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information on choosing where to start, see <a href="../../workfront-fusion/modules/choose-where-trigger-module-starts.md" class="MCXref xref" xrefformat="{para}">Choose where a trigger module starts</a>.</li>
  -->

* For more information on choosing where to start, see [Choose where a trigger module starts](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information on mapping items, see <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref" xrefformat="{para}">Map information from one module to another</a>.</li>
  -->

* For more information on mapping items, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"><a name="Add"></a>Add the second module and specify what it will do</h2>
-->

## Add the second module and specify what it will do

<ol data-mc-continue="false"> <draft-comment>
  <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the right handle of the <span class="bold">Salesforce</span> module.</li>
 </draft-comment>
 <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the right handle of the <span class="bold">Salesforce</span> module.</li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <span class="bold">Workfront </span>><span class="bold"> Create Record</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <span class="bold">Workfront </span>><span class="bold"> Create Record</span>.</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Normally, in the box that displays for setting up the module, you would need to create a connection between <em>Workfront Fusion</em> and the module. This won't be necessary for the <em>Workfront</em> module.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Normally, in the box that displays for setting up the module, you would need to create a connection between <em>Workfront Fusion</em> and the module. This won't be necessary for the <em>Workfront</em> module.</p> </li> 
 <li value="3"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> In the <span class="bold">Workfront</span> box, under <span class="bold">Record type</span>, click <span class="bold">Project</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode"> In the <span class="bold">Workfront</span> box, under <span class="bold">Record type</span>, click <span class="bold">Project</span>.</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The box expands to display all the fields available for a <em>Workfront</em> project. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">The box expands to display all the fields available for a <em>Workfront</em> project. </p> </li> 
 <li value="4"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">We're going to choose the <span class="bold">Name</span> field so that this module creates each project with the same name as the corresponding closed opportunity in Salesforce. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">We're going to choose the <span class="bold">Name</span> field so that this module creates each project with the same name as the corresponding closed opportunity in Salesforce. </p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can use Ctrl-F to find the field you want quickly.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can use Ctrl-F to find the field you want quickly.</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/name-field.png"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/name-field.png"> </p> </li> <draft-comment>
  <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Click the <span class="bold">Name</span> field, then click the <span class="variable">Name </span>variable in the list that appears. </li>
 </draft-comment>
 <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Click the <span class="bold">Name</span> field, then click the <span class="variable">Name </span>variable in the list that appears. </li> 
</ol>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"><a name="Test"></a>Test the scenario</h2>
-->

## Test the scenario

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Before you activate your scenario, it's important to test your scenario by running it at least once and viewing the results. This helps you understand how data flows through the scenario and find any errors it contains.</p>
-->

Before you activate your scenario, it's important to test your scenario by running it at least once and viewing the results. This helps you understand how data flows through the scenario and find any errors it contains.

<ol> 
 <li value="1"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <span class="bold">Run once</span> in the lower-left corner of the scenario editor.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <span class="bold">Run once</span> in the lower-left corner of the scenario editor.</p> </li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">After the scenario finishes running, click the bubble above a module. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">After the scenario finishes running, click the bubble above a module. </p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/click-bubble.png"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/click-bubble.png"> </p> </li> 
 <li value="3"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the box that appears, view information about the bundles of data that the module processed, including the number of operations that occurred in it. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the box that appears, view information about the bundles of data that the module processed, including the number of operations that occurred in it. </p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can look at each individual operation to see which module settings were used and which bundles were returned by which module. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can look at each individual operation to see which module settings were used and which bundles were returned by which module. </p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/view-each-operation.png"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/view-each-operation.png"> </p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the past 6 months, the scenario found 1 Salesforce opportunity that closed. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the past 6 months, the scenario found 1 Salesforce opportunity that closed. </p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/1-bundle.png"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/1-bundle.png"> </p> </li> 
</ol>

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can learn more about how to read scenario execution information in the following articles:</p>
-->

You can learn more about how to read scenario execution information in the following articles:

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For general information, see <a href="../../workfront-fusion/scenarios/scenario-execution-flow.md" class="MCXref xref" xrefformat="{para}">Scenario execution flow</a>.</li>
  -->

* For general information, see [Scenario execution flow](../../workfront-fusion/scenarios/scenario-execution-flow.md).

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about processed bundles, see <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref" xrefformat="{para}">Scenario execution, cycles, and phases</a>.</li>
  -->

* For information about processed bundles, see [Scenario execution, cycles, and phases](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about number of operations, see .</li>
  -->

* For information about number of operations, see .

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"><a name="Activate"></a>Activate the scenario</h2>
-->

## Activate the scenario

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Your scenario is almost ready for use, but it's still inactive.</p>
-->

Your scenario is almost ready for use, but it's still inactive.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To activate the scenario:</p>
-->

To activate the scenario:

<ol> 
 <li value="1"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the left arrow <img src="assets/left-arrow-exit-editing.png"> near the upper-left corner of the scenario editor to exit the editor and return to the scenario page.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the left arrow <img src="assets/left-arrow-exit-editing.png"> near the upper-left corner of the scenario editor to exit the editor and return to the scenario page.</p> </li> <draft-comment>
  <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">To activate the scenario, click the <span class="bold">On/Off</span> button at the top of the scenario page.</li>
 </draft-comment>
 <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">To activate the scenario, click the <span class="bold">On/Off</span> button at the top of the scenario page.</li> 
</ol>

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">After you active a scenario, it scenario runs according to its schedule.</p>
-->

After you active a scenario, it scenario runs according to its schedule.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about activating scenarios, see <a href="../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md" class="MCXref xref" xrefformat="{para}">Activate or deactivate a scenario</a>.</p>
-->

For more information about activating scenarios, see [Activate or deactivate a scenario](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about schedules, see <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref" xrefformat="{para}">Schedule a scenario</a>.</p>
-->

For more information about schedules, see [Schedule a scenario](../../workfront-fusion/scenarios/schedule-a-scenario.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">&nbsp;</p>
-->

&nbsp;

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">&nbsp;</p>
-->

&nbsp;

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">&nbsp;</p>
-->

&nbsp;

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Mapping is the process of assigning a module's outputs, structured into items, to the module's input fields. You can learn a lot about mapping items between modules in the following articles:</p>
-->

Mapping is the process of assigning a module's outputs, structured into items, to the module's input fields. You can learn a lot about mapping items between modules in the following articles:

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information on triggers, see <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref" xrefformat="{para}">Types of modules</a>.</li>
  -->

* For more information on triggers, see [Types of modules](../../workfront-fusion/modules/module-types.md).

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information on connections, see <a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref" xrefformat="{para}">About connecting Adobe Workfront Fusion to an app or service</a>.</li>
  -->

* For more information on connections, see [About connecting Adobe Workfront Fusion to an app or service](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information on choosing where to start, see <a href="../../workfront-fusion/modules/choose-where-trigger-module-starts.md" class="MCXref xref" xrefformat="{para}">Choose where a trigger module starts</a>.</li>
  -->

* For more information on choosing where to start, see [Choose where a trigger module starts](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information on mapping items, see <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref" xrefformat="{para}">Map information from one module to another</a>.</li>
  -->

* For more information on mapping items, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

