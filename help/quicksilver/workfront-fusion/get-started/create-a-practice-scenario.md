---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Create a practice integration scenario in Adobe Workfront Fusion
description: This article describes how to create an integration scenario with Adobe Workfront Fusion. Integration scenarios connect separate apps together, allowing your data to flow through different applications.
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
---
# Create a practice integration scenario in Adobe Workfront Fusion

This article describes how to create an integration scenario with Adobe Workfront Fusion. Integration scenarios connect separate apps together, allowing your data to flow through different applications.

To create an integration scenario, your organization must have a Workfront Fusion for Work Automation and Integration license.

For instructions on building a Workfront-only automation scenario, see [Create a practice automation scenario in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

For more information on Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

>[!NOTE]
>
>Your organization may not allow access to Google Sheets. If that is the case, you will not be able to set up this integration, but the information presented here can be used as a general example of how integration scenarios function.

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Create a practice scenario

The role of Adobe Workfront Fusion is to automate your processes so that you can concentrate on new tasks rather than repeating the same tasks again and again. It works by linking actions within and between apps and services to create a scenario that transfers and transforms your data automatically. The scenario you create watches for data in an app or service and processes that data to provide the result you want.

A scenario is comprised of a series of modules that indicate how data should be transformed within an app or transferred between apps and web services.

To explain how to create a scenario and reinforce best practices as you learn to use Workfront Fusion, this article takes you through the process step-by-step. We will create a scenario that creates a new record in Workfront for every row in a Google Sheets spreadsheet.

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>A scenario like this would be useful if you had a spreadsheet listing projects that need to be worked on using projects in Workfront. The scenario could "watch" the spreadsheet for new rows and add a new project in Workfront for each one.

Creating a scenario consists of several main tasks:

## Choose the apps and name the scenario

1. Download this [spreadsheet](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx), then upload it to your Google Drive for use throughout this exercise.

   Or

   Create or find your own simple Google Sheets spreadsheet similar to this one:

   ![](assets/spreadsheet-headers-350x55.png)

1. Sign into your Workfront Fusion account.
1. Click **Scenarios** ![](assets/scenarios-icon.png) in the left panel.

   In the left panel that displays, you can organize your scenarios into folders.

   At the top of the main area to the right, you can view **All** scenarios you have built, your **Active Scenarios** and **Inactive Scenarios**, and **Concepts**, which are scenarios that need some more work before Workfront Fusion can classify them as active or inactive.

   ![](assets/scenarios-left-panel-350x215.png)

1. In the left panel, click the **Add folder** icon ![](assets/add-folder-icon.png), then type a name like "Practice scenarios" for your first folder.

1. Open the folder, then click **Create a new scenario** in the upper-right corner of the page.

   The landing page that displays lets you pre-load any apps you want to use in the scenario you are going to build.

1. For this exercise, search for and select the **Google Sheets** app.
1. Click **Continue** in the upper-right corner.

   The scenario editor displays, containing an empty module in the center, the Google Sheets app you pre-loaded, and some options in the toolbar at the bottom.

   ![](assets/scenario-editor-350x235.png)

   When you begin creating a new scenario, it's a good idea to start by creating a name for it. 

1. Select the **New scenario** placeholder name in the upper-left corner, then type a name such as "Practice scenario 1."
1. Continue with [Add and configure the first module](#add-and-configure-the-first-module) below.

## Add and configure the first module {#add-and-configure-the-first-module}

The empty module with a question mark represents the trigger module you need to add. This module will start the scenario each time it runs. The clock icon on the empty module indicates that is a scheduled module.

![](assets/empty-module.png)

This module will contain the data that you want the scenario to watch for.

1. Click the empty module to choose the app from which you will select a module.

   The app you pre-loaded earlier displays next to the empty module. You can add any other apps that have modules using the Search box.

   ![](assets/pre-loaded-apps-350x139.png)

1. Click **Google Sheets**.

   The list changes to display all Google Sheets modules that you can use as a trigger module.

1. Click the trigger module **Watch for Records**.

   Now you need to establish an authenticated connection to your Google account. Every module you add to a scenario must have a connection to its app.

1. In the **Google Sheets** box, under **Connection**, click **Add**, then type a name for the connection, such as "Olivia's Google account," then click **Continue**.
1. Authenticate the connection in the window that displays.

   The process for authenticating a connection can vary a bit between apps. You may need to log in to the app. You will usually need to click an **Allow** button. If you need help, see [About connecting Adobe Workfront Fusion to an app or service](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Configure the first module

After you connect Workfront Fusion to your Google Sheets account, you can specify a Google Sheets spreadsheet that you have access to and the data there that you want the first module to process.

1. Click the **Spreadsheet** box, then select the **Workfront Fusion practice scenario #1** spreadsheet in the list that appears.

   This spreadsheet contains 2 sheets (tabs), so we need to specify which sheet contains the data we want:

1. In the **Sheet** drop-down list, select **Projects**.

   Our spreadsheet contains headers and we want the module to use them to identify the data we want to process:

   ![](assets/spreadsheet-headers-350x55.png)

1. Leave **Yes** selected for **Table contains headers**.

1. In the **Row with headers** box, you could specify a range of rows that you want to include, but let's leave the default A1:Z1 there for this exercise.
1. In the **Limit** box, type 1.

   This way, every time you run the scenario, the module will process only 1 row in the spreadsheet. This is useful for simplifying your test runs while you are building the scenario.

1. Click **OK**.

   The **Choose where to start** box prompts you to specify where in the spreadsheet you want the module to start processing.

1. Click **Choose manually**, select the top option in the list that appears, then click **OK**.
1. Right-click the module, click **Rename**, then type a name the describes what you want the module to do (such as "Watch the project list)," then click **OK**.

   The name appears just below the module. Below that, Workfront Fusion includes a brief description of the type of action performed by the module.

   ![](assets/module-renamed-350x388.png)

1. Continue with [Add and configure the second module](#add-and-configure-the-second-module).

## Add and configure the second module {#add-and-configure-the-second-module}

1. Click the partial circle to the right of the of the module to **Add another module**.

   This second module needs to be a Workfront module, but we didn't pre-load the Workfront app.

1. To find the Workfront app, start typing "workfront" and click the app when it appears.
1. In the list of Workfront modules that appears, click**Create Record**.

   >[!IMPORTANT]
   >
   >As you continue these steps, don't click outside the Workfront box until you click OK in step 10. Clicking away from the box cancels the work you've done inside it.

1. As you did before with the Google Sheets app, click **Add** in the Workfront box to add a connection between Workfront Fusion and Workfront.

   Now we will start specifying what we want to do with the data from the spreadsheet.

1. Click **Record type**, then select **Project** because we want to create a project in Workfront using a row from the spreadsheet.

   >[!TIP]
   >
   >You can easily find **Project** in the list if you start typing the word "project."

   The box expands to display all of the available Workfront project fields where you can put the information found by the first module.

   We're going to use the **Name** field: we want this module to name each project in Workfront using the text in the corresponding Google Sheets row.

1. Find and click the **Name** field.

   >[!TIP]
   >
   >You can use **Command+F** (Mac OS) or **Ctrl-F**(Windows OS) to find a field quickly.

   This opens the list of variables that you can use in the **Name** field to define the name for each project created in Workfront.

   ![](assets/list-of-available-variables-350x261.png)

   Notice that the variables near the top of the list correspond to the column headers in the spreadsheet.

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. Click the variable **My Project Name (A)** to add it to the **Name** field.

   You have just mapped your first piece of data for this scenario.

   Let's map one more piece of data from the spreadsheet to Workfront: the start date for each project.

1. Find and click the **Planned Start Date** field, then click the **Planned Begin Date (E)** variable, to pull data from that column in the spreadsheet.

1. Click **OK** (and note again how important this step is).

   Now you have a working scenario.

1. Give the second module a name such as "Create Workfront project," then continue with [Test the scenario](#test-the-scenario).

## Test the scenario {#test-the-scenario}

Before you activate your scenario, it's important to test it by running it at least once and viewing the results. This helps you understand how data flows through the scenario and find any errors.

We chose to have 1 row from the spreadsheet processed to create a project in Workfront. If you run the scenario, that is what should happen.

1. Click **Run once** in the lower-left corner of the scenario editor.
1. After the scenario finishes running, click the bubble above the Google Sheets module.

   ![](assets/click-bubble.png)

   In the box that appears, you can view information about the bundle of data that the module processed, including the actual data that was pulled from the spreadsheet for the row you started with.

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. Click the execution inspector bubble above the Workfront module to see the input of information and the output, which is the ID of the project now created in Workfront

   ![](assets/execution-inspector-wf-350x384.png)

   You can learn more about how to read scenario execution information in the following articles:

   * For general information, see [Scenario execution flow in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * For information about processed bundles, see [Scenario execution, cycles, and phases in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Go to Workfront and search for "soho downtown loft" to see the project that the scenario created. This was the last row in the spreadsheet.
1. In Workfront Fusion, click **Save** ![](assets/save-icon.png) near the lower-left corner to save your progress on the scenario.

   >[!IMPORTANT]
   >
   >Save often as you hone and test a scenario.

## Finalize the scenario and test it again

We still need to configure the scenario to create projects for all the other rows in the spreadsheet.

1. Click the **Watch Rows** module you created for Google Sheets.
1. Change the **Limit** to 100.

   Specifying a number higher than the number of rows you know are are in the spreadsheet assures that the scenario will capture all of them.

1. Right-click the **Watch Rows** module, click **Choose where to start**, click **All**, then click **OK**.

1. Click **Run once** and watch what happens in the execution inspector bubbles.

   The Google Sheets **Watch Rows** module runs once to read all of the rows. Then the Workfront **Create Record** module runs 20 times to create a project for each of the remaining 20 rows in the spreadsheet.

1. Click the execution inspector bubble for the Workfront module to view all 20 operations, then click one of the operations to view the information about the project created.
1. Click **Save** ![](assets/save-icon.png) near the lower-left corner.
1. Go to Workfront to see the projects that the scenario created.

>[!TIP]
>
>We recommend the optional but useful practice of adding notes about each module.
>
>1. Right-click the Workfront module, then click **Add a note**.
>1. In the note that displays, type an overview for the module.
>
>   This is helpful because you won't have to continually open the module to see what it does. You could type something like "Creates a project with Name, Planned Start Date, and Priority mapped from spreadsheet."
>
>   For the Google Sheets module, you could type something like "Watch Project List for new rows/projects added."
>
>   You can add multiple notes for a module.
>
>1. Close the **Notes** area.
>
>   After you add a note to a scenario, an orange dot displays on the **Notes** icon ![](assets/notes-icon-w-dot.png) at the bottom of the scenario editor.
>
>1. Click the **Notes** icon ![](assets/notes-icon-w-dot.png) to view your notes.
>

## Activate the scenario

If this were a scenario you would be using for real data, the last thing you would do is activate it. After you activate a scenario, by default, it runs every 15 minutes. You can change this by defining when and how often you want it to run.

For more information about activating scenarios, see [Activate or deactivate a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

For information about schedules, see [Schedule a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).
