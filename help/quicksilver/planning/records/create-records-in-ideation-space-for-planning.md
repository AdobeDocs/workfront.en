---
title: Create Planning Records from Ideation Space Briefs
description: This article walks through how to use the Ideation space for Workfront Planning to brainstorm campaign ideas and connect them to real Workfront Planning records. 
feature: Workfront Planning
role: User, Admin
author: Alina
---

# Create Planning records from Ideation space briefs

<!--
Will this release JUST to preview? If not - hide the preview portion below
-->

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

This article walks through how to use the Ideation space for Workfront Planning to brainstorm campaign ideas and connect them to real Workfront Planning records. 

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
   <td> <p>Contribute or higher permissions to the workspace and record type where you want to add records. </p>
   <p>View or higher permissions to the workspace and record type to create records using the Request record button on the record page</p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr>  
</tbody> 
</table> 

For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Create records using the Ideation space for Workfront Planning

1. From the Worfront Planning landing page, click the card for a workspace that you can manage. 
1. Click the card for a record type you can add records to. 
1. From any view of the record type page, click **New record** in the upper-right corner of the page. 
1. In the **Choose a way to add your records** box, click **Open the Ideation space**, then click **Continue**. <!--check the UI name for this and get another screen shot below-->

    ![New record box with Open Ideation space button](assets/new-record-creation-picker-with-ideation.png)

    The Ideation space opens with a prompt. 

1. In the **What are you working on?** prompt box, describe what kind of record you want to create.
The more details you share, the more useful the information provided by the ideation space will be.

    Type a description of the campaign you're planning — for example: "back to school campaign for a marketing agency". 
    
1. Click **Start ideating**.

    The Ideation space works through the following steps while it builds your idea: <!--check some of these in the UI - there might have been UI text changes-->

    1. Understand your goal and context
    2. Review your space and selected materials
    3. Gather evidence from documents, web, and data
    4. Synthesize findings into a research summary
    5. Create and refine cards with citations

    During this process you'll see the Ideation space actively searching connected Workfront Planning data or information available on the web.
    
    For example, it might search for existing programs, products, personas, or regions, as well as for similar concepts available online. <!--check on this with Et-->    

    When the ideation completes, the following things are added to the Ideation space: 
    
    * A summary of the AI findings which is linked to several cards with detailed information about things to consider. The details cards display in a new section. A connector indicates which card section belongs to which summary.  

    * A **Brief** file in the lower-left corner of the ideation space. The brief is a draft of the future record and it displays as a record's Details page. 

    ![Ideation card with branches](assets/ideation-card-with-branched-off-additional-cards.png)         

1. (Optional) Click **Sources** on each of the cards to display the sources used which can be either Workfront Planning or the Web. 
    <!--
    1. (Optional) Use the thumbs up or thumbs down icons on a card to give feedback.
    -->
1.  Click the **Select** icon ![Select icon in Ideation space](assets/select-icon-ideation.png) in the upper-left corner of the page and click a card to select it, then either click **Add to brief** to add the card's information to the brief

    Or 

    Click **Ask AI to ...** to choose additional ideas that AI might search for to add to the space. 


1. Click **Add documents** ![Add documents to Ideation space](assets/add-documents-in-ideation-space.png) in the upper-left corner of the page to drag and drop, browse, or search for documents already uploaded to the ideation space. 

   You can upload the following document types: PDF, CSV, Word, Excel, Powerpoint, any image file format. 

1. Click **Add Add WF Taxonomy Card** ![Add records from Planning to Ideation space](assets/add-from-wf-planning-on-ideations-space.png) in the upper-left corner of the page to browse for records and add them to the ideation space. <!--double check the name of the UI element/ tooltip-->






## Step 5: Open the Workfront Planning Records panel

To bring real Workfront Planning records into your canvas (rather than just AI-generated ideas), click the **records icon** in the left-hand toolbar (third icon down). This opens the **Workfront Planning Records** panel, listing all **Connected Record types** available in your Planning environment — for example:

- Products
- Regions
- Personas
- Channels
- Activations
- Project
- Test Record
- Experience Manager Assets

Each type shows a count of existing records. Click a record type to drill in and see the individual records available.

![Workfront Planning Records panel](images/04_planning_records_panel.png)

---

## Step 6: Drag real records onto the canvas

Search or browse within a record type (e.g., **Products** or **Personas**), then drag the record you want directly onto the canvas. In the example, an existing **Nike product** record and a **Deep testing** persona record were both dragged in and positioned near the relevant concept cards.

This lets you visually connect your AI-generated ideas to the actual records that already exist in Workfront Planning, grounding the ideation in real data rather than hypothetical entities.

![Dragging a persona record onto the canvas](images/05_drag_persona_record.png)

---

## Step 7: Refine with follow-up prompts

Use the **Ask anything** box in the bottom-right corner at any time to refine the canvas — for example, typing `regenerate` against a specific card to have Catalyze redo that section using updated context. Catalyze will re-run its reasoning steps (searching, synthesizing, citing) and update the affected cards in place.

---

## Step 8: Review the full canvas

Zoom out to see the complete picture: your original campaign goal, all AI-generated concept cards with citations, the real Workfront Planning records you've pulled in (Products, Personas, etc.), and a **Campaign Brief** summary card in the corner pulling it all together.

![Full canvas overview](images/06_full_canvas_overview.png)

---

## Tips

- **Be specific in Step 2** — richer campaign descriptions produce more relevant, better-grounded cards.
- **Check citations** before trusting a generated fact — click **Sources** on any card.
- **Mix AI cards with real records** — dragging in actual Products, Personas, Regions, etc. keeps the canvas tied to your real Planning data, not just AI speculation.
- Responses are AI-generated and may be inaccurate — always verify against the linked sources before finalizing a record.
