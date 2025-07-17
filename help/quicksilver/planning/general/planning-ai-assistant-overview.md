---
title: Adobe Workfront Planning AI Assistant Overview
description: You can use the AI assistant to generate, update, or remove records based on the current page context and record structure. The user's commands and the AI's execution of those commands work together to ensure that changes made by the AI are accurately reflected in your environment.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
---

# Adobe Workfront Planning AI Assistant overview

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> 


{{planning-important-intro}}

You can use the AI Assistant to generate, update, or remove records based on the current page context and record structure. 

The user's commands and the AI's execution of those commands work together to ensure that changes made by the AI are accurately reflected in your environment. 

## Considerations about the AI Assistant

* The AI Assistant must be enabled for your organization before it is available for users in your company. For information, see [AI Assistant overview](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md). 
* After Workfront has enabled the AI Assistant for your organization, it is available for the main Workfront administrator. For information, see [Configure basic information for your system](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md). 

* The Workfront administrator must enable the AI Assistant for all other users. For more information, see [Enable or disable AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md). 

* The AI Assistant works in the context of each page. The requests you are submitting for the AI Assistant must reference functionality that is available in the page that you have open. 

* The actions performed by the AI Assistant in the Planning area are in the context of your Workfront Planning permissions and your Workfront access level. For information, see the following articles: 

    * [Overview of sharing permissions in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
    * [License type overview when using Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Changes made by the AI Assistant on the user's behalf are tracked in the record's history panel. 

* You can use commands to undo your actions. For example, you can type "Undo last change" to revert your change. 

* <span class="preview"> When creating, updating, or deleting an object through AI Assistant, AI Assistant displays the intended actions and asks for confirmation. You can then confirm or cancel the actions. </span>

## Functionality currently available for the AI Assistant

Currently, the AI Assistant is available in the Planning area of Workfront for the following pages:

* Workspace page
* Record type page
* Record page

You can use the AI Assistant to perform the following actions, at this time:

* Search for records. You can search by information contained in any record fields. 
* Create records. An ID with a link to the new record displays after the record is created. You can specify the fields you want to update during the creation process, like dates or description. 
* Create records based on a document that you upload. Workfront supports the following document formats for the AI Assistant:

    PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT, and most image formats
* Update fields for the records you see on the screen
* Delete records
* Restore records that you just deleted


## Locate the AI Assistant in Workfront Planning

You can locate the AI Assistant in the following areas of Workfront Planning:

* The main navigation bar, in the upper-right corner of the screen.
* Inside the details area of a record, after you opened the record in the preview or after you opened the record's page.

## Access the AI Assistant in the Planning area

1. Log in to Workfront, then click the **Main Menu** icon ![Dots main menu](assets/dots-main-menu.png) in the upper-right corner of the screen, or the **Main Menu** icon ![Lines main menu](assets/lines-main-menu.png) in the upper-left corner, if available.

. Click **Planning**. The Planning area opens. 

1. Click a **workspace card**. 

1. (Optional) Click a **record type card**. 

1. (Optional) Click a **record** to open the record's **Details** page.

1. Click the **AI Assistant icon** in the upper-right corner of the screen in the global navigation bar or in the upper-right corner of the record's preview or page.

    ![AI Assistant icon](assets/ai-assistant-icon-highlighted.png)

1. In the space provided, start typing commands for the AI Assistant, then click Enter when you are done. 

    ![AI Assistant panel with empty command box](assets/ai-assistant-panel-with-empty-command-box.png)

    For example, you may type one of the following:

    * Create a campaign with a start date of July 4 and end date of July 30
    * Update the Description field of the Summer Campaign record with date to be determined
    * Delete the last record
    * Restore the record 

    A visual indicator displays while the AI Assistant processes commands, setting expectations for response time.
    
    After receiving a successful response, follow the links provided or notice the changes on the left.



