---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Trello modules
description: In an Adobe Workfront Fusion scenario, you can automate workflows that use Trello, as well as connect it to multiple third-party applications and services.
author: Becky
feature: Workfront Fusion
---

# Trello modules

In an Adobe Workfront Fusion scenario, you can automate workflows that use Trello, as well as connect it to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
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
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use Trello modules, you must have a Trello account.

## Connect Trello to Workfront Fusion

For instructions about connecting your Trello account to Workfront Fusion, see [Create a connection to Adobe Workfront Fusion - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md)

## Trello modules and their fields

When you configure Trello modules, Workfront Fusion displays the fields listed below. Along with these, additional Trello fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Boards](#boards) 
* [Lists](#lists) 
* [Cards](#cards) 
* [Members](#members) 
* [Checklists](#checklists) 
* [Labels](#labels) 
* [Comments](#comments)

### Boards {#boards}

* [Watch Boards](#watch-boards) 
* [Create a Board](#create-a-board) 
* [Edit a Board](#edit-a-board) 
* [Get a Board](#get-a-board) 
* [Search for Boards](#search-for-boards) 
* [Archive or Unarchive a Board](#archive-or-unarchive-a-board) 
* [Assign a Member to a Board](#assign-a-member-to-a-board) 
* [Unassign a Member from a Board](#unassign-a-member-from-a-board)

#### Watch Boards {#watch-boards}

This trigger module begins a scenario when a new board is added.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>The maximum number of boards Workfront Fusion will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create a Board {#create-a-board}

This action module creates a new board with the selected settings.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Name </td> 
   <td> <p>Enter or map a name for the new board.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Description</td> 
   <td> <p>Enter or map the board description if needed.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Organization ID</p> </td> 
   <td> <p>Enter or map the ID of the organization. The Organization ID can be retrieved by using another module, such as the Watch Activities module.</p> <p> <img src="assets/id-of-org.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Permission level</p> </td> 
   <td> <p>Boards have different voting and commenting rules for each permission level. For example: if your board is Private and you set the voting and commenting rules as All, you receive an error. </p> <p>Voting and commenting is limited to the following groups for each permission level:</p> 
    <ul> 
     <li><strong>Private</strong>: 
      -->Members, Members and Observers</li> 
     <li><strong>For organization</strong>: 
      -->Members, Members and Observers, Organization Members</li> 
     <li><strong>Public</strong>: 
      -->Members, Members and Observers, Organization Members, All</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Voting</p> </td> 
   <td> <p>Select an option to specify who can vote on this board. See the Permission level field for voting limitations on permission levels.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Comments</p> </td> 
   <td> <p>Select an option to specify who can comment on cards for this board. See the Permission level field for commenting limitations on permission levels.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Invitations</p> </td> 
   <td> <p>Select who can invite other people to this board.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Self-join</p> </td> 
   <td> <p>Select whether team members can join the board themselves or they have to be invited.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Default labels</p> </td> 
   <td> <p>Select whether to use the default set of labels for the new board.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Default lists</p> </td> 
   <td> <p>Select whether to add the default set of lists to the board (To Do, Doing, Done).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Board source ID</p> </td> 
   <td> <p>Select or map the ID of the board that you want to copy into the new board.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Card Covers</p> </td> 
   <td> <p>Select <strong>Yes</strong> if you want to enable card covers for the board.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Background</p> </td> 
   <td> <p>Select the color of the background or the custom background.</p> <p>Note: Custom backgrounds are available only to Trello Gold and Business Class subscribers.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Card aging</p> </td> 
   <td> <p>Select between two modes of card aging. </p> 
    <ul> 
     <li><strong>Regular</strong>: Cards become progressively more transparent as they age. </li> 
     <li><strong>Pirate</strong>: Cards will tear, yellow, and crack like an old pirate map as they age.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Edit a Board {#edit-a-board}

This action module edits the settings of an existing board.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Board ID</p> </td> 
   <td> <p>Enter or map the unique Trello ID of the board that you want the module to create. You can retrieve the Board ID using another module, such as the Watch Boards module</p> <p> <img src="assets/watch-boards.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">New name</td> 
   <td> <p> Enter or map a new name for the board.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">New description</td> 
   <td> <p> Enter or map a new board description if needed.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Organization ID</p> </td> 
   <td> <p>Enter or map the unique Trello ID of the board that you want the module to edit. You can retrieve the Board ID using another module, such as the Watch Activities module.</p> <p> <img src="assets/org-id.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Subscribe </td> 
   <td> <p>Select an option to specify whether the acting user is subscribed to the board.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Permission level</p> </td> 
   <td> <p>Boards have different voting and commenting rules for each permission level. For example: if your board is Private and you set the voting and commenting rules as All, you receive an error. </p> <p>Voting and commenting is limited to the following groups for each permission level:</p> 
    <ul> 
     <li><strong>Private</strong>: 
      -->Members, Members and Observers</li> 
     <li><strong>For organization</strong>: 
      -->Members, Members and Observers, Organization Members</li> 
     <li><strong>Public</strong>: 
      -->Members, Members and Observers, Organization Members, All</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Voting</p> </td> 
   <td> <p>Select an option to specify who can vote on this board. See the Permission level field for voting limitations on permission levels.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Comments</p> </td> 
   <td> <p>Select an option to specify who can comment on cards for this board. See the Permission level field for commenting limitations on permission levels.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Invitations </td> 
   <td> <p>Select who can invite people to this board.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Self-join</td> 
   <td> <p> Select whether team members can join the board themselves or they have to be invited.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Card covers</td> 
   <td> <p> Select whether card covers should be displayed on this board.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Background </td> 
   <td> <p>Select the color of the background or the custom background.</p> <p>Note: Custom backgrounds are available only to Trello Gold and Business Class subscribers.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Background ID</td> 
   <td> <p> If you have selected to use a custom background in the Background field, enter or map the ID&nbsp;of the background you want to use..</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Card aging</p> </td> 
   <td> <p>Select between two modes of card aging. </p> 
    <ul> 
     <li><strong>Regular</strong>: Cards become progressively more transparent as they age. </li> 
     <li><strong>Pirate</strong>: Cards will tear, yellow, and crack like an old pirate map as they age.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calendar feed enabled</td> 
   <td> <p> Select whether the calendar feed is enabled or not.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">&lt;Color&gt; label name</td> 
   <td> <p> Assign a name to the desired color label.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Archive </td> 
   <td> <p>Select an option to indicate whether you want to archive (close) the board. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a Board {#get-a-board}

This action module retrieves a board's details.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Board ID</p> </td> 
   <td> <p>Enter or map the ID of the board you want to retrieve information about.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Search for Boards {#search-for-boards}

This search module retrieves information about a board that you specify .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query </td> 
   <td> <p>Enter or map the name (or a part of the name) of the board that you want to get information about.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned boards</td> 
   <td> <p> Enter the maximum number of boards Workfront Fusion will return during one execution cycle. This value must be less than or equal to 1000.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Partial </p> </td> 
   <td> <p>By default, this module searches member content for exact matches of each word in your query. When Partial is enabled, the module looks for content that starts with any word in your query.</p> <p> For example If you are using the word “development” to look for a board titled "My Development Status Report," by default you would need to search for the entire word. If you have Partial enabled, you would be able to search for "dev" but not "velopment."</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Boards </td> 
   <td> <p>Enter "mine," or map a comma-separated list of board IDs.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Archive or Unarchive a Board {#archive-or-unarchive-a-board}

This action module closes or re-opens a board that you specify .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Board ID</td> 
   <td> <p> Enter or map the ID of the board you want to close or re-open.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Archive or unarchive</td> 
   <td> <p> Select whether you want to close (archive) or re-open (unarchive) the board.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Assign a Member to a Board {#assign-a-member-to-a-board}

This action module assigns a member to a board that you specify .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Board ID</td> 
   <td> <p> Select the board where you want to add a member.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Email address</td> 
   <td> <p> Enter or map the email address of the member you want to add to the board.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Member type</p> </td> 
   <td> <p>Select the type of member you want to add to the board.</p> 
    <ul> 
     <li><strong>Admin</strong>: A board administrator can perform any board action on the board.</li> 
     <li><strong>Normal</strong>: A normal member is simply a member of the board.</li> 
     <li><strong>Observer</strong>: An observer is a member with read-only access to the board. <br>Observers are only available to teams with Trello Business Class.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Full name</td> 
   <td> <p> Enter the full name of the user you want to add to the board.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Unassign a Member from a Board {#unassign-a-member-from-a-board}

This action module removes a member from a board.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Board ID</td> 
   <td> <p> Enter (map or select) the ID of the board you want to remove the user from.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Member </td> 
   <td> <p>Select the member you want to remove from the board.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Lists {#lists}

* [Watch cards moved to a list](#watch-cards-moved-to-a-list) 
* [Create a List](#create-a-list) 
* [Edit a List](#edit-a-list) 
* [Get a List](#get-a-list)

#### Watch cards moved to a list {#watch-cards-moved-to-a-list}

This trigger module activates when a card is moved to a specific list.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Board</td> 
   <td>Select the board that contains the list that you want to watch for cards.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">List</td> 
   <td>Select the list that you want to watch for cards.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>The maximum number of cards Workfront Fusion will return during one execution cycle.</p>  </td> 
  </tr> 
 </tbody> 
</table>

#### Create a List {#create-a-list}

This action module creates a list on a board that you specify .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Board ID</td> 
   <td> <p> Enter or map the ID of the board where you want to create a list.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Name </td> 
   <td> <p>Enter or map a name for the new list.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Position </td> 
   <td> <p>Select whether you want to add the list to the top or append it to the bottom of the card.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Copy list</td> 
   <td> <p> Select how you want to enter the ID of the list you want to copy.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>In the <strong>List ID</strong> field, enter or map the ID&nbsp;of the list you want to copy.<br></p> </li> 
     <li> <p><strong>Select</strong> </p> <p>Select the board that contains the list you want to copy, then select the list.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Edit a List {#edit-a-list}

This action module edits an existing list.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">List ID</td> 
   <td> <p> Enter or map the ID of the list you want to update.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Name </td> 
   <td> <p>Enter or map a new name for the list.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Board ID</td> 
   <td> <p> Map or select the board where you want to move the list.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Position </td> 
   <td> <p>Select whether you want to add the list to the top or append it to the bottom of the card.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Subscribed</td> 
   <td> <p>Enable this option if you want to subscribe the active member to the list.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a List {#get-a-list}

This action module retrieves details about a specific list.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>List ID</p> </td> 
   <td> <p>Enter or map the ID of the list you want to retrieve information about.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Cards {#cards}

* [Watch cards](#watch-cards) 
* [Create a card](#create-a-card) 
* [Edit a Card](#edit-a-card) 
* [Get a Card](#get-a-card) 
* [Search for Cards](#search-for-cards) 
* [Archive or Unarchive a Card](#archive-or-unarchive-a-card) 
* [Add an Attachment](#add-an-attachment)

#### Watch cards {#watch-cards}

This trigger module activated when a new card is added.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Watched object</td> 
   <td> <p>Select the location you want to watch for cards.</p> 
    <ul> 
     <li><strong>All cards</strong> </li> 
     <li> <p><strong>Cards on specific board</strong> </p> <p>Select the board that you want to watch for cards</p> </li> 
     <li> <p><strong>Cards on specific list</strong> </p> <p>Select the board that contains the list you want to watch for cards, then select the list.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>The maximum number of cards Workfront Fusion will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create a card {#create-a-card}

This action module creates a card in a selected list.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enter a list ID</td> 
   <td> <p> Select how you want to enter the ID of the list where you want to add a card.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>In the <strong>List ID</strong> field, enter or map the ID&nbsp;of the list where you want to add a card.<br></p> </li> 
     <li> <p><strong>Select</strong> </p> <p>Select the board that contains the list you want to copy, then select the list.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Labels </td> 
   <td> <p>For each label that you want to add to the card, enter the ID of the label. The ID can be retrieved, for example, using the Retrieve Labels module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Members</td> 
   <td>For each member that you want to add to the card, enter the ID of the member. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Name </td> 
   <td> <p>Enter a name for the new card.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Description</p> </td> 
   <td> <p>Enter the description for the card.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Position </td> 
   <td> <p>Select whether you want to add the card to the top or append the card to the bottom of the list.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Due date</td> 
   <td> <p> Enter a due date for the card. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Due complete</td> 
   <td> <p> Enable this option to mark the card is complete on the due date.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">File URL</td> 
   <td> <p>Enter or map the URL of a file that you want to add as an attachment to the card.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Source file</p> </td> 
   <td> <p>Enter or map information for a file you to want to add as an attachment to the card.</p> 
    <ul> 
     <li>File name: Enter or map the file name, including the file extension.</li> 
     <li> <p>File data: Enter or map the file data (from previous module, e.g. <strong>Dropbox &gt; Get a File or Google Drive &gt; Get a File</strong>)</p> <p>Note: There is a 10 MB file upload limit per attachment. However, Business Class and Trello Gold members have a 250 MB file upload limit per attachment.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Copy card</td> 
   <td> <p> Select how you want to enter the ID of the card you want to copy.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>In the <strong>Card ID</strong> field, enter or map the ID&nbsp;of the card you want to copy.<br></p> </li> 
     <li> <p><strong>Select</strong> </p> <p>Select the board that contains the card you want to copy, then select the list that contains the card, then select the card.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Edit a Card {#edit-a-card}

This action module edits an existing card.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enter Card ID</td> 
   <td> <p> Select how you want to enter the ID of the card you want to edit.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>In the <strong>Card ID</strong> field, enter or map the ID&nbsp;of the card you want to edit.<br></p> </li> 
     <li> <p><strong>Select</strong> </p> <p>Select the board that contains the card you want to edit, then select the list that contains the card, then select the card.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">New name</td> 
   <td> <p>Enter or map a new name for the card.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>New description</p> </td> 
   <td> <p>Enter or map a new description for the card.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Move a card</p> </td> 
   <td> <p>Select the board or the board and list where you want to move the card.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Labels </td> 
   <td> <p>Add the IDs of any labels you want to add to the card. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Position </td> 
   <td> <p>Select whether you want to add the card to the top or append the card to the bottom of the list.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Due date</td> 
   <td> <p> Enter a due date for the card. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Due complete</td> 
   <td> <p> If this option is enabled the card is marked complete on the due date.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Members </td> 
   <td> <p>Add or map the ID of any members you want to add to the card.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Attachment cover ID</p> </td> 
   <td> <p>Enter or map the ID of the image attachment that you want the card to use as its cover.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Subscribe </td> 
   <td> <p>Select whether the member should be subscribed to the card.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Archive </td> 
   <td> <p>Select an option to indicate whether you want to archive (close) the card. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a Card {#get-a-card}

This action module retrieves a selected card's details.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Board ID</td> 
   <td> <p>Enter the ID of the board that contains the card that you want to retrieve details about. This allows you to see names of the board's custom fields.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enter card ID</td> 
   <td> <p> Select how you want to enter the ID of the card you want to retrieve details about.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>In the <strong>Card ID</strong> field, enter or map the ID&nbsp;of the card you want to retrieve details about.<br></p> </li> 
     <li> <p><strong>Select</strong> </p> <p>Select the board that contains the card you want to retrieve details about, then select the list that contains the card, then select the card.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Search for Cards {#search-for-cards}

This action module returns cards that match the search query.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Board </td> 
   <td> <p>Select the boards you want to search through. If no board is selected, all boards will be searched.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Query</p> </td> 
   <td> <p>Enter the search query. You can refine your search using the following search operators:</p> 
    <ul> 
     <li><code><strong>-operator</strong></code> <p>You can add “-” to any operator to do a negative search, such as <code>-has:members</code> to search for cards without any members assigned.</p> </li> 
     <li><code><strong>@name</strong></code> <p>Returns cards assigned to a member. You can also use <code>member:</code>. Use <code>@me</code> to include only your cards.</p> </li> 
     <li><code><strong>#label</strong></code> <p>Returns labeled cards. You can also use <code>label:</code>. For example, <code>label:"FIX IT"</code> will return cards with the label named “FIX IT”.</p> </li> 
     <li><code><strong>board:id</strong></code> <p>Returns cards within a specific board. For example, <code>board:Trello</code> will return cards on boards with Trello in the board name.</p> </li> 
     <li><code><strong>list:name</strong></code> <p>Returns cards within the list named “name”.</p> </li> 
     <li><code><strong>has:attachments</strong></code> <p>Returns cards with attachments. The <code>has</code>: operator can also be used with other attributes, such as <code>has:description</code>, <code>has:cover</code>, <code>has:members</code>, or <code>has:stickers</code>.</p> </li> 
     <li><code><strong>due:day</strong></code> <p>Returns cards due within 24 hours. The <code>due:</code> operator can also be used with other timeframes, such as <code>due:week</code>, <code>due:month</code>, or <code>due:overdue</code>. You can also search for a specific day range. For example, adding <code>due:14</code> to search includes cards due in the next 14 days.</p> </li> 
     <li><code><strong>created:day</strong></code> <p>Returns cards created in the last 24 hours. The<code> created:</code> operator can also be used with other timeframes such as <code>created:week</code> or <code>created:month</code>. You can also search for a specific day range. For example, adding <code>created:14</code> to the search includes cards created in the last 14 days.</p> </li> 
     <li><code><strong>edited:day</strong></code> <p>Returns cards edited in the last 24 hours. The <code>edited:</code> operator can also be used with other timeframes, such as <code>edited:week</code> or <code>edited:month</code>. You can also search for a specific day range. For example, adding <code>edited:21</code> to the search includes cards edited in the last 21 days.</p> </li> 
     <li><code><strong>description:</strong>, <strong>checklist:</strong>, <strong>comment:</strong>, and <strong>name:</strong></code> <p>Returns cards matching the text of card descriptions, checklists, comments, or names. For example, comment:"FIX IT" will return cards with “FIX IT” in a comment.</p> </li> 
     <li><code><strong>is:open</strong> and <strong>is:archived</strong></code> <p>Returns cards that are open or archived. If neither is specified, Trello returns both types.</p> </li> 
     <li><code><strong>is:starred</strong> </code> <p>Only includes cards on starred boards.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned cards</td> 
   <td> <p> The maximum number of cards Workfront Fusion will return during one execution cycle. This value must be less than or equal to 1000.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Partial </td> 
   <td> <p>By default, this module searches member content for exact matches of each word in your query. When Partial is enabled, the module looks for content that starts with any word in your query.</p> <p> For example If you are using the word “development” to look for a board titled "My Development Status Report," by default you would need to search for the entire word. If you have Partial enabled, you would be able to search for "dev" but not "velopment."</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cards </td> 
   <td> <p>Add any cards you want to specifically search for.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Archive or Unarchive a Card {#archive-or-unarchive-a-card}

This action module archives or sends a card back to the board.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Card ID</td> 
   <td> <p> Enter or map the ID of the card you want to archive or send back to the board.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Archive or unarchive</td> 
   <td> <p> Select whether you want to close the card (archive) or send it back to the board (unarchive).</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Add an Attachment {#add-an-attachment}

This action module adds an attachment to the selected card.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enter card ID</td> 
   <td> <p> Select how you want to enter the ID of the card you want to retrieve details about.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>In the <strong>Card ID</strong> field, enter or map the ID&nbsp;of the card you want to retrieve details about.<br></p> </li> 
     <li> <p><strong>Select</strong> </p> <p>Select the board that contains the card you want to retrieve details about, then select the list that contains the card, then select the card.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Attachment type</p> </td> 
   <td> <p>Select whether you want to upload the file directly or provide a URL to the file.</p> 
    <ul> 
     <li> <p><strong>File</strong> </p> <p>Select a source file from a previous module, or map the source file's name and data.</p> </li> 
     <li> <p><strong>URL</strong> </p> <p>Enter the URL to the file, and provide a name for the attachment.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Members {#members}

* [Assign a Member to a Board](#assign-a-member-to-a-board) 
* [Unassign a Member from a Board](#unassign-a-member-from-a-board) 
* [Add a Member to a Card](#add-a-member-to-a-card) 
* [Search for Members](#search-for-members)

#### Assign a Member to a Board {#assign-a-member-to-a-board-1}

See [Assign a Member to a Board](#assign-a-member-to-a-board) in this article.

#### Unassign a Member from a Board {#unassign-a-member-from-a-board-1}

See [Unassign a Member from a Board](#unassign-a-member-from-a-board) in this article.

#### Add a Member to a Card {#add-a-member-to-a-card}

This action module adds the specified member to the specified card.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Enter card ID and member ID</p> </td> 
   <td> <p>Choose how you want to enter the card ID and the member ID.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>Enter or map the <strong>Card ID</strong> and the <strong>Member ID</strong>.</p> </li> 
     <li> <p><strong>Select</strong> </p> <p>Select the board that contains the card you want to add a member to, then select the list that contains the card, the card itself, and the member that you want to add to the card.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Search for Members {#search-for-members}

This action module retrieves information about Trello members.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query </td> 
   <td> <p>Enter the full name or username of the user you want to find.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Partial </td> 
   <td> <p>By default, this module searches member content for exact matches of each word in your query. When Partial is enabled, the module looks for content that starts with any word in your query.</p> <p> For example If you are using the word “development” to look for a board titled "My Development Status Report," by default you would need to search for the entire word. If you have Partial enabled, you would be able to search for "dev" but not "velopment."</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned members</td> 
   <td> <p> The maximum number of members Workfront Fusion will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Checklists {#checklists}

* [Create a Checklist](#create-a-checklist) 
* [Create a Checklist Item](#create-a-checklist-item) 
* [Edit a Checklist Item](#edit-a-checklist-item)

#### Create a Checklist {#create-a-checklist}

This action module creates a checklist on the selected card.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enter a card ID</td> 
   <td> <p> Select how you want to enter the ID of the card where you want to add a checklist.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>In the <strong>Card ID</strong> field, enter or map the ID&nbsp;of the card where you want to add a checklist.<br></p> </li> 
     <li> <p><strong>Select</strong> </p> <p>Select the board that contains the card where you want to add a checklist, then select the list that contains the card, then select the card.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Name </td> 
   <td> <p>Enter or map a name for the checklist.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Position </td> 
   <td> <p>Select whether you want to add the checklist to the top or append the checklist to the bottom of the card.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Enter checklist ID</p> </td> 
   <td> <p>Enter or map the ID of a source checklist that you want to copy into the new one.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create a Checklist Item {#create-a-checklist-item}

This action module adds an item to a specific checklist.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enter checklist ID</td> 
   <td> <p> Select how you want to enter the ID of the checklist where you want to add an item.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>In the <strong>Checklist ID</strong> field, enter or map the ID&nbsp;of the card where you want to add a checklist.<br></p> </li> 
     <li> <p><strong>Select</strong> </p> <p>Select the board that contains the card where you want to add a checklist, then select the list that contains the card, then select the card, then select the checklist.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Item name</p> </td> 
   <td> <p>Enter or map a name for the new item.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Position</p> </td> 
   <td> <p>Select whether you want to add the item to the top or append to the bottom of the checklist.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Checked</p> </td> 
   <td> <p>Enable this option if you want to add the item as already checked.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Edit a Checklist Item {#edit-a-checklist-item}

This action module edits an existing checklist.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enter a Card ID and Checklist Item ID</td> 
   <td> <p> Select how you want to enter the ID of the card and checklist where you want to edit an item.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>In the <strong>Checklist ID</strong> field, enter or map the ID&nbsp;of the card where you want to add a checklist.</p> <p>In the <strong>Checklist Item ID</strong> field, enter or map the ID&nbsp;of the checklist.</p> </li> 
     <li> <p><strong>Select</strong> </p> <p>Select the board that contains the card where you want to add a checklist, then select the list that contains the card, then select the card, then select the checklist.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Checklist ID</td> 
   <td>Select or map the checklist that you want to move the checklist item to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Item name</p> </td> 
   <td> <p>Enter or map a name for the new item.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Position</p> </td> 
   <td> <p>Select whether you want to add the item to the top or append to the bottom of the checklist.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>State</p> </td> 
   <td> <p>Select whether the checklist item is complete or incomplete.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Labels {#labels}

#### Add a Label to a Card

This action module adds a label to a selected card.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enter card ID</td> 
   <td> <p> Select how you want to enter the ID of the card where you want to add a checklist.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>In the <strong>Card ID</strong> field, enter or map the ID&nbsp;of the card where you want to add a checklist. In the<strong>Label ID</strong> field, enter or map the ID&nbsp;of the label that you want to add.<br></p> </li> 
     <li> <p><strong>Select</strong> </p> <p>Select the board that contains the card where you want to add a checklist, then select the list that contains the card, then select the card. </p> <p>Select the label that you want to add to the card.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Comments {#comments}

* [Watch Comments](#watch-comments) 
* [Create a Comment in a Card](#create-a-comment-in-a-card) 
* [List Comments in a Card](#list-comments-in-a-card)

#### Watch Comments {#watch-comments}

Retrieves comment details when there is a new comment in a specified location.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Watched object</td> 
   <td> <p>Select the location you want to watch for comments.</p> 
    <ul> 
     <li><strong>All cards everywhere</strong> </li> 
     <li> <p><strong>Board</strong> </p> <p>Select the board that you want to watch for comments</p> </li> 
     <li> <p><strong>List</strong> </p> <p>Select the board that contains the list you want to watch for comments, then select the list.</p> </li> 
     <li><strong>Card</strong> </li> 
     <li>Select the board that contains the card you want to watch for comments, then select the list that contains the card, then select the card.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>The maximum number of comments Workfront Fusion will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create a Comment in a Card {#create-a-comment-in-a-card}

This action module adds a comment to a selected card.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enter a card ID</td> 
   <td> <p> Select how you want to enter the ID of the card where you want to add a comment.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>In the <strong>Card ID</strong> field, enter or map the ID&nbsp;of the card where you want to add a comment.<br></p> </li> 
     <li> <p><strong>Select</strong> </p> <p>Select the board that contains the card where you want to add a comment, then select the list that contains the card, then select the card.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Comment </td> 
   <td> <p>Enter the comment that you want to add to the selected card.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Comments in a Card {#list-comments-in-a-card}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Trello account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enter a card ID</td> 
   <td> <p> Select how you want to enter the ID of the card where you want to add a comment.</p> 
    <ul> 
     <li> <p><strong>Enter manually</strong> </p> <p>In the <strong>Card ID</strong> field, enter or map the ID&nbsp;of the card where you want to add a comment.<br></p> </li> 
     <li> <p><strong>Select</strong> </p> <p>Select the board that contains the card where you want to add a comment, then select the list that contains the card, then select the card.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned comments</td> 
   <td> <p> Enter the maximum number of comments Workfront Fusion will return during one execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Since </td> 
   <td> <p>Set the start date of the period in which the comment was created. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Before </td> 
   <td> <p>Set the end date of the period in which the comment was created. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type coercion in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Trello Object IDs

* [How to find the ID or the shortlink of a card in Trello](#how-to-find-the-id-or-the-shortlink-of-a-card-in-trello) 
* [How to find IDs of other objects in Trello](#how-to-find-ids-of-other-objects-in-trello)

### How to find the ID or the shortlink of a card in Trello {#how-to-find-the-id-or-the-shortlink-of-a-card-in-trello}

If you want to edit a card or create a new comment, you need to know the ID of the card or its shortlink. You can get this information from the output of the New Card trigger. The shortlink for a card can also be obtained by opening the card and clicking on the Share button. The shortlink can be found in the Link to this card box, at the end of the URL after `https://trello.com/c/`.

![](assets/share-and-more-350x575.png)

### How to find IDs of other objects in Trello {#how-to-find-ids-of-other-objects-in-trello}

Board, list and comment IDs can only be obtained using triggers. The trello.com website does not show these IDs.
