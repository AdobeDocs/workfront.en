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

<!--
I started with this under Records first but what if Ideation will be added to other products and it will generate record types in those products? keep it here so it can be moved, if needed, to a standalone product one day?
-->

<!--
*********************** IMPORTANT ***************
THIS ARTICLE HAS 2 DRAFTS IN 2 SEPARATE AREAS FROM CLAUDE - THEY WERE CREATED AT DIFFERENT TIMES - WHICH ONE WOULD YOU KEEP OR MERGE THEM INTO ONE ARTICLE
-->

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

This article describes how to use the Ideation space for Workfront Planning to brainstorm ideas, create briefs and either generate Planning records or connect them to existing ones. 

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
      <p>View permissions to Workfront objects to add them to briefs</p>
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

## Considerations about using the Ideation space to create records

* You can only launch the Ideation space from Workfront Planning, as you create or edit records. The Ideation space does not exist outside of Workfront Planning. 
* To access the Ideation space, you must have a workspace and a record type in Workfront Planning.
* New records always start with placeholder content, regardless of how you create them. 
* When you delete a Planning record linked to an Ideation brief, the brief remains in the Ideation space, and its associated canvas in the Ideation space is not deleted.
* Synchronization of information happens only from the Ideation space to Workfront Planning. There is no reverse or automatic sync from a Planning record to the Ideation space brief. 
* The following scenarios exist when fields are created, edited or removed in Workfront Planning: 

    * New fields created on records linked to Ideation briefs are added daily to the brief. New fields appear empty in the Ideation brief. 
    * Removed fields remain on the brief and keep their prior values. 
    * Renamed fields update their names in the brief. 
* You can add documents as cards in the Ideation space. This also includes images.

    The following file types are supported: PDF, Excel, CSV, PNG (and other image formats), Word, PowerPoint. Videos are not supported. 

    All uploaded documents are converted to PDF on the backend for processing.
* You can drag and drop records directly from Workfront Planning onto the space, and they appear the same way as manually uploaded files.

## Create records using the Ideation space

1. From the Workfront Planning landing page, click the card for a workspace that you can manage. 
1. Click the card for a record type you can add records to. 
1. Do one of the following to create a record:

    * From any view of the record type page, click **New record** in the upper-right corner of the page and in the **Choose a way to add your records** box, click **Open the Ideation space**, then click **Continue**. 
    * Scroll to the bottom of the record table and click **New row**, then click **Open the Ideation space**.

        >[!TIP]
        >
        >Selecting **Don't show** permanently dismisses the future prompt. Clicking the Close icon **X** closes this box, but it will reappear next time you add a record inline.

    ![New record box with Open Ideation space button](assets/new-record-creation-picker-with-ideation.png)

    The Ideation space opens in a new tab with an empty prompt. 

    The record is created immediately with placeholder text.

1. (Optional) Click **Use existing brief** in the prompt box to browse and add an existing document which the Ideation space will use to create the brief and the future record. 

    ![Empty ideation brief prompt](assets/empty-ideation-prompt.png)

1. (Optional) Click the **Open previous canvases** <!--accurate??--> icon ![Open existing briefs icon](assets/open-existing-briefs-icon.png) in the upper-right corner of the prompt box, to open existing briefs

1. In the **What are you working on?** prompt box, describe what kind of record you want to create.

    The more details you share, the more useful the information provided by the ideation space will be. For example, type a description of the campaign you're planning: "back to school campaign for a marketing agency". 

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

1. (Optional) Click **Sources** on each of the cards to view where information was imported from. Information can be imported either from Workfront Planning or the Web. 

1. (Optional) Use the thumbs up or thumbs down icons on a card to give feedback.<!--is this still available??-->
1. Click the **Select** icon ![Select icon in Ideation space](assets/select-icon-ideation.png) in the upper-left corner of the page and click a card to select it, then either click **Add to brief** to add the card's information to the brief

    Or 

    Click **Ask AI to ...** to prompt for additional ideas that AI might generate to add to the space. 

