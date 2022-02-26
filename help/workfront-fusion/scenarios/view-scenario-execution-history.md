---
filename: view-scenario-execution-history
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: View a scenario's execution history
description: You can display information about all the runs for a scenario, or you can search all executions of the scenario for specific data.
---

# View a scenario's execution history

You can display information about all the runs for a scenario, or you can search all executions of the scenario for specific data.

A scenario's execution history displays all of a scenario's executions for the last 30 days.

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

## View all executions of a scenario

### View scenario execution history on the Scenario Detail page

<ol> 
 <li value="1"> <p>Click the <span class="bold">Scenario</span> tab in the left panel, then click the scenario.</p> <p>Or</p> <p>If you are working on the scenario in the Scenario editor, click the left arrow <img src="assets/exit-editing-arrow.png"> near the upper-left corner of the window.</p> </li> 
 <li value="2"> <p>View the information in the list on the right.</p> <p> <img src="assets/open-history-tab-350x202.png" style="width: 350;height: 202;"> </p> <p>C</p> <p>You can also click to see a full-page view of this information. The full-page view allows you to filter the history to view specific executions.</p> <p>The following details are listed for every execution of the scenario:</p> 
  <ul> 
   <li>Date when the run was <span class="bold">Started</span></li> 
   <li><span class="bold">Status</span> (success or failed)</li> 
   <li>Run <span class="bold">Duration</span></li> 
   <li>Number of <span class="bold">Operations</span> </li> 
   <li>Size of <span class="bold">Data Transfer</span></li> 
   <li>Link to <span class="bold">Details</span></li> 
  </ul> </li> 
</ol>

### View scenario execution history on the History tab

The History tab shows more detail than is available on the Scenario detail page. You can also filter and sort the executions on the History tab.

<ol> 
 <li value="1"> <p>Click the <span class="bold">Scenario</span> tab in the left panel, then click the scenario.</p> <p>Or</p> <p>If you are working on the scenario in the Scenario editor, click the left arrow <img src="assets/exit-editing-arrow.png"> near the upper-left corner of the window.</p> </li> 
 <li value="2"> <p>Click the <span class="bold">History</span> tab near the upper-left corner of the page</p> </li> 
 <li value="3"> <p>(Optional) For detailed information about a selected scenario run, including which bundles were processed, click the <span class="bold">Details</span> link. </p> <p>For more information on processing bundles, see <a href="../../workfront-fusion/scenarios/scenario-execution-flow.md" class="MCXref xref">Scenario execution flow</a>.</p> <note type="note">
   The details link is visible only if the execution has details available. 
  </note> </li> 
</ol>

## Filter the scenario execution history

You can filter the execution history to view only executions with the specified values.

<ol> 
 <li value="1"> <p>Open the full-page history for a scenario as described in <a href="#view2" class="MCXref xref">View scenario execution history on the History tab</a> in this article.</p> </li> 
 <li value="2"> <p>Click the filter icon <img src="assets/fusion-scenario-filter-icon.png"> in the header of the column you want to filter by.</p> </li> 
 <li value="3"> <p>In the filter dialog, enter the values that you want to filter by.</p> </li> 
 <li value="4"> <p>Click <b>Save</b>.</p> </li> 
</ol>

The filter icon is orange in columns with a currently active filter.

## Sort the scenario execution history

You can sort the scenario execution history.

1. Open the full-page history for a scenario as described in [View scenario execution history on the History tab](#view2) in this article.
1. Click the Sort icon in the header of the column you want to filter by.
1. Optional: To reverse the order of the sort, click the Sort icon again.

## Search all executions of a scenario for specific data

<ol> 
 <li value="1"> <p>Click the <span class="bold">Scenario</span> icon <img src="assets/scenarios-icon.png"> in the left panel, then click the scenario.</p> <p>Or</p> <p>If you are working on the scenario in the Scenario editor, click the left arrow <img src="assets/exit-editing-arrow.png"> near the upper-left corner of the window.</p> </li> 
 <li value="2"> <p>Click the <span class="bold">History</span> tab near the upper-left corner of the screen.</p> </li> 
 <li value="3"> <p>Click <span class="bold" style="font-weight: bold;">Fulltext search</span> in the upper-right corner of the screen.</p> </li> 
 <li value="4"> <p>Enter the search term.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span>If you want to find the execution that created a specific project, enter the project ID into the Fulltext search bar.</p> </li> 
 <li value="5"> <p>(Optional) Click on a result of the fulltext search to examine the scenario module output bundle that contains the information.</p> </li> 
</ol>

