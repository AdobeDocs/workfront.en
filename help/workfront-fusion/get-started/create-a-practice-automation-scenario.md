---
filename: create-a-practice-automation-scenario
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Create a practice automation scenario
description: This article describes how to create an automation scenario with Adobe Workfront Fusion. Automation scenarios automate Workfront processes, including data manipulation and transformation. This example takes you through the process of creating a scenario that searches for a project and then returns all of the tasks associated with that project.
---

# Create a practice automation scenario

This article describes how to create an automation scenario with Adobe Workfront Fusion. Automation scenarios automate `Workfront` processes, including data manipulation and transformation. This example takes you through the process of creating a scenario that searches for a project and then returns all of the tasks associated with that project.

For instructions on building an integration scenario that connects separate apps, see [Create a practice integration scenario](../../workfront-fusion/get-started/create-a-practice-scenario.md).

For more information on functionality available with each `Workfront Fusion` license, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p><span>Pro</span> or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront Fusion</span> license**</td> 
   <td> <p><span>Workfront Fusion for Work Automation and Integration</span> </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <span>Adobe Workfront Fusion</span> as well as <span>Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

&#42;&#42;For information on `Adobe Workfront Fusion` licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Create a practice scenario

The role of `Adobe Workfront Fusion` is to seamlessly connect your apps and web services and automate your processes so that you can concentrate on new tasks rather than repeating the same tasks again and again. It works by linking actions within and between apps and services to create a scenario that transfers and transforms your data automatically. The scenario you create watches for data in an app or service and processes that data to provide the result you want.

A scenario is comprised of a series of modules that indicate how data should be transformed within an app or transferred between apps and web services.
This example takes you through the process of creating a scenario that searches for a `Workfront` project and returns the tasks in the project.

![](assets/create-practice-scenario-wf-only-350x157.png)

Creating a scenario consists of several main tasks:

## Choose the apps and name the scenario

<ol> 
 <li value="1">Sign into your <span>Workfront Fusion</span> account.</li> 
 <li value="2"> <p>Click <span class="bold">Scenarios</span> <img src="assets/scenarios-icon.png"> in the left panel.</p> <p>In the left panel that displays, you can organize your scenarios into folders.</p> <p>At the top of the main area to the right, you can view <span class="bold">All</span> scenarios you have built, your <span class="bold">Active Scenarios</span>, <span class="bold">Inactive Scenarios</span>, and <span class="bold">Concepts</span>. Concepts are scenarios that need some more work before <span>Workfront Fusion</span> can classify them as active or inactive.</p> <p> <img src="assets/scenarios-left-panel-350x215.png" style="width: 350;height: 215;"> </p> </li> 
 <li value="3">In the left panel, click the <span class="bold">Add folder</span> icon <img src="assets/add-folder-icon.png">, then type a name like "Practice scenarios" for your first folder.</li> 
 <li value="4"> <p>Open the folder, then click <span class="bold">Create a new scenario</span> in the upper-right corner of the page.</p> <p>The landing page that displays lets you pre-load any apps you want to use in the scenario you are going to build.</p> </li> 
 <li value="5"> <p>For this exercise, search for and select the <span class="bold">Workfront</span> app.</p> </li> 
 <li value="6"> <p>Click <span class="bold">Continue</span> in the upper-right corner.</p> <p>The scenario editor displays, containing an empty module in the center, the <span>Workfront</span> app you pre-loaded, and some options in the toolbar at the bottom.</p> <p> <img src="assets/scenario-editor-350x235.png" style="width: 350;height: 235;"> </p> <p>When you begin creating a new scenario, it's a good idea to start by creating a name for it. </p> </li> 
 <li value="7">Select the <span class="bold">New scenario</span> placeholder name in the upper-left corner, then type a name such as "Practice scenario 1."</li> 
 <li value="8">Continue with <a href="#build" class="MCXref xref">Add and configure the first module</a> below.</li> 
</ol>

## Add and configure the first module

The empty module with a question mark represents the trigger module you need to add. This module will start the scenario each time it runs. The clock icon on the empty module indicates that is a scheduled module.

![](assets/empty-module.png)

This module will contain the data that you want the scenario to watch for.

For this example, we are not using a trigger module. Instead, this scenario begins with a search.

