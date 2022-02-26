---
filename: sharing-permissions-on-objects-overview
content-type: overview
navigation-topic: grant-and-request-access-to-objects
title: Overview of sharing permissions on objects in Adobe Workfront
description: The highlighted information on this page refers to functionality available only in the new Workfront experience beta.
---

# Overview of sharing permissions on objects in *Adobe Workfront*

The highlighted information on this page refers to functionality available only in the new Workfront experience beta.

You do not have to be an *Adobe Workfront administrator* to share permissions on objects that you have access to, but permissions on objects work within the access levels set by the *Workfront administrator*.

For more information about access levels and permissions, see [How access levels and permissions work together](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

You can share or remove permissions to an object you created or an object that was shared with you. When you are not the creator of the object, you must have Share access on the object that you want to share in your access level in addition to Share permissions on the object. For information about access levels, see [Access levels overview](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!NOTE]
>
>A *Workfront administrator* can add or remove permissions to any items in the system, for all users, without being the owner of those items.

## Objects that you can share in *Workfront*

You can share the following objects in&nbsp;*Workfront* with other users:

* `Projects`: For more information, see [Share a project in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* `Templates`: For more information, see [Share project templates](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* `Portfolios`: For more information, see [Share a portfolio in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio..md).

* `Programs`: For information, see [Share a program in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md) .

* `Tasks`: For information, see [Share a task in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

* `Issues`: For information, see [Share an issue in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

* `Documents`: For information, see [Share a document in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

* **Document Folders**: For information, see [Share a document folder](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

* **Proofs**: For information, see [Share a Proof in Workfront Proof](../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md). 

* `Reports, dashboards, and calendars`: For information, see [Share reports, dashboards, and calendars in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).&nbsp;Additionally, see the following articles:

  * [Share a report in Adobe Workfront](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
  * [Share a dashboard in Adobe Workfront](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
  * [Share a calendar report](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* **Filters, views, and groupings**: For information, see [Share a filter, view, or grouping in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p><span><span class="bold">Plans</span>: For information, see <a href="../../scenario-planner/share-a-plan.md" class="MCXref xref">Share a plan in the Adobe Workfront Scenario Planner</a>.</span> </p> <p><span>This requires an additional license. </span> </p> </li>
  -->

* ` `Plans`: For information, see [Share a plan in the Adobe Workfront Scenario Planner](../../scenario-planner/share-a-plan.md).`

  `This requires an additional license.` 

* 

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><b>Goals</b>: For information, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Adobe Workfront Goals</a>. </p>
  -->

  **Goals**: For information, see [Share a goal in Adobe Workfront Goals](../../workfront-goals/workfront-goals-settings/share-a-goal.md).

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">This requires an additional license.</p>
  -->

  This requires an additional license.

## Considerations about sharing objects

<ul> 
 <li> <p> You can share only the same level or a lower level of permissions you have on the object.</p> <p>For example, if you have Contribute permissions on the object, you cannot grant another user Manage permissions on that object.</p> </li> 
 <li> <p>You cannot share an object with a permission level higher than the access level of a user.&nbsp;For example, if a user has View access to Projects in their access level, you cannot give them Manage permissions on a project. </p> </li> 
 <li> <p>A user with permissions to at least View an object can share that object with someone else.</p> </li> 
 <li> <p>You can share objects with active users, job roles, teams, groups, or companies.</p> <note type="note"> 
   <p> &nbsp;<span>You can share a plan or a goal only with other active users</span><span>.</span><span> This requires additional licenses.</span></p> 
   <p><span>For more information see:</span> </p> 
   <ul> 
    <li> <p><a href="../../scenario-planner/share-a-plan.md" class="MCXref xref">Share a plan in the Adobe Workfront Scenario Planner</a> </p> </li> 
    <li> <p><a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Adobe Workfront Goals</a> </p> </li> 
   </ul> 
  </note> </li> 
</ul>

## Share limitations

You can share an object with up to 100 entities (users, teams, groups, job roles, companies). We recommend that you share objects with groups, teams, or companies rather than with individual users, to avoid this limitation.

## Share permissions for objects

The following table illustrates the level of permissions that you can select when sharing an object. Not all objects have all these settings available. You can grant another entity permissions to View or Manage an object. If you are sharing a project, task, or issue, you can also grant permissions to Contribute to it.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">View</td> 
   <td> <p>You can perform the following actions on the object:</p> 
    <ul> 
     <li>View the object</li> 
     <li>Add documents to the object</li> 
     <li>View Finance information about the object</li> 
     <li> <p>Share the object<br></p> <p>When you share the object, you can grant other users the same permission level you have only on the object, not a higher level.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Contribute</td> 
   <td> <p>You can perform the following actions on the object:</p> 
    <ul> 
     <li>View it</li> 
     <li>All the actions included with the View permission.</li> 
     <li>Add Expenses to it</li> 
     <li>Add issues to it (if it is a task or a project)</li> 
     <li>Add tasks to it (if it is a project)</li> 
     <li>Edit Custom Forms on it</li> 
     <li>Log Hours on the object</li> 
     <li>Make assignments in it</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Manage</td> 
   <td> <p>You can perform the following actions on the object:</p> 
    <ul> 
     <li>View it</li> 
     <li>All the actions included with the View and Contribute permissions</li> 
     <li>Delete it</li> 
     <li>Manage Finance information in it</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Make this public to external users</td> 
   <td> <p>Anyone without a <em>Workfront</em> account can view the object by clicking a link to it. This is not available for all objects.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Make this visible system-wide</td> 
   <td> <p>The object can be found in searches and viewed by anyone with a <em>Workfront</em> account.</p> </td> 
  </tr> 
 </tbody> 
</table>

##

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2><a name="Share"></a> </h2>
<h2>Share an object</h2>
<p>Sharing objects is identical for all the objects that can be shared<draft-comment>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
, except for plans in the
<em>Workfront Scenario Planner</em> and goals in
<em>Workfront Goals</em>
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
, except for plans in the
<em>Workfront Scenario Planner</em> and goals in
<em>Workfront Goals</em>
</MadCap:conditionalText>. </p>
<p> <draft-comment>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<span>For more information about sharing plans and goals, see:</span>
</MadCap:conditionalText>
</draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<span>For more information about sharing plans and goals, see:</span>
</MadCap:conditionalText> </p> <draft-comment>
<ul data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<li><a href="../../scenario-planner/share-a-plan.md" class="MCXref xref">Share a plan in the Adobe Workfront Scenario Planner</a> </li>
<li><a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Adobe Workfront Goals</a> </li>
</ul>
</draft-comment>
<ul data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<li><a href="../../scenario-planner/share-a-plan.md" class="MCXref xref">Share a plan in the Adobe Workfront Scenario Planner</a> </li>
<li><a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Adobe Workfront Goals</a> </li>
</ul>
<ol>
<li value="1">Go to the object you want to share. <p>For information about which objects can be shared, see the <a href="#sharing" class="MCXref xref">Share limitations</a> section this article. </p></li>
<li value="2">Do either&nbsp;of the following, depending on the type of object you are sharing:<br>
<ul>
<draft-comment>
<li data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span>When sharing a project, task, issue, portfolio, program, template, report, dashboard, </span>or<span> calendar, </span>click the <span class="bold">More</span> icon<img src="assets/more-icon.png">, then click&nbsp;<span class="bold">Sharing.</span><br><img src="assets/sharing-a-task-350x157.png" style="width: 350;height: 157;"></li>
</draft-comment>
<li data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span>When sharing a project, task, issue, portfolio, program, template, report, dashboard, </span>or<span> calendar, </span>click the <span class="bold">More</span> icon<img src="assets/more-icon.png">, then click&nbsp;<span class="bold">Sharing.</span><br><img src="assets/sharing-a-task-350x157.png" style="width: 350;height: 157;"></li>
<li><span>When sharing a document that does not contain a <em>proof</em>,</span> select the document that you want to share, then click <span class="bold">Share</span>&nbsp;> <span class="bold">Document</span>.<br><note type="tip">
You can share multiple documents at the same time by holding the Shift key to select multiple documents, then clicking
<span class="bold">Share</span>.
</note><br><draft-comment>
<img src="assets/share-a-document-350x160.png" style="width: 350;height: 160;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
</draft-comment><img src="assets/share-a-document-350x160.png" style="width: 350;height: 160;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></li>
<li><span>When sharing a <em>proof</em> link, </span>select the document that contains the <em>proof</em>, then click <span class="bold">Share</span> > <span class="bold">Proof Link</span>.<br>For more information about sharing a <em>proof</em> (either by sharing a link or by adding users to a <em>proof</em>), see <a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md" class="MCXref xref">Share a proof within Adobe Workfront</a>.</li>
</ul></li>
<li value="3"> <p>In the <span class="bold">Give <Object&nbsp;Name> access to</span>&nbsp;field, begin typing the name of the user, team, role, group, or company with whom you want to share the object, then click the name when it appears in the drop-down list. </p> <p>For example, if you are sharing a project, use the <span class="bold">Give project access to</span>&nbsp;field.<br>If you have multiple entities named similarly, they should all be listed under their type. The names of the entities appear in alphabetical order. However, the order in which the entity types appear is random. Select the one with which you want to share the project.&nbsp;</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="4"> <p>(Optional) Repeat step 3 for each user, team, role, or group who you want to grant access to the object. </p> <draft-comment>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-project-sharing-modal-350x456.png" style="width: 350;height: 456;"> </p>
</draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-project-sharing-modal-350x456.png" style="width: 350;height: 456;"> </p> </li>
<li value="5">Specify the permissions for each user, team, role,&nbsp;group, or company that you added in Step 3 by clicking&nbsp;the drop-down menu, then selecting the permission level that you want to grant. <p>The following options are available:</p>
<ul>
<li><p><span class="bold">View:</span>&nbsp;Users can&nbsp;review and share&nbsp;the item.&nbsp;</p></li>
<li><p><span class="bold">Contribute</span><span class="bold">:</span>&nbsp;Users can&nbsp;make&nbsp;updates, log&nbsp;information, make minor edits, and share, plus all View permissions. </p><note type="note">
<p>You cannot grant Contribute permissions to the following objects:&nbsp;</p>
<ul>
<li><p>Template</p></li>
<li><p>Documents</p></li>
<li><p>Reports</p></li>
<li><p>Dashboards</p></li>
<li><p>Calendars</p></li>
<li><p>Filters</p></li>
<li><p>Views</p></li>
<li><p>Groupings</p></li>
</ul>
</note></li>
<li><p><span class="bold">Manage:&nbsp;</span>Users&nbsp;have full access to the object, minus administrative&nbsp;rights which are granted at the access level, plus all View and Contribute permissions.<br><note type="note">
&nbsp;The
<em>Workfront administrator</em> or the creator of the object has the ability to remove permissions from these entities.
</note></p><p>&nbsp;</p><p><img src="assets/screen-shot-2013-12-04-at-1.13.11-pm.png" alt=""></p><p>&nbsp;</p></li>
</ul></li>
<li value="6">(Optional) Click <span class="bold">Advanced Options</span>&nbsp;to configure specific permissions&nbsp;on the object. <p>View, Manage and Contribute have different advanced options depending on the the object and permission selected.<br>For more information about the permissions levels, see the <a href="#sharing" class="MCXref xref">Share limitations</a> section in this article. </p><p><img src="assets/screen-shot-2013-12-04-at-1.14.11-pm.png" alt=""></p></li>
<li value="7">(Optional)&nbsp;To make this object available to all users in the system, click the <span class="bold">Gear</span> icon<img src="assets/gear-icon-settings-with-dn-arrow.jpg"> , then in the drop-down menu click <span class="bold">Make this visible system-wide</span>. <p>All users can&nbsp;see the object based on the permissions that you set.</p></li>
<li value="8">(Optional) When sharing a project, click the <span class="bold">Gear</span> icon <img src="assets/gear-icon-settings-with-dn-arrow.jpg">, then in the drop-down menu click <span class="bold">Set as my project access template</span>&nbsp;to set the permissions as a template.<br>After you have defined permissions on one project, these same permissions are automatically applied the next time you create a project from scratch.<br><note type="note">
The project access template overrides the sharing defaults granted to you by the
<em>Workfront administrator</em> in your Access Level.
<br>For more information about specifying sharing defaults for projects in the Access Level, see
<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>&nbsp;
</note><br></li>
<li value="9">(Optional) To make the object public, click <span class="bold">Make this public to external users</span>.
<ol>
<li value="1">Click <span class="bold">copy link,</span>&nbsp;then distribute the link to external users at your discretion.<br>Any users with the link are able to view the object.</li>
</ol></li>
<li value="10">Click <span class="bold">Save</span>.</li>
</ol>
<h2><a name="bulk-sharing"></a>Share objects in bulk</h2>
<p>From a list of objects, you can share multiple objects at one time with other users, teams, groups, job roles, or companies.&nbsp;&nbsp;</p> <note type="important">
When you share objects in bulk, the names of the entities that have permissions to the individual objects do not display. When sharing objects in bulk the entities you add to the sharing list are added to the objects selected. They do not override the entities associated with the individual objects.&nbsp;
</note>
<p>To share objects in bulk:</p>
<ol>
<li value="1">Navigate to a list of objects.</li>
<li value="2">Select&nbsp;two or more objects in the list.</li>
<li value="3">Click&nbsp;<span class="bold">Share</span>.<br>Users who already have access to the object&nbsp;are not listed as available when bulk sharing.<br><note type="note">
If you do not have permissions to share an object that you selected, the
<span class="bold">Share</span> button is not visible.
</note></li>
<li value="4">In the <span class="bold">Edit <Object Name> access for</span> field, start typing the name of a user, team, group, job role, or company to which you want to grant permissions.<br>If you have multiple entities named similarly, they should all be listed under their type. The names of the entities appear in alphabetical order. However, the order in which the entity types appear is random. Select the one with which you want to share the project.<br><img src="assets/screen-shot-2014-05-29-at-2.54.51-pm-350x405.png" alt="" style="width: 350;height: 405;"></li>
<li value="5">(Optional) Click the gear icon, then click <span class="bold">Make this available system-wide&nbsp;</span>to make the objects selected available to all <em>Workfront</em> users.</li>
<li value="6">Click <span class="bold">Save</span>.</li>
</ol>
</div>
-->

##

## Share an object

Sharing objects is identical for all the objects that can be shared`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> , except for plans in the  <em>Workfront Scenario Planner</em> and goals in  <em>Workfront Goals</em></MadCap:conditionalText>`.

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <span>For more information about sharing plans and goals, see:</span> </MadCap:conditionalText>`

* [Share a plan in the Adobe Workfront Scenario Planner](../../scenario-planner/share-a-plan.md) 
* [Share a goal in Adobe Workfront Goals](../../workfront-goals/workfront-goals-settings/share-a-goal.md)

<ol> 
 <li value="1">Go to the object you want to share. <p>For information about which objects can be shared, see the <a href="#sharing" class="MCXref xref">Share limitations</a> section this article. </p></li> 
 <li value="2">Do either&nbsp;of the following, depending on the type of object you are sharing:<br>
  <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span>When sharing a project, task, issue, portfolio, program, template, report, dashboard, </span>or<span> calendar, </span>click the <span class="bold">More</span> icon<img src="assets/more-icon.png">, then click&nbsp;<span class="bold">Sharing.</span><br><img src="assets/sharing-a-task-350x157.png" style="width: 350;height: 157;"></li>
   <li><span>When sharing a document that does not contain a <em>proof</em>,</span> select the document that you want to share, then click <span class="bold">Share</span>&nbsp;> <span class="bold">Document</span>.<br><note type="tip">
      You can share multiple documents at the same time by holding the Shift key to select multiple documents, then clicking 
     <span class="bold">Share</span>.
    </note><br><img src="assets/share-a-document-350x160.png" style="width: 350;height: 160;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></li>
   <li><span>When sharing a <em>proof</em> link, </span>select the document that contains the <em>proof</em>, then click <span class="bold">Share</span> > <span class="bold">Proof Link</span>.<br>For more information about sharing a <em>proof</em> (either by sharing a link or by adding users to a <em>proof</em>), see <a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md" class="MCXref xref">Share a proof within Adobe Workfront</a>.</li>
  </ul></li> 
 <li value="3"> <p>In the <span class="bold">Give <Object&nbsp;Name> access to</span>&nbsp;field, begin typing the name of the user, team, role, group, or company with whom you want to share the object, then click the name when it appears in the drop-down list. </p> <p>For example, if you are sharing a project, use the <span class="bold">Give project access to</span>&nbsp;field.<br>If you have multiple entities named similarly, they should all be listed under their type. The names of the entities appear in alphabetical order. However, the order in which the entity types appear is random. Select the one with which you want to share the project.&nbsp;</p> <note type="tip">
   You can share an object only with active users, teams, 
   <span>roles,</span> or companies.
  </note> </li> 
 <li value="4"> <p>(Optional) Repeat step 3 for each user, team, role, or group who you want to grant access to the object. </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-project-sharing-modal-350x456.png" style="width: 350;height: 456;"> </p> </li> 
 <li value="5">Specify the permissions for each user, team, role,&nbsp;group, or company that you added in Step 3 by clicking&nbsp;the drop-down menu, then selecting the permission level that you want to grant. <p>The following options are available:</p>
  <ul>
   <li><p><span class="bold">View:</span>&nbsp;Users can&nbsp;review and share&nbsp;the item.&nbsp;</p></li>
   <li><p><span class="bold">Contribute</span><span class="bold">:</span>&nbsp;Users can&nbsp;make&nbsp;updates, log&nbsp;information, make minor edits, and share, plus all View permissions. </p><note type="note">
     <p>You cannot grant Contribute permissions to the following objects:&nbsp;</p>
     <ul>
      <li><p>Template</p></li>
      <li><p>Documents</p></li>
      <li><p>Reports</p></li>
      <li><p>Dashboards</p></li>
      <li><p>Calendars</p></li>
      <li><p>Filters</p></li>
      <li><p>Views</p></li>
      <li><p>Groupings</p></li>
     </ul>
    </note></li>
   <li><p><span class="bold">Manage:&nbsp;</span>Users&nbsp;have full access to the object, minus administrative&nbsp;rights which are granted at the access level, plus all View and Contribute permissions.<br><note type="note">
      &nbsp;The 
      <em>Workfront administrator</em> or the creator of the object has the ability to remove permissions from these entities.
     </note></p><p>&nbsp;</p><p><img src="assets/screen-shot-2013-12-04-at-1.13.11-pm.png" alt=""></p><p>&nbsp;</p></li>
  </ul></li> 
 <li value="6">(Optional) Click <span class="bold">Advanced Options</span>&nbsp;to configure specific permissions&nbsp;on the object. <p>View, Manage and Contribute have different advanced options depending on the the object and permission selected.<br>For more information about the permissions levels, see the <a href="#sharing" class="MCXref xref">Share limitations</a> section in this article. </p><p><img src="assets/screen-shot-2013-12-04-at-1.14.11-pm.png" alt=""></p></li> 
 <li value="7">(Optional)&nbsp;To make this object available to all users in the system, click the <span class="bold">Gear</span> icon<img src="assets/gear-icon-settings-with-dn-arrow.jpg"> , then in the drop-down menu click <span class="bold">Make this visible system-wide</span>. <p>All users can&nbsp;see the object based on the permissions that you set.</p></li> 
 <li value="8">(Optional) When sharing a project, click the <span class="bold">Gear</span> icon <img src="assets/gear-icon-settings-with-dn-arrow.jpg">, then in the drop-down menu click <span class="bold">Set as my project access template</span>&nbsp;to set the permissions as a template.<br>After you have defined permissions on one project, these same permissions are automatically applied the next time you create a project from scratch.<br><note type="note">
    The project access template overrides the sharing defaults granted to you by the 
   <em>Workfront administrator</em> in your Access Level. 
   <br>For more information about specifying sharing defaults for projects in the Access Level, see 
   <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>&nbsp;
  </note><br></li> 
 <li value="9">(Optional) To make the object public, click <span class="bold">Make this public to external users</span>. 
  <ol>
   <li value="1">Click <span class="bold">copy link,</span>&nbsp;then distribute the link to external users at your discretion.<br>Any users with the link are able to view the object.</li>
  </ol></li> 
 <li value="10">Click <span class="bold">Save</span>.</li> 
</ol>

## Share objects in bulk

From a list of objects, you can share multiple objects at one time with other users, teams, groups, job roles, or companies.&nbsp;&nbsp;

>[!IMPORTANT]
>
>When you share objects in bulk, the names of the entities that have permissions to the individual objects do not display. When sharing objects in bulk the entities you add to the sharing list are added to the objects selected. They do not override the entities associated with the individual objects.&nbsp;

To share objects in bulk:

<ol> 
 <li value="1">Navigate to a list of objects.</li> 
 <li value="2">Select&nbsp;two or more objects in the list.</li> 
 <li value="3">Click&nbsp;<span class="bold">Share</span>.<br>Users who already have access to the object&nbsp;are not listed as available when bulk sharing.<br><note type="note">
    If you do not have permissions to share an object that you selected, the 
   <span class="bold">Share</span> button is not visible.
  </note></li> 
 <li value="4">In the <span class="bold">Edit <Object Name> access for</span> field, start typing the name of a user, team, group, job role, or company to which you want to grant permissions.<br>If you have multiple entities named similarly, they should all be listed under their type. The names of the entities appear in alphabetical order. However, the order in which the entity types appear is random. Select the one with which you want to share the project.<br><img src="assets/screen-shot-2014-05-29-at-2.54.51-pm-350x405.png" alt="" style="width: 350;height: 405;"></li> 
 <li value="5">(Optional) Click the gear icon, then click <span class="bold">Make this available system-wide&nbsp;</span>to make the objects selected available to all <em>Workfront</em> users.</li> 
 <li value="6">Click <span class="bold">Save</span>.</li> 
</ol>

## Understand inherited permissions and the hierarchy of objects

* [Permissions inherited from parent objects](#inherited-permissions-from-higher-ranking-objects) 
* [Permissions acquired through organizational memberships](#permissions-acquired-via-memberships)&nbsp;

### Permissions inherited from parent objects

Permissions in *Workfront* are inherited hierarchically. This means that if you are granting permissions to a user on a parent object, they gain the same permissions on the children objects associated with it by default.

For example, if you give a user Contribute permissions to a project, the user has Contribute permissions to all tasks and issues (child objects) associated with that project.

Continuing with the example above, you cannot restrict permissions to child objects. If you do not want the user to have Contribute permissions to child objects associated with the project, you must manually remove the Inherited Permissions from the objects and then adjust the permissions for the individual user, including any Advanced Settings.&nbsp;

For more information about the hierarchy and interdependency of objects in *Workfront*, see the section [Interdependency and hierarchy of objects](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) in the article [Understand objects in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Your *Workfront administrator* can disable inherited permissions for documents in your access level.&nbsp;For more information about disabling inherited permissions for documents in the access level, see [Create or modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### Permissions acquired through organizational memberships&nbsp;

If you grant Manage permissions to a Group of users on an object, and you grant View permissions to an individual user in that Group on the same object, the user has the highest level of permissions (Manage) granted through the Group membership on the object.&nbsp;

If you want to grant lower permissions to a user who is already part of an organizational unit (Group, Team, Job Role, or Company) with a higher permission level, you must remove the permissions from the organizational unit, and add users individually with a lower level of permissions.&nbsp;&nbsp;

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2><a name="Removing"></a>Remove permissions from objects</h2>
<p>You can remove permissions from objects you have access to Share. Removing permissions from objects is identical for all objects that can be shared.&nbsp;</p> <note type="note">
&nbsp;You cannot remove permissions when you share items in bulk. You can remove permissions only when selecting individual items.&nbsp;
</note>
<p>To remove permissions from objects consider the following:&nbsp;</p>
<ul>
<li><a href="#removing-entities-from-objects" class="MCXref xref">Remove entities from the sharing list of an object</a> </li>
<li><a href="#remove-inherited-permissions" class="MCXref xref">Remove inherited permissions</a> </li>
<li><a href="#making-an-object-private" class="MCXref xref">Make an object private</a> </li>
</ul>
<h3><a name="removing-entities-from-objects"></a>Remove entities from the sharing list of an object</h3>
<p>You can remove entities from the sharing list of an object to remove their permissions from the object.</p>
<p>To remove permissions from objects:&nbsp;</p>
<ol>
<li value="1">Navigate to an object on which you want to modify the permissions.</li>
<li value="2">Click the <span class="bold">Actions</span> menu, then click <span class="bold">Sharing</span>.<br>For example, on a project, click <span class="bold">Project Actions</span>, then <span class="bold">Sharing</span>.&nbsp;</li>
<li value="3">Click the <span class="bold">x</span> next to the name of a user, team, group, company, job role to remove them.<br></li>
<li value="4">In the <span class="bold"><User Name>'s <em>Workfront</em> access will be removed from this</span> drop-down menu, select whether you want their access to be removed just from the object you have selected, or from all children objects associated with it.<br>The following scenarios exist:
<ul>
<li>If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they are granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.&nbsp;</li>
<li>If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they have been given individual permission on each child object.&nbsp;</li>
</ul></li>
<li value="5">Click <span class="bold">Save</span>.</li>
</ol>
<p> <h3><a name="remove-inherited-permissions"></a>Remove inherited permissions</h3> </p>
<p>Inherited permissions can be removed from objects allowing for owners to specifically&nbsp;identify who will get access to children objects regardless of the access of a user to a parent object. Only users with Manage permission are able to remove inherited permissions.</p>
<p>To remove inherited permissions:</p>
<ol>
<li value="1">Navigate to an object to which you have Manage permissions. <br>For example, navigate to a task.</li>
<li value="2">Go to the sharing list as described in the <a href="#share" class="MCXref xref"></a> section in this article. </li>
<li value="3">Select the <span class="bold">X</span>&nbsp;mark next to <span class="bold">Inherited Permission</span>&nbsp;on the sharing box to remove&nbsp;anyone listed there.<br><br>This ensures that no one who is granted permissions to the parent object (for example, the project) has permissions to this task by default. You must list&nbsp; individual entities in the sharing list of the task to grant permissions on the task.<br><note type="note">
You cannot remove individual entities from the Inherited Permissions list. You can only disable the Inherited Permissions for all entities listed.
</note></li>
<li value="4">Click <span class="bold">Save</span>.&nbsp;</li>
</ol>
<h3><a name="making-an-object-private"></a>Make an object private</h3>
<p>If you have shared an object system-wide, or you have shared it with external uses by making it public, you can make it private again by removing the system-wide or public permissions.&nbsp;</p>
<p>For more information about making an object available system-wide, or publicly, see the section <a href="#share" class="MCXref xref"></a> in this article.</p>
<p>To make an object private:</p>
<ol>
<li value="1">Go to the object you want to make private.<br>For example, navigate to a report.</li>
<li value="2">Click <span class="bold">Report Actions</span>, then <span class="bold">Sharing</span>.<br><br></li>
<li value="3">Click <span class="bold">Remove public access</span> to remove the access of external users to viewing the report.</li>
<li value="4">Click <span class="bold">Remove system-wide access</span> to stop sharing it with all <em>Workfront</em> users.&nbsp;</li>
<li value="5">Click <span class="bold">Save</span>.</li>
</ol>
</div>
-->

## Remove permissions from objects

You can remove permissions from objects you have access to Share. Removing permissions from objects is identical for all objects that can be shared.&nbsp;

>[!NOTE]
>
>&nbsp;You cannot remove permissions when you share items in bulk. You can remove permissions only when selecting individual items.&nbsp;

To remove permissions from objects consider the following:&nbsp;

* [Remove entities from the sharing list of an object](#removing-entities-from-objects) 
* [Remove inherited permissions](#remove-inherited-permissions) 
* [Make an object private](#making-an-object-private)

### Remove entities from the sharing list of an object

You can remove entities from the sharing list of an object to remove their permissions from the object.

To remove permissions from objects:&nbsp;

1. Navigate to an object on which you want to modify the permissions.
1. Click the `Actions` menu, then click `Sharing`.  
   For example, on a project, click `Project Actions`, then `Sharing`.&nbsp;

1. Click the `x` next to the name of a user, team, group, company, job role to remove them.  

1. In the `<User Name>'s *Workfront* access will be removed from this` drop-down menu, select whether you want their access to be removed just from the object you have selected, or from all children objects associated with it.  
   The following scenarios exist:

  * If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they are granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.&nbsp;
  * If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they have been given individual permission on each child object.&nbsp;

1. Click `Save`.

### Remove inherited permissions

Inherited permissions can be removed from objects allowing for owners to specifically&nbsp;identify who will get access to children objects regardless of the access of a user to a parent object. Only users with Manage permission are able to remove inherited permissions.

To remove inherited permissions:

<ol> 
 <li value="1">Navigate to an object to which you have Manage permissions. <br>For example, navigate to a task.</li> 
 <li value="2">Go to the sharing list as described in the <a href="#share" class="MCXref xref"></a> section in this article. </li> 
 <li value="3">Select the <span class="bold">X</span>&nbsp;mark next to <span class="bold">Inherited Permission</span>&nbsp;on the sharing box to remove&nbsp;anyone listed there.<br><br>This ensures that no one who is granted permissions to the parent object (for example, the project) has permissions to this task by default. You must list&nbsp; individual entities in the sharing list of the task to grant permissions on the task.<br><note type="note">
    You cannot remove individual entities from the Inherited Permissions list. You can only disable the Inherited Permissions for all entities listed.
  </note></li> 
 <li value="4">Click <span class="bold">Save</span>.&nbsp;</li> 
</ol>

### Make an object private

If you have shared an object system-wide, or you have shared it with external uses by making it public, you can make it private again by removing the system-wide or public permissions.&nbsp;

For more information about making an object available system-wide, or publicly, see the section [](#share) in this article.

To make an object private:

1. Go to the object you want to make private.  
   For example, navigate to a report.
1. Click `Report Actions`, then `Sharing`.

1. Click `Remove public access` to remove the access of external users to viewing the report.
1. Click `Remove system-wide access` to stop sharing it with all *Workfront* users.&nbsp;

1. Click `Save`.

## Share an object

For information about how to share objects, see [Share an object in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

## Remove permissions from objects

For information about how to remove permissions from objects, see [Remove permissions from objects in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Request permissions to objects

When someone sends you a link to an object which you do not have permissions to View, or when you have lower permissions on an object and you want to request a higher level of permissions, you can request permissions on the object.&nbsp;

You can request access to an object from anyone who has Share permission to the object.&nbsp;

For more information about requesting permissions to objects, see [Request access to objects in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/request-access.md).