1. Click **Add documents** ![Add documents to Ideation space](assets/add-documents-in-ideation-space.png) in the upper-left corner of the page to drag and drop, browse, or search for documents already uploaded to the ideation space. 

   You can upload the following document types: PDF, CSV, Word, Excel, PowerPoint, any image file format. 

1. Click **Add WF Taxonomy Card** ![Add records from Planning to Ideation space](assets/add-from-wf-planning-on-ideations-space.png) in the upper-left corner of the page to browse for records in Workfront Planning and add them to the ideation space. <!--double check the name of the UI element/ tooltip-->

    Records are listed under their respective record type. Each type shows a count of existing records. Click a record type to expand it and view the individual records available. 

    <!--replace the shot-->

    <!--![Workfront Planning Records panel](images/04_planning_records_panel.png)-->

1. Search or browse for records within a record type, then drag and drop the record you want directly onto the canvas. 

    This lets you visually connect your AI-generated ideas to the actual records that already exist in Workfront Planning.

    <!--replace the shot-->

    <!--![Dragging a persona record onto the canvas](images/05_drag_persona_record.png)-->

1. (Optional) Use the **Ask anything** box in the bottom-right corner at any time to refine your ideation.

    For example, type `regenerate` for a specific card to have AI redo that card using updated context. The ideation space reruns its reasoning steps (searching, synthesizing, citing) and updates the affected cards.

1. Zoom out to see the complete picture: your original campaign goal, all AI-generated concept cards with citations, the real Workfront Planning records you've pulled in (Products, Personas, etc.). The **Brief** summary card in the lower-left corner pulls it all together.

1. Click the brief preview image in the lower-left corner and review the brief, then click one of the following options: 

    * Export to file. You can export the brief to the following file types:

        * PDF
        * Word
        * PowerPoint (with or without a template)
    * **Export to Workfront Planning**. The export overwrites all existing field data in the record in Workfront Planning.

    This finishes creating the record with the additional information and it adds it to the record type you originally selected.

## Edit existing records in Ideation space

You can open the Ideation space from existing records to update them. 

You cannot bulk-edit records in the Ideation space.

1. Go to an existing record in Workfront Planning and open its details page. 

1. Click **Open in Ideation space**. This opens the Ideation space in a new tab.

    If an ideation for the record already exists, it opens that space.
    
    If no ideation exists, it creates an ideation space and a brief. 

    >[!TIP]
    >
    >Bulk-editing records using the Ideation space is not available.

    <!-- 
    I don't think these steps are still valid but the environment was not available to test: 
    - If a record is already linked to a Catalyze canvas, a link appears beneath the record title; clicking it opens the associated canvas.
    - If a linked canvas hasn't been exported/pushed back yet, the record shows a placeholder message ("This record has active Canvas...") even if the canvas itself has a real name in Catalyze.
    -->

