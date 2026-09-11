---
title: Create briefs in the ideation space
description: This article describes how you can brainstorm and strategize in the Ideation space to create briefs. You can export finished Ideation briefs to a file or to Workfront Planning to create or update records. 
feature: Workfront Planning
role: User, Admin
author: Alina
---

# Create briefs in the Ideation space

<!-- add to TOC and miniTOC-->

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only as part of the **Ideation space Beta** program. </span>   

<span class="preview">For more information, see [Get started with the Ideation space for Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>

{{planning-important-intro}}

Using the Ideation Space, a new capability from Adobe Workfront Planning, you can turn briefs into Planning records. Exported briefs create new records or update existing ones.

This article describes how you can brainstorm and strategize in the Ideation space to create briefs. To create or update records, export finished Ideation briefs to a file or to Workfront Planning. 

## Access requirements

+++ Expand to view the access requirements for the functionality in this article. 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul> 
<li><p>Any Workfront or Workflow with a Planning package</p></li>
Or
<li><p>Any Planning package when purchased as a standalone product</p></li></ul>
   </td> 

<tr> 
   <td role="rowheader"><p>Additional products</p></td> 
   <td><ul>
   <li><p>Adobe GenStudio for Performance Marketing</p></li>
   <!--
   <li><p>Adobe Customer Journey Analytics</p></li>
   -->
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workflow license</p></td> 
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
   <ul>
   <li><p>You must add both a Workflow and a Planning license type to the access level when you have both a Workflow and a Planning package</p>   </li>
   <li><p>The Disable Ideation space setting in your access level must be deselected</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Contribute or higher permissions to the workspace and record type where you want to add records </p>
      <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
      <p>View permissions to Workfront objects to add them to briefs <!--not sure if this is available--></p>
      <p>Editor permissions on the Ideation space to create briefs</p>
   </td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
   <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
   <li>GenStudio System Manager to access Activations <!--and Events--></li></ul>
   For information, see <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
   </p>
  </td> 
  </tr> 
</tbody> 
</table> 

For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  

## Create Ideation space briefs

1. Start in Workfront Planning and either create or edit a record using the Ideation space. 

    For more information, see [Create Planning records from Ideation space briefs](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md). 
1. When the **Ideation space** opens, use the prompt provided to describe the kind of brief you want to create. 

    For example, type "Create a back-to-school campaign for K-12 students to run through the month of august, for parents and teachers in the US".  To make the brief as complete as possible, indicate as much information as you have available for what kind of campaign, the timeline, the stakeholders, and other details. 

1. Click **Start ideating**.  

    Once opened, the Ideation space agent goes through the following steps:

    1. **Data ingestion and synthesis**:  Pulls relevant information from connected sources. For example: 
    
        * Existing record types or the existing record type that you started from. 
        * Recent documents you might have uploaded in the ideation space. 
        * Web information that matches your prompt criteria.

            >[!TIP]
            >
            >The Web search setting must be turned on for AI to be able to look for information on the web.  
            >For information, see the section [Configure the Ideation space](#configure-the-ideation-space)in this article.
            >
    1. **Audience definition**: Identifies or recommends target audience parameters based on historical patterns
    1. **Strategy framing**: Structures the strategic narrative for the campaign
    1. **Messaging and concept ideation**: Generates initial message options and creative concept directions
    1. **Brief generation and planning handoff**: Produces a structured brief that feeds back into the Workfront Planning workspace

        When the Ideation agent finishes the process of collecting all the information, the following things occur: 
    
        * Five cards are created and are organized by relevant and like-information. 

            The cards are titled using various steps in the creation of the requested record, for easy recognition. 
    
            For example, they could be named:

            * Plan
            * Timeline
            * Segments
            * Mechanics  
            * Messaging 

        The cards titles are custom to each card in the ideation. 

        * The cards are placed inside the same frame indicating this is the result of one ideation. 

        * A brief is created and displays in a preview image in the lower-left corner of the Ideation space. <!--add screen shot??-->
    
        The brief contains suggested fields that the system considers pertinent to the ideas you are exploring. 

1. (Optional) Click the **Help** icon ![](assets/more-information-icon.png) in the upper-right corner for a list of keyboard shortcuts to help you navigate through the Ideation space. 

1. (Optional) Click **Sources** at the bottom of every card to understand where the information was collected from. 

    Information can be imported either from Workfront Planning or the Web. 
1. (Optional) Use the thumbs up or thumbs down icons on a card to give feedback.<!--is this still available??-->
1. Click a card or click the frame containing all the cards, then click **Add to brief** to add their information to the brief. 

    Workfront matches each piece of information with the field it finds the most likely to store it. 

    For example, timelines are added to date-type fields, descriptions to paragraph-type fields. 
    1. (Conditional) Click a card, then click **Ask AI to ...** to get ideas of the next step, before adding the information to the brief. The answers are in the context of each card's information. 
    1. Click the **Add documents** icon ![Add documents icon](assets/add-documents-in-ideation-space.png) in the upper-left corner of the Ideation space to upload documents to the space. You can add new documents or documents you have already added to the space before. 

        >[!TIP]
        >
        >The Documents setting must be turned on to be able to access documents and upload them to the space.
        >For information, see the section [Configure the Ideation space](#configure-the-ideation-space) in this article.
        > 
    1. Click the **Add WF Taxonomy card** icon ![Add from Workfront Planning](assets/add-from-wf-planning-on-ideations-space.png) <!--send this tooltip to be revised--> and select a connected record type, then a record from each type to add that record's information to the record type you selected. 

        A card is created for the record you selected to add to the space. The record type displays in the upper-left corner of the record's card. 
    1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) and click **View in Workfront**. 

        The record's details page opens in another browser tab in Workfront Planning. 
    1. (Optional) Select the ideation frame or a card, click the Delete icon, then click Delete to confirm. The card is removed from the Ideation space. 

        When you delete cards corresponding to a stored document or a record, the items are removed from the Ideation space but they remain in their respective applications. 

1. (Optional) Use the **Ask anything** box in the lower-right corner at any time to refine your ideation.

    For example, type `regenerate` for a specific card to have AI redo that card using updated context. The ideation space reruns its reasoning steps (searching, synthesizing, citing) and updates the affected cards.

1. (Optional) In the **Ask anything** box, ask a new question to start a new ideation. 

    A new set of cards is generated, after the space reruns its reasoning steps.
    
1. (Optional) Click one of the purple connectors from any ideation card sets, then click the **Copy to prompt bar** icon to rerun the ideation reasoning. 

    ![Copy to prompt bar icon](assets/copy-to-prompt-bar-icon-highlighted.png)

1. (Optional) Click the **Undo** or **Redo** icons ![Undo and redo icons](assets/undo-redo-icons.png) at the top of the page to cancel or reverse an action. 
1. Zoom out to see the complete picture: your original campaign goal, all AI-generated concept cards with citations, additional documents, the real Workfront Planning records you've pulled in (Products, Personas, etc.). The **Brief** summary card in the lower-left corner pulls it all together.

1. Click the brief preview image in the lower-left corner and review the brief, then click one of the following options: 

    * **Export to file**. You can export the brief to the following file types:

        * PDF
        * Word
        * PowerPoint (with or without a template)
    * **Export to Workfront Planning**. The export overwrites all existing field data in the record in Workfront Planning.

    This finishes creating the record with the additional information and it adds it to the record type you originally selected.

    For more information about updating Planning records using briefs, see the "ConsiderationsConsiderations about using the Ideation space to create records" section in the article [Create Planning records from Ideation space briefs](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md). 


## Configure the Ideation space

There are controls for the Ideation space that configure what you see on the screen as well as help you navigate the space. 

1. Click the **Settings** icon ![Settings](assets/setting-icon.png) to control where AI pulls information from, then choose from the following **Source Types**:

    * **Documents** — documents uploaded to the selected space
    * **Web Search** — external web research
    * **CJA** — Adobe Customer Journey Analytics

1. Click **Save**. 

1. Click the **Help** icon ![Help icon](assets/more-information-icon.png) to review the keyboard shortcuts you can use to navigate the ideation space or select a different zoom value. 

    Choose from the following zoom levels:
    
    * Zoom to 100%
    * Zoom to 200%
    * Zoom to fit

    Or use one of the following shortcuts to navigate on the page: 

    | Action | Shortcut |
    |---|---|
    | Zoom in / out | Ctrl/⌘ + / − |
    | Zoom to fit / fit selection | — |
    | Zoom to cursor | Ctrl/⌘ + scroll |
    | Pan the canvas | Hold Space + drag |
    | Show/hide dot grid | G |

1. Click the Search icon to search for items in the ideation space, then click when it displays in the list to navigate to it. 








