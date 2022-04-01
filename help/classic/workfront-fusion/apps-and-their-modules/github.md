---
filename: github
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: GitHub modules
description: In a Adobe Workfront Fusion scenario, you can connect your GitHub account to multiple third-party applications and services.
---

# GitHub modules

In a Adobe Workfront Fusion scenario, you can connect your GitHub account to multiple third-party applications and services.

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use GitHub modules, you must hava a GitHub account.

## Connect GitHub to Workfront Fusion

For instructions about connecting your GitHub account to Workfront Fusion, see [Create a connection to Workfront Fusion - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md)

## GitHub modules and their fields.

When you configure GitHub modules, Workfront Fusion displays the fields listed below. Along with these, additional GitHub fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers) 
* [Actions](#actions)

### Triggers {#triggers}

* [Watch Issues](#watch-issues) 
* [Watch Repositories](#watch-repositories) 
* [Watch Forks](#watch-forks) 
* [Watch Comments](#watch-comments) 
* [Watch Pull Requests](#watch-pull-requests)

#### Watch Issues {#watch-issues}

This module triggers when a new issue is added or an existing issue is modified.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your GitHub account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">I want to watch</td> 
   <td>Select whether you want to watch all repositories, or only one repository.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Repository</td> 
   <td>If you have chosen to watch issues in only one repository, select the repository that you want to watch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned issues</td> 
   <td>Set the maximum number of results that Workfront Fusion will work with during one cycle. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Watch</td> 
   <td>Select whether you want to watch for only new issues, or new issues and all changes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filter</td> 
   <td> <p>You can filter the issues you want to watch for by how you are associated with them.</p> 
    <ul> 
     <li>All issues</li> 
     <li>Only issues assigned to me</li> 
     <li>Only issues created by me</li> 
     <li>Only issues mentioning me</li> 
     <li>Only issues I'm subscribed to updates for</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">State</td> 
   <td>Select whether you want to watch only open issues, or only closed issues. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Labels</td> 
   <td>Add a tag. The module watches for issues with this tag.</td> 
  </tr> 
 </tbody> 
</table>

#### Watch Repositories {#watch-repositories}

This module triggers when a repository is created or modified.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your GitHub account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned repositories</td> 
   <td>Set the maximum number of results that Workfront Fusion will work with during one cycle. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Watch</td> 
   <td>Select whether you want to watch for new repositories and all changes, or only new repositories.</td> 
  </tr> 
 </tbody> 
</table>

#### Watch Forks {#watch-forks}

This module triggers when a new fork is created.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your GitHub account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Repository</td> 
   <td>Select the repository that you want to watch for forks.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned forks</td> 
   <td>Set the maximum number of results that Workfront Fusion will work with during one cycle. </td> 
  </tr> 
 </tbody> 
</table>

#### Watch Comments {#watch-comments}

This module triggers when a new comment is added or an existing comment is modified.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your GitHub account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Repository</td> 
   <td>Select the repository that you want to watch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Issue number</td> 
   <td>If you want to restrict the search by only searching for new comments made on a specific issue, enter the issue number.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned issues</td> 
   <td>Set the maximum number of results that Workfront Fusion will work with during one cycle. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Watch</td> 
   <td>Select whether you want to watch for only new comments, or comments and all changes.</td> 
  </tr> 
 </tbody> 
</table>

#### Watch Pull Requests {#watch-pull-requests}

This module triggers when a new pull request is added or an existing pull request is modified.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your GitHub account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Repository</td> 
   <td>Select the repository that you want to watch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned pull requests</td> 
   <td>Set the maximum number of results that Workfront Fusion will work with during one cycle. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">State</td> 
   <td>Select whether you want to watch only open pull requests, only closed ones, or all pull requests. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Watch</td> 
   <td>Select whether you want to watch for only new pull requests, or new pull requests and all changes.</td> 
  </tr> 
 </tbody> 
</table>

### Actions {#actions}

* [Search for an issue](#search-for-an-issue) 
* [Create an issue](#create-an-issue) 
* [Update an issue](#update-an-issue) 
* [Get an issue](#get-an-issue) 
* [Add assignees](#add-assignees) 
* [Remove assignees](#remove-assignees) 
* [Add labels to an issue](#add-labels-to-an-issue) 
* [Remove a label from an issue](#remove-a-label-from-an-issue) 
* [Create a comment](#create-a-comment) 
* [List comments](#list-comments)

#### Search for an issue {#search-for-an-issue}

This module searches for issues that match your search criteria.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your GitHub account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned issues</td> 
   <td>Set the maximum number of results that Workfront Fusion will work with during one cycle (the number of repetitions per scenario run). </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sort by</td> 
   <td> <p>Select how you want to sort the results of the search.</p> 
    <ul> 
     <li> <p>Best match </p> </li> 
     <li>Date created</li> 
     <li>Date updated</li> 
     <li>Number of comments</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sort direction</td> 
   <td> <p>Select ascending or descending. </p> <p>For dates, selecting <strong>descending</strong>will return the most recent date first. </p> <p>For number of comments, selecting <strong>descending</strong>will return the issue with the highest number of comments first.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query</td> 
   <td>Enter or map your search query. For a detailed description of search options, see <a href="https://docs.github.com/en/github/searching-for-information-on-github/searching-issues-and-pull-requests">Searching issues and pull requests</a> on the GitHub help site.</td> 
  </tr> 
 </tbody> 
</table>

#### Create an issue {#create-an-issue}

This module creates a new issue in the selected repository.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your GitHub account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Repository</td> 
   <td>Select the repository that you want to create an issue in.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Assignee</td> 
   <td>Select the people that you want to assign to the issue. Available assignees include anyone with write permissions to the repository, and organization members with read permissions to the repository. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Milestone</td> 
   <td>Select the milestone that you want to associate with the new issue. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Labels</td> 
   <td>Select any labels that you want to apply to the new issue. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Title</td> 
   <td>Enter or map a title for the new issue.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body</td> 
   <td>Enter or map the body of the issue, such as a description or additional information</td> 
  </tr> 
 </tbody> 
</table>

#### Update an issue {#update-an-issue}

This module updates an existing GitHub issue.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your GitHub account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Repository</td> 
   <td>Select the repository that you want to update an issue in.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Assignee</td> 
   <td>Select the people that you want to assign to the issue. Available assignees include anyone with write permissions to the repository and organization members with read permissions to the repository. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Milestone</td> 
   <td>Select the milestone that you want to associate with the issue. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Labels</td> 
   <td>Select any labels that you want to apply to the issue. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Number</td> 
   <td>Enter or map the issue number of the issue you want to update. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">State</td> 
   <td>Select the state that you want to update the issue to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Title</td> 
   <td>Enter or map a title for the issue.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body</td> 
   <td>Enter or map the body of the issue, such as a description or additional information</td> 
  </tr> 
 </tbody> 
</table>

#### Get an issue {#get-an-issue}

This module retrieves details about the specified issue

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your GitHub account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Repository</td> 
   <td>Select the repository that contains the issue that you want to retrieve details about.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Number</td> 
   <td>Enter or map the issue number of the issue that you want to retrieve details about. </td> 
  </tr> 
 </tbody> 
</table>

#### Add assignees {#add-assignees}

This module adds assignees to the specified issue

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your GitHub account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Repository</td> 
   <td>Select the repository that contains the issue to which you want to add assignees.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Assignee</td> 
   <td>Select the people that you want to assign to the issue. Available assignees include anyone with write permissions to the repository and organization members with read permissions to the repository. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Number</td> 
   <td>Enter or map the issue number of the issue to which you want to add assignees. </td> 
  </tr> 
 </tbody> 
</table>

#### Remove assignees {#remove-assignees}

This module removes assignees from the specified issue.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your GitHub account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Repository</td> 
   <td>Select the repository that contains the issue from which you want to remove assignees.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Assignee</td> 
   <td>Select the people that you want to remove from the issue. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Number</td> 
   <td>Enter or map the issue number of the issue from which you want to remove assignees. </td> 
  </tr> 
 </tbody> 
</table>

#### Add labels to an issue {#add-labels-to-an-issue}

This module adds labels to an issue. Labels are defined on the repository level, and can only be created by someone with write access to the repository.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your GitHub account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Repository</td> 
   <td>Select the repository that contains the issue to which you want to add labels.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Labels</td> 
   <td>Select the labels that you want to add to the issue.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Number</td> 
   <td>Enter or map the issue number of the issue to which you want to add labels.</td> 
  </tr> 
 </tbody> 
</table>

#### Remove a label from an issue {#remove-a-label-from-an-issue}

This module removes a single label from an issue.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your GitHub account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Repository</td> 
   <td>Select the repository that contains the issue from which you want to remove a label.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Labels</td> 
   <td>Select the label that you want to remove from the issue.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Number</td> 
   <td>Enter or map the issue number of the issue from which you want to remove a label.</td> 
  </tr> 
 </tbody> 
</table>

#### Create a comment {#create-a-comment}

This module creates a comment on the specified issue.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your GitHub account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Repository</td> 
   <td>Select the repository that contains the issue on which you want to create a comment.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Number</td> 
   <td>Enter or map the issue number of the issue on which you want to create a comment.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body</td> 
   <td>Enter or map the content of the comment.</td> 
  </tr> 
 </tbody> 
</table>

#### List comments {#list-comments}

This module lists all comments on the specified issue.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your GitHub account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Repository</td> 
   <td>Select the repository that contains the issue from which you want to list comments.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Number</td> 
   <td>Enter or map the issue number of the issue from which you want to list comments.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Since</td> 
   <td>The module will return comments created after this date. For a list of supported date formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned comments</td> 
   <td>Set the maximum number of results that Workfront Fusion will work with during one cycle. </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"><a name="Troubles"></a>Troubleshooting</h2>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Module does not receive any events</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a module does not receive any events, check the webhook settings in Github and make sure that:</p>
-->

* 

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have set the correct type of event that the chosen module should receive</p>
  -->

* 

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have entered the correct Payload URL</p>
  -->

