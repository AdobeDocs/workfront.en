---
filename: create-scorecard
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Create a scorecard
description: A scorecard is used to measure how well a project aligns with the previously established criteria of a portfolio. A scorecard often reflects an organization’s mission, values, and strategic goals.
---

# Create a scorecard

A scorecard is used to measure how well a project aligns with the previously established criteria of a portfolio. A scorecard often reflects an organization’s mission, values, and strategic goals.

Portfolio managers usually define the scorecard questions and answers to ensure they are meaningful and valuable during project prioritization and selection. An `Adobe Workfront administrator` builds the scorecards based on the recommendations from portfolio managers.

The questions and answers chosen for a scorecard must be quantifiable in order to provide an alignment value to compare different projects.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan</td> 
   <td> <p><span>Business</span> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Create a scorecard

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2"> <p>Click <span class="bold">Scorecards</span>, then click <span class="bold">New Scorecard</span> to create a new scorecard and launch the scorecard builder.</p> <p> <img src="assets/new-scorecard-350x173.png" alt="new_scorecard.png" style="width: 350;height: 173;"> </p> </li> 
 <li value="3"> <p>Specify the following information for the new scorecard:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Scorecard Name</td> 
     <td>The name of the scorecard. This name is displayed&nbsp;when you are associating the scorecard with the project.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Description</td> 
     <td>Specify a description for the scorecard. The description is displayed next to the scorecard name in the scorecard list.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="4"> <p>Click the <span class="bold">Add Question</span> drop-down menu to open the scorecard question section.</p> <p> <img src="assets/3-350x76.png" alt="" style="width: 350;height: 76;"> </p> <p>Specify the following information for your question:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Question</td> 
     <td>Specify the question you want to include in the scorecard.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Points</td> 
     <td>Specify the maximum points possible for this&nbsp;question.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Negative Points</td> 
     <td>Select this option&nbsp;to indicate that <span>Workfront</span> should subtract from the total possible points. Negative scores cannot be added to the maximum possible points of a scorecard.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Display Type</td> 
     <td> <p>Select from the following options:</p> </td> 
    </tr> 
   </tbody> 
  </table> 
  <ul> 
   <li><span class="bold">Value(0-100)</span>: This is a numerical value. If selected, a numeric field is displayed in the scorecard where users can specify any value between 0-100.</li> 
   <li> <p><span class="bold">Drop Down:</span>&nbsp;If selected, the <span class="bold">Options</span> section is now displayed.</p> <p> <img src="assets/drop-down-menu-with-answers-ui-for-scorecards-350x40.png" alt="drop_down_menu_with_answers_UI_for_scorecards.png" style="width: 350;height: 40;"> </p> <p>Click <span class="bold">Answer</span> to add a possible answer to your question.</p> 
    <table cellspacing="0"> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td role="rowheader">Answer Text</td> 
       <td>Specify one of the possible answers for your question.</td> 
      </tr> 
      <tr> 
       <td role="rowheader">Value</td> 
       <td>Specify the value in percentage points of this answer, in case that it is fulfilled. If you choose 100%, the number of points allotted for this question is fully achieved. If you want to indicate that this answer carries only a portion of the total amount of points allotted to this question, select a lower percentage value for this answer. For example, if your question is valued at 10 points, and you want this answer to carry 5 of those points, choose 50% for your <span class="bold">Value</span>.</td> 
      </tr> 
      <tr> 
       <td role="rowheader">Default</td> 
       <td>Specify whether this answer is the default one.</td> 
      </tr> 
      <tr> 
       <td role="rowheader">Delete</td> 
       <td>You can&nbsp;delete an answer, if you consider it to no longer be pertinent.</td> 
      </tr> 
     </tbody> 
    </table> </li> 
   <li> <p><span class="bold">Radio Button:</span> If selected, the <span class="bold">Options</span> section is now displayed.</p> <p> <img src="assets/drop-down-menu-with-answers-ui-for-scorecards--1--350x40.png" alt="drop_down_menu_with_answers_UI_for_scorecards__1_.png" style="width: 350;height: 40;"> </p> <p>Click <span class="bold">Answer</span> to add a possible answer to your question.<br><span class="bold">Answer Text</span>: Specify one of the possible answers for your question.<br><span class="bold">Value</span>: Specify the value in percentage points of this answer, in case that it is fulfilled. If you choose 100%, the number of points allotted for this question is fully achieved. If you want to indicate that this answer carries only a portion of the total amount of points allotted to this question, select a lower percentage value for this answer. For example, if your question is valued at 10 points, and you want this answer to carry 5 of those points, choose 50% for your <span class="bold">Value</span>.</p> <p><span class="bold">Default</span>: Specify whether this answer is the default one.<br><span class="bold">Delete</span>: You can&nbsp;delete an answer, if you consider it to no longer be pertinent.</p> </li> 
  </ul> </li> 
 <li value="5"> <p>Click <span class="bold">Add Question</span> to add more questions and answers to your scorecard, following the same steps.</p> <note type="note">
   You can reorder the questions in your scorecard by dragging and dropping the questions in the correct order.
   <br>
  </note> </li> 
 <li value="6"> <p>Click <span class="bold">Save</span> when you are finished entering your data.</p> <p> <img src="assets/5-350x289.png" alt="" style="width: 350;height: 289;"> </p> </li> 
</ol>

## Apply a scorecard to a project

A user with manage permissions to a project can apply a scorecard to a project, after the scorecard has been created by the `Workfront administrator`.  
For more information about&nbsp;creating scorecards, see [Create a scorecard](#creating-a-scorecard).  
For more information about project permissions, see [Share a project in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

A scorecard is added to a project as part of creating a business case for the project. For more information about&nbsp;adding a scorecard to a project, see [Apply a scorecard to a project and generate an Alignment Score](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).
