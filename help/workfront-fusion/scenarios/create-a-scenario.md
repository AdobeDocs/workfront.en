---
filename: create-a-scenario
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Create a scenario
description: The following tasks explain how to create a Adobe Workfront Fusion scenario.
---

# Create a scenario

The following tasks explain how to create a *Adobe Workfront Fusion* scenario.

For a practice exercise that walks you through this process using data that we provide, see [Create a practice integration scenario](../../workfront-fusion/get-started/create-a-practice-scenario.md).

>[!NOTE]
>
>To create a scenario from a template, see [Create scenarios with Adobe Workfront Fusion templates](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p><em>Pro</em> or higher</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
    <td> <p>Plan, Work</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront Fusion</em> license**</td> 
   <td> <p><em>Workfront Fusion for Work Automation and Integration</em> </p> <draft-comment>
     <p data-mc-conditions="SnippetConditions.HIDE"><em>Workfront Fusion for Work Automation</em> </p>
    </draft-comment><p data-mc-conditions="SnippetConditions.HIDE"><em>Workfront Fusion for Work Automation</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <em>Adobe Workfront Fusion</em> as well as <em>Adobe Workfront</em> to use functionality described in this article.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

&#42;&#42;For information on *Adobe Workfront Fusion* licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Begin creating a scenario

<ol> 
 <li value="1">Click <span class="bold">Scenarios</span> <img src="assets/scenarios-icon.png"> in the left panel.</li> 
 <li value="2"> <p>Click <span class="bold">Create a new scenario</span> in the upper-right corner of the page. </p> </li> 
 <li value="3"> <p>(Optional) Under <span class="bold">What services do you want to integrate</span>, if you are creating a new scenario, select apps you want to work with in the scenario, then click <span class="bold">Continue</span>.</p> <p>Or</p> <p>Click <span class="bold">Skip</span> if you want to choose the apps from within the scenario editor.</p> </li> 
 <li value="4">In the screen that appears (the scenario editor), if you are creating a new scenario, click <span class="bold">New scenario</span> in the upper-left corner and type a name for the scenario.</li> 
 <li value="5">Continue on to <a href="#add" class="MCXref xref">Add a module in a scenario</a>.</li> 
</ol>

## Add a module in a scenario

<ol> 
 <li value="1"> <p>To add the first module to the scenario, click the question mark icon. <img src="assets/question-mark-icon.gif"></p> <p>Or</p> <p>To add additional modules to the scenario, click the handle on the right side of the module you want it to follow.</p> </li> 
 <li value="2"> <p>In the box that displays, find and click the app or service that you want to start with.</p> <p>If you selected any apps in step 2, they are displayed in the box for easy access (and in the <span class="bold">Favorites</span> section at the bottom of the screen).</p> <p>If you click <span class="bold">Add another module</span>, the modules that display depend on where in the scenario you are adding the module. Some modules can be placed only in between other modules, and others only at the beginning of the scenario. </p> <note type="tip">
   The two most common types of modules are actions and triggers. For more information, see 
   <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Types of modules</a>.
  </note> </li> 
 <li value="3"> <p>In the list of modules that displays, click the first module you want to add to the scenario.</p> <p>The modules that display depend on where you want to add a module in your scenario. Some modules can be placed only in between other modules, and others only at the beginning of the scenario. </p> <p>The two most common types of modules are actions and triggers. For more information, see <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Types of modules</a>.</p> </li> 
 <li value="4">Continue on to <a href="#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a>.</li> 
</ol>

## Connect the module's app or web service to *Workfront Fusion*

Workfront Fusion modules that connect to an app (such as Workfront, Salesforce, or Jira) feature the Connection field. Here, you can specify the connection that you want this module to use to connect to the app. You can select an existing connection from the dropdown, or create a new connection.

When you select or create a connection for an app in a scenario, other modules for that app automatically use the same connection unless you select a different one when setting up the later modules.

For more information, see [About connecting Adobe Workfront Fusion to an app or service](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

![](assets/connection-field-350x169.png)

To create a connection inside a *Workfront Fusion* module:

1. Click `Add` to open the `Create a connection` box.
1. (Optional) Change the default `Connection name`.
1. (Conditional) If the app requires advanced connection settings, such as an ID, key, or secret, enter that information.

   You might need to click `Show advanced settings` to display the fields where you can enter this kind of information.

1. Click `Continue`.
1. In the sign-in window that displays, enter your credentials to log in to the app if you haven't already done so.
1. (Conditional) If an `Allow` button displays, examine the actions that the connector will be able to take, then click the button to connect the app to *Workfront Fusion*.

   <!--
   <li value="7" data-mc-conditions="SnippetConditions.HIDE">Continue on to <a href="#configur" class="MCXref xref">Configure the module</a>.</li>
   -->

1. Continue on to [Configure the module](#configur).

## Configure the module

<ol> 
 <li value="1"> <p>In the fields below the Connection field, configure the settings for the module, then click <span class="bold">OK</span>.</p> <p> <img src="assets/conf-settigs-mod-350x547.png" style="width: 350;height: 547;"> </p> <p>These settings are different for every module. A bolded title indicates a required setting.</p> 
  <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
   <span class="autonumber"><span><b>Tip: </b></span></span> 
   <p>As you work on your scenario, you can click the module to display this box of settings at any time. </p> 
   <p>If you see a black circle on a module, you haven't finished configuring its settings. Click the module to open it and continue configuring. </p> 
   <p> <img src="assets/black-error-circle-on-module.png"> </p> 
  </div> </li> 
 <li value="2"> <p>If you are adding the first module in your scenario, select an option to indicate where you want the scenario to start each time it runs.</p> <p> <img src="assets/choose-where-start-350x194.png" style="width: 350;height: 194;"> </p> </li> 
 <li value="3">Repeat the steps in the sections <a href="#add" class="MCXref xref">Add a module in a scenario</a> and <a href="#configur" class="MCXref xref">Configure the module</a> to add other modules to the scenario.</li> 
 <li value="4"> <p>(Optional) Copy and paste a module or group of modules.</p> <p>For more information, see <a href="../../workfront-fusion/scenarios/copy-modules-or-scenarios.md" class="MCXref xref">Copy modules or scenarios</a>.</p> </li> 
 <li value="5">Continue on to <a href="#configur2" class="MCXref xref">Configure and work with your scenario</a>.</li> 
</ol>

## Configure and work with your scenario

<ol> 
 <li value="1"> <p> Do any of the following to configure your scenario:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Specify when and how often the scenario will execute</td> 
     <td> <p>Click the clock icon. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>For more information, see <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Schedule a scenario</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Set up a route</td> 
     <td> <p>Click the wrench icon <img src="assets/wrench-icon.gif"> between the two modules and use any of the following options. For more information, see <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Add a filter to a scenario</a>.</p> 
      <ul> 
       <li><span class="bold">Set up a filter</span>: Control which bundles are used at certain points in the scenario.</li> 
       <li><span class="bold">Unlink</span>: Removes a route.</li> 
       <li><span class="bold">Add a router</span>: Adds a router between modules. </li> 
       <li><span class="bold">Add a module</span>: Adds a new module between modules.</li> 
       <li><span class="bold">Add a note</span>: Adds a note to the route.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Configure the scenario settings</td> 
     <td>Click the Scenario settings icon. <img src="assets/gear-icon-settings.png"> These settings are intended primarily for advanced users. For more information, see <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Scenario settings panel</a>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Configure Flow Control settings</td> 
     <td> <p>Click the Flow Control icon. <img src="assets/flow-control-icon.gif"> You can set a task to repeat a given number of times, convert an array into a series of bundles, and merge several bundles into one single bundle. For more information, see <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Flow control</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Enhance the scenario using advanced tools</td> 
     <td>Click the Tools icon. <img src="assets/tools-icon.gif"> You can create triggers, actions, aggregators, and transformers. For more information, see <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Tools</a>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">User text parsing tools</td> 
     <td>Click the Text parser icon <img src="assets/text-parser-icon.gif">. You can retrieve elements from HTML code, find and extract string elements matching a search pattern, search and replace text, and "scrape" data from a website. For more information, see <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Tools</a>.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="2"> <p>Do any of the following to work with your scenario:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">View a log of the events that occur when the scenario runs</td> 
     <td> <p>Click the Exit editing arrow <img src="assets/exit-editing-arrow.png"> in the scenario editor to view the Scenario detail page. The log displays at the bottom of the window, or in the lower-right corner. It contains information about the difficulty of each phase and any errors encountered during the execution of the scenario.</p> <p>To return to working with your scenario in the scenario editor, click anywhere on the Scenario detail page.</p> <p>For more information about the Scenario detail page, see <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Scenario detail</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Access your most commonly used apps and services</td> 
     <td> Click an icon in the <span class="bold">Favorites</span> section at the bottom of the screen. Icons display in this section automatically as you add apps and services to your scenario. You can also click the Add icon <img src="assets/add-icon.gif"> to add apps and services to this area manually.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">View an animation showing how data flows through the scenario</td> 
     <td>Click the Explain flow icon <img src="assets/explain-flow-airplane-icon.gif">.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Auto-align the layout of the modules </td> 
     <td>Click the Auto-align icon <img src="assets/auto-align-icon.gif">.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Type or view notes about the scenario</td> 
     <td>Click the Notes icon <img src="assets/notes-icon.gif">.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Remove a module</td> 
     <td>Right-click the module, then click <span class="bold">Delete module</span>.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="3"> <p>To test-run the scenario, click <span class="bold">Run once</span>.</p> <p>It's important to verify that the scenario runs as you expect before you activate it. Once activated, the scenario will execute according to its schedule. If everything does not run as expected, see <a href="../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Error handling</a>.</p> </li> 
 <li value="4"> <p>When you finish editing the scenario (or at any time while you are editing), click the Save icon at the bottom of the window <img src="assets/save-icon.gif">.</p> </li> 
</ol>

For information about activating a scenario, see [Activate or deactivate a scenario](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

## *Workfront Fusion* scenario keyboard shortcuts

You can use the following keyboard shortcuts when creating or editing a scenario:

<table cellspacing="0"> <draft-comment>
  <col data-mc-conditions="">
 </draft-comment>
 <col data-mc-conditions=""> <draft-comment>
  <col data-mc-conditions="">
 </draft-comment>
 <col data-mc-conditions=""> <draft-comment>
  <col data-mc-conditions="">
 </draft-comment>
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p>Action</p> </th> 
   <th>Windows</th> 
   <th> <p>MacOS</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Save </td> 
   <td>Ctrl+Shift+S</td> 
   <td><span style="font-weight: normal;">Cmd+Shift+S</span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Run Once</td> 
   <td>Ctrl+Shift+Enter</td> 
   <td><span style="font-weight: normal;">Cmd+Shift+Enter</span> </td> 
  </tr> 
 </tbody> 
</table>

