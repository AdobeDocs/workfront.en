---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Create a simple scenario in [!DNL Adobe Workfront Fusion]
description: Learn how to create a simple automation scenario with Adobe Workfront Fusion. Automation scenarios automate Workfront processes, including data manipulation and transformation. This example takes you through the process of creating a scenario that searches for a task and then converts it to a project.
author: Becky
feature: Workfront Fusion
---
# Create a simple scenario in [!DNL Adobe Workfront Fusion]

The role of [!DNL Adobe Workfront Fusion] is to automate your processes so that you can concentrate on new tasks rather than repeating the same tasks again and again. It works by linking actions within and between apps and services to create a scenario that transfers and transforms your data automatically. The scenario you create watches for data in an app or service and processes that data to provide the result you want.

A scenario is comprised of a series of modules that indicate how data should be transformed within an app or transferred between apps and web services.

This example takes you through the process of creating a scenario that searches for a [!DNL Workfront] task in Workfront and the converts it to a project.

<!--# Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>
To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## Create a practice scenario

### Begin creating the scenario

1. In the **Scenarios** area, click **Create a new scenario**.

    To locate the Scenarios area, see <!--navigation article-->

   The scenario editor displays, containing an empty module in the center.

   <!--picture?-->

1. Select the **[!UICONTROL New scenario]** placeholder name in the upper-left corner, then enter a name.
1. Continue with [Add and configure the first module](#add-and-configure-the-first-module) below.

### Add and configure the first module

1. Click the empty module to choose the app from which you will select a module.

   A list of apps appears to the right of the module.

1. Select **[!DNL Adobe Workfront]**. If it is not visible, click the search bar at the bottom of the list, type "Workfront," and select it when it appears in the list.

   The list changes to display all [!DNL Workfront] modules that you can use.

1. Click the **[!UICONTROL Search]** module.

   The module configuration window opens.

1. In the [!UICONTROL Connection] box, select your Workfront connection. 

   If you do not have a Workfront connection, see [Create a connection to [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)
1. In the [!UICONTROL Record Type] box, select **[!UICONTROL Task]**. This sets the module to search only tasks.

   You can find **[!UICONTROL Task]** in the list if you start typing the word "[!UICONTROL task]."

   <!--Becky continue editing from here-->

1. In the **[!UICONTROL Result Set]** box, select **[!UICONTROL First Matching Record]**. 

   This sets the module to return only the first record it finds that meets the criteria. For this example, we need only one record returned.
1. In the **[!UICONTROL Search criteria]** area, configure the criteria to return the specific task.

   1. In the first box under [!UICONTROL Search Criteria], select the field that you want to include in your search. For this example, select **[!UICONTROL Name]**.

      You can find **[!UICONTROL Name]** in the list if you start typing the word "[!UICONTROL name]."
   1. For the operator, click the dropdown arrow next to **Exist** and change it to [!UICONTROL **Contains (case insensitive)**]. 
      
      This allows the module to find projects with your chosen words in its name, even if you do not enter the entire name, or enter the name with the incorrect case (such as all caps).
   1. In the last field under [!UICONTROL Search Criteria], enter a word or phrase that you know is in the name of the task you are searching for.

1. In the **[!UICONTROL Outputs]** list, select the fields that you want the module to output. For this example, select the **[!UICONTROL ID]** and **[!UICONTROL Name]** fields.

   >[!TIP]
   >
   >You can use **Cmd+F** ([!DNL Mac] OS) or **Ctrl-F** ([!DNL Windows] OS) to find a field quickly.

1. Click **[!UICONTROL OK]** to save the module configuration.

1. Right-click the module, click **[!UICONTROL Rename]**, then type a name the describes what you want the module to do (such as "Search for task)," then click **[!UICONTROL OK]**.

   The name appears just below the module. Below that, [!DNL Workfront Fusion] includes a brief description of the type of action performed by the module.

   ![](assets/module-renamed-wf.png)

1. Continue with [Add and configure the second module](#add-and-configure-the-second-module).

## Add and configure the second module

1. Hover over the partial circle to the right of the of the module, then click **[!UICONTROL Add another module]**. <!--becky continue here-->
1. Select [!DNL Workfront] from the list of applications, then choose the search module **[!UICONTROL Read Related Records]**.
1. You already created a connection to [!DNL Workfront] for the previous module. You don't need to create it again here, but you must make sure this module is using the same connection as the previous module.\
   In the **[!UICONTROL Connection]** box, select the connection that you created for the previous module.
1. Click **[!UICONTROL Record type]**, then select **[!UICONTROL Project]**, because we want to read records related to a project.

   >[!TIP]
   >
   >You can find **[!UICONTROL Project]** in the list if you start typing the word "project."

1. Click the **[!UICONTROL Parent Record ID]** field. This field requires the Workfront ID of the project that you want to return tasks from.

   Clicking the field opens the list of variables that you can use in the **[!UICONTROL Parent Record ID]** field to identify the project in Workfront.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Click the variable **[!UICONTROL ID]** to add it to the **[!UICONTROL Parent Record ID]** field. This allows the ID returned from the first module to be used as the identifier for the project that you want to work with in the second module, which ensures that the tasks returned will belong to that project.
1. In the **[!UICONTROL Collections]** field, select **[!UICONTROL Tasks]**. This indicates that the module is to return tasks associated with the chosen project.
1. Click **[!UICONTROL OK]**

   Now you have a working scenario.

1. Give the second module a name such as "Return tasks associated with project," then continue with [Test the scenario](#test-the-scenario).

## Test the scenario

Before you activate your scenario, it's important to test it by running it at least once and viewing the results. This helps you understand how data flows through the scenario and find any errors.

We chose to have 1 project returned, as well as the tasks associated with that project. If you run the scenario, that is what should happen.

1. Click **[!UICONTROL Run once]** in the lower-left corner of the scenario editor.
1. After the scenario finishes running, click the bubble above the first module.

   ![](assets/click-bubble.png)

   In the box that appears, you can view information about the bundle of data that the module processed, including the actual data that was pulled from the project that the module returned.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. Click the execution inspector bubble above the Second module to see the input of information and the output, which is a collection of tasks contained in the project.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   You can learn more about how to read scenario execution information in the following articles:

   * For general information, see [Scenario execution flow in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * For information about processed bundles, see [Scenario execution, cycles, and phases in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. In [!DNL Workfront Fusion], click **[!UICONTROL Save]** ![](assets/save-icon.png) near the lower-left corner to save your progress on the scenario.

   >[!IMPORTANT]
   >
   >Save often as you hone and test a scenario.

>[!TIP]
>
>We recommend the optional but useful practice of adding notes about each module.
>
>1. Right-click a [!DNL Workfront] module, then click **[!UICONTROL Add a note]**.
>1. In the note that displays, type an overview for the module.
>
>    You can add multiple notes for a module.
>
>1. Close the **[!UICONTROL Notes]** area.
>
>     After you add a note to a scenario, an orange dot displays on the **[!UICONTROL Notes]** icon ![](assets/notes-icon-w-dot.png) at the bottom of the scenario editor.
>
>1. Click the **[!UICONTROL Notes]** icon ![](assets/notes-icon-w-dot.png) to view your notes.
>



## Activate the scenario

This example scenario does not have a trigger module. If this were a scenario you would be using for real data it would start with a trigger module, and the last thing you would do is activate it. After you activate a scenario, by default, it runs every 15 minutes. You can change this by defining when and how often you want it to run.

For more information about activating scenarios, see [Activate or deactivate a scenario in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

For information about schedules, see [Schedule a scenario in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
