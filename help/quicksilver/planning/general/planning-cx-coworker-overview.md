---
title: Adobe Workfront Planning CX Coworker Overview
description: You can use the CX Coworker in Workfront Planning to perform similar actions to records and other objects in Planning that you would normally perform in the interface. The user's commands and the AI's execution of those commands work together to ensure that changes made by the AI are accurately reflected in your environment.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
---

# Adobe Workfront Planning CX Coworker overview

<!--replaced information from the AI Assistant for Planning article with CX Coworker-->

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

The CX Coworker is a conversational interface where you describe a goal in plain language, and then it plans, executes, and validates the work across your Workfront Planning and other connected Adobe systems before bringing it back for your approval. 

The CX Coworker preserves everything AI Assistant does today while adding more powerful end-to-end capabilities in both a new full-screen experience and the Workfront right rail. 

It operates within your organization's existing product-level access controls, so users can only take actions they're already permitted to in Workfront, with read-only access by default and write access controlled by Workfront administrators.

>[!IMPORTANT]
>
>CX Coworker is not currently available to organizations in health care, finance, or some other industries with sensitive data. AI Assistant is available to these organizations. 
>
>For more information, see [AI Assistant overview](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).


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
<p>Any Workfront or Workflow with a Planning package</p>
Or
<p>Any Planning package when purchased as a standalone product</p>
   </td> </tr>
 <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe Planning license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td>  
   <p>Your administrator must do the following to allow access to the CX Coworker in Planning:</p>
   <ul>
   <li><p>Add both a Workflow and a Planning license type to your access level when you have both a Workflow and a Planning package</p></li>
   <li><p>Deselect Disable the CX Coworker panel in Workfront setting in your access level. It is selected by default.</p></li></ul>
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  

  <tr> 
   <td role="rowheader"><p>System settings</p></td> 
   <td>   <p>Your Workfront administrator must select the Read-only and Write-only MCP tools in the System Preferences area of Setup. The Read-only MCP tools is selected by default.</p> 
    </td> 
  </tr> 
</tbody> 
</table> 

 For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerations for the CX Coworker

* The CX Coworker must be enabled for your organization before it is available for users in your company. 

  For information, see [CX Coworker overview](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md). 

* After Workfront has enabled the agent for your Workfront instance, it is available for the main Workfront administrator and they can enable it for your organization. For information, see [Configure system preferences](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

* The Workfront administrator must also enable the CX Coworker for you, in your access level. For information, see [Create and modify access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* The CX Coworker works with information and objects that are in Workfront or Workfront Planning and that you have permission to access. In the Planning right rail, the Coworker panel operates in the context of the workspace, record type, or record page that you have open. 

* The actions performed by the CX Coworker in the Planning area are in the context of your Workfront Planning permissions and your Workfront access level. For information, see the following articles: 

    * [Overview of sharing permissions in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
    * [License type overview when using Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Changes made by the CX Coworker on the user's behalf are tracked in the record's history panel. 

* Actions done by the CX Coworker are permanent and could be irreversible. For example, deleting a field cannot be reversed. Review all actions that are proposed by the CX Coworker before accepting them.

* When creating, updating, or deleting an object through the CX Coworker, the CX Coworker displays the intended actions and asks for confirmation. You can then confirm or cancel the actions. 

## Functionality currently available for the CX Coworker

Currently, the CX Coworker is available in the Planning area of Workfront and it uses a set of skills to access and manipulate information for Planning objects. For more information, see [CX Coworker skills](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-skills.md). 

You can use the CX Coworker to perform the following actions:

* Search for records. You can search by information contained in any record fields. 
* Create records. An ID with a link to the new record displays after the record is created. You can specify the fields you want to update during the creation process, like dates or description. 
* Create records based on a document that you upload. Workfront supports the following document formats for the CX Coworker:

    PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT, and most image formats
* Update fields for the records you see on the screen
* Delete, duplicate, or restore records
* Link records to other records
* View a record's change history


## Locate the CX Coworker in Workfront Planning

You can locate the CX Coworker in the following areas of Workfront Planning:

* The main navigation bar, in the upper-right corner of the screen.
* Inside the details area of a record when you open it in a new tab.

## Access the CX Coworker in the Planning area

1. Log in to Workfront, then click the **Main Menu** icon ![Lines main menu](assets/lines-main-menu.png) in the upper-left corner, then click **Planning**. 

    The Planning area opens. 

    Locate the **Coworker** icon ![Coworker icon](assets/coworker-icon.png) in the upper-right corner of the page, or continue to the steps below. 

1. Click a **workspace card**. 

1. Click a **record type card**. 

1. Click a **record** to open the record's **Details** page, then click the **Open in new tab** icon ![Open in new tab](assets/open-workspace-on-new-tab-icon.png) .

1. Click the **CX Coworker icon** ![Coworker icon](assets/coworker-icon.png) in the upper-right corner of the screen.

1. In the space provided, start typing commands for the CX Coworker, then click Enter when you are done. 

    ![CX Coworker panel with empty command box](assets/cx-coworker-right-rail.png)

    For example, you may type one of the following:

      * Create a new campaign record called Summer Sale 2026
      * Update the budget field in the Summer Campaign record to $75,000
      * Delete the campaign record named Old Promo
      * Restore the campaign I accidentally deleted

    >[!TIP]
    >
    >Ensure your Workfront administrator enabled Write-only MCP Tools in your System Preferences before asking the CX Coworker to perform editing actions on objects.

    A visual indicator displays while the CX Coworker processes commands, setting expectations for response time.
    
    After receiving a successful response, follow the links provided or notice the changes on the left.
    
  
1. (Optional) Click the **Expand full screen** icon ![Expand full screen icon](assets/expand-full-screen-icon.png) to open the Coworker chat box in a full browser tab.