<ol> 
 <li value="1"> <p>Click the empty module to choose the app from which you will select a module.</p> <p>The app you pre-loaded earlier displays next to the empty module. You can add any other apps that have modules using the Search box.</p> <p> <img src="assets/pre-loaded-app-wf-350x172.png" style="width: 350;height: 172;"> </p> </li> 
 <li value="2"> <p>Click <span class="bold"><span>Workfront</span></span>.</p> <p>The list changes to display all <span>Workfront</span> modules that you can use as a trigger module.</p> </li> 
 <li value="3"> <p>Click the Search module <span class="bold">Search</span>.</p> <p>Now you need to establish an authenticated connection to your <span>Workfront</span> account. Every module you add to a scenario must have a connection to its app.</p> </li> 
 <li value="4"> <p>In the <span class="bold"><span>Workfront</span></span> box, under <span class="bold">Connection</span>, click <span class="bold">Add</span>, then type a name for the connection, such as "Olivia's <span>Workfront</span> account," then click <span class="bold">Continue</span>.</p> </li> 
 <li value="5"> <p>Authenticate the connection in the window that displays.</p> <p>The process for authenticating a connection can vary a bit between apps. The following process is specific to <span>Workfront</span>, but the process is similar to many apps.</p> 
  <ol> 
   <li value="1"> <p>Enter your <span>Workfront</span> domain, then click <b>Continue</b>. </p> </li> 
   <li value="2"> <p>Log into <span>Workfront</span>.</p> </li> 
   <li value="3"> <p>Examine the access that <span>Workfront Fusion</span> is requesting, then click Allow Access.</p> </li> 
  </ol> <p> If you need help, see <a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref">About connecting Adobe Workfront Fusion to an app or service</a>.</p> </li> 
</ol>

## Configure the first module

After you connect `Workfront Fusion` to your `Workfront` account, you can specify a Workfront request queue that you have access to and the data there that you want the first module to process.

