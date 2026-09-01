---
title: Configure the Ideation Space and Create Briefs
description: This article walks describes how you can configure the Ideation space and how you can create briefs which later could be saved as Adobe Workfront Planning records. 
feature: Workfront Planning
role: User, Admin
author: Alina
---

# Configure the Ideation space and create briefs

<!-- add to TOC and miniTOC-->

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

This article walks describes the following: 

* How to configure the Ideation space
* How you create briefs which later could be saves as Adobe Workfront Planning records. 

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
   <li><p>Adobe Customer Journey Analytics</p></li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe Planning license</p></td> 
   <td><p>Planning Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>You must add both a Workflow and a Planning license type to the access level when you have both a Workflow and a Planning package</p>   
</td> 
  </tr>  
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Contribute or higher permissions to the workspace and record type where you want to add records </p>
      <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
      <p>View permissions to Workfront objects to add them to briefs</p>
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

    For example, you might type something like "Create a back-to-school campaign for K-12 students to run through the month of august, for parents and teachers in the US".  

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

        The cards titles are custom to each ideation. 

    * The cards are placed inside the same frame indicating this is the result of one ideation. 

    * A brief is created and displays in a preview image in the lower-left corner of the Ideation space. <!--add screen shot??-->
    
        The brief contains the same fields as the record you are trying to create or edit. 

1. (Optional) Click **Sources** at the bottom of every card to understand where the information was collected from. 
1. Click a card or click the frame containing all the cards, then click **Add to brief** to add their information to the brief. 

    Workfront will match each piece of information with the field it finds the most likely to store it. 

    For example, timelines are added to date-type fields, descriptions to paragraph-type fields. 
    1. Click a card, then  click **Ask AI to ...** to get ideas of what the next step might be, before adding the information to the brief. 
    1. Click the **Documents** icon <!-- screen shot--> in the upper-left corner of the Ideation space to upload documents to the space. You can add new documents or documents you have already added to the space before. 

        >[!TIP]
        >
        >The Documents setting must be turned on to be able to access documents and upload them to the space.
        >For information, see the section [Configure the Ideation space](#configure-the-ideation-space)in this article.
        > 
    1. Click the **Add WF Taxonomy card** icon <!--screen shot and revise this UI tooltip - submit a bug for this--> and select a connected record type, and then a record to add that record's information to the record type you selected. 


        A card is created for the record you selected to add to the space. 
    1. (Optional) Hover over the record's card and click the **More** menu <!--screen shot--> and click **View in Workfront**. 

        The record's details page opens in another browser tab. 


## Configure the Ideation space

Settings
Search icon
Share
Zoom resolution
Info icon for keyboard shortcuts
Redo and undo icons
How you open a new AI prompt window

    







