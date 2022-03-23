---
filename: create-a-practice-scenario-2
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Get started creating a scenario: Exercise 2
description: 
hidefromtoc: true
---

# Get started creating a scenario: Exercise 2

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">--------------------</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">We will create a scenario that creates a new project in Adobe Workfront Fusion for every sales opportunity that is closed in Salesforce.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">RESHOOT - this is alloy</p>
-->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Type</strong> box, select <strong>Opportunity</strong> to specify the type of information the module will be looking for.</p>
   -->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Maximum count of records</strong> box, type the number of opportunities you want the module to watch to see if they close.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">We'll type 10 for this example.</p>
   -->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Watch</strong> box, select an option to indicate whether you want the module to watch <strong>Only new records</strong> or <strong>New records and all changes</strong>.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Let's select <strong>New records and all changes</strong>.</p>
   -->

   <!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>OK</strong>.</li>
   -->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Choose where to start</strong> box, specify where you want the module to start its processing.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Let's select <strong>Records from after a specific date</strong>, then select a date about 6 months ago.</p>
   -->

   <!--
   <li value="6" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>OK</strong>.</li>
   -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Mapping is the process of assigning a module's outputs, structured into items, to the module's input fields. You can learn a lot about mapping items between modules in the following articles:</p>
-->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about trigger modules, see <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref" xrefformat="{para}">Types of modules</a>.</li>
  -->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about connecting Workfront Fusion to an app, see <a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref" xrefformat="{para}">About connecting Adobe Workfront Fusion to an app or service</a>.</li>
  -->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information on choosing where to start, see <a href="../../workfront-fusion/modules/choose-where-trigger-module-starts.md" class="MCXref xref" xrefformat="{para}">Choose where a trigger module starts</a>.</li>
  -->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information on mapping items, see <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref" xrefformat="{para}">Map information from one module to another</a>.</li>
  -->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"><a name="Add"></a>Add the second module and specify what it will do</h2>
-->

   <!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the right handle of the <strong>Salesforce</strong> module.</li>
   -->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Workfront</strong>><strong>Create Record</strong>.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Normally, in the box that displays for setting up the module, you would need to create a connection between Workfront Fusion and the module. This won't be necessary for the Workfront module.</p>
   -->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> In the <strong>Workfront</strong> box, under <strong>Record type</strong>, click <strong>Project</strong>.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The box expands to display all the fields available for a Workfront project. </p>
   -->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">We're going to choose the <strong>Name</strong> field so that this module creates each project with the same name as the corresponding closed opportunity in Salesforce. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can use Ctrl-F to find the field you want quickly.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/name-field.png"> </p>
   -->

   <!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Click the <strong>Name</strong> field, then click the <span class="variable">Name </span>variable in the list that appears. </li>
   -->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"><a name="Test"></a>Test the scenario</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Before you activate your scenario, it's important to test your scenario by running it at least once and viewing the results. This helps you understand how data flows through the scenario and find any errors it contains.</p>
-->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Run once</strong> in the lower-left corner of the scenario editor.</p>
   -->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">After the scenario finishes running, click the bubble above a module. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/click-bubble.png"> </p>
   -->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the box that appears, view information about the bundles of data that the module processed, including the number of operations that occurred in it. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can look at each individual operation to see which module settings were used and which bundles were returned by which module. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/view-each-operation.png"> </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the past 6 months, the scenario found 1 Salesforce opportunity that closed. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/1-bundle.png"> </p>
   -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can learn more about how to read scenario execution information in the following articles:</p>
-->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For general information, see <a href="../../workfront-fusion/scenarios/scenario-execution-flow.md" class="MCXref xref" xrefformat="{para}">Scenario execution flow</a>.</li>
  -->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about processed bundles, see <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref" xrefformat="{para}">Scenario execution, cycles, and phases</a>.</li>
  -->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about number of operations, see .</li>
  -->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"><a name="Activate"></a>Activate the scenario</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Your scenario is almost ready for use, but it's still inactive.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To activate the scenario:</p>
-->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the left arrow <img src="assets/left-arrow-exit-editing.png"> near the upper-left corner of the scenario editor to exit the editor and return to the scenario page.</p>
   -->

   <!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">To activate the scenario, click the <strong>On/Off</strong> button at the top of the scenario page.</li>
   -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">After you active a scenario, it scenario runs according to its schedule.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about activating scenarios, see <a href="../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md" class="MCXref xref" xrefformat="{para}">Activate or deactivate a scenario</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about schedules, see <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref" xrefformat="{para}">Schedule a scenario</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Mapping is the process of assigning a module's outputs, structured into items, to the module's input fields. You can learn a lot about mapping items between modules in the following articles:</p>
-->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information on triggers, see <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref" xrefformat="{para}">Types of modules</a>.</li>
  -->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information on connections, see <a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref" xrefformat="{para}">About connecting Adobe Workfront Fusion to an app or service</a>.</li>
  -->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information on choosing where to start, see <a href="../../workfront-fusion/modules/choose-where-trigger-module-starts.md" class="MCXref xref" xrefformat="{para}">Choose where a trigger module starts</a>.</li>
  -->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information on mapping items, see <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref" xrefformat="{para}">Map information from one module to another</a>.</li>
  -->

