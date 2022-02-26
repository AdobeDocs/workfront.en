---
filename: customize-terminology
title: Customize user interface terminology using a Layout Template
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
title: Customize user interface terminology using a layout template
description: As an Adobe Workfront administrator, you can use a layout template to change the labels of some objects that appear throughout Workfront to match terms used in your organization.
---

# Customize user interface terminology using a layout template

As an *Adobe Workfront administrator*, you can use a layout template to change the labels of some objects that appear throughout *Workfront* to match terms used in your organization.

After you save a layout template where you changed terminology, then log out of *Workfront* and back in again, the labels that you changed appear where the default labels would appear in most areas throughout *Workfront*:

* Main Menu
* All areas accessed from the Main Menu
* All tabs
* All menus
* Report Builder and reporting elements (views, filters and groupings)
* Save buttons
* Exported files
* Emails
* Mobile Apps

>[!NOTE]
>
>* The Outlook Add-in area does not display the customized labels.
>* You might encounter grammar and other problems when you customize labels. For example, if you change "Issue" to "Request," there may be places in the UI where you see the phrase "An request." For more information, see [Implications of customizing object names](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names) in the article [Understand objects in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
>

For information about layout templates for groups, see [Create and modify a group’s layout templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Customize user interface terminology

<ol> 
 <li value="1">Begin working on a layout template, as described in <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</li> 
 <li value="2">Click <span class="bold">Set Terminology</span> near the upper-right corner of the page.</li> 
 <li value="3">Do any of the following:
  <ul>
   <li><p>To use an alternative term provided by <em>Workfront</em>, click the down arrow&nbsp;<img src="assets/dropdown-arrow.png"> next to the label, then click the alternative label you want in the drop-down list.</p><note type="note">
     Alternative labels provided in the drop-down lists are supported in versions of 
     <em>Workfront</em> localized for non-English languages.
    </note></li>
   <li><p>To provide your own custom alternative for the label displayed for an object, click <span class="bold">Set custom name</span> to the right of the label, then type the <span class="bold">Singular</span> and <span class="bold">Plural</span> forms of the custom term. You can click <span class="bold">Reset</span> if you change your mind.</p><p>You can customize the following object names:</p>
    <table cellspacing="0">
     <col>
     <col>
     <col>
     <tbody>
      <tr>
       <td role="rowheader"><p><em>Workfront</em> objects</p></td>
       <td>
        <ul>
         <li>Portfolio</li>
         <li>Program</li>
         <li>Project</li>
         <li>Task</li>
         <li>Issue</li>
         <li>Goal</li>
         <li>Result</li>
         <li>Activity</li>
        </ul></td>
       <td><p>For more information about these objects, see <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>.</p></td>
      </tr>
      <tr>
       <td role="rowheader"><p><em>Workfront Goals</em> objects</p></td>
       <td>
        <ul>
         <li>Goal</li>
         <li>Result</li>
         <li>Activity</li>
        </ul></td>
       <td><p>These objects require an additional license. For more information, see <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Adobe Workfront Goals overview</a>.</p></td>
      </tr><draft-comment>
       <tr data-mc-conditions="">
        <td role="rowheader"><p><em>Workfront Scenario Planner</em> objects</p></td>
        <td>
         <ul>
          <li>Initiative</li>
          <li>Scenario</li>
          <li>Plan </li>
         </ul></td>
        <td><p>These objects require an additional license. For information, see <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">Get started with the Adobe Workfront Scenario Planner</a>.</p></td>
       </tr>
      </draft-comment>
      <tr data-mc-conditions="">
       <td role="rowheader"><p><em>Workfront Scenario Planner</em> objects</p></td>
       <td>
        <ul>
         <li>Initiative</li>
         <li>Scenario</li>
         <li>Plan </li>
        </ul></td>
       <td><p>These objects require an additional license. For information, see <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">Get started with the Adobe Workfront Scenario Planner</a>.</p></td>
      </tr>
     </tbody>
    </table></li>
  </ul></li> 
 <li value="4"> <p>When you are finished, click <span class="bold">Done</span>.</p> <note type="tip">
   After you click Done (and even after you save your layout template), you can always return to the Set Terminology settings and click Reset next to any custom terms to return them to their default state.
  </note> </li> 
 <li value="5"> <p> <p>Continue customizing the layout template.</p> <p>Or</p> <p>If you are finished customizing, click <span class="bold">Save</span>.</p> </p> </li> 
 <li value="6">To see your terminology changes:
  <ol>
   <li value="1"><p>Log out and back in to <em>Workfront</em>.</p></li>
   <li value="2">Close all browser tabs that you have open for your <em>Workfront</em> environment.</li>
  </ol><note type="important">
   This is also required for anyone who used the layout template before you made the terminology changes.
  </note></li> 
</ol>

For more information about layout templates, see [Create and manage layout templates](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
