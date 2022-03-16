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

-->

<!--
--------------------
-->

<!--
We will create a scenario that creates a new project in Adobe Workfront Fusion for every sales opportunity that is closed in Salesforce.
-->

<!--
RESHOOT - this is alloy
-->

1. 

   <!--
   In the Type box, select Opportunity to specify the type of information the module will be looking for.
   -->

1. 

   <!--
   In the Maximum count of records box, type the number of opportunities you want the module to watch to see if they close.
   -->

   <!--
   We'll type 10 for this example.
   -->

1. 

   <!--
   In the Watch box, select an option to indicate whether you want the module to watch Only new records or New records and all changes.
   -->

   <!--
   Let's select New records and all changes.
   -->

   <!--
   Click OK.
   -->

1. 

   <!--
   In the Choose where to start box, specify where you want the module to start its processing.
   -->

   <!--
   Let's select Records from after a specific date, then select a date about 6 months ago.
   -->

   <!--
   Click OK.
   -->

<!--
Mapping is the process of assigning a module's outputs, structured into items, to the module's input fields. You can learn a lot about mapping items between modules in the following articles:
-->

  <!--
  For more information about trigger modules, see Types of modules.
  -->

  <!--
  For more information about connecting Workfront Fusion to an app, see About connecting Adobe Workfront Fusion to an app or service.
  -->

  <!--
  For more information on choosing where to start, see Choose where a trigger module starts.
  -->

  <!--
  For more information on mapping items, see Map information from one module to another.
  -->

<!--
Add the second module and specify what it will do
-->

   <!--
   Click the right handle of the Salesforce module.
   -->

1. 

   <!--
   Click Workfront > Create Record.
   -->

   <!--
   Normally, in the box that displays for setting up the module, you would need to create a connection between Workfront Fusion and the module. This won't be necessary for the Workfront module.
   -->

1. 

   <!--
   In the Workfront box, under Record type, click Project.
   -->

   <!--
   The box expands to display all the fields available for a Workfront project.
   -->

1. 

   <!--
   We're going to choose the Name field so that this module creates each project with the same name as the corresponding closed opportunity in Salesforce.
   -->

   <!--
   You can use Ctrl-F to find the field you want quickly.
   -->

   <!--

   -->

   <!--
   Click the Name field, then click the Name variable in the list that appears.
   -->

<!--
Test the scenario
-->

<!--
Before you activate your scenario, it's important to test your scenario by running it at least once and viewing the results. This helps you understand how data flows through the scenario and find any errors it contains.
-->

1. 

   <!--
   Click Run once in the lower-left corner of the scenario editor.
   -->

1. 

   <!--
   After the scenario finishes running, click the bubble above a module.
   -->

   <!--

   -->

1. 

   <!--
   In the box that appears, view information about the bundles of data that the module processed, including the number of operations that occurred in it.
   -->

   <!--
   You can look at each individual operation to see which module settings were used and which bundles were returned by which module.
   -->

   <!--

   -->

   <!--
   In the past 6 months, the scenario found 1 Salesforce opportunity that closed.
   -->

   <!--

   -->

<!--
You can learn more about how to read scenario execution information in the following articles:
-->

  <!--
  For general information, see Scenario execution flow.
  -->

  <!--
  For information about processed bundles, see Scenario execution, cycles, and phases.
  -->

  <!--
  For information about number of operations, see .
  -->

<!--
Activate the scenario
-->

<!--
Your scenario is almost ready for use, but it's still inactive.
-->

<!--
To activate the scenario:
-->

1. 

   <!--
   Click the left arrow near the upper-left corner of the scenario editor to exit the editor and return to the scenario page.
   -->

   <!--
   To activate the scenario, click the On/Off button at the top of the scenario page.
   -->

<!--
After you active a scenario, it scenario runs according to its schedule.
-->

<!--
For more information about activating scenarios, see Activate or deactivate a scenario.
-->

<!--
For more information about schedules, see Schedule a scenario.
-->

<!--

-->

<!--

-->

<!--

-->

<!--
Mapping is the process of assigning a module's outputs, structured into items, to the module's input fields. You can learn a lot about mapping items between modules in the following articles:
-->

  <!--
  For more information on triggers, see Types of modules.
  -->

  <!--
  For more information on connections, see About connecting Adobe Workfront Fusion to an app or service.
  -->

  <!--
  For more information on choosing where to start, see Choose where a trigger module starts.
  -->

  <!--
  For more information on mapping items, see Map information from one module to another.
  -->

