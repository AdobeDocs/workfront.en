---
filename: approve-business-case
navigation-topic: business-case-and-scorecards
title: Approve a Business Case
description: After you complete and submit the Business Case for a project request, the Business Case must be approved. This depends on the workflow in your organization. A project can start without the Business Case having to be approved, but your Adobe Workfront administrator and project owners might not consider it ideal to do so.
---

# Approve a Business Case

After you complete and submit the Business Case for a project request, the Business Case must be approved. This depends on the workflow in your organization. A project can start without the Business Case having to be approved, but your *Adobe Workfront administrator* and project owners might not consider it ideal to do so.&nbsp;

For more information about completing and submitting a Business Case, see the article [Create a Business Case for a project in Adobe Workfront](../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p><em>Pro</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <draft-comment>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p>
    </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <draft-comment>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p>
    </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Overview of Business Case approval

Consider the following when approving a Business Case of a project:

* You must have Manage permissions to a project to approve the Business Case for it.&nbsp;
* You will not be able to see the projects which are waiting for the Business Case to be approved under your Approvals in Home.
* You must manually go to the individual projects that need Business Case approval to see that they are pending approval. There is no *Workfront* notification mechanism that alerts someone that they must approve the Business Case of a project. 
* You can find the projects waiting for the approval of the Business Case either by building a project report, or by accessing the portfolio they are associated with.&nbsp;

  For more information about Portfolios, see the article [Portfolio overview in Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

## Approve the Business Case by building a project report

You can build a report for projects to see what projects need their Business Case approved.&nbsp;

To build a report for projects which are pending approval of their Business Cases:

<ol> 
 <li value="1"> <p>Create a report for projects.</p> <p>For more information about creating reports, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li> 
 <li value="2">Select the <span class="bold">View</span> tab of the report, then click <span class="bold">Add Column</span>.</li> 
 <li value="3"> <p>Start typing "Status" in the <span class="bold">Show in this column</span> field, and select this field when it appears in the list.</p> <p>&nbsp;This column will display the status of the projects.</p> </li> 
 <li value="4">Select the <span class="bold">Filters</span> tab of the report, then click <span class="bold">Add a Filter Rule</span>.</li> 
 <li value="5">Start typing "Status" in the <span class="bold">Only show me Projects in which the ...</span> field, and select it when it appears in the list.</li> 
 <li value="6">Select <span class="bold">Equal</span> for the filter modifier.</li> 
 <li value="7"> <p>Start typing "Requested" in the available field.&nbsp;</p> <p>This ensures that the report includes only projects which are in the Requested status.</p> <p>&nbsp;<img src="assets/requested-projects-filter-350x14.png" alt="requested_projects_filter.png" style="width: 350;height: 14;"></p> </li> 
 <li value="8"> <p>(Optional) Click <span class="bold">Add another Filter Rule</span>.</p> <p>You can add additional filters, to show only projects where you are the Project Owner, or the Project Sponsor, or the Portfolio Owner.</p> <p>For example, you can use the following filter statements:&nbsp; </p> 
  <ul> 
   <li><code>Project Sponsor ID Equals $$USER.ID</code> to display projects where you are designated as the Project Sponsor</li> 
   <li><code>Project Owner ID Equals $$USER.ID</code> to display projects where you are designated as the Project owner</li> 
   <li><code>Project Portfolio Owner ID Equals $$USER. ID</code> to display where you are designated as the Portfolio Manager.&nbsp;</li> 
  </ul> </li> 
 <li value="9"> <p>Click <span class="bold">Save+Close</span>.</p> <p>Notice that all projects in the report are in the status of <span class="bold">Requested</span>.</p> </li> 
 <li value="10"> <p>Click the name of a project in the report to open it.</p> </li> 
 <li value="11"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click 
    <span class="bold">Business Case</span> in the left panel. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click 
   <span class="bold">Business Case</span> in the left panel. 
  </MadCap:conditionalText></li> 
 <li value="12"> <p>Click <span class="bold">Approve</span> or <span class="bold">Reject</span> in the Business Case Summary area to approve or reject the Business Case.&nbsp;</p> <p> <img src="assets/business-case-summary-with-rp-information--1-.png"> </p> <p>The project status is changed to <span class="bold">Approved</span> if the Business Case is approved. </p> <p>The project status is changed to <span class="bold">Rejected</span> if the Business case is rejected.</p> <note type="note">
   There are no notifications that alert the user who submitted the approval of the business case whether their project request was approved or rejected.
  </note> </li> 
</ol>

##

##  

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Approve the Business Case by accessing Requested projects in a portfolio
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Approve the Business Case by accessing Requested projects in a portfolio</MadCap:conditionalText>`

For more information about reviewing 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Requested
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Requested </MadCap:conditionalText>`projects, see the article [Review Requested Projects](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md).
