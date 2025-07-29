---
product-area: home
navigation-topic: use-the-home-area
title: Move from Legacy home to New Home
description: Legacy Home will be removed from Workfront on 10/17 with the Q4 release. This article provides information on which functionality will be available in new home as well as recommendations for moving users to the New Home experience. 
author: Courtney
hide: yes
hidefromtoc: yes
feature: Get Started with Workfront
---

# Move from Legacy Home to New Home

Legacy Home will be removed from Workfront on 10/17 with the Q4 release. This article provides information on which functionality will be available in new home as well as recommendations for Workfront administrators moving users to the New Home experience. 

For more information on the Legacy Home deprecation, see the [Legacy Home Deprecation Guide].


## Understand what is changing from Legacy Home to New Home

### Work list

#### Organize work with the My Work widget

The My Work widget was created in widget-form to mirror the Legacy Home worklist as closely as possible. Users can group and filter their Work list in the My Work widget with similar filters and groupings: 

| **Filter** | **Grouping** |
|------------|-----------|
| - Working on <br> - Ready to start <br> - Not ready <br> - Requested <br> - Delegated <br> - Completed | - Project <br> - Status  <br> - Due Date <br> - Nothing |


**Legacy Home groupings not available in New Home**

* Planned Completion Date - Renamed to Due Date in New Home
* Planned start 
* Commit Date 
* My Priority 

| **Legacy Home** | **New Home** |
|------------|-----------|
|       ![](assets/filter-list-legacy.png)     |    ![](assets/filter-list-my-work.png)         |

#### Delegate work

Users can still delegate work from New Home in the following widgets:

* My Work
* My Tasks
* My Issues
* My Approvals

Users can find work delegated to them in the following widgets:

* My Work widget using the Delegated to me filter
* My Approvals using the Delegated approvals filter

| **Legacy Home** | **New Home** |
|------------|-----------|
|       ![](assets/delegate-legacy.png)     |    ![](assets/delegate-my-work.png)         |

#### Use the calendar view

The calendar view is no longer available in New Home; however, a calendar replacement is on the roadmap for Priorities. 

#### Create a personal task

Users can no longer create a personal task the exact same way they did in Legacy Home, Instead, users can create To-do items. 

#### View approvals I've submitted

Users can view approvals they have submitted in New Home in the My approvals widget using the Approvals I've Submitted filter.

#### Add items to My Priority

Users no long have access to a My Priority feature in New Home. We are introducing a new My Focus column with Priorities that will replace this. 

Users can use the Boards widget to track high priority items if desired. 

### Update work items

In Legacy home, users could use the right panel to update their work. In New Home, users now use the Summary panel to update work. This is the same Summary panel available in Projects, Tasks, Issues, and Documents.

#### Use the Summary panel

In the Summary, users can

* Update the percent complete
* Add an Update
* Navigate to the Documents area to upload a document
* View work item details and update custom fields
    Workfront administrators can customize which fields appear in the Summary in the Layout template. For more information, see [Customize Home and Summary using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).
* Change the work item status
* View subtasks
* Log time
* View attached approval processes
* Upload files - This functionality is new 

| **Legacy Home** | **New Home** |
|------------|-----------|
|   ![](assets/right-panel-legacy.png)         |     ![](assets/summary-new-home.png)        |


#### Open the summary panel

Users can open the Summary panel by hovering over the work item, then clicking the **Summary** icon ![](assets/open-summary-new-home.png).

For additional information about how to use the Summary panel, see [Summary overview](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md).

#### Use quick actions

In addition to the Summary panel, users can also use quick actions to
 
* Log time
* Add an Update
* Update a custom form
* Upload a file

To locate the quick actions menu, hover over the work item. The quick actions list displays near the **Work On It** or **Done** button. 

![](assets/quick-actions-new-home.png)


### View approvals and team requests

Users can still manage approvals and team requests in New Home using the following widgets:

* My approval
* All approvals
* Team requests 

For information about adding widgets to your New Home page, see [Add, edit, or remove widgets in New Home].

## Learn about available widgets

Widgets are the foundation of the New Home. By adding widgets to the Home page, users can choose the type of information that displays to best meet their work needs. Some widgets are only available to specific license types, as the objects they track are only available to those licenses. 

Workfront administrators can customize which widgets are available in New Home using a layout template. For more information, see [Customize new Home using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md).

+++ Expand to view a detailed list of the available widgets
Below are the 11 widgets currently available to choose from, as well as a summary of the information they display:

* **My Work**\
   Displays all of your assigned tasks, issues, and requests in one place. You can click the Work On It button to start working on an item, or the Done button to mark them complete. You can also update information (Status, Condition, Percent Complete) about tasks and issues, log time, and add updates from the My Work widget. 

* **Boards**\
    Displays any boards you have created or have been invited to use. You can also create a new board based on the following templates: Basic board, Kanban board, Retrospective board, Dynamic board.

