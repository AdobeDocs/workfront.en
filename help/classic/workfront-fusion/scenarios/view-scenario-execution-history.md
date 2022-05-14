---
filename: view-scenario-execution-history
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: View a scenario's execution history in Adobe Workfront Fusion
description: You can display information about all the runs for a scenario, or you can search all executions of the scenario for specific data.
---

# View a scenario's execution history in Adobe Workfront Fusion

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

You can display information about all the runs for a scenario, or you can search all executions of the scenario for specific data.

A scenario's execution history displays all of a scenario's executions for the last 30 days.

## Access requirements

You must have the following access to use the functionality in this article:

<table> 
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
   <td> <p>Workfront Fusion for Work Automation and Integration </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## View all executions of a scenario

### View scenario execution history on the Scenario Detail page

1. Click the **Scenario** tab in the left panel, then click the scenario.

   Or

   If you are working on the scenario in the Scenario editor, click the left arrow ![](assets/exit-editing-arrow.png) near the upper-left corner of the window.

1. View the information in the list on the right.

   ![](assets/open-history-tab-350x202.png)

   C

   You can also click to see a full-page view of this information. The full-page view allows you to filter the history to view specific executions.

   The following details are listed for every execution of the scenario:

   * Date when the run was **Started**
   * **Status** (success or failed)
   * Run **Duration**
   * Number of **Operations** 
   * Size of **Data Transfer**
   * Link to **Details**

### View scenario execution history on the History tab {#view-scenario-execution-history-on-the-history-tab}

The History tab shows more detail than is available on the Scenario detail page. You can also filter and sort the executions on the History tab.

1. Click the **Scenario** tab in the left panel, then click the scenario.

   Or

   If you are working on the scenario in the Scenario editor, click the left arrow ![](assets/exit-editing-arrow.png) near the upper-left corner of the window.

1. Click the **History** tab near the upper-left corner of the page
1. (Optional) For detailed information about a selected scenario run, including which bundles were processed, click the **Details** link.

   For more information on processing bundles, see [Scenario execution flow in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >The details link is visible only if the execution has details available.

## Filter the scenario execution history

You can filter the execution history to view only executions with the specified values.

1. Open the full-page history for a scenario as described in [View scenario execution history on the History tab](#view-scenario-execution-history-on-the-history-tab) in this article.
1. Click the filter icon ![](assets/fusion-scenario-filter-icon.png) in the header of the column you want to filter by.
1. In the filter dialog, enter the values that you want to filter by.
1. Click **Save**.

The filter icon is orange in columns with a currently active filter.

## Sort the scenario execution history

You can sort the scenario execution history.

1. Open the full-page history for a scenario as described in [View scenario execution history on the History tab](#view-scenario-execution-history-on-the-history-tab) in this article.
1. Click the Sort icon in the header of the column you want to filter by.
1. Optional: To reverse the order of the sort, click the Sort icon again.

## Search all executions of a scenario

1. Click the **Scenario** icon ![](assets/scenarios-icon.png) in the left panel, then click the scenario.

   Or

   If you are working on the scenario in the Scenario editor, click the left arrow ![](assets/exit-editing-arrow.png) near the upper-left corner of the window.

1. Click the **History** tab near the upper-left corner of the screen.
1. Click **Fulltext search** in the upper-right corner of the screen.

   <!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Click <strong>Fulltext search</strong> at the top of the list of executions.</p> <p>Or</p> <p>Type <b>Ctrl+Shift+F</b> (Windows) or <b>Cmd+Shift+F</b> (Mac)</p> <p>The Search in history window opens.</p> </li>
   -->

1. (Optional) To search for executions that contain specific text, enter the text in the search bar of the **Search in history** window.

   **Example:** If you want to find the execution that created a specific project, enter the project ID into the Fulltext search bar.

   <!--
   <li value="6" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(Optional) To limit your search by date range, select the beginning and ending dates of your desired search in the <b>By date range</b> area. </p> <note type="note">
   Executions are available only for the previous 30 days.
   </note> </li>
   -->

   <!--
   <li value="7" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(Optional) To limit your search by status, select the desired status in the <b>By status</b> dropdown.</p> <p>Available statuses are:</p>
   <ul>
   <li> <p>All</p> </li>
   <li> <p>Error</p> </li>
   <li> <p>Warning</p> </li>
   <li> <p>Success</p> </li>
   </ul> </li>
   -->

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(Optional) Change the order that results display in the <b>Sort by dates</b> dropdown.</p> </li>
   -->

   <!--
   <li value="9" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(Optional) To copy a scenario execution ID, click the <b>Copy execution ID</b> icon <img src="assets/copy-fusion-execution-id-icon.png"> in the row of the desired execution. </p> </li>
   -->

1. (Optional) Click on a result of the Fulltext search to examine the scenario module output bundle that contains the information.

