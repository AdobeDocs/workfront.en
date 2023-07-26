---
filename: gitlab-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: GitLab modules
description: Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
author: Becky
feature: Workfront Fusion
exl-id: bf6c1d82-7926-4bf9-8424-e658650ee6b1
---

# [!UICONTROL GitLab] modules

Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!UICONTROL GitLab], as well as connect it to multiple third-party applications and services.

>[!NOTE]
>
>This article expects some familiarity with API documentation, and of [!DNL GitLab] functionality in general.

If you need instructions on creating a scenario, see [Create a scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] or higher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
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

## Connect [!DNL GitLab] to [!DNL Workfront Fusion] {#connect-gitlab-to-workfront-fusion}

1. In any [!DNL Workfront Fusion] [!DNL Gitlab] module, click **[!UICONTROL Add]** next to the connection field.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name]</td> 
      <td> <p>Enter a name for the connection.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL GitLab] URL]</td> 
      <td>Enter the URL of your [!DNL GitLab] instance.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Access Token]</td> 
      <td><p>Enter your [!UICONTROL Private Token] or [!UICONTROL Personal Access Token].</p><p>For information on locating or creating a personal access token in [!DNL GitLab], see "Create a personal access token" in <a href="https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html">Personal access tokens</a> in the [!DNL GitLab] documentation.</p></td> 
     </tr> 
    </tbody> 
   </table>


1. Click **[!UICONTROL Continue]**.
1. Click **[!UICONTROL Authorize]** to create the connection and return to the module.

## [!DNL GitLab] modules and their fields

When you configure [!DNL GitLab] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL GitLab] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

+++**[!UICONTROL Watch build status]**

This instant trigger module starts a scenario when the status of a build changes.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>[!UICONTROL Add]</b> next to the [!UICONTROL webhook] field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for build status changes</li></ul></li><li>Click <b>[!UICONTROL Save]</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch commit/MR/issue/snippet comments]**

This instant trigger module starts a scenario when a comment is made on a commit, merge request, issue, or code snippet.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>[!UICONTROL Add]</b> next to the [!UICONTROL webhook] field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for comments</li></ul></li><li>Click <b>[!UICONTROL Save]</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch commits (pushes)]**

This instant trigger module starts a scenario when a commit is pushed to a repository. This module does not start a scenario when a tag is pushed.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>[!UICONTROL Add]</b> next to the [!UICONTROL webhook] field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for commits</li></ul></li><li>Click <b>[!UICONTROL Save]</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch issue comment]**

This instant trigger module starts a scenario when a comment is made on an issue.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>[!UICONTROL Add]</b> next to the [!UICONTROL webhook] field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for issue comments</li></ul></li><li>Click <b>[!UICONTROL Save]</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch issues]**

This [!UICONTROL instant trigger] module starts a scenario when an issue is created or when an existing issue is updated, closed, or reopened.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>[!UICONTROL Add]</b> next to the [!UICONTROL webhook] field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for issues</li></ul></li><li>Click <b>[!UICONTROL Save]</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch merge requests]**

This instant trigger module starts a scenario when one of the following occurs:

* A new merge request is created
* An existing merge request is updated, merged, or closed
* A commit is added in the source branch


<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>[!UICONTROL Add]</b> next to the [!UICONTROL webhook] field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for merge requests</li></ul></li><li>Click <b>[!UICONTROL Save]</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch merge request comments]**

This instant trigger module starts a scenario when a comment is made on a merge request.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>[!UICONTROL Add]</b> next to the [!UICONTROL webhook] field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for merge request comments</li></ul></li><li>Click <b>[!UICONTROL Save]</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch pipeline status]**

This instant trigger module starts a scenario when the status of a pipeline changes.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>[!UICONTROL Add]</b> next to the [!UICONTROL webhook] field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for pipeline status changes</li></ul></li><li>Click <b>[!UICONTROL Save]</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch projects]**

This scheduled trigger module starts a scenario when a new project is added, of which the authenticated user is a member.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions about connecting your [!DNL GitLab] account to [!DNL Workfront] Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect [!DNL GitLab] to [!DNL Workfront] Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Max Results</td> 
   <td> <p>Enter or map the maximum number of records you want the module to watch during each scenario execution cycle.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch repository branches]**