* **My projects**\
    Displays _projects you own_ or _projects you are on_ in a list. You can use  existing filters, views, or groupings to customize the list, or you can create a project directly from the widget.

* **My tasks**\
    Displays tasks that are assigned to you in a list. You can use  existing filters, views, or groupings to customize the list, or you can create a task directly from the widget. You can also delegate your tasks while you are away from the office. 

* **My issues**\
    Displays issues that are assigned to you in a list. You can use existing filters, views, or groupings to customize the list, or you can create an issue directly from the widget. This widget only includes issues whose associated projects are set to Current and doesn't include completed projects. You can also delegate your issues while you are away from the office. 

* **My requests**\
    Displays all requests you have submitted, a filter to only display open requests, and a button that opens the summary panel for a request.

    <span class="preview">In the Preview environment, this widget displays all requests you have submitted, a filter to display only requests that meet criteria you specify, and a button that allows you to rearrange the columns in the widget.</span>

* **Team requests**\
    Displays all pending requests for teams that you are on sorted by team, as well as buttons to directly assign a request to a user or to work on it yourself.

* **My approval**\
    Displays all of your pending assigned or delegated approvals, a button to delegate approvals, and buttons to make approval decisions directly within the widget.

* **All approvals**\
        Displays 2 charts with information about average approval time and decisions as well as list views of pending and overdue approvals. <span style="color: #ff0000;">This feature is part of a phased release and is currently only available for specific customers.</span>

* **Mentions**\
    Displays recent comment threads from across Workfront, similar to the My Updates page. You can use the reply button to compose a reply within the widget. This widget also shows comments made on tasks and issues that you are assigned to, that you assigned to another user, that you own, that you are primary contact on, or that you created—as long as the task or issue has been updated in the last 30 days.

* **To-dos**\
    This unique widget allows you to add items to a personal checklist that you can freely edit. To-dos are tracked as tasks in your personal project, and remain for up to two weeks after completion.

    >[!NOTE]
    >
    >You must have permission to create tasks in order to create to-dos in the To-dos widget, and only personal tasks that are entered by the current user will appear in the widget.

+++

![](assets/widgets-menu.png)

### View widgets available for each license type

By default, the Home page is populated with a few specific widgets based on your license type. The tables below outline which widgets users of each license type see when they first navigate to New Home.

<table border=1 class="inlineTable">
    <tr>
        <td><b>New license type</b></td>
        <td><b>Default widgets</b></td>
    </tr>
    <tr>
        <td>Standard</td>
        <td>My Projects, My Work, Mentions, To-dos</td>
    </tr>
    <tr>
        <td>Light</td>
        <td>My Work, My approval</td>
    </tr>
    <tr>
        <td>Contributor</td>
        <td>My Requests, Mentions, My approval, Boards</td>
    </tr>
    <tr>
        <td>External</td>
        <td>My approval</td>
    </tr>
</table>

<table border=1 class="inlineTable">
    <tr>
        <td><b>Current license type</b></td>
        <td><b>Default widgets</b></td>
    </tr>
    <tr>
        <td>Plan</td>
        <td>My Projects, Mentions, To-dos</td>
    </tr>
    <tr>
        <td>Work</td>
        <td>My Work, Mentions, To-dos</td>
    </tr>
    <tr>
        <td>Review</td>
        <td>My Work, Mentions</td>
    </tr>
    <tr>
        <td>Request</td>
        <td>My Projects, My approval</td>
    </tr>
    <tr>
        <td>Contribute</td>
        <td>My Work, Mentions</td>
    </tr>
    <tr>
        <td>External</td>
        <td>My approval</td>
    </tr>
</table>

## Prepare for the deprecation

To help minimize disruption for you and your organization, below are some recommendations that will help ease the transition.

### Begin the transition to New Home

Our primary recommendation is to begin transitioning to new Home as soon as possible. Organizationally, this means your administrator customizing users' experiences through layout templates—similar to legacy Home—to make sure each user has what they need. 

We recommend administrators:

1. Build a default New Home page layout using layout templates (or, optionally, create one for each user, team, group, or job role that requires a unique layout.) See [Customize new Home using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md) for more information.

1. Assign your new layout templates to a small number of test users, who can verify that their widgets and general settings meet their work needs.

1. Reassign the rest of your users to the New Home page layout.

Doing this as soon as possible will then give your users time to adjust to the new experience and customize their New Home pages to best suit their individual needs. See [Remove, add, and rearrange widgets in new Home]for information on how a user can customize the widgets on their own new Home page.

### Resources for end users

**Help articles**

* [Manage your work with the My Work widget]

**Training**

* [Remove, add, and rearrange widgets in Home tutorial](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home/remove-add-and-rearrange-widgets)
* [Worker Fundamentals in Adobe Workfront](https://adobe-ats.sabacloud.com/Saba/Web_spf/PRODTNT100/app/me/learningeventdetail/cours000000000098821?regId=regdw000000001250612)

>[!IMPORTANT]
>
>This is a free course, but you must log in and enroll to access it.