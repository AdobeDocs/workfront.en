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
hidefromtoc: true
---

# GitLab modules

Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
In an Adobe Workfront Fusion scenario, you can automate workflows that use GitLab, as well as connect it to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Connect GitLab to Workfront Fusion {#connect-gitlab-to-workfront-fusion}

1. In any Workfront Fusion Gitlab module, click **Add** next to the connection field.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Connection name</td> 
      <td> <p>Enter a name for the connection.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">GitLab URL</td> 
      <td>Enter the URL of your GitLab instance.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Access Token</td> 
      <td>Enter your Private Token or Personal Access Token.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Continue**.
1. Click **Authorize** to create the connection and return to the module.

## GitLab modules and their fields

When you configure GitLab modules, Workfront Fusion displays the fields listed below. Along with these, additional GitLab fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

#### Watch build status {#watch-build-status}

This instant trigger module starts a scenario when the status of a build changes.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Webhook</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>Add</b> next to the webhook field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for build status changes</li></ul></li><li>Click <b>Save</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

#### Watch commit/MR/issue/snippet comments {#watch-commit-mr-issue-snippet-comments}

This instant trigger module starts a scenario when a comment is made on a commit, merge request, issue, or code snippet.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Webhook</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>Add</b> next to the webhook field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for comments</li></ul></li><li>Click <b>Save</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

#### Watch commits (pushes) {#watch-commits-pushes}

This instant trigger module starts a scenario when a commit is pushed to a repository. This module does not start a scenario when a tag is pushed.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Webhook</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>Add</b> next to the webhook field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for commits</li></ul></li><li>Click <b>Save</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

#### Watch issue comment {#watch-issue-comment}

This instant trigger module starts a scenario when a comment is made on an issue.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Webhook</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>Add</b> next to the webhook field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for issue comments</li></ul></li><li>Click <b>Save</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

#### Watch issues {#watch-issues}

This instant trigger module starts a scenario when an issue is created or when an existing issue is updated, closed, or reopened.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Webhook</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>Add</b> next to the webhook field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for issues</li></ul></li><li>Click <b>Save</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

#### Watch merge requests {#watch-merge-requests}

This instant trigger module starts a scenario when one of the following occurs:

* A new merge request is created
* An existing merge request is updated, merged, or closed
* A commit is added in the source branch


<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Webhook</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>Add</b> next to the webhook field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for merge requests</li></ul></li><li>Click <b>Save</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

#### Watch merge request comments {#watch-merge-request-comments}

This instant trigger module starts a scenario when a comment is made on a merge request.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Webhook</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>Add</b> next to the webhook field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for merge request comments</li></ul></li><li>Click <b>Save</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

#### Watch pipeline status {#watch-pipeline-status}

This instant trigger module starts a scenario when the status of a pipeline changes.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Webhook</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>Add</b> next to the webhook field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for pipeline status changes</li></ul></li><li>Click <b>Save</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

#### Watch projects {#watch-projects}

This scheduled trigger module starts a scenario when a new project is added, of which the authenticated user is a member.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Max Results</td> 
   <td> <p>Enter or map the maximum number of records you want the module to watch during each scenario execution cycle.</p> </td> 
   </tr> 
   </tbody> 
</table>

#### Watch repository branches {#watch-repository-branches}

This scheduled trigger module starts a scenario when a new branch is added to a repository.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Max Results</td> 
   <td> <p>Enter or map the maximum number of records you want the module to watch during each scenario execution cycle.</p> </td> 
   </tr> 
   </tbody> 
</table>

#### Watch repository tags {#watch-repository-tags}

This instant trigger module starts a scenario when a tag is created or deleted in a repository.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Webhook</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>Add</b> next to the webhook field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for tags</li></ul></li><li>Click <b>Save</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

#### Watch snippet comments {#watch-snippet-comments}

This instant trigger module starts a scenario when a new comment is made on a snippet.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Webhook</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>Add</b> next to the webhook field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for comments</li></ul></li><li>Click <b>Save</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

#### Watch todos {#watch-todos}

This scheduled trigger module starts a scenario when a new todo is added. When no filter is applied, the trigger is run when a new pending todo is added.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select the project that you want to watch for todos.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Author ID</td> 
   <td> Enter or map the ID of the author that you want to return todos for.  </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Action</td> 
   <td> <p>Select the type of action that created the todos you want to watch.</p>
   <ul><li>Assigned:</li>
   <li>Mentioned</li>
   <li>Build failed: The </li>
   <li>Marked</li>
   <li>Approval required</li></ul>
    </td> 
   </tr> 
   <tr> 
   <td role="rowheader">State</td> 
   <td> Select whether you want to watch Pending todos or Done todos. </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Max Results</td> 
   <td> <p>Enter or map the maximum number of records you want the module to watch during each scenario execution cycle.</p> </td> 
   </tr> 
   </tbody> 
</table>

#### Watch wiki page {#watch-wiki-page}

This instant trigger module starts a scenario when a wiki page is create or edited.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Webhook</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>Add</b> next to the webhook field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The project that you want the webhook to watch for wiki pages</li></ul></li><li>Click <b>Save</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

### Actions

#### Accept merge request

This action module merges submitted with the given merge request.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select the project that contains the merge request you want to accept.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Merge Request ID</td> 
   <td> <p>Enter or map the ID of the merge request that you want to accept.</p> <p>To search for a merge request, click <b>Search</b> and select the state of the merge requests you want to search. Select the merge request from the list.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Merge commit message</td> 
   <td> Enter or map a commit message for the merge.
    </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Should remove source branch</td> 
   <td>Select whether you want to remove the source branch when the merge is complete.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Merge when build succeeds</td> 
   <td>Select whether to merge the merge request as soon as the build is completed.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">SHA</td> 
   <td>If present, then this SHA must match the HEAD of the source branch. If it does not match, the merge fails.</td> 
   </tr> 
   </tbody> 
</table>

#### Cancel a build

This action module cancels a single build of a project.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select or map the project that contains the build you want to cancel.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Build ID</td> 
   <td>Select or map the build that you want to cancel.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Merge commit message</td> 
   <td> Enter or map a commit message for the merge.
    </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Should remove source branch</td> 
   <td>Select whether you want to remove the source branch when the merge is complete.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Merge when build succeeds</td> 
   <td>Select whether to merge the merge request as soon as the build is completed.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">SHA</td> 
   <td>If present, then this SHA must match the HEAD of the source branch. If it does not match, the merge fails.</td> 
   </tr> 
   </tbody> 
</table>

#### Cancel a pipeline's builds

This action module cancels the builds for a single pipeline.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select or map the project that contains the pipeline that you want to cancel builds for.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Pipeline ID</td> 
   <td>Select the pipeline that you want to cancel builds for.</td> 
   </tr> 
   </tbody> 
</table>

#### Cancel merge when pipeline succeeds

If a merge request is set to merge when a pipeline succeeds, this action module cancels that action.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select or map the project that contains the pipeline that you want to cancel the merge for.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Merge Request ID</td> 
   <td> <p>Enter or map the ID of the merge request that you want to cancel.</p> <p>To search for a merge request, click <b>Search</b> and select the state of the merge requests you want to search. Select the merge request from the list.</p></td> 
   </tr> 
   </tbody> 
</table>

#### Cherry pick a commit

This action module cherry picks a commit to a given branch.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select or map the project that contains the commit that you want to cherry-pick.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Commit SHA</td> 
   <td> Enter or map the commit hash for the commit you want to cherry pick</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Branch Name</td> 
   <td>Select the branch for which you want to cherry-pick the commit.</td> 
   </tr> 
   </tbody> 
</table>

#### Create a new label

This action module creates a new label for the given repository.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select or map the project that you are creating a label for.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Name</td> 
   <td> Enter or map a name for the new label</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Color</td> 
   <td>Enter the color in 6 digit hex notation with a leading # sign.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Description</td> 
   <td>Enter or map a description for the new label.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Priority</td> 
   <td>Enter or map the priority of the label. Must be greater than or equal to zero. To remove priority, or to not set priority, leave this field blank. </td> 
   </tr> 
   </tbody> 
</table>

#### Create a new pipeline

This action module creates a new pipeline for the given project.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select or map the project that you are creating a pipeline for.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Commit Ref</td> 
   <td>Select the branch or tag to run the pipeline on. To select a reference, click <b>Select</b> and fill in the type of reference, the reference's name, and the dates that you want to search for. </td> 
   </tr> 
   </tbody> 
</table>

#### Create a new release

This action module adds release notes to the existing git tag.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select or map the project that you are creating a release for.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Tag name</td> 
   <td>Enter or map the name of the tag that the release is created from. </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Description</td> 
   <td>Enter or map a description for the release. You can use Markdown in this description.</td> 
   </tr> 
   </tbody> 
</table>

#### Create a new tag

This action module creates a new tag in the repository that points to the supplied ref.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select or map the project that you are creating a tag for.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Tag name</td> 
   <td>Enter or map the name of the new tag. </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Ref Type</td> 
   <td><p>Select the ref that you are using to create the tag</p><ul><li><p>Branch</p><p>Select the branch that you want to use for this tag.</p></li><li><p>Commit</p><p>Enter or map the commit SHA that you want to use for this tag.</p></li><li><p>Tag</p><p>Enter or map the name of the tag that you want to create this new tag from.</p></li></td> 
   <tr> 
   <td role="rowheader">Message</td> 
   <td>To create an annotated tag, enter a message. An annotated tag is an unchangeable part of Git history.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Release description</td> 
   <td>To add release notes to the Git tag and store it in the GitLab database, add a release description. </td> 
   </tr> 
   </tr> 
   </tbody> 
</table>

#### Create a todo

This action module creates a todo for the current user on the selected issue. The current user is the user identified by the credentials on the connection used for this module.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select or map the project that you are creating a todo for.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Issue ID</td> 
   <td>Enter or map the ID of the issue that you want to create a todo for. </td> 
   </tr> 
      </tbody> 
</table>

#### Create a todo on a merge request

This action module creates a todo for the current user on the selected merge request. The current user is the user identified by the credentials on the connection used for this module.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select or map the project that you are creating a todo for.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Merge request ID</td> 
   <td><p>Enter or map the ID of the merge request that you want to create a todo for. </p><p>To locate a specific merge request, click <b>Search</b>, select the state of the merge request, and select the merge request from the list.</p> </td> 
   </tr> 
   </tbody> 
   </table>

#### Create merge request

This action module creates a new merge request on a project.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select or map the project where you want to create a merge request.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Source branch</td> 
   <td> <p>Enter or map the branch that you want to use as the source branch. </p><p>To select the branch from a list, click <b> Select</b> and select the branch.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Target branch</td> 
   <td> Enter or map a title for the new merge request.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Assignee ID</td> 
   <td> <p>Enter or map the ID of the user that you want to assign to this merge request. </p><p>To locate a user's ID, click <b> Select</b> and select the user. Workfront Fusion then inserts the selected user's ID into this field.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Description</td> 
   <td>Enter or map a description for the new merge request.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Target project ID</td> 
   <td><p>Enter or map the ID of the target project for this merge request. </p><p>To locate a project's ID, click <b> Select</b> and select the project. Workfront Fusion then inserts the selected project's ID into this field.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Labels</td> 
   <td>Enter or map a comma-separated list of labels to add to this new merge request.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Milestone ID</td> 
   <td><p>Enter or map the ID of the target project for this merge request. </p><p>To locate a milestone's ID, click <b> Select</b>, select whether to search active or closed milestones, and select the milestone. Workfront Fusion then inserts the selected milestone's ID into this field.</p></td> 
   </tr> 
   <tr> 
   <td role="rowheader">Remove source branch</td> 
   <td>Indicate whether you would like to remove the source branch after the merge request successfully merges.</td> 
   </tr> 
   </tbody> 
</table>

#### Create new file in repository

This action module creates a new file in the selected repository.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select or map the project where you want to create a file.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Full path</td> 
   <td> <p>Enter or map the full path to the file in the repository. Use URL encoding. Example: <code>lib%2Fclass%2Erb</code>. </p></td> 
   </tr> 
   <tr> 
   <td role="rowheader">Branch name</td> 
   <td> Enter or map a name for the new branch that the commit for the file will be added to.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Encoding</td> 
   <td> Enter the encoding for this file. Options are <code>base64</code> and <code>text</code>. Default value is <code>text</code>.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Author email</td> 
   <td>Enter or map the email address of the user that is the author of this commit.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Source file</td> 
   <td>Select a source file from a previous module, or map the source file's content.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Commit message</td> 
   <td>Enter or map the text of the commit message for the commit that adds the file.</td> 
   </tr> 
   </tbody> 
</table>

#### Create new issue note

This action module creates an issue note for a single project issue.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select or map the project that contains the issue where you want to create a note.</p> </td> 
   </tr> 
   <td role="rowheader">Issue ID</td> 
   <td> <p>Enter or map the ID of the issue where you want to create a note.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Body</td> 
   <td>Enter or map the body text for the note.</td> 
   </tr> 
   </tbody> 
   </table>

#### Create new merge request note

This action module creates note for a single merge request.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select or map the project that contains the merge request where you want to create a note.</p> </td> 
   </tr> 
   <td role="rowheader">Merge request ID</td> 
   <td><p>Enter or map the ID of the merge request where you want to create a note. </p><p>To locate a merge request's ID, click <b> Search</b>, select the status of merge requests to search, and select the merge request. Workfront Fusion then inserts the selected merge request's ID into this field.</p></td> 
   </tr> 
   <tr> 
   <td role="rowheader">Body</td> 
   <td>Enter or map the body text for the note.</td> 
   </tr> 
   </tbody> 
   </table>

#### Create a new milestone

This action module creates a new milestone for a project.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select or map the project where you want to create a milestone.</p> </td> 
   </tr> 
   <td role="rowheader">Title</td> 
   <td>Enter a title for new milestone.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Description</td> 
   <td>Enter or map a description for the new milestone.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Due date</td> 
   <td><p>Enter or map the due date for the new milestone.</p><p>For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion in Adobe Workfront Fusion</a>.</p></td> 
   </tr> 
   <tr> 
   <td role="rowheader">Start date</td> 
   <td><p>Enter or map the start date for the new milestone.</p><p>For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion in Adobe Workfront Fusion</a>.</p></td> 
   </tr> 
   </tbody> 
   </table>

#### Create new snippet note

This action module creates note for a single snippet.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select or map the project that contains the snippet where you want to create a note.</p> </td> 
   </tr> 
   <td role="rowheader">Snippet ID</td> 
   <td><p>Enter or map the ID of the snippet where you want to create a note. </p></td> 
   </tr> 
   <tr> 
   <td role="rowheader">Body</td> 
   <td>Enter or map the body text for the note.</td> 
   </tr> 
   </tbody> 
   </table>

#### Create repository branch

This action module creates a single repository branch.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select or map the project that you want to create a branch in.</p> </td> 
   </tr> 
   <td role="rowheader">Branch name</td> 
   <td><p>Enter or map a name for the new branch</p></td> 
   </tr> 
   <tr> 
   <td role="rowheader">Ref Type</td> 
   <td><p>Select whether you want to create the new branch from another branch or from a specific commit.</p><ul><li><p><b>Branch</b></p><p>Select the branch that you want to create the new branch from.</p></li><li><p><b>Commit</b></p><p>Select the commit SHA to build the new branch from</p><p>To locate an SHA, click <b>Select</b>, then select the whether you want to search branches or tags, the branch or tag name, and any limiting dates. Select the branch or tag from the list.  Workfront Fusion then inserts the SHA for the selected branch or tag into this field.</td> 
   </tr> 
   </tbody> 
   </table>

#### Create build variable

This action module creates a new build variable.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your GitLab account to Workfront Fusion, see <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Project ID</td> 
   <td> <p>Select or map the project that you want to create a variable in.</p> </td> 
   </tr> 
   <td role="rowheader">Key</td> 
   <td><p>Enter or map the key for the new variable. The key must have the following features.</p></td> 
   </tr> 
   <tr> 
   <td role="rowheader">Ref Type</td> 
   <td><p>Select whether you want to create the new branch from another branch or from a specific commit.</p><ul><li><p><b>Branch</b></p><p>Select the branch that you want to create the new branch from.</p></li><li><p><b>Commit</b></p><p>Select the commit SHA to build the new branch from</p><p>To locate an SHA, click <b>Select</b>, then select the whether you want to search branches or tags, the branch or tag name, and any limiting dates. Select the branch or tag from the list.  Workfront Fusion then inserts the SHA for the selected branch or tag into this field.</td> 
   </tr> 
   </tbody> 
   </table>



















<!--

Everything beyond this point is the draft as moved over from Flare. Included here as source material or in case we go back to what it was.

## Connect GitLab to Workfront Fusion {#connect-gitlab-to-workfront-fusion}

The procedure for connecting GitLab to Workfront Fusion is different based on whether you are connecting to a GitLab private server using a private token, or .connecting to GitLab.com using OAuth

>[!TIP]
>
>We recommend connecting Workfront Fusion to a GitLab private server.

* [Connect to a GitLab private server](#connect-to-a-gitlab-private-server) 
* [Connect to GitLab using gitlab.com](#connect-to-gitlab-using-gitlab-com)

### Connect to a GitLab private server {#connect-to-a-gitlab-private-server}

1. In any Workfront Fusion Gitlab module, click **Add** next to the connection field.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Connection type</td> 
      <td>Select <b>GitLab (private server)</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Connection name</td> 
      <td> <p>Enter a name for the connection.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Domain</td> 
      <td>Enter your GitLab server domain, such as <code>gitlab.com</code> (default) or <code>gitlab.&lt;your server&gt;.com</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Private token</td> 
      <td>Enter your private token. For information on creating a private token, see <a href="https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html#creating-a-personal-access-token">Creating a personal access token</a> in the GitLab documentation.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Continue** to save the connection and return to the module.

### Connect to GitLab using gitlab.com {#connect-to-gitlab-using-gitlab-com}

1. In any Workfront Fusion Gitlab module, click **Add** next to the connection field.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Connection type</td> 
      <td>Select <b>GitLab (gitlab.com)</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Connection name</td> 
      <td> <p>Enter a name for the connection.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Continue**.
1. Click **Authorize** to create the connection and return to the module.

## GitLab modules and their fields

When you configure GitLab modules, Workfront Fusion displays the fields listed below. Along with these, additional GitLab fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p><a href="#projects" class="MCXref xref">Projects</a> </p> </li> 
     <li> <p><a href="#issues" class="MCXref xref">Issues</a> </p> </li> 
     <li> <p><a href="#issue-notes" class="MCXref xref">Issue Notes</a> </p> </li> 
     <li> <p><a href="#pushes" class="MCXref xref">Pushes</a> </p> </li> 
     <li> <p><a href="#commits" class="MCXref xref">Commits</a> </p> </li> 
     <li> <p><a href="#merge-requests" class="MCXref xref">Merge Requests</a> </p> </li> 
     <li> <p><a href="#merge-request-notes" class="MCXref xref">Merge Request Notes</a> </p> </li> 
     <li> <p><a href="#repositories" class="MCXref xref">Repositories</a> </p> </li> 
     <li> <p><a href="#branches" class="MCXref xref">Branches</a> </p> </li> 
     <li> <p><a href="#pipeline" class="MCXref xref">Pipeline</a> </p> </li> 
     <li> <p><a href="#jobs" class="MCXref xref">Jobs</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#tags" class="MCXref xref">Tags</a> </p> </li> 
     <li> <p><a href="#to-do-items" class="MCXref xref">To-do Items</a> </p> </li> 
     <li> <p><a href="#labels" class="MCXref xref">Labels</a> </p> </li> 
     <li> <p><a href="#milestones" class="MCXref xref">Milestones</a> </p> </li> 
     <li> <p><a href="#variables" class="MCXref xref">Variables</a> </p> </li> 
     <li> <p><a href="#wiki-pages" class="MCXref xref">Wiki Pages</a> </p> </li> 
     <li> <p><a href="#snippets" class="MCXref xref">Snippets</a> </p> </li> 
     <li> <p><a href="#groups" class="MCXref xref">Groups</a> </p> </li> 
     <li> <p><a href="#deployments" class="MCXref xref">Deployments</a> </p> </li> 
     <li> <p><a href="#releases" class="MCXref xref">Releases</a> </p> </li> 
     <li> <p><a href="#other" class="MCXref xref">Other</a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Projects {#projects}

* [Watch projects](#watch-projects) 
* [Search Projects](#search-projects) 
* [List Owned Projects](#list-owned-projects) 
* [List a Project's Users](#list-a-project-s-users) 
* [Get a Project](#get-a-project)

#### Watch projects {#watch-projects}

This trigger module retrieves project details when a new project is created.

For information on fields, see [List all projects](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) in the GitLab documentation.

#### Search Projects {#search-projects}

This search module retrieves all projects in your account by the specified filter settings.

For information on fields, see [List all projects](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) in the GitLab documentation.

#### List Owned Projects {#list-owned-projects}

This search module retrieves projects where the authenticated user is set as owner.

For information on fields, see [List user projects](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) in the GitLab documentation.

#### List a Project's Users {#list-a-project-s-users}

This search module retrieves the users of the project.

For information on fields, see [Get project users](https://docs.gitlab.com/ee/api/projects.html#get-project-users) in the GitLab documentation.

#### Get a Project {#get-a-project}

This action module retrieves project details.

For information on fields, see [Get single project](https://docs.gitlab.com/ee/api/projects.html#get-single-project) in the GitLab documentation.

### Issues {#issues}

* [Watch Issues](#watch-issues) 
* [Get an Issue](#get-an-issue) 
* [Search Issues](#search-issues) 
* [List Project Issues](#list-project-issues) 
* [List Milestone Issues](#list-milestone-issues) 
* [List Issues That Close on Merge](#list-issues-that-close-on-merge) 
* [Create an Issue](#create-an-issue) 
* [Update an Issue](#update-an-issue) 
* [Delete an Issue](#delete-an-issue)

#### Watch Issues {#watch-issues}

This trigger module starts a scenario when a new issue is created, or an existing issue is updated, closed, or reopened.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook name</td> 
   <td> <p>Enter the name of the webhook.</p> <p>For more information on webhooks in Workfront Fusion, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref" data-mc-variable-override="">Instant triggers (webhooks) in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>To create a new connection, see <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect GitLab to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project</td> 
   <td> <p>Select the project where you want to watch issues.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get an Issue {#get-an-issue}

This action module retrieves issue details.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>To create a new connection, see <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project</td> 
   <td> <p>Select the project that contains the issue you want to retrieve details about.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Issue ID</td> 
   <td> <p>Enter or map the name of the issue you want to retrieve details about.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Search Issues {#search-issues}

This search module returns all issues by the specified filter settings.

For information on fields, see [List issues](https://docs.gitlab.com/ee/api/issues.html#list-issues) in the GitLab documentation.

#### List Project Issues {#list-project-issues}

This search module returns all issues in a specified project.

For information on fields, see [List project issues](https://docs.gitlab.com/ee/api/issues.html#list-project-issues) in the GitLab documentation.

#### List Milestone Issues {#list-milestone-issues}

This search module retrieves all issues assigned to a single project milestone.

For information on fields, see [Get all issues assigned to a single milestone](https://docs.gitlab.com/ee/api/milestones.html#get-all-issues-assigned-to-a-single-milestone) in the GitLab documentation.

#### List Issues That Close on Merge {#list-issues-that-close-on-merge}

This search module retrieves all the issues that would be closed by merging the provided merge request.

For information on fields, see [List issues that will close on merge](https://docs.gitlab.com/ee/api/merge_requests.html#list-issues-that-will-close-on-merge) in the GitLab documentation.

#### Create an Issue {#create-an-issue}

This action module creates a new project issue.

For information on fields, see [New issue](https://www.integromat.com/en/help/app/gitlab) in the GitLab documentation.

#### Update an Issue {#update-an-issue}

This action module updates an existing project issue. This call is also used to mark an issue as closed.

For information on fields, see [Edit issue](https://docs.gitlab.com/ee/api/issues.html#edit-issue) in the GitLab documentation.

#### Delete an Issue {#delete-an-issue}

This action module deletes an issue.

For information on fields, see [Delete an issue](https://docs.gitlab.com/ee/api/issues.html#delete-an-issue) in the GitLab documentation.

### Issue Notes {#issue-notes}

* [Watch Issue Notes](#watch-issue-notes) 
* [List Issue Notes](#list-issue-notes) 
* [Get an Issue Note](#get-an-issue-note) 
* [Create an Issue Note](#create-an-issue-note) 
* [Update an Issue Note](#update-an-issue-note)

#### Watch Issue Notes {#watch-issue-notes}

This trigger module starts a scenario when a new comment is made on commits, merge requests, issues, and code snippets.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook name</td> 
   <td> <p>Enter the name of the webhook.</p> <p>For more information on webhooks in Workfront Fusion, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref" data-mc-variable-override="">Instant triggers (webhooks) in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>To create a new connection, see <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect GitLab to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project</td> 
   <td> <p>Select the project where you want to watch issue notes.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Issue Notes {#list-issue-notes}

This search module retrieves a list of all notes for a single issue.

For information on fields, see [List project issue notes](https://docs.gitlab.com/ee/api/notes.html#list-project-issue-notes) in the GitLab documentation.

#### Get an Issue Note {#get-an-issue-note}

This action module retrieves a single note for a specific project issue.

For information on fields, see [Get single issue note](https://docs.gitlab.com/ee/api/notes.html#get-single-issue-note) in the GitLab documentation.

#### Create an Issue Note {#create-an-issue-note}

This action module creates a new note to a single project issue.

For information on fields, see [Create new issue note](https://docs.gitlab.com/ee/api/notes.html#create-new-issue-note) in the GitLab documentation.

#### Update an Issue Note {#update-an-issue-note}

Modifies an existing note of an issue.

For information on fields, see [Modify existing issue note](https://docs.gitlab.com/ee/api/notes.html#modify-existing-issue-note) in the GitLab documentation.

### Pushes {#pushes}

#### Watch Push Event

This trigger module starts a scenario when you push to the repository, except when pushing tags.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook name</td> 
   <td> <p>Enter the name of the webhook.</p> <p>For more information on webhooks in Workfront Fusion, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref" data-mc-variable-override="">Instant triggers (webhooks) in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>To create a new connection, see <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect GitLab to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project</td> 
   <td> <p>Select the project where you want to watch pushes.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Commits {#commits}

* [List Commit Comments](#list-commit-comments) 
* [Search Repository Commits](#search-repository-commits) 
* [Get a Commit](#get-a-commit) 
* [Get a Diff of a Commit](#get-a-diff-of-a-commit) 
* [Post a Comment to Commit](#post-a-comment-to-commit) 
* [Cherry Pick a Commit](#cherry-pick-a-commit)

#### List Commit Comments {#list-commit-comments}

This search module retrieves comments of a commit in a project.

For information on fields, see [Get the comments of a commit](https://docs.gitlab.com/ee/api/commits.html#get-the-comments-of-a-commit) in the GitLab documentation.

#### Search Repository Commits {#search-repository-commits}

This search module retrieves a list of repository commits in a project.

For information on fields, see [List repository commits](https://docs.gitlab.com/ee/api/commits.html#list-repository-commits) in the GitLab documentation.

#### Get a Commit {#get-a-commit}

This action module retrieves a specific commit identified by the commit hash or name of a branch or tag.

For information on fields, see [Get a single commit](https://docs.gitlab.com/ee/api/commits.html#get-a-single-commit) in the GitLab documentation.

#### Get a Diff of a Commit {#get-a-diff-of-a-commit}

This action module gets the diff of a commit in a project.

For information on fields, see [Get the diff of a commit](https://docs.gitlab.com/ee/api/commits.html#get-the-diff-of-a-commit) in the GitLab documentation.

#### Post a Comment to Commit {#post-a-comment-to-commit}

This action module adds a comment to a commit.

For information on fields, see [Post comment to commit](https://docs.gitlab.com/ee/api/commits.html#post-comment-to-commit) in the GitLab documentation.

#### Cherry Pick a Commit {#cherry-pick-a-commit}

This action module cherry picks a commit to a given branch.

For information on fields, see [Cherry pick a commit](https://docs.gitlab.com/ee/api/commits.html#cherry-pick-a-commit) in the GitLab documentation.

### Merge Requests {#merge-requests}

* [Watch Merge Requests](#watch-merge-requests) 
* [Search Merge Requests](#search-merge-requests) 
* [List Merge Request Changes](#list-merge-request-changes) 
* [List Merge Requests Closing an Issue](#list-merge-requests-closing-an-issue) 
* [Get a Merge Request](#get-a-merge-request) 
* [Get Merge Request Commits](#get-merge-request-commits) 
* [Create a Merge Request](#create-a-merge-request) 
* [Update a Merge Request](#update-a-merge-request) 
* [Create a To-do Item on a Merge Request](#create-a-to-do-item-on-a-merge-request) 
* [Accept a Merge Request](#accept-a-merge-request) 
* [Delete a Merge Request](#delete-a-merge-request) 
* [Cancel Merge When Pipeline Succeeds](#cancel-merge-when-pipeline-succeeds)

#### Watch Merge Requests {#watch-merge-requests}

This trigger module starts a scenario when a new merge request is created, an existing merge request was updated/merged/closed, or a commit is added in the source branch.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook name</td> 
   <td> <p>Enter the name of the webhook.</p> <p>For more information on webhooks in Workfront Fusion, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref" data-mc-variable-override="">Instant triggers (webhooks) in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>To create a new connection, see <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect GitLab to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project</td> 
   <td> <p>Select the project where you want to watch merge requests.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Search Merge Requests {#search-merge-requests}

This search module retrieves all merge requests by the filter settings.

For information on fields, see [List merge requests](https://docs.gitlab.com/ee/api/merge_requests.html#list-merge-requests) in the GitLab documentation.

#### List Merge Request Changes {#list-merge-request-changes}

This search module retrieves information about the merge request including its files and changes.

For information on fields, see [Get single merge request changes](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-changes) in the GitLab documentation.

#### List Merge Requests Closing an Issue {#list-merge-requests-closing-an-issue}

This search module retrieves all the issues that will be closed by merging the provided merge request.

For information on fields, see [List issues that will close on merge](https://docs.gitlab.com/ee/api/merge_requests.html#list-issues-that-will-close-on-merge) in the GitLab documentation.

#### Get a Merge Request {#get-a-merge-request}

This action module retrieves information about a single merge request.

For information on fields, see [Get single merge request](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr) in the GitLab documentation.

#### Get Merge Request Commits {#get-merge-request-commits}

This action module retrieves a list of merge request commits.

For information on fields, see [Get single merge request commits](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-commits) in the GitLab documentation.

#### Create a Merge Request {#create-a-merge-request}

This action module creates a new merge request.

For information on fields, see [Create merge request](https://docs.gitlab.com/ee/api/merge_requests.html#create-mr) in the GitLab documentation.

#### Update a Merge Request {#update-a-merge-request}

This action module updates an existing merge request. You can change the target branch, title, or even close the MR.

For information on fields, see [Update merge request](https://docs.gitlab.com/ee/api/merge_requests.html#update-mr) in the GitLab documentation.

#### Create a To-do Item on a Merge Request {#create-a-to-do-item-on-a-merge-request}

This action module manually creates a to-do item for the current user on a merge request.

For information on fields, see [Create a to-do](https://docs.gitlab.com/ee/api/merge_requests.html#create-a-todo) in the GitLab documentation.

#### Accept a Merge Request {#accept-a-merge-request}

This action module merges changes submitted with merge request.

For information on fields, see [Accept merge request](https://docs.gitlab.com/ee/api/merge_requests.html#accept-mr) in the GitLab documentation.

#### Delete a Merge Request {#delete-a-merge-request}

This action module is only for admins and project owners. It deletes the merge request in question

For information on fields, see Delete a merge request in the GitLab documentation.

#### Cancel Merge When Pipeline Succeeds {#cancel-merge-when-pipeline-succeeds}

This action module cancels a merge request when the pipeline succeeds.

For information on fields, see [Cancel merge when pipeline succeeds](https://docs.gitlab.com/ee/api/merge_requests.html) in the GitLab documentation.

### Merge Request Notes {#merge-request-notes}

* [List Merge Request Notes](#list-merge-request-notes) 
* [Get a Merge Request Note](#get-a-merge-request-note) 
* [Create a Merge Request Note](#create-a-merge-request-note) 
* [Update a Merge Request Note](#update-a-merge-request-note)

#### List Merge Request Notes {#list-merge-request-notes}

This search module retrieves a list of all notes for a single merge request.

For information on fields, see [List all merge request notes](https://docs.gitlab.com/ee/api/notes.html#list-all-merge-request-notes) in the GitLab documentation.

#### Get a Merge Request Note {#get-a-merge-request-note}

This action module returns a single note for a given merge request.

For information on fields, see [Get single merge request note](https://docs.gitlab.com/ee/api/notes.html#get-single-merge-request-note) in the GitLab documentation.

#### Create a Merge Request Note {#create-a-merge-request-note}

Creates a new note for a single merge request.

For information on fields, see [Create new merge request note](https://docs.gitlab.com/ee/api/notes.html#create-new-merge-request-note) in the GitLab documentation.

#### Update a Merge Request Note {#update-a-merge-request-note}

Modifies the existing note of a merge request.

For information on fields, see [Modify existing merge request note](https://docs.gitlab.com/ee/api/notes.html#modify-existing-merge-request-note) in the GitLab documentation.

### Repositories {#repositories}

* [List Repository Contributors](#list-repository-contributors) 
* [List Repository Tree](#list-repository-tree) 
* [Get a File From Repository](#get-a-file-from-repository) 
* [Get a Raw File From Repository](#get-a-raw-file-from-repository) 
* [Create a File in Repository](#create-a-file-in-repository) 
* [Delete a File in Repository](#delete-a-file-in-repository)

#### List Repository Contributors {#list-repository-contributors}

This search module retrieves a repository contributors list.

For information on fields, see [Contributors](https://docs.gitlab.com/ee/api/repositories.html#contributors) in the GitLab documentation.

#### List Repository Tree {#list-repository-tree}

This search module retrieves a list of repository files and directories in a project.

For information on fields, see [List repository tree](https://docs.gitlab.com/ee/api/repositories.html#list-repository-tree) in the GitLab documentation.

#### Get a File From Repository {#get-a-file-from-repository}

This action module retrieves information about a file in the repository like name, size, or content.

For information on fields, see [Get file from repository](https://docs.gitlab.com/ee/api/repository_files.html#get-file-from-repository) in the GitLab documentation.

#### Get a Raw File From Repository {#get-a-raw-file-from-repository}

This action module retrieves file content from a repository.

For information on fields, see [Get raw file from repository](https://docs.gitlab.com/ee/api/repository_files.html#get-raw-file-from-repository) in the GitLab documentation.

#### Create a File in Repository {#create-a-file-in-repository}

This action module adds a file to the repository.

For information on fields, see [Create new file in repository](https://docs.gitlab.com/ee/api/repository_files.html#create-new-file-in-repository) in the GitLab documentation.

#### Delete a File in Repository {#delete-a-file-in-repository}

This action module deletes an existing file from the repository.

For information on fields, see [Delete existing file in repository](https://docs.gitlab.com/ee/api/repository_files.html#delete-existing-file-in-repository) in the GitLab documentation.

### Branches {#branches}

* [Search Repository Branches](#search-repository-branches) 
* [Get a Repository Branch](#get-a-repository-branch) 
* [Create a Repository Branch](#create-a-repository-branch) 
* [Delete a Repository Branch](#delete-a-repository-branch)

#### Search Repository Branches {#search-repository-branches}

This module searches for repository branches by the search term.

For information on fields, see [List repository branches](https://docs.gitlab.com/ee/api/branches.html#list-repository-branches) in the GitLab documentation.

#### Get a Repository Branch {#get-a-repository-branch}

This action module retrieves repository branch details.

For information on fields, see [Get single repository branch](https://docs.gitlab.com/ee/api/branches.html#get-single-repository-branch) in the GitLab documentation.

#### Create a Repository Branch {#create-a-repository-branch}

This action module creates a new branch in the repository.

For information on fields, see [Create repository branch](https://docs.gitlab.com/ee/api/branches.html#create-repository-branch) in the GitLab documentation.

#### Delete a Repository Branch {#delete-a-repository-branch}

This action module deletes a branch from the repository.

For information on fields, see [Delete repository branch](https://docs.gitlab.com/ee/api/branches.html#delete-repository-branch) in the GitLab documentation.

### Pipeline {#pipeline}

* [Watch Pipelines](#watch-pipelines) 
* [Search Pipelines](#search-pipelines) 
* [Get a Pipeline](#get-a-pipeline) 
* [Retry Failed Jobs in a Pipeline](#retry-failed-jobs-in-a-pipeline) 
* [Create a Pipeline](#create-a-pipeline) 
* [Cancel a Pipeline's Jobs](#cancel-a-pipeline-s-jobs)

#### Watch Pipelines {#watch-pipelines}

This trigger module starts a scenario when the status changes on a Pipeline.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook name</td> 
   <td> <p>Enter the name of the webhook.</p> <p>For more information on webhooks in Workfront Fusion, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref" data-mc-variable-override="">Instant triggers (webhooks) in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>To create a new connection, see <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect GitLab to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project</td> 
   <td> <p>Select the project where you want to watch pipelines.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Search Pipelines {#search-pipelines}

This search module retrieves all pipelines for the project.

For information on fields, see [List project pipelines](https://docs.gitlab.com/ee/api/pipelines.html#list-project-pipelines) in the GitLab documentation.

#### Get a Pipeline {#get-a-pipeline}

This module retrieves pipeline details.

For information on fields, see [Get a single pipeline](https://docs.gitlab.com/ee/api/pipelines.html#get-a-single-pipeline) in the GitLab documentation.

#### Retry Failed Jobs in a Pipeline {#retry-failed-jobs-in-a-pipeline}

This action module retries failed builds in a pipeline.

For information on fields, see [Retry jobs in a pipeline](https://docs.gitlab.com/ee/api/pipelines.html#retry-jobs-in-a-pipeline) in the GitLab documentation.

#### Create a Pipeline {#create-a-pipeline}

This action module creates a new pipeline.

For information on fields, see [Create a new pipeline](https://docs.gitlab.com/ee/api/pipelines.html#create-a-new-pipeline) in the GitLab documentation.

#### Cancel a Pipeline's Jobs {#cancel-a-pipeline-s-jobs}

This action module cancels a pipeline's builds.

For information on fields, see [Cancel a pipeline's jobs](https://docs.gitlab.com/ee/api/pipelines.html#cancel-a-pipelines-jobs) in the GitLab documentation.

### Jobs {#jobs}

* [Watch Jobs](#watch-jobs) 
* [List Jobs](#list-jobs) 
* [Get a Job](#get-a-job) 
* [Cancel a Job](#cancel-a-job) 
* [Play a Job](#play-a-job) 
* [Erase a Job](#erase-a-job) 
* [Keep Artifacts](#keep-artifacts)

#### Watch Jobs {#watch-jobs}

This trigger module starts a scenario when the status of a job changes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook name</td> 
   <td> <p>Enter the name of the webhook.</p> <p>For more information on webhooks in Workfront Fusion, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref" data-mc-variable-override="">Instant triggers (webhooks) in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>To create a new connection, see <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect GitLab to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project</td> 
   <td> <p>Select the project where you want to watch jobs.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Jobs {#list-jobs}

This search module retrieves a list of jobs in a project.

For information on fields, see [List project jobs](https://docs.gitlab.com/ee/api/jobs.html#list-project-jobs) in the GitLab documentation.

#### Get a Job {#get-a-job}

This action module retrieves a single job of a project.

For information on fields, see [Get a single job](https://docs.gitlab.com/ee/api/jobs.html#get-a-single-job) in the GitLab documentation.

#### Cancel a Job {#cancel-a-job}

This action module cancels a single job of a project.

For information on fields, see [Cancel a job](https://docs.gitlab.com/ee/api/jobs.html#cancel-a-job) in the GitLab documentation.

#### Play a Job {#play-a-job}

This action module triggers a manual action to start a job.

For information on fields, see [Play a job](https://docs.gitlab.com/ee/api/jobs.html#play-a-job) in the GitLab documentation.

#### Erase a Job {#erase-a-job}

This action module erases a job of a project (removes job artifacts and job log).

For information on fields, see [Erase a job](https://docs.gitlab.com/ee/api/jobs.html#erase-a-job) in the GitLab documentation.

#### Keep Artifacts {#keep-artifacts}

Prevents artifacts from being deleted when expiration is set.

For information on fields, see [Keep artifacts](https://docs.gitlab.com/ee/api/job_artifacts.html#keep-artifacts) in the GitLab documentation.

### Tags {#tags}

* [Watch Tags](#watch-tags) 
* [List Repository Tags](#list-repository-tags) 
* [Get a Tag](#get-a-tag) 
* [Create a Tag](#create-a-tag) 
* [Delete a Tag](#delete-a-tag)

#### Watch Tags {#watch-tags}

This trigger module starts a scenario when you create (or delete) tags in the repository.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook name</td> 
   <td> <p>Enter the name of the webhook.</p> <p>For more information on webhooks in Workfront Fusion, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref" data-mc-variable-override="">Instant triggers (webhooks) in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>To create a new connection, see <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect GitLab to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project</td> 
   <td> <p>Select the project where you want to watch tags.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Repository Tags {#list-repository-tags}

This search module retrieves a list of repository tags from a project, sorted by name in reverse alphabetical order.

For information on fields, see [List project repository tags](https://docs.gitlab.com/ee/api/tags.html#list-project-repository-tags) in the GitLab documentation.

#### Get a Tag {#get-a-tag}

This action module retrieves a specific repository tag determined by its name.

For information on fields, see [Get a single repository tag](https://docs.gitlab.com/ee/api/tags.html#get-a-single-repository-tag) in the GitLab documentation.

#### Create a Tag {#create-a-tag}

This action module creates a new tag in the repository that points to the supplied ref.

For information on fields, see [Create a new tag](https://docs.gitlab.com/ee/api/tags.html#create-a-new-tag) in the GitLab documentation.

#### Delete a Tag {#delete-a-tag}

This action module deletes a tag.

For information on fields, see [Delete a tag](https://docs.gitlab.com/ee/api/tags.html#delete-a-tag) in the GitLab documentation.

### To-do Items {#to-do-items}

* [Watch To-do Items](#watch-to-do-items) 
* [List To-do Items](#list-to-do-items) 
* [Create a To-do Item](#create-a-to-do-item) 
* [Mark a To-do Item as Done](#mark-a-to-do-item-as-done)

#### Watch To-do Items {#watch-to-do-items}

This module retrieves to-do item details when a new item is added.

For information on fields, see [Get a list of to dos](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) in the GitLab documentation.

#### List To-do Items {#list-to-do-items}

This search module retrieves a list of to-do items.

For information on fields, see [Get a list of to dos](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) in the GitLab documentation.

#### Create a To-do Item {#create-a-to-do-item}

This action module creates a to-do item for the authenticated user on an issue.

For information on fields, see [Create a to do](https://docs.gitlab.com/ee/api/issues.html#create-a-todo) in the GitLab documentation.

#### Mark a To-do Item as Done {#mark-a-to-do-item-as-done}

This action module marks a single pending to-do item given by its ID for the current user as done.

For information on fields, see [Mark a to do item as done](https://docs.gitlab.com/ee/api/todos.html#mark-a-todo-as-done) in the GitLab documentation.

### Labels {#labels}

* [List Labels](#list-labels) 
* [Get a Label](#get-a-label) 
* [Create a Label](#create-a-label) 
* [Update a Label](#update-a-label) 
* [Delete a Label](#delete-a-label)

#### List Labels {#list-labels}

This search module retrieves all labels in the project.

For information on fields, see [List labels](https://docs.gitlab.com/ee/api/labels.html#list-labels) in the GitLab documentation.

#### Get a Label {#get-a-label}

This action module retrieves label details.

For information on fields, see [Get a single project label](https://docs.gitlab.com/ee/api/labels.html#get-a-single-project-label) in the GitLab documentation.

#### Create a Label {#create-a-label}

This action module creates a new label for the given repository with the given name and color.

For information on fields, see [Create a new label](https://docs.gitlab.com/ee/api/labels.html#create-a-new-label) in the GitLab documentation.

#### Update a Label {#update-a-label}

Updates an existing label with new name or new color.

For information on fields, see [Edit an existing label](https://docs.gitlab.com/ee/api/labels.html#edit-an-existing-label) in the GitLab documentation.

#### Delete a Label {#delete-a-label}

This action module deletes a project label.

For information on fields, see [Delete a label](https://docs.gitlab.com/ee/api/labels.html#delete-a-label) in the GitLab documentation.

### Milestones {#milestones}

* [List Milestones](#list-milestones) 
* [Get a Milestone](#get-a-milestone) 
* [Create a Milestone](#create-a-milestone) 
* [Update a Milestone](#update-a-milestone) 
* [Delete a Label](#delete-a-label)

#### List Milestones {#list-milestones}

This search module retrieves all milestones in the project.

For information on fields, see [List project milestones](https://docs.gitlab.com/ee/api/milestones.html#list-project-milestones) in the GitLab documentation.

#### Get a Milestone {#get-a-milestone}

This action module retrieves milestone details.

For information on fields, see [Get single milestone](https://docs.gitlab.com/ee/api/milestones.html#get-single-milestone) in the GitLab documentation.

#### Create a Milestone {#create-a-milestone}

This action module creates a new project milestone.

For information on fields, see [Create new milestone](https://docs.gitlab.com/ee/api/milestones.html#create-new-milestone) in the GitLab documentation.

#### Update a Milestone {#update-a-milestone}

This action module updates an existing project milestone.

For information on fields, see [Edit milestone](https://docs.gitlab.com/ee/api/milestones.html#edit-milestone) in the GitLab documentation.

#### Delete a Milestone

This action module deletes a milestone.

For information on fields, see [Delete project milestone](https://docs.gitlab.com/ee/api/milestones.html#delete-project-milestone) in the GitLab documentation.

### Variables {#variables}

* [List Variables](#list-variables) 
* [Get a Variable](#get-a-variable) 
* [Create a Variable](#create-a-variable) 
* [Update a Variable](#update-a-variable) 
* [Delete a Variable](#delete-a-variable)

#### List Variables {#list-variables}

This search module retrieves a list of a project's variables.

For information on fields, see [List project variables](https://docs.gitlab.com/ee/api/project_level_variables.html#list-project-variables) in the GitLab documentation.

#### Get a Variable {#get-a-variable}

This module retrieves details of a project's specific variable.

For information on fields, see [Show variable details](https://docs.gitlab.com/ee/api/project_level_variables.html#show-variable-details) in the GitLab documentation.

#### Create a Variable {#create-a-variable}

This action module creates a new variable.

For information on fields, see [Create variable](https://docs.gitlab.com/ee/api/project_level_variables.html#create-variable) in the GitLab documentation.

#### Update a Variable {#update-a-variable}

This action module updates a project's variable.

For information on fields, see [Update variable](https://docs.gitlab.com/ee/api/project_level_variables.html#update-variable) in the GitLab documentation.

#### Delete a Variable {#delete-a-variable}

This action module removes a project's variable.

For information on fields, see [Remove variable](https://docs.gitlab.com/ee/api/project_level_variables.html#remove-variable) in the GitLab documentation.

### Wiki Pages {#wiki-pages}

#### Watch Wiki Pages

This trigger module starts a scenario when a wiki page is created, updated, or deleted.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook name</td> 
   <td> <p>Enter the name of the webhook.</p> <p>For more information on webhooks in Workfront Fusion, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref" data-mc-variable-override="">Instant triggers (webhooks) in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>To create a new connection, see <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect GitLab to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project</td> 
   <td> <p>Select the project where you want to watch wiki pages.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Snippets {#snippets}

* [List Snippet Notes](#list-snippet-notes) 
* [Get a Snippet Note](#get-a-snippet-note) 
* [Create a Snippet Note](#create-a-snippet-note) 
* [Update a Snippet Note](#update-a-snippet-note)

#### List Snippet Notes {#list-snippet-notes}

This module gets a list of all notes for a single snippet. Snippet notes are comments users can post to a snippet.

For information on fields, see [List all snippet notes](https://docs.gitlab.com/ee/api/notes.html#list-all-snippet-notes) in the GitLab documentation.

#### Get a Snippet Note {#get-a-snippet-note}

This module retrieves a single note for a given snippet.

For information on fields, see [Get a single snippet note](https://docs.gitlab.com/ee/api/notes.html#get-single-snippet-note) in the GitLab documentation.

#### Create a Snippet Note {#create-a-snippet-note}

This action module creates a new note for a single snippet. Snippet notes are comments users can post to a snippet.

For information on fields, see [Create new snippet note](https://docs.gitlab.com/ee/api/notes.html#create-new-snippet-note) in the GitLab documentation.

#### Update a Snippet Note {#update-a-snippet-note}

This action module modifies an existing note of a snippet.

For information on fields, see [Modify existing snippet note](https://docs.gitlab.com/ee/api/notes.html#modify-existing-snippet-note) in the GitLab documentation.

### Groups {#groups}

* [Search Groups](#search-groups) 
* [Create a Group](#create-a-group)

#### Search Groups {#search-groups}

This search module retrieves a list of visible groups for the authenticated user based on specified filter settings.

For information on fields, see [List groups](https://docs.gitlab.com/ee/api/groups.html#list-groups) in the GitLab documentation.

#### Create a Group {#create-a-group}

This action module creates a new project group.

For information on fields, see [New groups](https://docs.gitlab.com/ee/api/groups.html#new-group) in the GitLab documentation.

### Deployments {#deployments}

#### List Deployments

This search module retrieves a list of deployments in a project.

For information on fields, see [List project deployments](https://docs.gitlab.com/ee/api/deployments.html#list-project-deployments) in the GitLab documentation.

### Releases {#releases}

* [Create a Release](#create-a-release) 
* [Update a Release](#update-a-release)

#### Create a Release {#create-a-release}

This action module creates a release.

For information on fields, see [Create a release](https://docs.gitlab.com/ee/api/releases/#create-a-release) in the GitLab documentation.

#### Update a Release {#update-a-release}

This action module updates a release.

For information on fields, see [Update a release](https://docs.gitlab.com/ee/api/releases/#update-a-release) in the GitLab documentation.

### Other {#other}

* [Get My Info](#get-my-info) 
* [Make an API Call](#make-an-api-call)

#### Get My Info {#get-my-info}

This module retrieves current authenticated user's details.

For information on fields, see [List current user](https://docs.gitlab.com/ee/api/users.html#list-current-user-for-normal-users) in the GitLab documentation.

#### Make an API Call {#make-an-api-call}

Allows you to perform a custom API call.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>To create a new connection, see <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Enter a path relative to <code>https://www.gitlab.com/api/</code></p> <p>Example: <code>/v4/projects</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP request methods in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p>Add the query for the API call in the form of a standard JSON object.</p> <p>For example: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>



-->