1. Continue editing the brief as described in the section [Create records using the ideation space](#create-records-using-the-ideation-space) in this article. 






<!-- this is from Claude, but rephrased and included most of this above: 

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

***************SECOND DRAFT FROM CLAUDE*******************
# Creating and Managing Records with Catalyze Ideation

> This workflow reflects the Closed Beta experience and is expected to evolve before Open Beta and GA. Confirm current behavior before publishing to customers.

This guide explains how to create and ideate on records using Catalyze within Workfront Planning. It covers all entry points, system behavior, data sync rules, and file-upload support.

## Before you start

- You must have access to a record list within Workfront Planning.
- Catalyze always opens in a **new browser tab** — this is consistent across every entry point.
- Any record created through Catalyze starts with **placeholder text** until you begin ideating.

## Option 1: Create a record via the top-level "New Record" button

1. Navigate to your record list in Workfront Planning.
2. Click the **New Record** button at the top of the page.
3. From the dropdown menu, select **Ideate in Catalyze**.
4. A new browser tab opens automatically, launching the Catalyze canvas.
5. A new record is created in Workfront Planning with placeholder text.
6. Begin ideation directly in Catalyze.

**Additional access from the record view:** Open the newly created record and, in its detail modal, click **Ideate in Catalyze**. This opens Catalyze in a new tab (same behavior as above).

## Option 2: Create a record via inline record creation (bottom of table)

1. Scroll to the bottom of the record table.
2. Click **New Record**.
3. The record is created immediately with placeholder text.
4. A pop-up appears with these options:
   - **Open Catalyze** — launches Catalyze in a new browser tab
   - **Don't Show Again** — permanently dismisses the future prompt
   - **X (Close)** — closes the pop-up; it will reappear next time
5. Click **Open Catalyze** to begin ideation.

## Working with existing records

**Contextual actions (bottom selection bar)**
- **Single record selected:** an "Ideate in Canvas" / "Open in Canvas" action appears.
  - If a canvas already exists, it opens that canvas.
  - If no canvas exists, it creates a new one.
- **Multiple records selected:** the Ideate/Open in Canvas action is **not available** — bulk ideation is not supported.

**Record detail panel**
- If no canvas is connected, an **Ideate in Catalyze** button appears in the record header.
- If a record is already linked to a Catalyze canvas, a link appears beneath the record title; clicking it opens the associated canvas.
- If a linked canvas hasn't been exported/pushed back yet, the record shows a placeholder message ("This record has active Canvas...") even if the canvas itself has a real name in Catalyze.

**When can you create a canvas for a record?**
A canvas can be created for a record that is in Workfront Planning and still in **draft** state (not yet marked "ready").

## Record deletion behavior

If a Planning record linked to a Catalyze canvas is deleted:
- The canvas remains intact in Catalyze.
- No data is removed from Catalyze.

## Data synchronization rules

**Sync direction:** One-way only, from Catalyze → Workfront Planning. There is no reverse or automatic sync from Planning back to Catalyze.

**Export process:**
1. In Catalyze, click **Export to Planning**.
2. Data is pushed to the connected Workfront Planning record.
3. The export **overwrites all existing field data** in the record.

**Important notes:**
- Changes made directly in Workfront Planning do **not** sync back to Catalyze.
- Data refresh in Workfront Planning is manual only (Beta behavior) — there is no scheduled/automatic sync.
- Schema updates do sync one direction: once connected, Planning schema changes propagate to Catalyze daily — added fields appear empty, removed fields keep their prior values, and renamed fields update in place.

## Uploading documents into the Catalyze canvas

- Files can be added as a "document card" on the canvas — this works the same whether the file is an image or another document type.
- You can drag and drop files directly from Workfront Planning onto the canvas, and they appear the same way as manually uploaded files.
- All uploaded documents are converted to PDF on the backend for processing.
- Supported file types (as of the Aug 2026 beta): **PDF, Excel, CSV, PNG (and likely other image formats), Word, PowerPoint.**
- **Not supported:** video files.
- You can include images directly in a prompt and Catalyze will recognize their content, though small-format legibility is still being refined.

## Key takeaways

- Use **Ideate in Catalyze** to connect records to the AI-assisted ideation workflow.
- Catalyze always launches in a separate browser tab.
- New records always start with placeholder content, regardless of entry point.
- Data flow between Catalyze and Planning is manual and one-directional (Catalyze → Planning).
- Deleting a Planning record does not delete its associated Catalyze canvas.

-->


<!--
Internal info: 

## The Ideation space and Adobe GenStudio

Adobe GenStudio for Performance Marketing is Adobe's end-to-end content supply chain solution, spanning five stages:

1. Strategy and Ideation
2. Workflow and Planning
3. Asset Management
4. Creation and Production
5. Delivery and Activation

The Ideation space fits in the **Strategy and Ideation** stage — the front door of the content supply chain — and is designed to work natively with the rest of GenStudio, so the briefs and strategic direction it generates flow directly into Workfront Planning for execution.
-->