This scheduled trigger module starts a scenario when a new branch is added to a repository.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions about connecting your [!DNL GitLab] account to [!DNL Workfront] Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect [!DNL GitLab] to [!DNL Workfront] Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Max Results</td> 
   <td> <p>Enter or map the maximum number of records you want the module to watch during each scenario execution cycle.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch repository tags]**

This instant trigger module starts a scenario when a tag is created or deleted in a repository.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>[!UICONTROL Add]</b> next to the [!UICONTROL webhook] field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for tags</li></ul></li><li>Click <b>[!UICONTROL Save]</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch snippet comments]**

This instant trigger module starts a scenario when a new comment is made on a snippet.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>[!UICONTROL Add]</b> next to the [!UICONTROL webhook] field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for comments</li></ul></li><li>Click <b>[!UICONTROL Save]</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch todos]**

This scheduled trigger module starts a scenario when a new todo is added. When no filter is applied, the trigger is run when a new pending todo is added.

For information on fields, see [Get a list of to dos](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Watch wiki page]**

This instant trigger module starts a scenario when a wiki page is create or edited.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>[!UICONTROL Add]</b> next to the [!UICONTROL webhook] field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for wiki pages</li></ul></li><li>Click <b>[!UICONTROL Save]</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

+++

### Actions

+++**[!UICONTROL Accept merge request]**

This action module merges submitted changes with the given merge request.

For information on fields, see [Accept merge request](https://docs.gitlab.com/ee/api/merge_requests.html#accept-mr) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Cancel a build]**

This action module cancels a single build of a project.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions about connecting your [!DNL GitLab] account to [!DNL Workfront] Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect [!DNL GitLab] to [!DNL Workfront] Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p>Select or map the project that contains the build you want to cancel.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Build ID]</td> 
   <td>Select or map the build that you want to cancel.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Merge commit message]</td> 
   <td> Enter or map a commit message for the merge.
    </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Should remove source branch]</td> 
   <td>Select whether you want to remove the source branch when the merge is complete.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Merge when build succeeds]</td> 
   <td>Select whether to merge the merge request as soon as the build is completed.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL SHA]</td> 
   <td>If present, then this SHA must match the HEAD of the source branch. If it does not match, the merge fails.</td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Cancel a pipeline's builds]**

This action module cancels the builds for a single pipeline.

