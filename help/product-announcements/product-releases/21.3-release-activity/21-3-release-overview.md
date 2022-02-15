---
filename: 21-3-release-overview
content-type: release-notes
keywords: notes,quarterly,update
navigation-topic: 2021-3-release-activity
---



# 21.3 Release overview {#release-overview}

This page provides information about functionality for both *`Adobe Workfront Classic`* and *`the new Adobe Workfront experience`* that is included in the 21.3 release.


These enhancements were made available in the Production environment the week of June 21, 2021.


## *`Adobe Workfront`* enhancements {#adobe-workfront-enhancements}




*  [Administrator enhancements](#administ) 
*  [Project enhancements](#project) 
*  [Resource Management enhancements](#resource) 
*  [Requests enhancements](#requests) 
*  [Proofing enhancements](#proofing) 
*  [Other enhancements](#other) 




### Administrator enhancements {#administrator-enhancements}


<table> 
 <col style="width: 50%;"> 
 <col style="width: 50%;"> 
 <tbody> 
  <tr> 
   <td> <p><span class="bold">Feature</span> </p> </td> 
   <td> <p><span class="bold">Release dates and environments</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-admin-enhancements.md#blueprin" class="MCXref xref" xrefformat="{para}">Blueprints available in Production with the 21.3 release</a> </p> <p>The blueprints functionality will be generally available with the 21.3 Production release the week of June 21, 2021.</p> <p>Blueprints provides basic building blocks to help you create a work management system that grows with you. System administrators can browse the blueprints catalog and install ready-to-use project templates.</p> </td> 
   <td><span class="bold">Available on these dates:</span> <p>Preview release:&nbsp;April 22, 2021 (with the 21.2 release)<br></p> <p>Production release:&nbsp;With the 21.3 release</p> <p><span class="bold">Available in these environments:</span> </p> <p><span class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-admin-enhancements.md#new" class="MCXref xref" xrefformat="{para}">New for group administrators: Create and manage statuses for a group at any level</a> </p> <p>To make it easier for all levels of an organization to manage and control their workflows independently, we’ve introduced the ability to create and manage statuses for subgroups. </p> </td> 
   <td><span class="bold">Available on these dates:</span> <p>Preview release:&nbsp;June 3, 2021<br></p> <p>Production release:&nbsp;With the 21.3 release</p> <p><span class="bold">Available in these environments:</span> </p> <p><span class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span> </p> <p><span class="mc-variable WFVariables.WorkfrontClassic variable varname">Adobe Workfront Classic</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-admin-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">New for administrators: Create a billing record custom form</a> </p> <p>Now you can improve how users capture billing information by creating a billing record custom form. Users can attach the custom form to a billing record, fill it out, and run reports that include the information in the form.</p> </td> 
   <td><span class="bold">Available on these dates:</span> <p>Preview release:&nbsp;May 20, 2021<br></p> <p>Production release:&nbsp;With the 21.3 release</p> <p><span class="bold">Available in these environments:</span> </p> <p><span class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span> </p> <p><span class="mc-variable WFVariables.WorkfrontClassic variable varname">Adobe Workfront Classic</span> </p> </td> 
  </tr> 
 </tbody> 
</table>



### Project enhancements {#project-enhancements}


<table> 
 <col style="width: 50%;"> 
 <col style="width: 50%;"> 
 <tbody> 
  <tr> 
   <td> <p><span class="bold">Feature</span> </p> </td> 
   <td> <p><span class="bold">Release dates and environments</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-project-enhancements.md#associat" class="MCXref xref" xrefformat="{para}">Associate a template with a group</a> </p> <p>To help you streamline the project creation process —and to help you more easily identify and report on which groups own which project templates—we’ve added the ability to assign a group to a project template.</p> <p>When you assign a group to a project template, all projects created from the template are automatically associated with the template's group.</p> <p>Also, you can attach a group approval process to a template and its template tasks if the template is associated with your group. </p> </td> 
   <td><span class="bold">Available on these dates:</span> <p>Preview release:&nbsp;June 3, 2021<br></p> <p>Production release:&nbsp;With the 21.3 release </p> <p><span class="bold">Available in these environments:</span> </p> <p><span class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-project-enhancements.md#easier" class="MCXref xref" xrefformat="{para}">Easier editing of fields in the Details section</a> </p> <p>Various improvements allow you to more easily edit information in the Details section of any object. These improvements include a gray outline around a field when hovering over it indicates that it is editable, as well as the ability to edit fields by clicking them once.</p> </td> 
   <td><span class="bold">Available on these dates:</span> <p>Preview release:&nbsp;June 3, 2021<br></p> <p>Production release:&nbsp;With the 21.3 release</p> <p><span class="bold">Available in these environments:</span> </p> <p><span class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-project-enhancements.md#consider" class="MCXref xref" xrefformat="{para}">Consider cross-project predecessors when calculating handoff dates</a> </p> <p>With a new improvement in the way Adobe Workfront calculates handoff dates for tasks, the cross-project dependencies are now taken into account. </p> <p>Previously, the handoff dates were calculated based only on the predecessors of the task from the same project. </p> <p>Now, to ensure you always have an accurate handoff date for a task with a cross-project predecessor, you must recalculate the timeline of the successor task's project. After recalculating the timeline, the handoff dates of the task calculates taking into account the cross-project dependencies of the tasks.</p> </td> 
   <td><span class="bold">Available on these dates:</span> <p>Preview release:&nbsp;June 3, 2021<br></p> <p>Production release:&nbsp;With the 21.3 release</p> <p><span class="bold">Available in these environments:</span> </p> <p><span class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span> </p> <p><span class="mc-variable WFVariables.WorkfrontClassic variable varname">Adobe Workfront Classic</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-project-enhancements.md#add" class="MCXref xref" xrefformat="{para}">Add existing stories and issues from the Scrum board</a> </p> <p>You can now add an existing story or issue directly from the Scrum board. This makes it easier to add existing stories to your current iteration without having to go to the backlog page.</p> </td> 
   <td><span class="bold">Available on these dates:</span> <p>Preview release:&nbsp;June 3, 2021<br></p> <p>Production release:&nbsp;With the 21.3 release</p> <p><span class="bold">Available in these environments:</span> </p> <p><span class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-project-enhancements.md#add2" class="MCXref xref" xrefformat="{para}">Add new stories and issues from the Scrum board</a> </p> <p>You can now create a new story or issue directly from the Scrum board. This makes it easier to quickly add a new story to your current iteration.</p> </td> 
   <td><span class="bold">Available on these dates:</span> <p>Preview release:&nbsp;June 3, 2021<br></p> <p>Production release:&nbsp;With the 21.3 release</p> <p><span class="bold">Available in these environments:</span> </p> <p><span class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-project-enhancements.md#delete" class="MCXref xref" xrefformat="{para}">Delete story or issue from the Kanban board</a> </p> <p>You can now delete a story or issue directly from your Kanban board by clicking the More icon on a story or issue card and selecting Delete. When you delete a story or issue, it is moved to the Recycle Bin for 30 days and can be recovered only by the system administrator.</p> </td> 
   <td><span class="bold">Available on these dates:</span> <p>Preview release:&nbsp;June 3, 2021<br></p> <p>Production release:&nbsp;With the 21.3 release</p> <p><span class="bold">Available in these environments:</span> </p> <p><span class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-project-enhancements.md#agile" class="MCXref xref" xrefformat="{para}">Agile card header and story board updates</a> </p> <p>On Kanban and Scrum boards, various enhancements are now available, including a fixed width for story cards and board columns, the renaming of the Stories column to Parent Story, and more.</p> </td> 
   <td><span class="bold">Available on these dates:</span> <p>Preview release:&nbsp;June 3, 2021<br></p> <p>Production release:&nbsp;With the 21.3 release</p> <p><span class="bold">Available in these environments:</span> </p> <p><span class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-project-enhancements.md#group" class="MCXref xref" xrefformat="{para}">Group project, task, and issue preferences</a> </p> <p>As we communicated earlier, we rolled out group-level customizations for project, task, and issue preferences in phases. Until June 24, 2021, they were available in Production for all EMEA customers and for a subset of all other customers. Now they are available to all customers.</p> </td> 
   <td><span class="bold">Available on these dates:</span> <p>Preview release:&nbsp;</p> <p>July 9, 2020 (project preferences for groups)</p> <p>December 3, 2020 (task and issue preferences for groups)<br></p> <p>Production release:&nbsp;With the 21.3 release (was available only for a limited number of customers, available to all customers June 24, 2021)</p> <p><span class="bold">Available in these environments:</span> </p> <p><span class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span> </p> <p><span class="mc-variable WFVariables.WorkfrontClassic variable varname">Adobe Workfront Classic</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-project-enhancements.md#allow" class="MCXref xref" xrefformat="{para}">Allow external users to approve a document</a> </p> <p>You can now use external email addresses to assign approvers to a document in the new Workfront experience.</p> <p>Previously, you could add external users by email address only in Workfront Classic.</p> </td> 
   <td><span class="bold">Available on these dates:</span> <p>Preview release:&nbsp;May 20, 2021<br></p> <p>Production release:&nbsp;With the 21.3 release</p> <p><span class="bold">Available in these environments:</span> </p> <p><span class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-project-enhancements.md#export" class="MCXref xref" xrefformat="{para}">Export information from the Details section of a portfolio or program</a> </p> <p>You can now export to a .pdf file information from the Details section of portfolios and programs. Prior to this enhancement, you could export information from the Details section only from projects, tasks and issues.</p> </td> 
   <td> <p><span class="bold">Available on these dates:</span> </p> <p>Preview release:&nbsp;May 20, 2021<br></p> <p>Production release:&nbsp;June 3, 2021</p> <p><span class="bold">Available in these environments:</span> </p> <p><span class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-project-enhancements.md#added" class="MCXref xref" xrefformat="{para}">Added Planned Completion Date timestamp in the object’s header</a> </p> <p>To facilitate easy access, convenience as well as accuracy, we have added the option to select a timestamp in the Planned Completion Date of the header of projects, tasks, or issues. </p> <p>Prior to this enhancement, when you updated the Planned Completion Date of an object, Workfront selected midnight as the default time. Now, you can customize the time as well as the completion date.</p> </td> 
   <td><span class="bold">Available on these dates:</span> <p>Preview release:&nbsp;May 20, 2021<br></p> <p>Production release:&nbsp;With the 21.3 release</p> <p><span class="bold">Available in these environments:</span> </p> <p><span class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-project-enhancements.md#add3" class="MCXref xref" xrefformat="{para}">Add a custom form to an object without editing it</a> </p> <p>We have made it easier to add a custom form that someone else will fill out—or that you will fill out later—to an object. The form no longer goes into editing mode automatically when you add it. You can simply save the empty form to the object.</p> <p>Previously, when you added a custom form to an object, the page went into editing mode and you had to complete any required fields on the form before you could save it to the object. This was inconvenient when the form was meant for another user to fill out, or when you did not know yet what to put in a required field on the form.</p> </td> 
   <td><span class="bold">Available on these dates:</span> <p>Preview release:&nbsp;May 20, 2021<br></p> <p>Production release:&nbsp;With the 21.3 release</p> <p><span class="bold">Available in these environments:</span> </p> <p><span class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span> </p> </td> 
  </tr> 
 </tbody> 
</table>



### Resource Management enhancements {#resource-management-enhancements}


<table> 
 <col style="width: 50%;"> 
 <col style="width: 50%;"> 
 <tbody> 
  <tr> 
   <td> <p><span class="bold">Feature</span> </p> </td> 
   <td> <p><span class="bold">Release dates and environments</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-resource-management-enhancements.md#deactiva" class="MCXref xref" xrefformat="{para}">Deactivate roles no longer in use</a> </p> <p>To offer you the same experience as with users, teams, and companies, we have introduced a new feature that allows you to deactivate roles you no longer use. When you deactivate a role, it is no longer available for selection in typeahead fields for assigning and sharing objects. Deactivated roles still appear in search fields and filter options.</p> <p>Tasks and issues assigned to a deactivated role as well as approval processes or routing rules continue to be assigned to these roles. You must update these objects to replace the inactive role with an active one, if they are yet to be completed.</p> </td> 
   <td> <p><span class="bold">Available on these dates:</span> </p> <p>Preview release:&nbsp;May 27, 2021<br></p> <p>Production release:&nbsp;June 10, 2021</p> <p><span class="bold">Available in these environments:</span> </p> <p><span class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span> </p> <p><span class="mc-variable WFVariables.WorkfrontClassic variable varname">Adobe Workfront Classic</span> </p> </td> 
  </tr> 
 </tbody> 
</table>



### Requests enhancements {#requests-enhancements}


<table> 
 <col style="width: 50%;"> 
 <col style="width: 50%;"> 
 <tbody> 
  <tr> 
   <td> <p><span class="bold">Feature</span> </p> </td> 
   <td> <p><span class="bold">Release dates and environments</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-requests-enhancements.md#find" class="MCXref xref" xrefformat="{para}">Find requests by recent paths or by searching using a keyword</a> </p> <p>To help you find the right request queue faster by referring to recently logged requests, we have introduced the following improvements to finding a recently used queue:</p> 
    <ul> 
     <li> <p>A list of the recent paths for which you have entered requests</p> </li> 
     <li> <p>The ability to search for a request type by any keyword included in a path.</p> </li> 
    </ul> <p>A path includes the request queue and all the topic groups and queue topics that you have selected before when submitting a request.</p> </td> 
   <td> <p><span class="bold">Available on these dates:</span> </p> <p>Preview release:&nbsp;June 3, 2021<br></p> <p>Production release:&nbsp;With the 21.3 release</p> <p><span class="bold">Available in these environments:</span> </p> <p><span class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span> </p> </td> 
  </tr> 
 </tbody> 
</table>



### Proofing enhancements {#proofing-enhancements}


<table> 
 <col style="width: 50%;"> 
 <col style="width: 50%;"> 
 <tbody> 
  <tr> 
   <td> <p><span class="bold">Feature</span> </p> </td> 
   <td> <p><span class="bold">Release dates and environments</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-proofing-enhancements.md#remove" class="MCXref xref" xrefformat="{para}">Remove ability to create a new document or proof version in a linked folder</a> </p> <p>We removed the ability to create a new version of a document or proof within a linked folder. You can still create a new version of a linked document or proof if they are outside of a linked folder.</p> <p>Previously, this option still displayed for documents and proofs in linked folders, but users were unable to create a new version of a document.</p> </td> 
   <td><span class="bold">Available on these dates:</span> <p>Preview release:&nbsp;June 3, 2021<br></p> <p>Production release:&nbsp;June 3, 2021</p> <p><span class="bold">Available in these environments:</span> </p> <p><span class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span> </p> <p><span class="mc-variable WFVariables.WorkfrontClassic variable varname">Adobe Workfront Classic</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-proofing-enhancements.md#users" class="MCXref xref" xrefformat="{para}">Users added to a proof automatically granted View access on a document</a> </p> <p>Users with Reviewer or Read-only selected as their proof role are automatically granted View access on the document if they had none previously.</p> <p>Previously, users with the proof roles mentioned above had to request access to documents when they were added to the proof.</p> </td> 
   <td><span class="bold"><p><span class="bold">Available on these dates:</span></p><p style="font-weight: normal;">Preview release:&nbsp;May 20, 2021<br></p><p style="font-weight: normal;">Production release:&nbsp;June 17, 2021</p><p><span class="bold">Available in these environments:</span></p><p><span style="font-weight: normal;" class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span> </p></span><span class="mc-variable WFVariables.WorkfrontClassic variable varname">Adobe Workfront Classic</span> </td> 
  </tr> 
 </tbody> 
</table>



### Other enhancements {#other-enhancements}


<table> 
 <col style="width: 50%;"> 
 <col style="width: 50%;"> 
 <tbody> 
  <tr> 
   <td> <p><span class="bold">Feature</span> </p> </td> 
   <td> <p><span class="bold">Release dates and environments</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-other-enhancements.md#home" class="MCXref xref" xrefformat="{para}">Home area redesign for mobile app</a> </p> <p>Various enhancements have been added to the home area in the Adobe Workfront mobile app, including: a redesigned work item widgets and a larger search box help you find what you need quickly; the navigation bar for home, virtual assistant, quick task, notifications, and user profile now "floats" over the home area for easy access; and the My Work menu scrolls horizontally and shows these items: Projects, Tasks &amp; Issues, Requests, Approvals, and Timesheets. Up to three cards for the selected item are displayed below the menu.</p> </td> 
   <td> <p><span class="bold">Available on these dates:</span> </p> <p>Preview release:&nbsp;N/A<br></p> <p>Production release:&nbsp;With the 21.3 release</p> <p><span class="bold">Available in these environments:</span> </p> <p>iOS</p> <p>Android</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="21-3-other-enhancements.md#event" class="MCXref xref" xrefformat="{para}">Event subscription filters</a> </p> <p>Event subscription filters are now enabled in preview environments. Event subscription filtering can be used to ensure that you receive only relevant messages. Creating filters for your subscriptions may significantly decrease the number of messages that your endpoint needs to consume. </p> </td> 
   <td><span class="bold"><p><span class="bold">Available on these dates:</span></p><p style="font-weight: normal;">Preview release:&nbsp;May 20, 2021<br></p><p style="font-weight: normal;">Production release:&nbsp;June 3, 2021</p><p><span class="bold">Available in these environments:</span></p><p><span style="font-weight: normal;" class="mc-variable WFVariables.Quicksilver-Capitalized variable varname">The new Adobe Workfront experience</span></p></span><span class="mc-variable WFVariables.WorkfrontClassic variable varname">Adobe Workfront Classic</span> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;


## *`Workfront`* *`Scenario Planner`* enhancements {#workfront-scenario-planner-enhancements}

New features are coming to Workfront Scenario Planner release with the 21.3 release. For information about these new features now available in Preview, see [Adobe Workfront Scenario Planner with the 21.3 release](sp-release-21-3.md).


## *`Workfront Fusion`* enhancements {#workfront-fusion-enhancements}

New features in *`Workfront Fusion`* are available in Production at a cadence outside of the 21.3 release schedule. For more information about the latest features, see [Adobe Workfront Fusion release activity](fusion-release-activity.md).


## *`Workfront Proof`* enhancements {#workfront-proof-enhancements}

New features in *`Workfront Proof`* are now available. For more information, see [Workfront Proof release activity: Week of May 17, 2021](wp-release-may-17.md).


## *`Workfront Goals`* enhancements {#workfront-goals-enhancements}

There are no *`Workfront Goals`* updates at this point in the release. This area will be updated when updates are available.


## Announcements {#announcements}



### Required IP allowlist update for using the Workfront for Jira integration {#required-ip-allowlist-update-for-using-the-workfront-for-jira-integration}

We've made some back-end updates to the Workfront for Jira integration. Please ensure that the following IP addresses listed in the [Configure your firewall](configure-your-firewall.md) article have been added to your allowlist for inbound and outbound connections:



*  34.213.36.118
*  35.160.0.242
*  3.209.27.146
*  18.205.251.4


These addresses were previously listed as necessary for other areas of Workfront, but are now also necessary for the Jira integration.


To prevent interruption in your Workfront for Jira integration, your organization must allow these IP addresses by August 4, 2021.


For more information on configuring the Jira integration, see [Install Adobe Workfront for Jira](install-workfront-for-jira.md).


### API version 13 {#api-version}

For API version 13, we've modified various resources and endpoints. Some of the changes support new functionality, and others make it easier for you to use the information available through the API.


For information on what's new and updated, see [What's new in API version 13](new-api-version-13.md).


## 21.3 Release Webinar {#release-webinar}

The *`Workfront`* 21.3 Release Webinar was presented on June 16, 2021. You can view the recording [here](https://webinars.on24.com/workfront/213Release?partnerref=WFAC).


## Functionality no longer supported {#functionality-no-longer-supported}



### Internet Explorer 11 {#internet-explorer}

With the removal of support for Internet Explorer, Workfront now officially supports Microsoft Edge.


For more information about supported browsers, see [Adobe Workfront browser requirements](workfront-browser-requirements.md).
