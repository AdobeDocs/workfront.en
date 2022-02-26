---
filename: gitlab-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: GitLab modules
description: Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
---

# GitLab modules

*Adobe Workfront Fusion* requires an *Adobe Workfront Fusion* license in addition to an *Adobe Workfront* license.
In a *Adobe Workfront Fusion* scenario, you can connect your *GitLab* account to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Connect GitLab to *Workfront Fusion*

The procedure for connecting GitLab to *Workfront Fusion* is different based on whether you are connecting to a GitLab private server using a private token, or .connecting to GitLab.com using OAuth

>[!TIP]
>
>We recommend connecting *Workfront Fusion* to a GitLab private server.

* [Connect to a GitLab private server](#connect2) 
* [Connect to GitLab using gitlab.com](#connect3)

### Connect to a GitLab private server

<ol> 
 <li value="1"> <p>In any <em>Workfront Fusion</em> Gitlab module, click <b>Add</b> next to the connection field.</p> </li> 
 <li value="2"> <p>Configure the following fields:</p> 
  <table cellspacing="0"> 
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
     <td>Enter your GitLab server domain, such as <code>gitlab.com</code> (default) or <code>gitlab.<your server>.com</code>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Private token</td> 
     <td>Enter your private token. For information on creating a private token, see <a href="https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html#creating-a-personal-access-token">Creating a personal access token</a> in the GitLab documentation.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="3"> <p>Click <b>Continue</b> to save the connection and return to the module.</p> </li> 
</ol>

### Connect to GitLab using gitlab.com

<ol> 
 <li value="1"> <p>In any <em>Workfront Fusion</em> Gitlab module, click <b>Add</b> next to the connection field.</p> </li> 
 <li value="2"> <p>Configure the following fields:</p> 
  <table cellspacing="0"> 
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
  </table> </li> 
 <li value="3"> <p>Click <b>Continue</b>.</p> </li> 
 <li value="4"> <p>Click <b>Authorize</b> to create the connection and return to the module.</p> </li> 
</ol>

## GitLab modules and their fields

When you configure *GitLab* modules, *Workfront Fusion* displays the fields listed below. Along with these, additional *GitLab* fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p><a href="#projects" class="MCXref xref">Projects</a> </p> </li> 
     <li> <p><a href="#issues" class="MCXref xref">Issues</a> </p> </li> 
     <li> <p><a href="#issue" class="MCXref xref">Issue Notes</a> </p> </li> 
     <li> <p><a href="#pushes" class="MCXref xref">Pushes</a> </p> </li> 
     <li> <p><a href="#commits" class="MCXref xref">Commits</a> </p> </li> 
     <li> <p><a href="#merge" class="MCXref xref">Merge Requests</a> </p> </li> 
     <li> <p><a href="#merge2" class="MCXref xref">Merge Request Notes</a> </p> </li> 
     <li> <p><a href="#reposito" class="MCXref xref">Repositories</a> </p> </li> 
     <li> <p><a href="#branches" class="MCXref xref">Branches</a> </p> </li> 
     <li> <p><a href="#pipeline" class="MCXref xref">Pipeline</a> </p> </li> 
     <li> <p><a href="#jobs" class="MCXref xref">Jobs</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#tags" class="MCXref xref">Tags</a> </p> </li> 
     <li> <p><a href="#to-do" class="MCXref xref">To-do Items</a> </p> </li> 
     <li> <p><a href="#labels" class="MCXref xref">Labels</a> </p> </li> 
     <li> <p><a href="#mileston" class="MCXref xref">Milestones</a> </p> </li> 
     <li> <p><a href="#variable" class="MCXref xref">Variables</a> </p> </li> 
     <li> <p><a href="#wiki" class="MCXref xref">Wiki Pages</a> </p> </li> 
     <li> <p><a href="#snippets" class="MCXref xref">Snippets</a> </p> </li> 
     <li> <p><a href="#groups" class="MCXref xref">Groups</a> </p> </li> 
     <li> <p><a href="#deployme" class="MCXref xref">Deployments</a> </p> </li> 
     <li> <p><a href="#releases" class="MCXref xref">Releases</a> </p> </li> 
     <li> <p><a href="#other" class="MCXref xref">Other</a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Projects

* [Watch projects](#watch) 
* [Search Projects](#search) 
* [List Owned Projects](#list) 
* [List a Project's Users](#list2) 
* [Get a Project](#get)

#### Watch projects

This trigger module retrieves project details when a new project is created.

For information on fields, see [List all projects](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) in the GitLab documentation.

#### Search Projects

This search module retrieves all projects in your account by the specified filter settings.

For information on fields, see [List all projects](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) in the GitLab documentation.

#### List Owned Projects

This search module retrieves projects where the authenticated user is set as owner.

For information on fields, see [List user projects](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) in the GitLab documentation.

#### List a Project's Users

This search module retrieves the users of the project.

For information on fields, see [Get project users](https://docs.gitlab.com/ee/api/projects.html#get-project-users) in the GitLab documentation.

#### Get a Project

This action module retrieves project details.

For information on fields, see [Get single project](https://docs.gitlab.com/ee/api/projects.html#get-single-project) in the GitLab documentation.

### Issues

* [Watch Issues](#watch2) 
* [Get an Issue](#get2) 
* [Search Issues](#search2) 
* [List Project Issues](#list3) 
* [List Milestone Issues](#list4) 
* [List Issues That Close on Merge](#list5) 
* [Create an Issue](#create) 
* [Update an Issue](#update) 
* [Delete an Issue](#delete)

#### Watch Issues

This trigger module starts a scenario when a new issue is created, or an existing issue is updated, closed, or reopened.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook name</td> 
   <td> <p>Enter the name of the webhook.</p> <p>For more information on webhooks in <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref" data-mc-variable-override="">Instant triggers (webhooks)</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>To create a new connection, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect GitLab to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project</td> 
   <td> <p>Select the project where you want to watch <em>issue</em>s.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get an Issue

This action module retrieves issue details.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>To create a new connection, see <a href="#connect" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</td> 
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

#### Search Issues

This search module returns all issues by the specified filter settings.

For information on fields, see [List issues](https://docs.gitlab.com/ee/api/issues.html#list-issues) in the GitLab documentation.

#### List Project Issues

This search module returns all issues in a specified project.

For information on fields, see [List project issues](https://docs.gitlab.com/ee/api/issues.html#list-project-issues) in the GitLab documentation.

#### List Milestone Issues

This search module retrieves all issues assigned to a single project milestone.

For information on fields, see [Get all issues assigned to a single milestone](https://docs.gitlab.com/ee/api/milestones.html#get-all-issues-assigned-to-a-single-milestone) in the GitLab documentation.

#### List Issues That Close on Merge

This search module retrieves all the issues that would be closed by merging the provided merge request.

For information on fields, see [List issues that will close on merge](https://docs.gitlab.com/ee/api/merge_requests.html#list-issues-that-will-close-on-merge) in the GitLab documentation.

#### Create an Issue

This action module creates a new project issue.

For information on fields, see [New issue](https://www.integromat.com/en/help/app/gitlab) in the GitLab documentation.

#### Update an Issue

This action module updates an existing project issue. This call is also used to mark an issue as closed.

For information on fields, see [Edit issue](https://docs.gitlab.com/ee/api/issues.html#edit-issue) in the GitLab documentation.

#### Delete an Issue

This action module deletes an issue.

For information on fields, see [Delete an issue](https://docs.gitlab.com/ee/api/issues.html#delete-an-issue) in the GitLab documentation.

### Issue Notes

* [Watch Issue Notes](#watch3) 
* [List Issue Notes](#list6) 
* [Get an Issue Note](#get3) 
* [Create an Issue Note](#create2) 
* [Update an Issue Note](#update2)

#### Watch Issue Notes

This trigger module starts a scenario when a new comment is made on commits, merge requests, issues, and code snippets.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook name</td> 
   <td> <p>Enter the name of the webhook.</p> <p>For more information on webhooks in <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref" data-mc-variable-override="">Instant triggers (webhooks)</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>To create a new connection, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect GitLab to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project</td> 
   <td> <p>Select the project where you want to watch <em>issue note</em>s.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Issue Notes

This search module retrieves a list of all notes for a single issue.

For information on fields, see [List project issue notes](https://docs.gitlab.com/ee/api/notes.html#list-project-issue-notes) in the GitLab documentation.

#### Get an Issue Note

This action module retrieves a single note for a specific project issue.

For information on fields, see [Get single issue note](https://docs.gitlab.com/ee/api/notes.html#get-single-issue-note) in the GitLab documentation.

#### Create an Issue Note

This action module creates a new note to a single project issue.

For information on fields, see [Create new issue note](https://docs.gitlab.com/ee/api/notes.html#create-new-issue-note) in the GitLab documentation.

#### Update an Issue Note

Modifies an existing note of an issue.

For information on fields, see [Modify existing issue note](https://docs.gitlab.com/ee/api/notes.html#modify-existing-issue-note) in the GitLab documentation.

### Pushes

#### Watch Push Event

This trigger module starts a scenario when you push to the repository, except when pushing tags.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook name</td> 
   <td> <p>Enter the name of the webhook.</p> <p>For more information on webhooks in <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref" data-mc-variable-override="">Instant triggers (webhooks)</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>To create a new connection, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect GitLab to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project</td> 
   <td> <p>Select the project where you want to watch <em>pushe</em>s.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Commits

* [List Commit Comments](#list7) 
* [Search Repository Commits](#search3) 
* [Get a Commit](#get4) 
* [Get a Diff of a Commit](#get5) 
* [Post a Comment to Commit](#post) 
* [Cherry Pick a Commit](#cherry)

#### List Commit Comments

This search module retrieves comments of a commit in a project.

For information on fields, see [Get the comments of a commit](https://docs.gitlab.com/ee/api/commits.html#get-the-comments-of-a-commit) in the GitLab documentation.

#### Search Repository Commits

This search module retrieves a list of repository commits in a project.

For information on fields, see [List repository commits](https://docs.gitlab.com/ee/api/commits.html#list-repository-commits) in the GitLab documentation.

#### Get a Commit

This action module retrieves a specific commit identified by the commit hash or name of a branch or tag.

For information on fields, see [Get a single commit](https://docs.gitlab.com/ee/api/commits.html#get-a-single-commit) in the GitLab documentation.

#### Get a Diff of a Commit

This action module gets the diff of a commit in a project.

For information on fields, see [Get the diff of a commit](https://docs.gitlab.com/ee/api/commits.html#get-the-diff-of-a-commit) in the GitLab documentation.

#### Post a Comment to Commit

This action module adds a comment to a commit.

For information on fields, see [Post comment to commit](https://docs.gitlab.com/ee/api/commits.html#post-comment-to-commit) in the GitLab documentation.

#### Cherry Pick a Commit

This action module cherry picks a commit to a given branch.

For information on fields, see [Cherry pick a commit](https://docs.gitlab.com/ee/api/commits.html#cherry-pick-a-commit) in the GitLab documentation.

### Merge Requests

* [Watch Merge Requests](#watch4) 
* [Search Merge Requests](#search4) 
* [List Merge Request Changes](#list8) 
* [List Merge Requests Closing an Issue](#list9) 
* [Get a Merge Request](#get6) 
* [Get Merge Request Commits](#get7) 
* [Create a Merge Request](#create3) 
* [Update a Merge Request](#update3) 
* [Create a To-do Item on a Merge Request](#create4) 
* [Accept a Merge Request](#accept) 
* [Delete a Merge Request](#delete2) 
* [Cancel Merge When Pipeline Succeeds](#cancel)

#### Watch Merge Requests

This trigger module starts a scenario when a new merge request is created, an existing merge request was updated/merged/closed, or a commit is added in the source branch.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook name</td> 
   <td> <p>Enter the name of the webhook.</p> <p>For more information on webhooks in <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref" data-mc-variable-override="">Instant triggers (webhooks)</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>To create a new connection, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect GitLab to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project</td> 
   <td> <p>Select the project where you want to watch <em>merge request</em>s.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Search Merge Requests

This search module retrieves all merge requests by the filter settings.

For information on fields, see [List merge requests](https://docs.gitlab.com/ee/api/merge_requests.html#list-merge-requests) in the GitLab documentation.

#### List Merge Request Changes

This search module retrieves information about the merge request including its files and changes.

For information on fields, see [Get single merge request changes](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-changes) in the GitLab documentation.

#### List Merge Requests Closing an Issue

This search module retrieves all the issues that will be closed by merging the provided merge request.

For information on fields, see [List issues that will close on merge](https://docs.gitlab.com/ee/api/merge_requests.html#list-issues-that-will-close-on-merge) in the GitLab documentation.

#### Get a Merge Request

This action module retrieves information about a single merge request.

For information on fields, see [Get single merge request](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr) in the GitLab documentation.

#### Get Merge Request Commits

This action module retrieves a list of merge request commits.

For information on fields, see [Get single merge request commits](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-commits) in the GitLab documentation.

#### Create a Merge Request

This action module creates a new merge request.

For information on fields, see [Create merge request](https://docs.gitlab.com/ee/api/merge_requests.html#create-mr) in the GitLab documentation.

#### Update a Merge Request

This action module updates an existing merge request. You can change the target branch, title, or even close the MR.

For information on fields, see [Update merge request](https://docs.gitlab.com/ee/api/merge_requests.html#update-mr) in the GitLab documentation.

#### Create a To-do Item on a Merge Request

This action module manually creates a to-do item for the current user on a merge request.

For information on fields, see [Create a to-do](https://docs.gitlab.com/ee/api/merge_requests.html#create-a-todo) in the GitLab documentation.

#### Accept a Merge Request

This action module merges changes submitted with merge request.

For information on fields, see [Accept merge request](https://docs.gitlab.com/ee/api/merge_requests.html#accept-mr) in the GitLab documentation.

#### Delete a Merge Request

This action module is only for admins and project owners. It deletes the merge request in question

For information on fields, see [Delete a merge request](http://For information on fields, see Accept merge request in the GitLab documentation.) in the GitLab documentation.

#### Cancel Merge When Pipeline Succeeds

This action module cancels a merge request when the pipeline succeeds.

For information on fields, see [Cancel merge when pipeline succeeds](https://docs.gitlab.com/ee/api/merge_requests.html) in the GitLab documentation.

### Merge Request Notes

* [List Merge Request Notes](#list10) 
* [Get a Merge Request Note](#get8) 
* [Create a Merge Request Note](#create5) 
* [Update a Merge Request Note](#update4)

#### List Merge Request Notes

This search module retrieves a list of all notes for a single merge request.

For information on fields, see [List all merge request notes](https://docs.gitlab.com/ee/api/notes.html#list-all-merge-request-notes) in the GitLab documentation.

#### Get a Merge Request Note

This action module returns a single note for a given merge request.

For information on fields, see [Get single merge request note](https://docs.gitlab.com/ee/api/notes.html#get-single-merge-request-note) in the GitLab documentation.

#### Create a Merge Request Note

Creates a new note for a single merge request.

For information on fields, see [Create new merge request note](https://docs.gitlab.com/ee/api/notes.html#create-new-merge-request-note) in the GitLab documentation.

#### Update a Merge Request Note

Modifies the existing note of a merge request.

For information on fields, see [Modify existing merge request note](https://docs.gitlab.com/ee/api/notes.html#modify-existing-merge-request-note) in the GitLab documentation.

### Repositories

* [List Repository Contributors](#list11) 
* [List Repository Tree](#list12) 
* [Get a File From Repository](#get9) 
* [Get a Raw File From Repository](#get10) 
* [Create a File in Repository](#create6) 
* [Delete a File in Repository](#delete3)

#### List Repository Contributors

This search module retrieves a repository contributors list.

For information on fields, see [Contributors](https://docs.gitlab.com/ee/api/repositories.html#contributors) in the GitLab documentation.

#### List Repository Tree

This search module retrieves a list of repository files and directories in a project.

For information on fields, see [List repository tree](https://docs.gitlab.com/ee/api/repositories.html#list-repository-tree) in the GitLab documentation.

#### Get a File From Repository

This action module retrieves information about a file in the repository like name, size, or content.

For information on fields, see [Get file from repository](https://docs.gitlab.com/ee/api/repository_files.html#get-file-from-repository) in the GitLab documentation.

#### Get a Raw File From Repository

This action module retrieves file content from a repository.

For information on fields, see [Get raw file from repository](https://docs.gitlab.com/ee/api/repository_files.html#get-raw-file-from-repository) in the GitLab documentation.

#### Create a File in Repository

This action module adds a file to the repository.

For information on fields, see [Create new file in repository](https://docs.gitlab.com/ee/api/repository_files.html#create-new-file-in-repository) in the GitLab documentation.

#### Delete a File in Repository

This action module deletes an existing file from the repository.

For information on fields, see [Delete existing file in repository](https://docs.gitlab.com/ee/api/repository_files.html#delete-existing-file-in-repository) in the GitLab documentation.

### Branches

* [Search Repository Branches](#search5) 
* [Get a Repository Branch](#get11) 
* [Create a Repository Branch](#create7) 
* [Delete a Repository Branch](#delete4)

#### Search Repository Branches

This module searches for repository branches by the search term.

For information on fields, see [List repository branches](https://docs.gitlab.com/ee/api/branches.html#list-repository-branches) in the GitLab documentation.

#### Get a Repository Branch

This action module retrieves repository branch details.

For information on fields, see [Get single repository branch](https://docs.gitlab.com/ee/api/branches.html#get-single-repository-branch) in the GitLab documentation.

#### Create a Repository Branch

This action module creates a new branch in the repository.

For information on fields, see [Create repository branch](https://docs.gitlab.com/ee/api/branches.html#create-repository-branch) in the GitLab documentation.

#### Delete a Repository Branch

This action module deletes a branch from the repository.

For information on fields, see [Delete repository branch](https://docs.gitlab.com/ee/api/branches.html#delete-repository-branch) in the GitLab documentation.

### Pipeline

* [Watch Pipelines](#watch5) 
* [Search Pipelines](#search6) 
* [Get a Pipeline](#get12) 
* [Retry Failed Jobs in a Pipeline](#retry) 
* [Create a Pipeline](#create8) 
* [Cancel a Pipeline's Jobs](#cancel2)

#### Watch Pipelines

This trigger module starts a scenario when the status changes on a Pipeline.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook name</td> 
   <td> <p>Enter the name of the webhook.</p> <p>For more information on webhooks in <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref" data-mc-variable-override="">Instant triggers (webhooks)</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>To create a new connection, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect GitLab to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project</td> 
   <td> <p>Select the project where you want to watch <em>pipeline</em>s.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Search Pipelines

This search module retrieves all pipelines for the project.

For information on fields, see [List project pipelines](https://docs.gitlab.com/ee/api/pipelines.html#list-project-pipelines) in the GitLab documentation.

#### Get a Pipeline

This module retrieves pipeline details.

For information on fields, see [Get a single pipeline](https://docs.gitlab.com/ee/api/pipelines.html#get-a-single-pipeline) in the GitLab documentation.

#### Retry Failed Jobs in a Pipeline

This action module retries failed builds in a pipeline.

For information on fields, see [Retry jobs in a pipeline](https://docs.gitlab.com/ee/api/pipelines.html#retry-jobs-in-a-pipeline) in the GitLab documentation.

#### Create a Pipeline

This action module creates a new pipeline.

For information on fields, see [Create a new pipeline](https://docs.gitlab.com/ee/api/pipelines.html#create-a-new-pipeline) in the GitLab documentation.

#### Cancel a Pipeline's Jobs

This action module cancels a pipeline's builds.

For information on fields, see [Cancel a pipeline's jobs](https://docs.gitlab.com/ee/api/pipelines.html#cancel-a-pipelines-jobs) in the GitLab documentation.

### Jobs

* [Watch Jobs](#watch6) 
* [List Jobs](#list13) 
* [Get a Job](#get13) 
* [Cancel a Job](#cancel3) 
* [Play a Job](#play) 
* [Erase a Job](#erase) 
* [Keep Artifacts](#keep)

#### Watch Jobs

This trigger module starts a scenario when the status of a job changes.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook name</td> 
   <td> <p>Enter the name of the webhook.</p> <p>For more information on webhooks in <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref" data-mc-variable-override="">Instant triggers (webhooks)</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>To create a new connection, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect GitLab to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project</td> 
   <td> <p>Select the project where you want to watch <em>job</em>s.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Jobs

This search module retrieves a list of jobs in a project.

For information on fields, see [List project jobs](https://docs.gitlab.com/ee/api/jobs.html#list-project-jobs) in the GitLab documentation.

#### Get a Job

This action module retrieves a single job of a project.

For information on fields, see [Get a single job](https://docs.gitlab.com/ee/api/jobs.html#get-a-single-job) in the GitLab documentation.

#### Cancel a Job

This action module cancels a single job of a project.

For information on fields, see [Cancel a job](https://docs.gitlab.com/ee/api/jobs.html#cancel-a-job) in the GitLab documentation.

#### Play a Job

This action module triggers a manual action to start a job.

For information on fields, see [Play a job](https://docs.gitlab.com/ee/api/jobs.html#play-a-job) in the GitLab documentation.

#### Erase a Job

This action module erases a job of a project (removes job artifacts and job log).

For information on fields, see [Erase a job](https://docs.gitlab.com/ee/api/jobs.html#erase-a-job) in the GitLab documentation.

#### Keep Artifacts

Prevents artifacts from being deleted when expiration is set.

For information on fields, see [Keep artifacts](https://docs.gitlab.com/ee/api/job_artifacts.html#keep-artifacts) in the GitLab documentation.

### Tags

* [Watch Tags](#watch7) 
* [List Repository Tags](#list14) 
* [Get a Tag](#get14) 
* [Create a Tag](#create9) 
* [Delete a Tag](#delete5)

#### Watch Tags

This trigger module starts a scenario when you create (or delete) tags in the repository.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook name</td> 
   <td> <p>Enter the name of the webhook.</p> <p>For more information on webhooks in <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref" data-mc-variable-override="">Instant triggers (webhooks)</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>To create a new connection, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect GitLab to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project</td> 
   <td> <p>Select the project where you want to watch <em>tag</em>s.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Repository Tags

This search module retrieves a list of repository tags from a project, sorted by name in reverse alphabetical order.

For information on fields, see [List project repository tags](https://docs.gitlab.com/ee/api/tags.html#list-project-repository-tags) in the GitLab documentation.

#### Get a Tag

This action module retrieves a specific repository tag determined by its name.

For information on fields, see [Get a single repository tag](https://docs.gitlab.com/ee/api/tags.html#get-a-single-repository-tag) in the GitLab documentation.

#### Create a Tag

This action module creates a new tag in the repository that points to the supplied ref.

For information on fields, see [Create a new tag](https://docs.gitlab.com/ee/api/tags.html#create-a-new-tag) in the GitLab documentation.

#### Delete a Tag

This action module deletes a tag.

For information on fields, see [Delete a tag](https://docs.gitlab.com/ee/api/tags.html#delete-a-tag) in the GitLab documentation.

### To-do Items

* [Watch To-do Items](#watch8) 
* [List To-do Items](#list15) 
* [Create a To-do Item](#create10) 
* [Mark a To-do Item as Done](#mark)

#### Watch To-do Items

This module retrieves to-do item details when a new item is added.

For information on fields, see [Get a list of to dos](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) in the GitLab documentation.

#### List To-do Items

This search module retrieves a list of to-do items.

For information on fields, see [Get a list of to dos](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) in the GitLab documentation.

#### Create a To-do Item

This action module creates a to-do item for the authenticated user on an issue.

For information on fields, see [Create a to do](https://docs.gitlab.com/ee/api/issues.html#create-a-todo) in the GitLab documentation.

#### Mark a To-do Item as Done

This action module marks a single pending to-do item given by its ID for the current user as done.

For information on fields, see [Mark a to do item as done](https://docs.gitlab.com/ee/api/todos.html#mark-a-todo-as-done) in the GitLab documentation.

### Labels

* [List Labels](#list16) 
* [Get a Label](#get15) 
* [Create a Label](#create11) 
* [Update a Label](#update5) 
* [Delete a Label](#delete6)

#### List Labels

This search module retrieves all labels in the project.

For information on fields, see [List labels](https://docs.gitlab.com/ee/api/labels.html#list-labels) in the GitLab documentation.

#### Get a Label

This action module retrieves label details.

For information on fields, see [Get a single project label](https://docs.gitlab.com/ee/api/labels.html#get-a-single-project-label) in the GitLab documentation.

#### Create a Label

This action module creates a new label for the given repository with the given name and color.

For information on fields, see [Create a new label](https://docs.gitlab.com/ee/api/labels.html#create-a-new-label) in the GitLab documentation.

#### Update a Label

Updates an existing label with new name or new color.

For information on fields, see [Edit an existing label](https://docs.gitlab.com/ee/api/labels.html#edit-an-existing-label) in the GitLab documentation.

#### Delete a Label

This action module deletes a project label.

For information on fields, see [Delete a label](https://docs.gitlab.com/ee/api/labels.html#delete-a-label) in the GitLab documentation.

### Milestones

* [List Milestones](#list17) 
* [Get a Milestone](#get16) 
* [Create a Milestone](#create12) 
* [Update a Milestone](#update6) 
* [Delete a Label](#delete6)

#### List Milestones

This search module retrieves all milestones in the project.

For information on fields, see [List project milestones](https://docs.gitlab.com/ee/api/milestones.html#list-project-milestones) in the GitLab documentation.

#### Get a Milestone

This action module retrieves milestone details.

For information on fields, see [Get single milestone](https://docs.gitlab.com/ee/api/milestones.html#get-single-milestone) in the GitLab documentation.

#### Create a Milestone

This action module creates a new project milestone.

For information on fields, see [Create new milestone](https://docs.gitlab.com/ee/api/milestones.html#create-new-milestone) in the GitLab documentation.

#### Update a Milestone

This action module updates an existing project milestone.

For information on fields, see [Edit milestone](https://docs.gitlab.com/ee/api/milestones.html#edit-milestone) in the GitLab documentation.

#### Delete a Milestone

This action module deletes a milestone.

For information on fields, see [Delete project milestone](https://docs.gitlab.com/ee/api/milestones.html#delete-project-milestone) in the GitLab documentation.

### Variables

* [List Variables](#list18) 
* [Get a Variable](#get17) 
* [Create a Variable](#create13) 
* [Update a Variable](#update7) 
* [Delete a Variable](#delete7)

#### List Variables

This search module retrieves a list of a project’s variables.

For information on fields, see [List project variables](https://docs.gitlab.com/ee/api/project_level_variables.html#list-project-variables) in the GitLab documentation.

#### Get a Variable

This module retrieves details of a project’s specific variable.

For information on fields, see [Show variable details](https://docs.gitlab.com/ee/api/project_level_variables.html#show-variable-details) in the GitLab documentation.

#### Create a Variable

This action module creates a new variable.

For information on fields, see [Create variable](https://docs.gitlab.com/ee/api/project_level_variables.html#create-variable) in the GitLab documentation.

#### Update a Variable

This action module updates a project’s variable.

For information on fields, see [Update variable](https://docs.gitlab.com/ee/api/project_level_variables.html#update-variable) in the GitLab documentation.

#### Delete a Variable

This action module removes a project’s variable.

For information on fields, see [Remove variable](https://docs.gitlab.com/ee/api/project_level_variables.html#remove-variable) in the GitLab documentation.

### Wiki Pages

#### Watch Wiki Pages

This trigger module starts a scenario when a wiki page is created, updated, or deleted.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook name</td> 
   <td> <p>Enter the name of the webhook.</p> <p>For more information on webhooks in <em>Workfront Fusion</em>, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref" data-mc-variable-override="">Instant triggers (webhooks)</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>To create a new connection, see <a href="#connect" class="MCXref xref" data-mc-variable-override="">Connect GitLab to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project</td> 
   <td> <p>Select the project where you want to watch <em>wiki page</em>s.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Snippets

* [List Snippet Notes](#list19) 
* [Get a Snippet Note](#get18) 
* [Create a Snippet Note](#create14) 
* [Update a Snippet Note](#update8)

#### List Snippet Notes

This module gets a list of all notes for a single snippet. Snippet notes are comments users can post to a snippet.

For information on fields, see [List all snippet notes](https://docs.gitlab.com/ee/api/notes.html#list-all-snippet-notes) in the GitLab documentation.

#### Get a Snippet Note

This module retrieves a single note for a given snippet.

For information on fields, see [Get a single snippet note](https://docs.gitlab.com/ee/api/notes.html#get-single-snippet-note) in the GitLab documentation.

#### Create a Snippet Note

This action module creates a new note for a single snippet. Snippet notes are comments users can post to a snippet.

For information on fields, see [Create new snippet note](https://docs.gitlab.com/ee/api/notes.html#create-new-snippet-note) in the GitLab documentation.

#### Update a Snippet Note

This action module modifies an existing note of a snippet.

For information on fields, see [Modify existing snippet note](https://docs.gitlab.com/ee/api/notes.html#modify-existing-snippet-note) in the GitLab documentation.

### Groups

* [Search Groups](#search7) 
* [Create a Group](#create15)

#### Search Groups

This search module retrieves a list of visible groups for the authenticated user based on specified filter settings.

For information on fields, see [List groups](https://docs.gitlab.com/ee/api/groups.html#list-groups) in the GitLab documentation.

#### Create a Group

This action module creates a new project group.

For information on fields, see [New groups](https://docs.gitlab.com/ee/api/groups.html#new-group) in the GitLab documentation.

### Deployments

#### List Deployments

This search module retrieves a list of deployments in a project.

For information on fields, see [List project deployments](https://docs.gitlab.com/ee/api/deployments.html#list-project-deployments) in the GitLab documentation.

### Releases

* [Create a Release](#create16) 
* [Update a Release](#update9)

#### Create a Release

This action module creates a release.

For information on fields, see [Create a release](https://docs.gitlab.com/ee/api/releases/#create-a-release) in the GitLab documentation.

#### Update a Release

This action module updates a release.

For information on fields, see [Update a release](https://docs.gitlab.com/ee/api/releases/#update-a-release) in the GitLab documentation.

### Other

* [Get My Info](#get19) 
* [Make an API Call](#make)

#### Get My Info

This module retrieves current authenticated user's details.

For information on fields, see [List current user](https://docs.gitlab.com/ee/api/users.html#list-current-user-for-normal-users) in the GitLab documentation.

#### Make an API Call

Allows you to perform a custom API call.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>To create a new connection, see <a href="#connect" class="MCXref xref">Connect GitLab to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Enter a path relative to <code>https://www.gitlab.com/api/</code></p> <p>Example: <code>/v4/projects</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP request methods</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p><em>Workfront Fusion</em> adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p>Add the query for the API call in the form of a standard JSON object.</p> <p>For example: <code>{“name”:“something-urgent”}</code></p> </td> 
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

