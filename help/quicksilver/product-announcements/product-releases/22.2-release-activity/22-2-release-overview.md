---
title: 22.2 Release overview
description: 22.2 Release overview
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: e490a955-b2cb-4b9b-9794-12ff2a2c2338
---
# 22.2 Release overview

This page provides information about functionality that is included in the 22.2 release. All features listed are available in the new Adobe Workfront experience. Some features are also available in Adobe Workfront Classic; however, [Workfront Classic will be discontinued in March 2022](https://one.workfront.com/s/new-workfront-experience), followed shortly by the end-of-life date for Workfront Classic in July 2022.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
to help you unlock productivity and collaboration.
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment. As the 22.2 release nears its planned Production release later this year
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
the week of January 17, 2022
</MadCap:conditionalText>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in October 2021
</MadCap:conditionalText>
, this page will be updated with all functionality included with 22.2. </p>
-->

These enhancements were made available in the Production environment the week of April 4, 2022.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment and will be made available in the Production environment
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
later this year
</MadCap:conditionalText>
the week of April 4, 2022, unless otherwise specified. For specific release dates and times for each cluster, see the <a href="https://status.adobe.com/en/products/5943" target="_blank">Adobe Workfront status page</a> on <a href="http://status.adobe.com/" target="_blank">status.adobe.com</a>. You must log in to see specific release times. </p>
-->

## Adobe Workfront enhancements

* [Administrator enhancements](#administrator-enhancements) 
* [Project enhancements](#project-enhancements) 
* [Resource Management enhancements](#resource-management-enhancements) 
* [Home enhancements](#home-enhancements) 
* [Mobile enhancements](#mobile-enhancements) 
* [Integrations enhancements](#integrations-enhancements) 
* [Other enhancements](#other-enhancements)

### Administrator enhancements {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Feature</strong> </p> </td> 
   <td> <p><strong>Release dates and environments</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">Configure a custom form to work with multiple object types</a> </p> <p>Now you can configure a new or existing custom form to work with multiple object types, making the form much more widely useful. Users will be able to attach and fill out the form on objects of all types that you configure it for.</p> <p>Previously you could configure a custom form to work with only one object type.</p> <p>This functionality works with all custom forms created previously in your Workfront system. For example, if you already have a custom form that was created for the Task object type, you can now configure it to work with other object types as well, such as Project and Issue.</p> </td> 
   <td> <p><b>Available on these dates:</b> </p> 
    <ul> 
     <li> <p>Preview release: March 10, 2022<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release </p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#blueprin" class="MCXref xref" xrefformat="{para}">Blueprints catalog is available to all users, and administrators can allow requests</a> </p> <p>All Adobe Workfront users can now browse the catalog of available blueprints. </p> <p>Additionally, the system administrator can enable access for users to request installation of blueprints. Assigning a request queue to store the requests allows users to make requests from the blueprints catalog. </p> </td> 
   <td> <p><b>Available on these dates:</b> </p> 
    <ul> 
     <li> <p>Preview release: March 10, 2022<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release </p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#add" class="MCXref xref" xrefformat="{para}">Add an image to a custom form</a> </p> <p>In a custom form that you create or edit, you can now add an image and include an informational or instructive tooltip that users can read when they hover over it.</p> <p>This could be helpful, for example, to show branding for a new product, or to provide visual information that people need when they are filling out the form.</p> <p>Previously, custom forms were completely text based.</p> </td> 
   <td> <p><b>Available on these dates:</b> </p> 
    <ul> 
     <li> <p>Preview release: March 10, 2022<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release </p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#deactiva" class="MCXref xref" xrefformat="{para}">Deactivate a group</a> </p> <p>As your internal organizations change, you might need to stop using certain groups in Workfront and create new ones. To help with this, we have added the ability to deactivate a group without losing its historical data. For regular users who don't need to see them, inactive groups are cleared from group type-ahead fields.</p> <p>You can still find and configure options, preferences, and object associations for inactive groups that you manage. And deactivating a group doesn't change anything about the objects that the group is attached to.</p> <p>Previously, it wasn't possible to deactivate a group.</p> </td> 
   <td> <p><b>Available on these dates:</b> </p> 
    <ul> 
     <li> <p>Preview release: March 10, 2022<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release </p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#new" class="MCXref xref" xrefformat="{para}">New default access level configurations</a> </p> <p>To better suit the needs of most administrators who create access levels, we've changed the default configuration for several of the “Fine-tune your settings” options that display when you click the gear icon on an Edit button.</p> <p>The options, previously enabled by default, are now disabled. If this doesn't suit the needs of your organization, you can enable them when you are setting up a new access level, or any time later.</p> </td> 
   <td> <p><b>Available on these dates:</b> </p> 
    <ul> 
     <li> <p>Preview release: January 27, 2022<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release </p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic will be discontinued in March 2022</a>, followed shortly by the end-of-life date for Workfront Classic in July 2022.)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#blueprin2" class="MCXref xref" xrefformat="{para}">Blueprints installation history enhancements</a> </p> <p>When you install a blueprint, a message now displays the specific objects (such as roles, teams, or groups) that were successfully installed with the blueprint and any objects that failed to install. You can also view the list of installed objects on the Blueprint Details page by clicking View Details next to a specific installation in the installation history table.</p> </td> 
   <td> <p><b>Available on these dates:</b> </p> 
    <ul> 
     <li> <p>Preview release: February 10, 2022<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release </p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#a" class="MCXref xref" xrefformat="{para}">A warning now displays when installing a Preview-only blueprint in Production</a> </p> <p>Certain blueprints are only available to install in the Preview environment for testing purposes.</p> <p>If you access Preview-only content in your Production environment, Sandbox 1, or Sandbox 2, the install button is not active, and you might see a warning message.</p> </td> 
   <td><b>Available on these dates:</b> 
    <ul> 
     <li> <p>Preview release: February 10, 2022<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release </p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Project enhancements {#project-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Feature</strong> </p> </td> 
   <td> <p><strong>Release dates and environments</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#adobe" class="MCXref xref" xrefformat="{para}">Adobe Workfront Boards are now available! </a> </p> <p>Boards are flexible tools that allow team collaboration by providing access to a shared board containing columns and cards. </p> <p>Using boards, you can quickly set up a task board with multiple columns, configure columns to show a status or category, add other users to the board and assign them to cards, and more.</p> </td> 
   <td> <p><b>Available on these dates:</b> </p> 
    <ul> 
     <li> <p>Preview release: March 10, 2022<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release </p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#addition" class="MCXref xref" xrefformat="{para}">Additional improvements to Workfront Boards</a></p> <p>The following additional improvements are now available for Workfront Boards:</p> 
    <ul> 
     <li> <p>Tag cards on Boards</p> </li> 
     <li> <p>Move cards</p> </li> 
     <li> <p>Copy cards</p> </li> 
     <li> <p>Search in Boards</p> </li> 
     <li> <p>Set a due date for a card in Boards</p> </li> 
    </ul> </td> 
   <td><b>Available on these dates:</b> 
    <ul> 
     <li> <p>Preview release: March 24, 2022<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release </p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#undo" class="MCXref xref" xrefformat="{para}">Undo option for Update posts</a> </p> <p>It is now easier to catch mistakes when posting an update. Finalizing a comment in an object's Update tab now creates a pop-up window for 7 seconds that allows you to cancel the post and return to editing--before the system timestamps it or sends any emails and in-app notifications. If you dismiss the pop-up window, leave the page, or wait 7 seconds for the window to time out, the post will be made normally.</p> </td> 
   <td> <p><b>Available on these dates:</b> </p> 
    <ul> 
     <li> <p>Preview release: March 10, 2022<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release </p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#new" class="MCXref xref" xrefformat="{para}">New experience when copying a project</a> </p> <p>To make your use of Workfront consistent with the new Adobe Workfront experience, we have redesigned the interface for copying projects. This is currently available when copying a project from the project page or when copying a project from a list or report. Prior to this update you could only copy a project from the project page.</p> </td> 
   <td> <p><b>Available on these dates:</b> </p> 
    <ul> 
     <li> <p>Preview release: March 10, 2022<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release </p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#ability" class="MCXref xref" xrefformat="{para}">Ability to manage projects from lists and reports from a new More menu</a> </p> <p>We have added a new More menu in project lists and reports to allow you to perform the following actions from these areas:</p> 
    <ul> 
     <li> <p>For several projects at a time:</p> </li> 
     <li> <p>Recalculate Timeline</p> </li> 
     <li> <p>Recalculate Finance</p> </li> 
     <li> <p>Recalculate Custom Expressions</p> </li> 
     <li> <p>For a single project:</p> </li> 
     <li> <p>Attach Template</p> </li> 
     <li> <p>Export to MS Project</p> </li> 
     <li> <p>Subscribe</p> </li> 
    </ul> </td> 
   <td> <p><b>Available on these dates:</b> </p> 
    <ul> 
     <li> <p>Preview release: March 10, 2022<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release </p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">New experience when converting an issue to a project using a template at the issue level</a> </p> <p>To make your use of Workfront consistent with the new Workfront experience, we have redesigned the interface for converting an issue to a project when using a template when you convert it from the issue page.</p> <p>You can now more easily access your list of favorites immediately after selecting to convert the issue.</p> <p>The redesigned interface matches the experience when creating a project from a template which we have also updated recently.</p> </td> 
   <td><strong>Available on these dates:</strong> 
    <ul> 
     <li> <p>Preview release:&nbsp;December 8, 2021<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.1 release <span style="color: #ff0000; font-weight: bold;">This feature was temporarily removed from the Production environment on March 4, 2022. It was later released in a phased roll-out beginning April 28, 2022. The roll-out was completed on May 5, 2022. This is now available in Preview and Production for all customers.</span></p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#convert" class="MCXref xref" xrefformat="{para}">Convert issues to projects using a template from lists, reports, and dashboards</a> </p> <p>To increase the efficiency of your work and make it easier for you to convert issues in a fast-paced environment, we have added the ability to convert an issue to a project using a template from a list, report, or a dashboard.</p> <p>Prior to this enhancement, this functionality existed only when you converted the issue from the issue page.</p> </td> 
   <td><strong>Available on these dates:</strong> 
    <ul> 
     <li> <p>Preview release:&nbsp;December 8, 2021<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.1 release <span style="color: #ff0000; font-weight: bold;">This feature was temporarily removed from the Production environment on March 4, 2022. It was later released in a phased roll-out beginning April 28, 2022. The roll-out was completed on May 5, 2022. This is now available in Preview and Production for all customers.</span></p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#updated" class="MCXref xref" xrefformat="{para}">Updated experience when copying and moving issues</a> </p> <p>To make your use of Workfront consistent with the new Adobe Workfront experience, we have redesigned the interface for copying and moving issues. This is currently available when copying or moving a single issue or when copying or moving issues in bulk from a list or report.</p> </td> 
   <td><strong>Available on these dates:</strong> 
    <ul> 
     <li> <p>Preview release: February 18, 2022<br></p> </li> 
     <li> <p>Production release: With the 22.2 release</p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#keep" class="MCXref xref" xrefformat="{para}">Keep users on the dashboard, list, or report after converting issue to project</a> </p> <p>To increase efficiency and eliminate the number of clicks, we have released an improvement when converting issues to projects from a list, report, or a dashboard.</p> <p>Users remain on the list, report or a dashboard after converting an issue to a project instead of being redirected to the project's page. A success notification with the link to the project displays after the conversion is complete, to allow you to easily navigate to the project, if needed. </p> </td> 
   <td><strong>Available on these dates:</strong> 
    <ul> 
     <li> <p>Preview release: February 10, 2022<br></p> </li> 
     <li> <p>Production release:&nbsp;February 24, 2022</p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#allocati" class="MCXref xref" xrefformat="{para}">Allocation hours will no longer be removed when making changes to assignments</a> </p> <p>To ensure the accuracy of your data, we have made a change to preserve allocation hours and to keep task Planned Hours unchanged when making changes to assignments on the task.</p> <p>The following changes have been made to tasks with a Simple Duration Type:</p> 
    <ul> 
     <li> <p>Individual assignment allocations are preserved when replacing users and roles.</p> </li> 
     <li> <p>Individual assignment allocations are preserved on the role when removing the user.</p> </li> 
     <li> <p>Planned Hours are preserved when removing all assignees. <span style="color: #ff0000;">(Removed from release. Now, Planned Hours will be set to 0 after removing all assignees.)</span></p> </li> 
    </ul> </td> 
   <td><strong>Available on these dates:</strong> 
    <ul> 
     <li> <p>Preview release: February 10, 2022<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release <span style="color: #ff0000; font-weight: bold;">This feature will be released to Production shortly after the 22.2 release</span></p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic will be discontinued in March 2022</a>, followed shortly by the end-of-life date for Workfront Classic in July 2022.)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#share" class="MCXref xref" xrefformat="{para}">Share folders only in the top five levels of a folder hierarchy</a> </p> <p>To ensure the best performance for users sharing folders, we are currently limiting sharing to the top five levels in a folder hierarchy on an object.</p> <p>Each folder at the sixth level or below inherits its sharing configurations from the folder directly above it.</p> </td> 
   <td><strong>Available on these dates:</strong> 
    <ul> 
     <li> <p>Preview release: February 10, 2022<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release <span style="color: #ff0000; font-weight: bold;">This feature is temporarily unavailable. This page will be updated when the feature is available in Production.</span></p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic will be discontinued in March 2022</a>, followed shortly by the end-of-life date for Workfront Classic in July 2022.)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Resource Management enhancements {#resource-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Feature</strong> </p> </td> 
   <td> <p><strong>Release dates and environments</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-resource-management-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">Improvements to the Workload Balancer navigation</a> </p> <p>To improve your experience when using the Workload Balancer, we have introduced the following enhancements:</p> 
    <ul> 
     <li> <p>The Cancel and Save buttons when adjusting allocations are now sticky, even when the task is longer than the timeframe included on the screen or when the Summary panel displays.</p> </li> 
     <li> <p>The left panel that displays the names of users and work items is now sticky, to allow you to scroll horizontally for longer timeframes and to still be able to read the names of items listed in the panel.</p> </li> 
     <li> <p>You can collapse and expand all items listed in the left panel with one click instead of at the user or project level.</p> </li> 
     <li> <p>The left panel is now also resizable.</p> </li> 
     <li> <p>There is now a full-screen mode for the Workload Balancer.</p> </li> 
    </ul> </td> 
   <td> <p><b>Available on these dates:</b> </p> 
    <ul> 
     <li> <p>Preview release: March 10, 2022<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release </p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-resource-management-enhancements.md#access" class="MCXref xref" xrefformat="{para}">Access Advanced Assignments in the Workload Balancer</a> </p> <p>To make assigning work items easier and more accurate, you can now make advanced assignments when you assign work items manually in the Workload Balancer. Prior to this enhancement, you could access Advanced Assignments when editing items, from the items' headers, or in lists.</p> </td> 
   <td> <p><b>Available on these dates:</b> </p> 
    <ul> 
     <li> <p>Preview release: March 10, 2022<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release </p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-resource-management-enhancements.md#new" class="MCXref xref" xrefformat="{para}">New formula for calculating user availability when The Default Schedule preference is selected</a> </p> <p>To provide more accurate information in resource management tools, we have changed the formula that Workfront uses to calculate user availability when the Workfront administrator selects The Default Schedule in Resource Management Preferences. With the new update, Workfront uses the following formula to calculate user availability:</p> <p>User Available Hours = (Default Schedule Hours - Exceptions) * FTE - Time off hours</p> <p>Prior to this update, Workfront used the following formula to calculate user availability when The Default Schedule was selected:</p> <p>User Available Hours = (Default Schedule Hours - (Schedule Exceptions + Time off hours)) * User FTE value</p> </td> 
   <td> <p><b>Available on these dates:</b> </p> 
    <ul> 
     <li> <p>Preview release: March 10, 2022<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release </p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic will be discontinued in March 2022</a>, followed shortly by the end-of-life date for Workfront Classic in July 2022.)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Home enhancements {#home-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Feature</strong> </p> </td> 
   <td> <p><strong>Release dates and environments</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-home-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">Improvements to filters in the Home Work List</a> </p> <p>To give more control and focus over your work list, we have implemented several improvements to the filters in the Home area. With the new improvements, you can select filters by object type and further narrow down your results by the state of your work items (for example, Ready to Start, Working On, or Requested). The new Home filters now provide a correct count of tasks, issues, personal work items, and approvals when you apply a combination of object type and work item state filters.</p> <p>Prior to this experience, the filters in the Home area did not provide an accurate count of the number of work items in the list when you selected one or more filters and they created confusion about the state of the work items.</p> </td> 
   <td> <p><b>Available on these dates:</b> </p> 
    <ul> 
     <li> <p>Preview release: March 10, 2022<br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release </p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Mobile enhancements {#mobile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Feature</strong> </p> </td> 
   <td> <p><strong>Release dates and environments</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-mobile-enhancements.md#drawings" class="MCXref xref" xrefformat="{para}">Drawings and comments on proof documents in the mobile app</a></p> <p>The Adobe Workfront mobile app now allows you to add drawings and comments on proof documents. A new toolbar on the proof contains drawing tools for shapes. You can choose settings such as color and line thickness for each shape. Drawing a shape on the proof connects your comment to that area of the proof document.</p> <p>You can also reply to comments that others have made on the proof.</p> </td> 
   <td><strong>Available on these dates:</strong> 
    <ul> 
     <li> <p>Preview release:&nbsp;N/A<br></p> </li> 
     <li> <p>Production release:&nbsp;mid to late-April 2022 </p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>iOS mobile app</p> </li> 
     <li> <p>Android mobile app</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-mobile-enhancements.md#enhancem" class="MCXref xref" xrefformat="{para}">Enhancements to proof functionality in mobile app</a> </p> <p>In the Adobe Workfront mobile app, you can now:</p> 
    <ul> 
     <li> <p>Share proofs with internal and external recipients</p> </li> 
     <li> <p>View proof comments</p> </li> 
     <li> <p>Download proofs</p> </li> 
    </ul> </td> 
   <td><strong>Available on these dates:</strong> 
    <ul> 
     <li> <p>Preview release:&nbsp;N/A<br></p> </li> 
     <li> <p>Production release:&nbsp;Early February 2022 (These enhancements were originally communicated with the 22.1 release.)</p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>iOS mobile app</p> </li> 
     <li> <p>Android mobile app</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Integrations enhancements {#integrations-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Feature</strong> </p> </td> 
   <td> <p><strong>Release dates and environments</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#adobe" class="MCXref xref" xrefformat="{para}">Adobe Workfront with Anaplan integration now available</a> </p> <p>To give you better flexibility and insight into the financial aspects of your Workfront projects, Workfront can now integrate with your Anaplan account. By linking Workfront objects to Anaplan objects, you can update information between the two accounts automatically, ensuring that the information in both is up-to-date and identical. </p> <p>You can also trigger automated processes in Anaplan based on actions in Workfront (or vice versa).</p> <p>For example, you can create a campaign in Anaplan, then create a Workfront project or program linked to the campaign. Any costs tracked in Workfront can then be uploaded back to Anaplan to review campaign performance.</p> </td> 
   <td><strong>Available on these dates:</strong> 
    <ul> 
     <li> <p>Preview release: March 10, 2022<br></p> </li> 
     <li> <p>Production release: With the 22.2 release</p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Workfront for Experience Manager enhanced connector updates</a> </p> <p>Workfront for Experience Manager enhanced connector now includes the following updates:</p> 
    <ul> 
     <li> <p>You can now create linked folders between Adobe Workfront and Adobe Experience Manager Assets as a Cloud Service even if there are multiple project linked folder configurations.</p> </li> 
     <li> <p>Added support for event subscription pagination</p> </li> 
     <li> <p>Added support for AEM 6.4.x</p> </li> 
     <li> <p>Added support for proxy environments</p> </li> 
     <li> <p>Several bug fixes based on partner and customer feedback</p> </li> 
    </ul> </td> 
   <td><strong>Available on these dates:</strong> 
    <ul> 
     <li> <p>Preview release: N/A<br></p> </li> 
     <li> <p>Production release: March 28, 2022</p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
     <li> <p>Adobe Workfront Classic </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#see" class="MCXref xref" xrefformat="{para}">See details of the Client Secret for custom OAuth2 or JWT integrations</a> </p> <p>To provide transparency into the use of your custom OAuth2 and JWT integrations, we've made it possible for you to see details of the Client Secrets your integrations use. Now, you can see the dates that the Client Secret was created and last used. You can also add and view your own notes about the Client Secret.</p> <p>Previously, these details were unavailable.</p> </td> 
   <td><strong>Available on these dates:</strong> 
    <ul> 
     <li> <p>Preview release: March 3, 2022<br></p> </li> 
     <li> <p>Production release: With the 22.2 release</p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#adobe2" class="MCXref xref" xrefformat="{para}">Adobe Creative Cloud integrations now use OAuth2</a> </p> <p>For greater security, and to make a more consistent experience across integrations, we've updated the Adobe Creative Cloud integrations to use OAuth2 authentication, an industry-standard way to authenticate users. Now, when your users log in, they can see the specific actions and areas that the integrations have access to, and allow access. After this, they do not need to log in as frequently.</p> </td> 
   <td><strong>Available on these dates:</strong> 
    <ul> 
     <li> <p>Preview release: February 24, 2022<br></p> </li> 
     <li> <p>Production release: With the 22.2 release</p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#see2" class="MCXref xref" xrefformat="{para}">See type of authentication in list of custom OAuth2 applications</a> </p> <p>Now, when you view the list of custom OAuth2 applications in your organization, you can see whether each application uses User authentication or Server authentication.</p> <p>Previously, you could see this information only by going into the edit options on each application.</p> </td> 
   <td><strong>Available on these dates:</strong> 
    <ul> 
     <li> <p>Preview release: February 17, 2022<br></p> </li> 
     <li> <p>Production release: With the 22.2 release</p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#set" class="MCXref xref" xrefformat="{para}">Set expiration for refresh tokens in your custom OAuth2 integrations</a> </p> <p>To better control access and security for your custom OAuth2 integrations, you can now customize the lifespan of refresh tokens. After a user's refresh token expires, they will need to log in to the integration again.</p> </td> 
   <td> <p><b>Available on these dates:</b> </p> 
    <ul> 
     <li> <p>Preview release: February 10, 2022 <br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release </p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#use" class="MCXref xref" xrefformat="{para}">Use public and private keys in your custom OAuth2 integrations for server-to-server apps</a> </p> <p>You can now set up server-to-server OAuth2 applications in your custom integrations. By setting up public and private keys, you can allow Workfront to communicate with another application without using login credentials.</p> <p>Previously, all authentication in your custom OAuth2 applications used the user's login credentials.</p> </td> 
   <td> <p><b>Available on these dates:</b> </p> 
    <ul> 
     <li> <p>Preview release: February 10, 2022 <br></p> </li> 
     <li> <p>Production release:&nbsp;With the 22.2 release </p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Other enhancements {#other-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Feature</strong> </p> </td> 
   <td> <p><strong>Release dates and environments</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-look-and-feel-updates.md#enhancem" class="MCXref xref" xrefformat="{para}">Look-and-feel updates during the 22.2 release timeframe</a> </p> <p>Minor updates to the look and feel of various areas of the Adobe Workfront application are being made within the 22.2 release timeframe. These enhancements will be made available in the Production environment a minimum of 2 weeks after releasing to Preview. </p> </td> 
   <td><strong>Available on these dates:</strong> 
    <ul> 
     <li> <p>Preview release:&nbsp;Throughout the 22.2 release timeframe<br></p> </li> 
     <li> <p>Production release:&nbsp;A minimum of 2 weeks after releasing to Preview</p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-other-enhancements.md#enhancem" class="MCXref xref" xrefformat="{para}">Enhancements to top navigation bar</a> </p> <p>We have made several enhancements to the Adobe Workfront top navigation bar.</p> 
    <ul> 
     <li> <p>Favorites and Recents now have separate icons in the top navigation bar. Each still displays the same content (pages you have marked as favorites, and pages you have visited recently), and you can continue to add and remove favorite pages in the same way.</p> </li> 
     <li> <p>The look and feel of both pins and the main menu was updated to Adobe design standards, including colors and fonts. The way you add and remove pins and the areas you have access to in your main menu have not changed.</p> </li> 
     <li> <p>The icons on the right of the top navigation bar were re-ordered to be more intuitive. The icon order is: help link, notifications, favorites, recents, search, main menu.</p> </li> 
    </ul> </td> 
   <td><strong>Available on these dates:</strong> 
    <ul> 
     <li> <p>Preview release: March 10, 2022<br></p> </li> 
     <li> <p>Production release: With the 22.2 release</p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-other-enhancements.md#redesign" class="MCXref xref" xrefformat="{para}">Redesigned timesheet lists</a> </p> <p>To make your use of Workfront consistent with the new Adobe Workfront experience, we have redesigned the timesheet lists in the Timesheets area. You can expect the same functionality in the timesheet list, only with a cleaner, more streamlined user experience.</p> <p>Some of the highlights of this redesign are:</p> 
    <ul> 
     <li> <p>The timesheet list now matches the experience in all other lists in Workfront.</p> </li> 
     <li> <p>The filter experience now matches the filters in all other lists. You will have more flexibility to create your own filters with the fields and attributes that make the most sense to you as well as share them with other users.</p> </li> 
    </ul> </td> 
   <td><strong>Available on these dates:</strong> 
    <ul> 
     <li> <p>Preview release: March 10, 2022<br></p> </li> 
     <li> <p>Production release: With the 22.2 release</p> </li> 
    </ul> <p><strong>Available in these environments:</strong> </p> 
    <ul> 
     <li> <p>The new Adobe Workfront experience </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront Fusion enhancements

New features in Workfront Fusion are available in Production at a cadence outside of the 22.2 release schedule. For more information about the latest features, see [Adobe Workfront Fusion release activity](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

## Workfront Scenario Planner enhancements

There are no Scenario Planner updates at this point in the release. This area will be updated when updates are available.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features are coming to Workfront Scenario Planner release with the 21.4 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-activity.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront Scenario Planner release activity</a>.</p>
-->

## Workfront Proof enhancements

There are no Workfront Proof updates at this point in the release. This area will be updated when updates are available.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features in Workfront Proof are now available. For more information, see <a href="../../../product-announcements/product-releases/workfront-proof-release-activity/wp-release-22-1.md" class="MCXref xref" xrefformat="{para}">Workfront Proof release activity:&nbsp;Week of November 29, 2021</a>.</p>
-->

## Workfront Goals enhancements

There are no Workfront Goals updates at this point in the release. This area will be updated when updates are available.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Most new features coming to Workfront Goals release with the 21.2 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/goals-release-activity/goals-21.2-release/goals-release-21-2.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Adobe Workfront Goals with the 21.2 release</a>.</p>
-->

## API version 14

For API version 14, we've modified some resources and endpoints. Some of the changes support new functionality, and others make it easier for you to use the information available through the API.

For information on what's new and updated, see [What's new in API version 14](../../../wf-api/api/new-api-version-14.md).

For information on API versions, see [API versioning and support schedule](../../../wf-api/api/api-version-support-schedule.md).

## Workfront Maintenance Updates

For information about the maintenance updates made during the 22.2 release, see [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

## 22.2 Release Webinar

The Workfront 22.2 Release Webinar will be presented on March 24, 2022 at 8:00 a.m. MST. You can register for the event on the [Events page on Workfront One](https://webinars.on24.com/adobe_workfront/WF22point2?partnerref=WFOne). 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This area will be updated as more information becomes available.
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
was presented on January 12, 2022. You can view the webinar recording on the
<a href="https://one.workfront.com/s/event">Events page on Workfront One</a>.
</MadCap:conditionalText>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Functionality being removed from Production</h2>
<h3>Feature rollback: Carry over the existing proof workflow when generating a new version</h3>
<p>Due to customer feedback, <b>Workfront is removing this change from Preview environments on March 30, 2021 and from Production environments on March 31, 2021</b>.</p>
<p>On March 11, 2021, Workfront released a change to existing proof workflows in both Workfront Classic and the new Workfront experience. The change allowed for an existing workflow to carry over to any new proof versions created by a user, regardless of the method used to generate them.</p>
<p>In the new Workfront experience after this change is removed, proofs created with the Simple proof selection will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>In Workfront Classic after this change is removed, the option to Generate Proof will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>Similar functionality to easily copy existing workflows might be added to Production at a future time.</p>
</div>
-->

## Training updates

Explore the latest updates made to learning programs, learning paths, videos, and guides for each Adobe Workfront product release. For more information, see the [Training release updates page](https://one.workfront.com/s/training-release-updates).

## Functionality no longer supported

### Internet Explorer 11

With the removal of support for Internet Explorer, Workfront now officially supports Microsoft Edge.

For more information about supported browsers, see [Adobe Workfront browser requirements](../../../workfront-basics/workfront-browser-requirements.md).