<ol> 
 <li value="1"> <p>In the Record Type box, select <b>Project</b>. This sets the module to search only projects.</p> <note type="tip">
   You can find 
   <span class="bold">Project</span> in the list if you start typing the word "project."
  </note> </li> 
 <li value="2"> <p>In the <span class="bold">Result Set</span> box, select <span class="bold">First Matching Record</span>. This sets the module to return only the first record it finds that meets the criteria. For this example, we need only one record returned. </p> </li> 
 <li value="3"> <p>In the <span class="bold">Search criteria</span> area, we'll set up a filter to return the specific project.</p> 
  <ol> 
   <li value="1"> <p>In the first box under Search Criteria, select the field that you want to search the values of. For this example, select <b>Name</b>.</p> </li> 
   <li value="2"> <p>For the operator, select Contains (case insensitive). This allows the module to find projects with your chosen words in its name, even if you do not enter the entire name, or enter the name with the incorrect case (such as all caps).</p> </li> 
   <li value="3"> <p>In the last field under Search Criteria, enter a word or phrase that you know is in the name of the project you are searching for.</p> </li> 
  </ol> </li> 
 <li value="4"> <p>In the <b>Outputs</b> list, select the fields that you want the issue to output. For this example, select the <b>ID</b> and <b>Name</b> fields.</p> <note type="tip">
   You can use 
   <span class="bold">Command+F</span> (Mac OS) or 
   <span class="bold">Ctrl-F</span>(Windows OS) to find a field quickly.
  </note> </li> 
 <li value="5"> <p>Click <span class="bold">OK</span>.</p> <note type="note"> 
   <p>(Information only) Since this is not a trigger module, you do not choose where to start it. When using a trigger module, you would now select where to start it. </p> 
   <p>For more information, see <a href="../../workfront-fusion/modules/choose-where-trigger-module-starts.md" class="MCXref xref">Choose where a trigger module starts</a>.</p> 
  </note> </li> 
 <li value="6"> <p>Right-click the module, click <span class="bold">Rename</span>, then type a name the describes what you want the module to do (such as "Search for project)," then click <span class="bold">OK</span>.</p> <p>The name appears just below the module. Below that, <span>Workfront Fusion</span> includes a brief description of the type of action performed by the module.</p> <p> <img src="assets/module-renamed-wf.png"> </p> </li> 
 <li value="7">Continue with <a href="#configur" class="MCXref xref">Add and configure the second module</a>.</li> 
</ol>

## Add and configure the second module

<ol data-mc-continue="false"> 
 <li value="1"> <p>Click the partial circle to the right of the of the module to <span class="bold">Add another module</span>.</p> </li> 
 <li value="2"> <p>Select <span>Workfront</span> from the list of applications, then choose the search module <b>Read Related Records</b>.</p> </li> 
 <li value="3"> <p>You already created a connection to <span>Workfront</span> for the previous module. You don't need to create it again here, but you must make sure this module is using the same connection as the previous module. <br>In the <b>Connection</b> box, select the connection that you created for the previous module.</p> </li> 
 <li value="4"> <p> Click <span class="bold">Record type</span>, then select <span class="bold">Project</span>, because we want to read records related to a project.</p> <note type="tip">
   You can find 
   <span class="bold">Project</span> in the list if you start typing the word "project."
  </note> </li> 
 <li value="5"> <p>Click the <span class="bold">Parent Record ID</span> field. This field requires the <span>Workfront</span> ID&nbsp;of the project that you want to return tasks from.</p> <p>Clicking the field opens the list of variables that you can use in the <span class="bold">Parent Record ID</span> field to identify the project in <span>Workfront</span>.</p> <p> <img src="assets/list-of-available-variables-wf-350x368.png" style="width: 350;height: 368;"> </p> </li> 
 <li value="6"> <p>Click the variable <span class="bold">ID</span> to add it to the <span class="bold">Parent Record ID</span> field. This allows the ID&nbsp;returned from the first module to be used as the identifier for the project that you want to work with in the second module, which ensures that the tasks returned will belong to that project.</p> </li> 
 <li value="7"> <p>In the <b>Collections</b> field, select <b>Tasks</b>. This indicates that the module is to return tasks associated with the chosen project.</p> </li> 
 <li value="8"> <p>Click <span class="bold">OK</span></p> <p>Now you have a working scenario.</p> </li> 
 <li value="9">Give the second module a name such as "Return tasks associated with project," then continue with <a href="#test" class="MCXref xref">Test the scenario</a>.</li> 
</ol>

## Test the scenario

Before you activate your scenario, it's important to test it by running it at least once and viewing the results. This helps you understand how data flows through the scenario and find any errors.

We chose to have 1 project returned, as well as the tasks associated with that project. If you run the scenario, that is what should happen.

<ol> 
 <li value="1"> <p>Click <span class="bold">Run once</span> in the lower-left corner of the scenario editor.</p> </li> 
 <li value="2"> <p>After the scenario finishes running, click the bubble above the first module.</p> <p> <img src="assets/click-bubble.png"> </p> <p>In the box that appears, you can view information about the bundle of data that the module processed, including the actual data that was pulled from the project that the module returned.</p> <p> <img src="assets/execution-inspector-wf-only-first-350x423.png" style="width: 350;height: 423;"> </p> </li> 
 <li value="3"> <p>Click the execution inspector bubble above the Second module to see the input of information and the output, which is a collection of tasks contained in the project.</p> <p> <img src="assets/execution-inspector-wf-only-second-350x738.png" style="width: 350;height: 738;"> </p> <p>You can learn more about how to read scenario execution information in the following articles:</p> 
  <ul> 
   <li>For general information, see <a href="../../workfront-fusion/scenarios/scenario-execution-flow.md" class="MCXref xref">Scenario execution flow</a>.</li> 
   <li>For information about processed bundles, see <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Scenario execution, cycles, and phases</a>.</li> 
  </ul> </li> 
 <li value="4"> <p>In <span>Workfront Fusion</span>, click <span class="bold">Save </span><img src="assets/save-icon.png"> near the lower-left corner to save your progress on the scenario.</p> <note type="important">
   Save often as you hone and test a scenario.
  </note> </li> 
</ol>

` `**Tip: **`` We recommend the optional but useful practice of adding notes about each module.

<ol> 
 <li value="1">Right-click a <span>Workfront</span> module, then click <span class="bold">Add a note</span>.</li> 
 <li value="2"> <p>In the note that displays, type an overview for the module.</p> <p>You can add multiple notes for a module.</p> </li> 
 <li value="3"> <p>Close the <span class="bold">Notes</span> area.</p> <p>After you add a note to a scenario, an orange dot displays on the <span class="bold">Notes</span> icon <img src="assets/notes-icon-w-dot.png"> at the bottom of the scenario editor.</p> </li> 
 <li value="4">Click the <span class="bold">Notes</span> icon <img src="assets/notes-icon-w-dot.png"> to view your notes.</li> 
</ol>

## Activate the scenario

This example scenario does not have a trigger module. If this were a scenario you would be using for real data it would start with a trigger module, and the last thing you would do is activate it. After you activate a scenario, by default, it runs every 15 minutes. You can change this by defining when and how often you want it to run.

For more information about activating scenarios, see [Activate or deactivate a scenario](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

For information about schedules, see [Schedule a scenario](../../workfront-fusion/scenarios/schedule-a-scenario.md).
