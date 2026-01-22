---
title: Get Started with the Adobe Workfront Planning Designer
description: Using the Adobe Planning Designer, you can generate a new workspace, complete with record types and fields in Workfront Planning, add objects to a workspace, or view change history on records. 
recommendations: noDisplay, noCatalog
hidefromtoc: yes
hide: yes
---

<!--add these at release to the metadata:

author: Alina, Becky
feature: Workfront Planning
role: User, Admin -->

# Get started with the Adobe Workfront Planning Designer

{{planning-important-intro}}

You can use the Adobe Planning Designer powered by AI to generate a new workspace, add objects to a workspace (record types, records, views, or fields), or view change history on records.

>[!IMPORTANT]
>
>The Planning Designer is currently only available for users participating in the Closed Beta program.

For information about Workfront Planning, see the following articles:

* [General information about Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md)
* [Get started with Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Adobe Workfront Planning access overview](/help/quicksilver/planning/access/access-overview.md)


## Access requirements 

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront packages</p></td> 
   <td> 
<p>Any Workfront and Planning package</p>
<p>Any Workflow and Planning package</p>
   </td> </tr>

  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table> 

 For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Enrolling in the Closed Beta program for the Planning Designer

<!--edit this Or create a new article under Beta programs?? -->

Currently, you can request to participate in the Closed Beta program for the Planning Designer. 

## Considerations about the Planning Designer

* To use the Planning Designer, your organization must meet the requirements to use the Workfront AI Assistant. 

    For details, see [Prerequisites to AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

* To use the Planning Designer, a system administrator must enable it in the System Preferences area of your Setup. 

* You can use prompts to build Planning objects either by using the Workfront AI Assistant from the Planning area, or by using the Planning Designer. 

* The actions performed by the AI Assistant in the Planning area or those performed by the Planning Designer are in the context of your Workfront Planning permissions and your Workfront access level. 

    For information, see the following articles: 

    * [Overview of sharing permissions in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
    * [License type overview when using Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Changes made by the Planning Designer on the user's behalf are tracked in the record's history panel. 

* You can use commands to undo your actions. For example, you can type "Undo last change" to revert your change. 

* When creating, updating, or deleting an object through the Planning Designer, it displays the intended actions and asks for confirmation. You can then confirm or cancel the actions. 

* When you create workspaces and record types using the Planning Designer, views and fields are also created automatically. 

## Functionality currently available for the Planning Designer

You can use either the Planning Designer or the AI Assistant to perform any of the following actions: 

* Create and configure workspaces 

* Create record types 

* Design fields or formula fields 

* Create, delete, duplicate, and restore records 

* Edit, update, append a field in a record 

* Link records to other records 

* Access record change history 

* Build custom views 

* Create records by importing a document. 

    Creating records from an imported document is available only in the Planning Designer, and not in the AI Assistant. 

    For information about the accepted file types and sizes, see the "Document guardrails" section in the article [Use Form Fill powered by AI to fill in a request using prompts or documents](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).

    <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Enable the Planing Designer for your organization

As a Workfront administrator, you must first enable the Planning Designer for your organization. 

<!--add steps here-->

1. Log in to Workfront as a System Adminstrator. 
1. Click **Main Menu** ![Main menu icon](assets/main-menu-shell.png) in the upper-left corner of the screen, then click **Setup**.
1. Click **System** >  in the left panel, then go to the **AI preferences** area.
1. Turn on the following settings: 
    * **Enable AI**
    * **Opt in to AI Betas**
    * **Planning Designer** 

    ![Planning Designer setting in System Preferences](assets/planning-designer-toggle-in-system-preferences.png)
1. Click **Save**.

    All users in the system that have a Standard license can now see the **Design with AI** button on the Workspaces main page in the Planning area. <!--check screen shot-->

    ![Design with AI button on the Worksapces page](assets/design-with-ai-button-on-workspaces-page.png)

    All users can now start and use the Planning Designer to create and update Workfront Planning objects. 

## Create or update objects using the Planning Designer

You can create or update objects in Workfront Planning either by using the Planning Designer, or the AI Assistant, unless otherwise specified. 

1. Log in to Workfront, then click the **Main Menu** icon ![Lines main menu](assets/lines-main-menu.png) in the upper-left corner.

1. Click **Planning**. The Planning area opens. 

1. Click **Design with AI**. 

    The **Planning Designer** window opens.

    ![Planning Designer window
    ](assets/planning-designer-window.png)

1. In the space provided, start typing commands for the AI Assistant, then click Enter when you are done. 

    <!--add screen shot-->

    For example, you may type a request similar to the ones below:

    * Create and configure a workspace with five record types to manage campaigns

    * Create marketing campaigns for every month of the current year

    * Add a campaign field for Status for the Marketing Design workspace

    * Delete all records in a Status of Stale

    * Update all Planning campaigns to a status of Active

    * Connect Campaigns to Personas in the Marketing Design workspace 

    * Display the change history for the "Valentine's Day" campaign 

    * Build a timeline view for campaigns in the Marketing Design workspace

    * Create records by importing a document. Creating records from an imported document is available only in the Planning Designer, and not in the AI Assistant. 

    <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->
    
1. After receiving a successful response, follow the links provided in the prompt area to create, update or review the object of your request. 

    When you agree to create your objects, your changes display to the right of the prompt area. 

    You can review workspaces, record types, fields, views and records in the preview area to the right of the prompt. 
1. (Optional) Type additional prompts to edit your objects further.
1. (Optional) Click the **Toggle the AI workspace preview screen** icon ![Hide or show preview screen icon](assets/hide-show-preview-screen-in-planning-designer.png) to open or close the preview screen on the right.
1. Click the **Open workspace in new tab icon** ![Open workspace in new tab icon](assets/open-workspace-on-new-tab-icon.png) to open the workspace you're updating in a new tab. 
1. Click the **Close** icon **X** to close the Planning Designer and open the Workspaces area. 
1. Open the  workspace you edited using the Planning Designer and make further changes to its objects.




