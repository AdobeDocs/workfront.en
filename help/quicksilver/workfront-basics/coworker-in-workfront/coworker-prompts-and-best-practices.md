---
title: CX Coworker prompts and best practices
content-type: reference
description: Learn about the best practices for using Coworker in Workfront and view a list of prompt examples.
author: Becky
feature: Get Started with Workfront
---
# CX Coworker prompts and best practices

With CX Coworker, you can use natural language to interact with Workfront Workflow and Workfront Planning. 

Coworker is part of the Adobe Experience Cloud Agent Orchestrator.

For more information on Agent Orchestrator, see [Adobe Experience Platform Agent Orchestrator](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/agents/agent-orchestrator).

## Access requirements

<!--Add info about how to qualify for agent orchestrator stuff-->

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Select, Prime, or Ultimate </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard or Light</p>
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td><p>For any functionality outside of the Foundational skills, your organization must have purchased Adobe Agent Orchestrator.</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td><p>You must have the appropriate permissions to interact with any object through Coworker.</p> <p>For example, to receive information about a project through Coworker, you must have at least View permission to that project.</p></td>
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

* Your Workfront administrator must have enabled AI Assistant for your organization.

    For more information, see [Prerequisites to AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant) in the article AI Assistant overview.
* Your Workfront administrator must have enabled AI Assistant for your access level.

   For more information, see [Enable or disable AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

## Considerations

Consider the following constraints when using CX Coworker:

### Reversibility

Some actions can be reversed. For example, if an object is created, that creation can be reversed. 

However, some actions, such as object deletion, can **not** be reversed. We recommend keeping this in mind when performing actions on your data through Coworker.

### Data / object coverage constraints

* Querying and reporting on custom fields is in early stages, and some skills (like API-based query helpers) do not yet handle arbitrary custom fields for aggregation and filtering.

### Interaction / UX limitations

* CX Coworker does not currently "learn" long-term from an individual user's style or preferences. Every chat uses only the current conversation and product knowledge.
* Conversation context is kept within a single chat session. Opening a new page or closing the assistant resets the conversation history.
* If approval procedures live in an outside application like Confluence or SharePoint, and are only linked via URL fields, Coworker does not currently fetch and reason over those pages.

### Data storage / Customer managed keys

* Because CX Coworker is part of the Adobe Experience Platform Agent Orchestrator, data from your interactions with Coworker are stored in Adobe Experience Platform, not in Workfront. Therefore, this data is not covered by Workfront Customer Managed Keys (BYOK) agreements.
                                             
## General-use foundational AI skills

>[!IMPORTANT]
>
>These general-use features are available to all users whose organization has a signed Adobe AI Agreement on file.

For best practices and prompts for these general-use skills, see [AI Assistant prompts and best practices](/help/quicksilver/workfront-basics/ai-assistant/ai-prompts-best-practices.md).

<!--Follow up with Oznur-->

### Product knowledge

CX Coworker can provide instructions or reference information pulled from the Workfront documentation. 

For more information about pulling information from Workfront documentation, see [Get help from AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

Example: How do I change task duration type?

### Project, task, and issue summarization

CX Coworker can summarize project, tasks, or issues<!--, or documents--> that have been uploaded to Workfront.

For more information about project, task, and issue summaries, see [Summarize using AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

Example: Summarize the project called Fall Campaign 2026.

<!--

### Locate work items

CX Coworker can find work items like projects, tasks, and issues

Example: Find all tasks assigned to me that are due this week.

For more information on using AI Assistant to locate project, tasks, and issues, see [se AI Assistant to work with projects, tasks, and issues](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

-->

<!--

Follow up on this to see if it's going away or what

### Catch Me Up 

Catch Me Up summarizes updates, uploaded documents, and other notable changes that have about your projects that have occurred in the last 24 hours, 3 days, or 7 days.  

For more information on Catch me up, see [Catch up on work in Priorities](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).

-->

<!--

### Smart filters

You can use natural language filters in Priorities to replace status, pre-built views to help you filter your work.

For more information on using Smart Filters, see [Filter your work with Smart filters](/help/quicksilver/workfront-basics/priorities/filter-group-work-priorities.md) in the article Filter and group your work with Priorities.

-->

## CX Coworker in Workfront

* [Project, task, and issue information](#project-task-and-issue-information)
* [Project and work management](#project-and-work-management)
* [Content and Approvals](#content-and-approvals)

### Project, task, and issue information

CX Coworker can give you information about project, tasks, and issues, including summaries and project health.

See example prompts for document and asset approvals in the following areas:

* [Find information about projects, tasks, or issues](#find-information-about-projects-tasks-or-issues)
* [Summarize projects, tasks, or issues](#summarize-projects-tasks-or-issues)
* [Show Project Health for projects, programs, or portfolios](#show-project-health-for-projects-programs-or-portfolios)

#### Find information about projects, tasks, or issues

* Projects
   * Show me all active projects for the Brand Marketing team
   * need a list of projects in the Q4 Campaigns portfolio under the "Digital" category.
   * Show me projects managed by users in the Creative Services company who are Project Managers.
* Tasks
   * Get me all tasks assigned to Joan Harris.
   * Show me tasks in the "Design" category assigned to the UX team.
   * I need tasks assigned to Copywriters in the Holiday Promotions program.
* Issues
   * Show me all issues in the "Website Redesign" project under the "Technical" category.
   * Get me all unresolved issues reported by the QA group.
   * I need issues assigned to Developers in the Global Tech company.

#### Summarize projects, tasks, or issues

* "Summarize this project"
* "Summarize the last week on this project"

#### Show Project Health for projects, programs, or portfolios

>[!NOTE]
>
>Your organization must be enrolled in the Project Health beta to use this feature.

* "Show me the health of my active projects"
* "Show me the health of this program"

### Project and work management

You can use CX Coworker to create and manage projects, including tasks and assignments. 

See example prompts for project and work management in the following areas:

* [Create, update, or delete projects](#create-update-or-delete-projects)
* [Identify the right project template based on user prompt](#identify-the-right-project-template-based-on-user-prompt)
* [Add, edit, or customize tasks in a project](#add-edit-or-customize-tasks-in-a-project)
<!--* [Create, update, or delete assignments](#create-update-or-delete-assignments)-->
<!--* [Recommend best matching user assignments for the task based on users' job role and availability](#recommend-best-matching-user-assignments-for-the-task-based-on-users-job-role-and-availability)-->

#### Create, update, or delete projects

You can create projects from scratch or from templates, update projects, and delete them.

* Create a blank project called Q2 Innovation Sandbox starting March 10 and ending April 30. Set me as the owner.
* Create a project called Lucent AI Launch – NA using the Integrated Marketing Campaign template. Start February 5 and set it to Current.
* Create a project called Website Redesign – EMEA starting March 1 and ending June 15. It's high priority, owned by EMEA Marketing, sponsored by the VP of Marketing, budgeted at $250K with about 1,200 planned hours, focused on Europe with the goal of improving conversions.
* For the Lucent AI Launch – NA project, move it to Q2, change the objective to driving free trials, push the finish to mid-April, increase the budget to $150K, and mark it as urgent.
* Show me all current marketing projects finishing in Q2 that are high or urgent priority, sorted by earliest end date.
* Delete the project called Q1 Test Campaign.

#### Add or edit tasks 

You can add or edit tasks in a project, and you can customize the task list of the template you use to create a project.

* Add a new task called Landing Page QA to the project and schedule it from April 22 to April 26.
* Update the Design Review task so it finishes on April 18 and assign it to the creative team.
* Remove the Print Asset Production task from the project.
* Show me all tasks in this project that are not completed and are scheduled to start between April 1 and April 30.
* Set Legal Approval as a predecessor of the Campaign Launch task.
* Add a new task called Final Copy Polish scheduled from April 15 to April 16, move the Copy Review task to April 10, remove the Extra Review Round task, and set Final Copy Polish as a predecessor of Email Build.
* During project creation flow try providing as much info as you can about deliverables that should ideally become tasks under the project.

#### Create, update, or delete assignments

You can create, update, and delete user or job role assignments.

* For the project 'Design Landing Page for Product Launch', identify the appropriate job roles and recommended planned hours for all currently unassigned tasks.
* I have several unassigned tasks, including 'Implement GA4 tracking for campaign site', 'Set up conversion events', and 'Validate analytics data'. Can you suggest the right job roles and estimated hours for each?
* For the creative tasks 'Create 3 banner variants for EMEA display ads', 'Apply revisions', and 'Export final assets', assign the best job roles and estimate the required effort for each task.
* Across the projects 'Q2 Product Launch', 'Website Redesign – EMEA', and 'Paid Media Campaign – NA', identify all unassigned tasks and assign the appropriate job roles with recommended planned hours for each.

<!--

#### Identify the right project template based on user prompt

* We're launching a new product feature with a landing page, emails, paid ads, and social posts. Which project template should we use?
* Create a project for a global marketing campaign with multiple channels and regional rollouts. (should suggest a template if provided more info)
* For Website Redesign – EMEA project, recommend and attach the correct project template.

-->

<!--

#### Recommend best matching user assignments for the task based on users' job role and availability

* Who is the best available user to assign to 'Design Landing Page Hero', considering who still has capacity today?
* Who should be assigned to 'Backend API integration for campaign reporting', considering engineering role alignment?
* For all unassigned tasks in this project, recommend the best users based on job role match and daily availability.
* Recommend users for the tasks 'QA testing for website launch' and 'Content review', prioritizing users whose job roles match and who are not over-allocated today.

-->

### Content and Approvals

CX Coworker can help manage document and asset approvals in Workfront. 

Consider the following when working with document and asset approvals:

* Content approvals must be enabled for your organization before you can use this functionality in Coworker.
* AI cannot approve or reject on behalf of humans. Decisions rely on users, with the exception of the Workfront AI Reviewer.

   For more information on the Workfront AI Reviewer, see [Get started with the Workfront AI Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).
* This functionality exists within Workfront, and cannot be used to interact with external tools or document providers.
* For the best experience, use this functionality with the Unified Approvals experience. 

   For more information on Unified Approvals, see [Unified Approvals overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

See example prompts for document and asset approvals in the following areas:

* [Add or remove approval participants](#add-or-remove-approval-participants)
* [Remind stakeholders of a single asset waiting for review](#remind-stakeholders-of-a-single-asset-waiting-for-review)
* [Add, update, or apply approval templates for a single asset](#add-update-or-apply-approval-templates-for-a-single-asset)

#### Add or remove approval participants

* Add Sarah Chen and Miguel Alvarez as approvers on the current document.
* Remove Jennifer Otto from this approval.
* Remove anyone who has not made an approval decision.
* Add a new stage to the spring-campaign.pdf called "Final review".
* Add Mark and Sarah as approvers and Phil as a reviewer on second stage of the winter-campaign.pdf
* For the winter-campaign.pdf, give the first stage a deadline for today at 5pm, and the final review a deadline for tomorrow at 5pm
* Add a Final check stage to the fall-campaign.png with a deadline for Thursday at 5pm and include Jim and Pam as approvers, also Oscar as a reviewer
* Add Mark Jones to the fall-campaign.png to the first and last stages as a reviewer.
* Let's get a multistage approval created for the fall-campaign.png with 3 stages, 1 Design 2 Copywriting and 3 Legal. I only need one decision required for each stage. Add Mike, Sally, Jane to design, Chris, Richard, Mark to copywriting and Phil, Tom, and Sarah to Legal. 

#### Remind stakeholders of a single asset waiting for review

* Send a reminder to approvers on the asset 'Spring Campaign Video' who haven't responded.
* Remind everyone who hasn't approved this asset 'Spring Campaign Video'.
* Who hasn't made a decision yet on the asset 'Brand Guidelines PDF'? Remind them.

#### Add, update, or apply approval templates for a single asset

* Apply the 'Marketing Launch' approval template to asset with the name 'Spring Campaign Video.
* Create a new approval template with 3 stages: Creative Review, Legal, and Final Approval. 
* Add Julia Santos and Shane Baker to stage 1.
* Edit the 'Product Launch' template to add Elizabeth Peterson to the final approval stage.
* Create a template called 'Urgent Review' with one stage and assign it to Olivia Kim.
* Update the 'Creative Review' template by removing Rick Kuvec and adding Karen Sterling to stage 2.


## CX Coworker in Workfront Planning

### Work with Planning records

* [Create, delete, duplicate, or restore records](#create-delete-duplicate-or-restore-records)
* [Link records to other records](#link-records-to-other-records)
* [Edit, update, or append a field to a record](#edit-update-or-append-a-field-to-a-record)
* [Access record change history](#access-record-change-history)

#### Create, delete, duplicate, or restore records

* Create a new campaign record called Summer Sale 2026
* Add a new product record with name Widget Pro and price $299
* Can you create a new lead record for John Smith?
* Delete the campaign record named Old Promo
* Remove the test record I just created
* Can you delete record ID Rc123abc456?
* Duplicate the Q1 Campaign record
* Can you copy this campaign to create a new one?
* Make a copy of the Holiday Promotion campaign
* Restore the campaign I accidentally deleted
* Can you recover the deleted project record?
* I accidentally deleted a record, can you restore it?

#### Link records to other records

* Link the Summer Campaign record to the Q2 Initiative
* Can you connect this product to the related marketing campaigns?
* I need to associate these three leads with the Enterprise Account record

#### Edit, update, or append a field to a record

* Update the budget field in the Summer Campaign to $75,000
* an you change the status of this project record to Completed?
* Add John Doe to the team members field for this initiative

#### Access record change history

* Show me the change history for the Summer Campaign record
* Can you display who modified this project and what they changed?
* I need to see all the updates made to this record in the last week

### Use System Designer in Workfront Planning

* [Create and configure workspaces](#create-and-configure-workspaces)
* [Define record types](#define-record-types)
* [Design fields and formula fields](#design-fields-and-formula-fields)
* [Build custom views](#build-custom-views)


#### Create and configure workspaces

* Create a new Planning workspace called Marketing Campaigns 2026
* Update my Product Planning workspace to change the color to blue and add a description
* Show me all the Planning workspaces I have access to

#### Define record types

* Create a new record type called Campaigns in my Planning workspace
* Update the Initiatives record type to change its icon and description
* Show me all the record types in my Marketing Planning workspace

#### Design fields and formula fields

* Add a Budget field to my Planning Campaigns record type with currency type
* Create a formula field in Planning that calculates days remaining until campaign end date
* Update the Priority field in my Planning workspace to add more dropdown options

#### Build custom views

* Create a timeline view in Planning to see my campaign schedule by start and end dates
* Add a new table view to my Planning Initiatives that filters only active status
* Duplicate my Planning Active Campaigns view and modify the sorting.
