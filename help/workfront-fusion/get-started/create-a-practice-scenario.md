---
filename: create-a-practice-scenario
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Create a practice integration scenario
description: This article describes how to create an integration scenario with Adobe Workfront Fusion. Integration scenarios connect separate apps together, allowing your data to flow through different applications.
---

# Create a practice integration scenario

This article describes how to create an integration scenario with Adobe Workfront Fusion. Integration scenarios connect separate apps together, allowing your data to flow through different applications.

To create an integration scenario, your organization must have a Workfront Fusion for Work Automation and Integration license.

For instructions on building a Workfront-only automation scenario, see [Create a practice automation scenario](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

For more information on Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Create a practice scenario

The role of Adobe Workfront Fusion is to seamlessly connect your apps and web services and automate your processes so that you can concentrate on new tasks rather than repeating the same tasks again and again. It works by linking actions within and between apps and services to create a scenario that transfers and transforms your data automatically. The scenario you create watches for data in an app or service and processes that data to provide the result you want.

A scenario is comprised of a series of modules that indicate how data should be transformed within an app or transferred between apps and web services.
To explain how to create a scenario and reinforce best practices as you learn to use Workfront Fusion, this article takes you through the process step-by-step. We will create a scenario that creates a new record in Workfront for every row in a Google Sheets spreadsheet.

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>A scenario like this would be useful if you had a spreadsheet listing projects that need to be worked on using projects in Workfront. The scenario could "watch" the spreadsheet for new rows and add a new project in Workfront for each one.

Creating a scenario consists of several main tasks:

## Choose the apps and name the scenario

<ol> 
 <li value="1"> <p>Download this <a href="https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx">spreadsheet</a>, then upload it to your Google Drive for use throughout this exercise.</p> <p>Or</p> <p>Create or find your own simple Google Sheets spreadsheet similar to this one:</p> <p> <img src="assets/spreadsheet-headers-350x55.png" style="width: 350;height: 55;"> </p> </li> 
 <li value="2">Sign into your Workfront Fusion account.</li> 
 <li value="3"> <p>Click <span class="bold">Scenarios</span> <img src="assets/scenarios-icon.png"> in the left panel.</p> <p>In the left panel that displays, you can organize your scenarios into folders.</p> <p>At the top of the main area to the right, you can view <span class="bold">All</span> scenarios you have built, your <span class="bold">Active Scenarios</span> and <span class="bold">Inactive Scenarios</span>, and <span class="bold">Concepts</span>, which are scenarios that need some more work before Workfront Fusion can classify them as active or inactive.</p> <p> <img src="assets/scenarios-left-panel-350x215.png" style="width: 350;height: 215;"> </p> </li> 
 <li value="4">In the left panel, click the <span class="bold">Add folder</span> icon <img src="assets/add-folder-icon.png">, then type a name like "Practice scenarios" for your first folder.</li> 
 <li value="5"> <p>Open the folder, then click <span class="bold">Create a new scenario</span> in the upper-right corner of the page.</p> <p>The landing page that displays lets you pre-load any apps you want to use in the scenario you are going to build.</p> </li> 
 <li value="6"> <p>For this exercise, search for and select the <span class="bold">Google Sheets</span> app.</p> </li> 
 <li value="7"> <p>Click <span class="bold">Continue</span> in the upper-right corner.</p> <p>The scenario editor displays, containing an empty module in the center, the Google Sheets app you pre-loaded, and some options in the toolbar at the bottom.</p> <p> <img src="assets/scenario-editor-350x235.png" style="width: 350;height: 235;"> </p> <p>When you begin creating a new scenario, it's a good idea to start by creating a name for it. </p> </li> 
 <li value="8">Select the <span class="bold">New scenario</span> placeholder name in the upper-left corner, then type a name such as "Practice scenario 1."</li> 
 <li value="9">Continue with <a href="#build" class="MCXref xref">Add and configure the first module</a> below.</li> 
</ol>

## Add and configure the first module

The empty module with a question mark represents the trigger module you need to add. This module will start the scenario each time it runs. The clock icon on the empty module indicates that is a scheduled module.

![](assets/empty-module.png)

This module will contain the data that you want the scenario to watch for.

<ol> 
 <li value="1"> <p>Click the empty module to choose the app from which you will select a module.</p> <p>The app you pre-loaded earlier displays next to the empty module. You can add any other apps that have modules using the Search box.</p> <p> <img src="assets/pre-loaded-apps-350x139.png" style="width: 350;height: 139;"> </p> </li> 
 <li value="2"> <p>Click <span class="bold">Google Sheets</span>.</p> <p>The list changes to display all Google Sheets modules that you can use as a trigger module.</p> </li> 
 <li value="3"> <p>Click the trigger module <span class="bold">Watch for Records</span>.</p> <p>Now you need to establish an authenticated connection to your Google account. Every module you add to a scenario must have a connection to its app.</p> </li> 
 <li value="4"> <p>In the <span class="bold">Google Sheets</span> box, under <span class="bold">Connection</span>, click <span class="bold">Add</span>, then type a name for the connection, such as "Olivia's Google account," then click <span class="bold">Continue</span>.</p> </li> 
 <li value="5"> <p>Authenticate the connection in the window that displays.</p> <p>The process for authenticating a connection can vary a bit between apps. You may need to log in to the app. You will usually need to click an <span class="bold">Allow</span> button. If you need help, see <a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref">About connecting Adobe Workfront Fusion to an app or service</a>.</p> </li> 
</ol>

## Configure the first module

After you connect Workfront Fusion to your Google Sheets account, you can specify a Google Sheets spreadsheet that you have access to and the data there that you want the first module to process.

<ol> 
 <li value="1"> <p>Click the <span class="bold">Spreadsheet</span> box, then select the <span class="bold">Workfront Fusion practice scenario #1</span> spreadsheet in the list that appears.</p> <p>This spreadsheet contains 2 sheets (tabs), so we need to specify which sheet contains the data we want:</p> </li> 
 <li value="2"> <p>In the <span class="bold">Sheet</span> drop-down list, select <span class="bold">Projects</span>.</p> <p>Our spreadsheet contains headers and we want the module to use them to identify the data we want to process:</p> <p> <img src="assets/spreadsheet-headers-350x55.png" style="width: 350;height: 55;"> </p> </li> 
 <li value="3">Leave <span class="bold">Yes</span> selected for <span class="bold">Table contains headers</span>.</li> 
 <li value="4">In the <span class="bold">Row with headers</span> box, you could specify a range of rows that you want to include, but let's leave the default A1:Z1 there for this exercise.</li> 
 <li value="5"> <p> In the <span class="bold">Limit</span> box, type 1.</p> <p>This way, every time you run the scenario, the module will process only 1 row in the spreadsheet. This is useful for simplifying your test runs while you are building the scenario.</p> </li> 
 <li value="6"> <p>Click <span class="bold">OK</span>.</p> <p>The <span class="bold">Choose where to start</span> box prompts you to specify where in the spreadsheet you want the module to start processing.</p> </li> 
 <li value="7"> <p>Click <span class="bold">Choose manually</span>, select the top option in the list that appears, then click <span class="bold">OK</span>.</p> </li> 
 <li value="8"> <p>Right-click the module, click <span class="bold">Rename</span>, then type a name the describes what you want the module to do (such as "Watch the project list)," then click <span class="bold">OK</span>.</p> <p>The name appears just below the module. Below that, Workfront Fusion includes a brief description of the type of action performed by the module.</p> <p> <img src="assets/module-renamed-350x388.png" style="width: 350;height: 388;"> </p> </li> 
 <li value="9">Continue with <a href="#configur" class="MCXref xref">Add and configure the second module</a>.</li> 
</ol>

## Add and configure the second module

<ol data-mc-continue="false"> 
 <li value="1"> <p>Click the partial circle to the right of the of the module to <span class="bold">Add another module</span>.</p> <p>This second module needs to be a Workfront module, but we didn't pre-load the Workfront app.</p> </li> 
 <li value="2"> <p>To find the Workfront app, start typing "workfront" and click the app when it appears.</p> </li> 
 <li value="3"> <p>In the list of Workfront modules that appears, click<span class="bold"> Create Record</span>.</p> <note type="important">
   As you continue these steps, don't click outside the Workfront box until you click OK in step 10. Clicking away from the box cancels the work you've done inside it.
  </note> </li> 
 <li value="4"> <p>As you did before with the Google Sheets app, click <span class="bold">Add</span> in the Workfront box to add a connection between Workfront Fusion and Workfront.</p> <p>Now we will start specifying what we want to do with the data from the spreadsheet.</p> </li> 
 <li value="5"> <p> Click <span class="bold">Record type</span>, then select <span class="bold">Project</span> because we want to create a project in Workfront using a row from the spreadsheet.</p> <note type="tip">
   You can easily find 
   <span class="bold">Project</span> in the list if you start typing the word "project."
  </note> <p>The box expands to display all of the available Workfront project fields where you can put the information found by the first module.</p> <p>We're going to use the <span class="bold">Name</span> field: we want this module to name each project in Workfront using the text in the corresponding Google Sheets row.</p> </li> 
 <li value="6"> <p>Find and click the <span class="bold">Name</span> field.</p> <note type="tip">
   You can use 
   <span class="bold">Command+F</span> (Mac OS) or 
   <span class="bold">Ctrl-F</span>(Windows OS) to find a field quickly.
  </note> <p>This opens the list of variables that you can use in the <span class="bold">Name</span> field to define the name for each project created in Workfront.</p> <p> <img src="assets/list-of-available-variables-350x261.png" style="width: 350;height: 261;"> </p> <p>Notice that the variables near the top of the list correspond to the column headers in the spreadsheet.</p> <p> <img src="assets/spreadsheet-headers-marked-350x55.png" style="width: 350;height: 55;"> </p> <p> <img src="assets/list-of-available-variables-marked-350x320.png" style="width: 350;height: 320;"> </p> </li> 
 <li value="7"> <p>Click the variable <span class="bold">My Project Name (A)</span> to add it to the <span class="bold">Name</span> field.</p> <p>You have just mapped your first piece of data for this scenario.</p> <p>Let's map one more piece of data from the spreadsheet to Workfront: the start date for each project.</p> </li> 
 <li value="8">Find and click the <span class="bold">Planned Start Date</span> field, then click the <span class="bold">Planned Begin Date (E)</span> variable, to pull data from that column in the spreadsheet.</li> 
 <li value="9"> <p>Click <span class="bold">OK</span> (and note again how important this step is).</p> <p>Now you have a working scenario.</p> </li> 
 <li value="10">Give the second module a name such as "Create Workfront project," then continue with <a href="#test" class="MCXref xref">Test the scenario</a>.</li> 
</ol>

## Test the scenario

Before you activate your scenario, it's important to test it by running it at least once and viewing the results. This helps you understand how data flows through the scenario and find any errors.

We chose to have 1 row from the spreadsheet processed to create a project in Workfront. If you run the scenario, that is what should happen.

<ol> 
 <li value="1"> <p>Click <span class="bold">Run once</span> in the lower-left corner of the scenario editor.</p> </li> 
 <li value="2"> <p>After the scenario finishes running, click the bubble above the Google Sheets module.</p> <p> <img src="assets/click-bubble.png"> </p> <p>In the box that appears, you can view information about the bundle of data that the module processed, including the actual data that was pulled from the spreadsheet for the row you started with.</p> <p> <img src="assets/execution-inspector-g-sheets-350x637.png" style="width: 350;height: 637;"> </p> </li> 
 <li value="3"> <p>Click the execution inspector bubble above the Workfront module to see the input of information and the output, which is the ID of the project now created in Workfront</p> <p> <img src="assets/execution-inspector-wf-350x384.png" style="width: 350;height: 384;"> </p> <p>You can learn more about how to read scenario execution information in the following articles:</p> 
  <ul> 
   <li>For general information, see <a href="../../workfront-fusion/scenarios/scenario-execution-flow.md" class="MCXref xref">Scenario execution flow</a>.</li> 
   <li>For information about processed bundles, see <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Scenario execution, cycles, and phases</a>.</li> 
  </ul> </li> 
 <li value="4"> <p>Go to Workfront and search for "soho downtown loft" to see the project that the scenario created. This was the last row in the spreadsheet.</p> </li> 
 <li value="5"> <p>In Workfront Fusion, click <span class="bold">Save </span><img src="assets/save-icon.png"> near the lower-left corner to save your progress on the scenario.</p> <note type="important">
   Save often as you hone and test a scenario.
  </note> </li> 
</ol>

## Finalize the scenario and test it again

We still need to configure the scenario to create projects for all the other rows in the spreadsheet.

<ol> 
 <li value="1">Click the <span class="bold">Watch Rows</span> module you created for Google Sheets.</li> 
 <li value="2"> <p>Change the <span class="bold">Limit</span> to 100.</p> <p>Specifying a number higher than the number of rows you know are are in the spreadsheet assures that the scenario will capture all of them.</p> </li> 
 <li value="3">Right-click the <span class="bold">Watch Rows</span> module, click <span class="bold">Choose where to start</span>, click <span class="bold">All</span>, then click <span class="bold">OK</span>.</li> 
 <li value="4"> <p>Click <span class="bold">Run once</span> and watch what happens in the execution inspector bubbles.</p> <p>The Google Sheets <span class="bold">Watch Rows</span> module runs once to read all of the rows. Then the Workfront <span class="bold">Create Record</span> module runs 20 times to create a project for each of the remaining 20 rows in the spreadsheet.</p> </li> 
 <li value="5"> <p>Click the execution inspector bubble for the Workfront module to view all 20 operations, then click one of the operations to view the information about the project created.</p> </li> 
 <li value="6"> <p>Click <span class="bold">Save </span><img src="assets/save-icon.png"> near the lower-left corner.</p> </li> 
 <li value="7">Go to Workfront to see the projects that the scenario created.</li> 
</ol>

` `**Tip: **`` We recommend the optional but useful practice of adding notes about each module.

<ol> 
 <li value="1">Right-click the Workfront module, then click <span class="bold">Add a note</span>.</li> 
 <li value="2"> <p>In the note that displays, type an overview for the module.</p> <p>This is helpful because you won't have to continually open the module to see what it does. You could type something like "Creates a project with Name, Planned Start Date, and Priority mapped from spreadsheet."</p> <p>For the Google Sheets module, you could type something like "Watch Project List for new rows/projects added."</p> <p>You can add multiple notes for a module.</p> </li> 
 <li value="3"> <p>Close the <span class="bold">Notes</span> area.</p> <p>After you add a note to a scenario, an orange dot displays on the <span class="bold">Notes</span> icon <img src="assets/notes-icon-w-dot.png"> at the bottom of the scenario editor.</p> </li> 
 <li value="4">Click the <span class="bold">Notes</span> icon <img src="assets/notes-icon-w-dot.png"> to view your notes.</li> 
</ol>

## Activate the scenario

If this were a scenario you would be using for real data, the last thing you would do is activate it. After you activate a scenario, by default, it runs every 15 minutes. You can change this by defining when and how often you want it to run.

For more information about activating scenarios, see [Activate or deactivate a scenario](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

For information about schedules, see [Schedule a scenario](../../workfront-fusion/scenarios/schedule-a-scenario.md).