For information on fields, see [Cancel a pipeline's jobs](https://docs.gitlab.com/ee/api/pipelines.html#cancel-a-pipelines-jobs) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Cancel merge when pipeline succeeds]**

If a merge request is set to merge when a pipeline succeeds, this action module cancels that action.

For information on fields, see [Cancel merge when pipeline succeeds](https://docs.gitlab.com/ee/api/merge_requests.html) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Cherry pick a commit]**

This action module cherry picks a commit to a given branch.

For information on fields, see [Cherry pick a commit](https://docs.gitlab.com/ee/api/commits.html#cherry-pick-a-commit) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Create a new label]**

This action module creates a new label for the given repository.

For information on fields, see [Create a new label](https://docs.gitlab.com/ee/api/labels.html#create-a-new-label) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Create a new pipeline]**

This action module creates a new pipeline for the given project.

For information on fields, see [Create a new pipeline](https://docs.gitlab.com/ee/api/pipelines.html#create-a-new-pipeline) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Create a new release]**

This action module adds release notes to the existing git tag.

For information on fields, see [Create a release](https://docs.gitlab.com/ee/api/releases/#create-a-release) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Create a new tag]**

This action module creates a new tag in the repository that points to the supplied ref.

For information on fields, see [Create a new tag](https://docs.gitlab.com/ee/api/tags.html#create-a-new-tag) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Create a todo]**

This action module creates a todo for the current user on the selected issue. The current user is the user identified by the credentials on the connection used for this module.

For information on fields, see [Create a to do](https://docs.gitlab.com/ee/api/issues.html#create-a-todo) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Create a todo on a merge request]**

This action module creates a todo for the current user on the selected merge request. The current user is the user identified by the credentials on the connection used for this module.

For information on fields, see [Create a to-do](https://docs.gitlab.com/ee/api/merge_requests.html#create-a-todo) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Create merge request]**

This action module creates a new merge request on a project.

For information on fields, see [Create merge request](https://docs.gitlab.com/ee/api/merge_requests.html#create-mr) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Create new file in repository]**

This action module creates a new file in the selected repository.

For information on fields, see [Create new file in repository](https://docs.gitlab.com/ee/api/repository_files.html#create-new-file-in-repository) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Create new issue note]**

This action module creates an issue note for a single project issue.

For information on fields, see [Create new issue note](https://docs.gitlab.com/ee/api/notes.html#create-new-issue-note) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Create new merge request note]**

This action module creates note for a single merge request.

For information on fields, see [Create new merge request note](https://docs.gitlab.com/ee/api/notes.html#create-new-merge-request-note) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Create a new milestone]**

This action module creates a new milestone for a project.

For information on fields, see [Create new milestone](https://docs.gitlab.com/ee/api/milestones.html#create-new-milestone) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Create new snippet note]**

This action module creates a new note for a single snippet. Snippet notes are comments users can post to a snippet.

For information on fields, see [Create new snippet note](https://docs.gitlab.com/ee/api/notes.html#create-new-snippet-note) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Create repository branch]**

This action module creates a single repository branch.

For information on fields, see [Create repository branch](https://docs.gitlab.com/ee/api/branches.html#create-repository-branch) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Create build variable]**

This action module creates a new build variable.

For information on fields, see [Create variable](https://docs.gitlab.com/ee/api/project_level_variables.html#create-variable) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Delete a merge request]**

This action module is only for admins and project owners. It deletes the merge request in question

For information on fields, see [Delete a merge request](https://docs.gitlab.com/ee/api/merge_requests.html#delete-a-merge-request) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Delete existing file in repository]**

This action module deletes an existing file from the repository.

For information on fields, see [Delete existing file in repository](https://docs.gitlab.com/ee/api/repository_files.html#delete-existing-file-in-repository) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Delete repository branch]**

This action module deletes a branch from the repository.

For information on fields, see [Delete repository branch](https://docs.gitlab.com/ee/api/branches.html#delete-repository-branch) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Edit issue]**

This action module updates an existing project issue. This call is also used to mark an issue as closed.

For information on fields, see [Edit issue](https://docs.gitlab.com/ee/api/issues.html#edit-issue) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Edit Milestone]**
This action module updates an existing project milestone.

For information on fields, see [Edit milestone](https://docs.gitlab.com/ee/api/milestones.html#edit-milestone) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Erase a build]**

This action module erases a build of a project (removes job artifacts and job log).

For information on fields, see [Erase a job](https://docs.gitlab.com/ee/api/jobs.html#erase-a-job) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Get a list of todos]**

This search module retrieves a list of to-do items.

For information on fields, see [Get a list of to dos](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Get a single build]**

This action module retrieves a single job of a project.

For information on fields, see [Get a single job](https://docs.gitlab.com/ee/api/jobs.html#get-a-single-job) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Get a single repository tag]**

This action module retrieves a specific repository tag determined by its name.

For information on fields, see [Get a single repository tag](https://docs.gitlab.com/ee/api/tags.html#get-a-single-repository-tag) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Get a specific deployment]**

This action module retrieves a specific deployment.

For information on fields, see [Get a specific deployment](https://docs.gitlab.com/ee/api/deployments.html#get-a-specific-deployment) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Get all issues assigned to a single milestone]**

This search module retrieves all issues assigned to a single project milestone.

For information on fields, see [Get all issues assigned to a single milestone](https://docs.gitlab.com/ee/api/milestones.html#get-all-issues-assigned-to-a-single-milestone) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Get file from repository]**

This action module retrieves information about a file in the repository like name, size, or content.

For information on fields, see [Get file from repository](https://docs.gitlab.com/ee/api/repository_files.html#get-file-from-repository) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Get project users]**

This search module retrieves the users of the project.

For information on fields, see [Get project users](https://docs.gitlab.com/ee/api/projects.html#get-project-users) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Get a single issue]**

This action module retrieves issue details.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>To create a new connection, see <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] to Workfront Fusion]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td> <p>Select the project that contains the issue you want to retrieve details about.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Issue ID]</td> 
   <td> <p>Enter or map the name of the issue you want to retrieve details about.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Get single issue note]**

This action module retrieves a single note for a specific project issue.

For information on fields, see [Get single issue note](https://docs.gitlab.com/ee/api/notes.html#get-single-issue-note) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Get single merge request]**

This action module retrieves information about a single merge request.

For information on fields, see [Get single merge request](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Get single merge request changes]**

This search module retrieves information about the merge request including its files and changes.

For information on fields, see [Get single merge request changes](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-changes) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Get single merge request commits]**

This action module retrieves a list of merge request commits.

For information on fields, see [Get single merge request commits](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-commits) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Get single merge request note]**

This action module returns a single note for a given merge request.

For information on fields, see [Get single merge request note](https://docs.gitlab.com/ee/api/notes.html#get-single-merge-request-note) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Get a Milestone]**

This action module retrieves milestone details.

For information on fields, see [Get single milestone](https://docs.gitlab.com/ee/api/milestones.html#get-single-milestone) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Get single project]**

This action module retrieves project details.

For information on fields, see [Get single project](https://docs.gitlab.com/ee/api/projects.html#get-single-project) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Get single repository branch]**

This action module retrieves repository branch details.

For information on fields, see [Get single repository branch](https://docs.gitlab.com/ee/api/branches.html#get-single-repository-branch) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Get snippet note]**

This module retrieves a single note for a given snippet.

For information on fields, see [Get a single snippet note](https://docs.gitlab.com/ee/api/notes.html#get-single-snippet-note) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Get the comments of a commit]**

This search module retrieves comments of a commit in a project.

For information on fields, see [Get the comments of a commit](https://docs.gitlab.com/ee/api/commits.html#get-the-comments-of-a-commit) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Get the diff of a commit]**

This action module gets the diff of a commit in a project.

For information on fields, see [Get the diff of a commit](https://docs.gitlab.com/ee/api/commits.html#get-the-diff-of-a-commit) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Keep artifacts]**

Prevents artifacts from being deleted when expiration is set.

For information on fields, see [Keep artifacts](https://docs.gitlab.com/ee/api/job_artifacts.html#keep-artifacts) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List all merge request notes]**

This search module retrieves a list of all notes for a single merge request.

For information on fields, see [List all merge request notes](https://docs.gitlab.com/ee/api/notes.html#list-all-merge-request-notes) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List all snippet notes]**

This module gets a list of all notes for a single snippet. Snippet notes are comments users can post to a snippet.

For information on fields, see [&#128279;](https://docs.gitlab.com/ee/api/notes.html#list-all-snippet-notes) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List commit builds]**

This search module returns a list of builds for a specific commit in a project.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>To create a new connection, see <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] to Workfront Fusion]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p>Select the project that contains the commit that you want to list builds for.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scope]</td> 
   <td> To limit the search to build with a specific status, select the status. Leaving this field blank returns all builds of the commit.  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL List issues]**

This search module returns all issues by the specified filter settings.

For information on fields, see [List issues](https://docs.gitlab.com/ee/api/issues.html#list-issues) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List Issues That Close on Merge]**

This search module retrieves all the issues that would be closed by merging the provided merge request.

For information on fields, see [List issues that will close on merge](https://docs.gitlab.com/ee/api/merge_requests.html#list-issues-that-will-close-on-merge) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List Labels]**

This search module retrieves all labels in the project.

For information on fields, see [List labels](https://docs.gitlab.com/ee/api/labels.html#list-labels) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List merge requests]**

This search module retrieves all merge requests by the filter settings.

For information on fields, see [List merge requests](https://docs.gitlab.com/ee/api/merge_requests.html#list-merge-requests) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List Owned Projects]**

This search module retrieves projects where the authenticated user is set as owner.

For information on fields, see [List user projects](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List project builds]**

This search module retrieves a list of builds in a project.

For information on fields, see [List project jobs](https://docs.gitlab.com/ee/api/jobs.html#list-project-jobs) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List project deployments]**

This search module retrieves a list of deployments in a project.

For information on fields, see [List project deployments](https://docs.gitlab.com/ee/api/deployments.html#list-project-deployments) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List project issue notes]**

This search module retrieves a list of all notes for a single issue.

For information on fields, see [List project issue notes](https://docs.gitlab.com/ee/api/notes.html#list-project-issue-notes) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List project issues]**

This search module returns all issues in a specified project.

For information on fields, see [List project issues](https://docs.gitlab.com/ee/api/issues.html#list-project-issues) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List project milestones]**

This search module retrieves all milestones in the project.

For information on fields, see [List project milestones](https://docs.gitlab.com/ee/api/milestones.html#list-project-milestones) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List project pipelines]**

This search module retrieves all pipelines for the project.

For information on fields, see [List project pipelines](https://docs.gitlab.com/ee/api/pipelines.html#list-project-pipelines) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List project repository tags]**

This search module retrieves a list of repository tags from a project, sorted by name in reverse alphabetical order.

For information on fields, see [List project repository tags](https://docs.gitlab.com/ee/api/tags.html#list-project-repository-tags) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List project variables]**

This search module retrieves a list of a project's variables.

For information on fields, see [List project variables](https://docs.gitlab.com/ee/api/project_level_variables.html#list-project-variables) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List projects]**

This search module retrieves all projects of which the authenticated user is a member.

For information on fields, see [List all projects](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List repository branches]**

This module searches for repository branches by the search term.

For information on fields, see [List repository branches](https://docs.gitlab.com/ee/api/branches.html#list-repository-branches) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List repository commits]**

This search module retrieves a list of repository commits in a project.

For information on fields, see [List repository commits](https://docs.gitlab.com/ee/api/commits.html#list-repository-commits) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List repository contributors]**

This search module retrieves a repository contributors list.

For information on fields, see [Contributors](https://docs.gitlab.com/ee/api/repositories.html#contributors) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL List repository tree]**

This search module retrieves a list of repository files and directories in a project.

For information on fields, see [List repository tree](https://docs.gitlab.com/ee/api/repositories.html#list-repository-tree) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Mark a todo as done]**

This action module marks a single pending to-do item given by its ID for the current user as done.

For information on fields, see [Mark a to do item as done](https://docs.gitlab.com/ee/api/todos.html#mark-a-todo-as-done) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Modify existing issue note]**

Modifies an existing note of an issue.

For information on fields, see [Modify existing issue note](https://docs.gitlab.com/ee/api/notes.html#modify-existing-issue-note) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Modify existing merge request note]**

Modifies the existing note of a merge request.

For information on fields, see [Modify existing merge request note](https://docs.gitlab.com/ee/api/notes.html#modify-existing-merge-request-note) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Modify existing snippet note]**

This action module modifies an existing note of a snippet.

For information on fields, see [Modify existing snippet note](https://docs.gitlab.com/ee/api/notes.html#modify-existing-snippet-note) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL New issue]**

This action module creates a new project issue.

For information on fields, see [New issue](https://www.integromat.com/en/help/app/gitlab) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Play a build]**

This action module triggers a manual action to start a job.

For information on fields, see [Play a job](https://docs.gitlab.com/ee/api/jobs.html#play-a-job) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Post comment to commit]**

This action module adds a comment to a commit.

For information on fields, see [Post comment to commit](https://docs.gitlab.com/ee/api/commits.html#post-comment-to-commit) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Remove variable]**

This action module removes a project's variable.

For information on fields, see [Remove variable](https://docs.gitlab.com/ee/api/project_level_variables.html#remove-variable) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Retry a build]**

This action module retries a single build in a commit.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>To create a new connection, see <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] to Workfront Fusion]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p>Select the project that contains the build you want to retry.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Build ID]</td> 
   <td> Select the build that you want to retry. </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Retry Failed Jobs in a Pipeline]**

This action module retries failed builds in a pipeline.

For information on fields, see [Retry jobs in a pipeline](https://docs.gitlab.com/ee/api/pipelines.html#retry-jobs-in-a-pipeline) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Get a Variable]**

This module retrieves details of a project's specific variable.

For information on fields, see [Show variable details](https://docs.gitlab.com/ee/api/project_level_variables.html#show-variable-details) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Update a release]**

This action module updates a release.

For information on fields, see [Update a release](https://docs.gitlab.com/ee/api/releases/#update-a-release) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Update merge request]**

This action module updates an existing merge request. You can change the target branch, title, or even close the MR.

For information on fields, see [Update merge request](https://docs.gitlab.com/ee/api/merge_requests.html#update-mr) in the [!DNL GitLab] documentation.

+++

+++**[!UICONTROL Update a Variable]**

This action module updates a project's variable.

For information on fields, see [Update variable](https://docs.gitlab.com/ee/api/project_level_variables.html#update-variable) in the [!DNL GitLab] documentation.

+++
