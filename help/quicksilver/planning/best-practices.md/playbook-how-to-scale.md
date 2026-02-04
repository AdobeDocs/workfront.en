---
title: "Playbook: Managed Scaling, After the First Win"
description: Learn how to roll out Adobe Workfront Planning after your first successful implementation
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: yes
hide: yes
---

# Playbook: managed scaling, after the first win 

**Version**: 1.0 

**Context**: "We've landed our first use case, and now everyone wants in." 

 

## 1. The "Success Trap" 

Sometimes it can feel like the most dangerous phase of WFP adoption is immediately after the first successful use case or POC. Enthusiasm is high, but the fear of "technical debt" and "administrative sprawl" can lead to two equally damaging responses: 

1.  **Over-Governance**: Locking down the system so tightly that new teams revert to spreadsheets. 

2.  **Zero-Governance**: Letting every team create their own fields and record types, recreating the fragmented metadata sprawl found in legacy environments. 

 

## 2. The Core Philosophy: WFP as the "Reconciliation Engine" 

Instead of trying to stop teams from being different, we position WFP as the place where those differences are **made visible so they can be reconciled**. 

 

*   **Managing Adoption Velocity**: It is natural to feel cautious about expanding into a new tool before "cleaning up" existing environments. While choosing to **Simplify First** provides a highly governed foundation, it can delay time-to-value for teams ready to align. We believe the most effective way to lead through this change is to recognize that **visibility is Step 1**. Momentum toward a shared, enterprise-ready tool (moving away from the sprawl of PPTs and spreadsheets) is what ultimately unblocks long-term goals.  

 

    **Recommendation**: Instead of a "Clean Up First" mandate, we recommend allocating a smaller portion of resources to ongoing maintenance and a significantly larger portion to solving pressing business needs. For example, spending a year solely on "cleaning up" taxonomies yields little incremental value. However, delivering **cross-team visibility** (e.g., through a Unified Enterprise Calendar or a consolidated GTM roadmap) provides the transformative value your stakeholders need, while providing the unified data structure you need to govern the environment over time. 

*   **Acknowledge the Reality**: Independent teams naturally develop their own processes, which often stay hidden in siloed spreadsheets. Transitioning to WFP doesn't create a mess; it shines a light on the one that already exists. By making these processes visible in a shared environment, you put them in the one place where they can finally be addressed and improved. 

*   **The Progress Signal**: When a team asks for their own fields, it's not "sprawl"—it's **Adoption**. It means they see WFP as their workspace. 

*   **Manage Debt, Don't Hide It**: It is natural to be concerned about the effort required to clean up divergent taxonomies later. However, the alternative—forcing strict standards too early—often drives teams back to spreadsheets where their processes (and their debt) remain hidden. By allowing teams to begin in WFP with their current classifications, you are moving that debt into a visible, governed environment. This makes the eventual reconciliation an iterative task rather than a single, overwhelming migration project. 

 

## 3. The "Lanes on a Road" Governance Model 

Scale without debt by defining "Global Lanes" and "Local Playgrounds." 

 

### A. The Global Lanes 

*   **Controlled Objects**: Objects that every team must use for enterprise reporting (e.g., `Strategic Pillar`, `Region`, `Fiscal Quarter`). 

*   **Managed By**: The Central COE/Marketing Ops Admin. 

*   **Rule**: These fields are "Shared" and mandatory. 

 

### B. The Local Playgrounds (Spokes) 

*   **Experimental Objects**: Fields or record types specific to a team's tactical needs (e.g., a Social team's `Influencer Handle` or a Web team's `URL Slug`). 

*   **Managed By**: The Team Lead (with light guidance). 

*   **Rule**: Teams can innovate here. If a "Local" field is adopted by >3 teams, it is "Promoted" to a Global Lane. 

 

## 4. The Governance Paradox: Teams First, Standards Follow 

A common challenge in scaling WFP is deciding which comes first: **Enterprise Governance** or **Team Operational Alignment**.  

 

We believe the most effective way to navigate this is to recognize that enterprise value is built on a two-way street: 

1.  **Teams need relevance**: The enterprise only realizes value when its teams are actively executing. Therefore, governance must **serve the teams** by providing structure that supports their known operational needs. 

2.  **The Enterprise needs visibility**: Leadership can only make informed decisions when data is clean enough to aggregate. Therefore, the teams must **serve the enterprise** by providing the minimum viable metadata required for portfolio visibility. 

 

The goal of "Managed Scaling" is to find the intersection of these two needs—standardizing enough to provide visibility, but not so much that you stall team execution. 

 

### A. Aligning Priorities: Data vs. Visualization 

When scaling, recognize that the definition of "Value" differs between personas: 

*   **The Admin/Product Owner**: Values **unified taxonomies and classifications**. Their goal is a clean data architecture that supports long-term scalability. 

*   **The Stakeholder/Leader**: Values **visualization and insight** (e.g., a Global Calendar or a Portfolio Timeline). Their goal is the "Lightning Moment" that makes the data actionable. 

 

**The Strategy**: Use the stakeholder's need for visualization as the *incentive* for the team's compliance with the admin's need for data standards. You get the unified taxonomy by delivering the "Super Calendar" that leadership demands. 

 

### B. The "Service-Led" Observation Phase 

During early scale-up, the Admin's role is to facilitate this exchange between teams and the enterprise. 

*   **Prioritize Operation over Standardization**: It is better to have teams actively planning in siloed workspaces than to have them stalled by a lack of global definitions. This activity is the "raw data" required to build healthy, real-world standards. 

*   **Identify the "Visibility Minimums"**: Work with leadership to identify the 3-5 fields that *must* be clean for enterprise reporting (e.g., `Strategic Alignment`, `Start Date`, `Budget`). Focus your enforcement energy ONLY here. 

 

### B. Retroactive Harmonization (Governance as a Service) 

Once a pattern of "known needs" emerges across teams, the enterprise can move to consolidate those patterns into a global service. 

1.  **Observe Successful Patterns**: Identify the "winning" taxonomies that teams have already built and adopted. 

2.  **The Collaborative Handshake**: Bring team champions together to refine their local successes into a shared enterprise standard. 

3.  **Deploy as a Service**: Roll out the new global lanes not as a "restriction," but as a way to simplify reporting and cross-team alignment for the people doing the work. 

 

**Key Takeaway**: Governance should be a response to operational success, not a prerequisite for it.  

 

## 5. Scaling Mechanics: The Pattern-Based Growth Model 

Applying this philosophy requires a thoughtful approach to data structure. To avoid "Governance Sprawl," resist the urge to build global fields for every individual request. Instead, use the **Field Maturity Path** to let real-world usage guide your enterprise standards: 

 

1.  **Level 1: Local Experiment**: Team A creates a custom field in their workspace. 

2.  **Level 2: Pattern Recognition**: The Admin notices Teams B and C are using or asking for a similar field. 

3.  **Level 3: Enterprise Standardization**: The Admin creates a single, standardized version of that field as a record type in the **Global Taxonomy Workspace** and syndicates it to teams. 

 

### The Mechanics of "Soft Retirement" 

Because WFP does not currently have a native "Archive" feature for fields, retiring a local field requires a deliberate "Soft Retirement" process to preserve historical data without cluttering the UI: 

 

1.  **Data Migration**: Use a table view (or Fusion) to bulk-copy values from the local "Shadow" field into the new Global Lane field. Ensure the data is validated and cleaned during this move. 

2.  **Rename for Deprecation**: Rename the local field with a prefix like `[DEPRECATED]` or `z_` (e.g., `z_Language (Old)`). This pushes the field to the bottom of field pickers and signals to users that it is no longer the "Source of Truth." 

3.  **Form Removal**: **This is the most critical step.** Remove the deprecated field from all **Record Forms**. This prevents new data from being entered while keeping the old data visible in existing table views or reports if needed. 

4.  **The "Sunset" Period**: Keep the deprecated field (prefixed and off-form) for 30-60 days to ensure no data was missed during migration. After this period, if the data is fully reconciled in the Global Lane, the local field can be deleted from the workspace. 

 

## 6. Avoiding the "Core Drift" (The Abstraction Rule) 

To prevent Planning from becoming as cluttered as Core: 

*   **The Abstraction Layer**: Every field in WFP should answer a **Strategic Question**. If a field is only used for tactical tracking (e.g., "Was this proof approved?"), keep it in Core. 

*   **Consolidation First**: If a team wants a new metadata field, invite them to check the Global Taxonomy first. This requires granting team leads **Read-Only access** to the Global Taxonomy workspace (see Section 7). By mapping their tactical needs to an existing strategic field, you prevent unnecessary duplication and maintain reporting integrity. 

 

## 7. The "Read-Only Access" Visibility Model 

Solve the "Siloed" feeling without the noise of "Siloed" work. 

*   **The Problem**: Teams in spokes feel isolated because they only see their own records. 

*   **The Fix**: Grant teams **Read-Only access to the workspaces designated as 'Primary' for those shared record types**.  

*   **The Result**: They can see the broader enterprise context for inspiration and alignment, but their local workspace remains clean and focused on their specific tasks. 

 

## 8. Managing Growth through Workshops 

Scaling WFP is as much a cultural challenge as a technical one. Use targeted workshops to bridge the "Governance Gap." 

 

### A. The "Necessary Mess" Discovery Workshop 

*   **Audience**: Regional Marketing Leads and Ops Champions. 

*   **Goal**: Document the current "Siloed Reality" (the fragmented operational data). 

*   **The Message**: "We aren't here to delete your fields. We're here to understand how they link to the global strategy." 

*   **Outcome**: A draft mapping of local tactical fields to global strategic lanes. 

 

### B. The "Strategic Visibility" Alignment Session 

*   **Audience**: High-level Marketing Stakeholders (leadership). 

*   **Goal**: Reframe the "Simplify First" anxiety. 

*   **The Message**: "We don't need a perfect taxonomy to start. We are using WFP as the environment to *build* the perfect taxonomy." 

*   **Outcome**: Approval to move forward with WFP as the reconciliation engine while Core remains in its current state. 

 

### C. The "Spoke-to-Global" Showcase 

*   **Audience**: New teams exploring WFP. 

*   **Goal**: Reduce the "siloed" feeling. 

*   **The Message**: "See how Team A's local work automatically feeds the designated Primary Workspace? You can have that same visibility for your work too." 

*   **Outcome**: Opt-in from new departments who see the benefit of being "connected" without losing their local independence. 

 

### D. The "Ongoing Support" Office Hours 

*   **Audience**: All WFP users (current and prospective). 

*   **Goal**: Provide a recurring, low-stakes environment for troubleshooting and tactical guidance. 

*   **The Message**: "There are no wrong questions. We are here to help you solve your specific planning challenges in real-time." 

*   **Outcome**: Increased user confidence, faster resolution of technical friction, and the identification of new patterns that might warrant global standardization. 

 

## 9. Staffing for Scale: Roles and Responsibilities 

Success in a managed scaling model requires more than just tool configuration; it requires a clear distribution of roles across the Global and Spoke teams. 

 

### A. The Enterprise Architect (Central COE/Marketing Ops) 

*   **Focus**: Enterprise integrity, system performance, and **unified data taxonomy**. 

*   **Responsibilities**: 

    *   Manages the **Global Taxonomy Workspace**. 

    *   Facilitates the **Field Maturity Path** (promoting local successes to global standards). 

    *   Maintains the **Primary Workspace** views for executive reporting. 

    *   Leads the monthly **Semantic Audit** across workspaces. 

 

### B. The Spoke Champion (Team Process Owner) 

*   **Focus**: Team relevance and adoption velocity. 

*   **Responsibilities**: 

    *   Acts as the single point of contact for the functional team. 

    *   Owns the local workspace structure and custom field experiments. 

    *   Ensures the team uses the **Governed Gateway** (Forms) for data entry. 

    *   Participates in the **Collaborative Handshake** during harmonization. 

 

### C. The Executive Sponsor (Marketing Leadership) 

*   **Focus**: Strategic alignment, OKR visibility, and **portfolio visualization (e.g., Global Calendaring)**. 

*   **Responsibilities**: 

    *   Defines the enterprise **Marketing OKRs** in the Global Taxonomy workspace. 

    *   Champions the value of "Visibility Step 1" to other leaders. 

    *   Reinforces the 80/20 resource allocation (Value over Cleanup). 

 

### D. The Enablement Lead (Change Management) 

*   **Focus**: Cultural shift and skill development. 

*   **Responsibilities**: 

    *   Hosts recurring **Office Hours** and **Discovery Workshops**. 

    *   Maintains the internal "Success Story" showcase. 

    *   Identifies technical friction points for the Enterprise Architect to resolve. 

 

## 10. Checklist for Scaling the Next Team 

* [ ] **Identify the Champion**: Who is the "Process Owner" or "Champion" of this new team? 

* [ ] **Define the "Local Delta"**: What 2-3 fields does this team need that the Global standard doesn't currently provide? 

* [ ] **Map to Global Lanes**: Which existing Global fields can satisfy 80% of their needs? 

* [ ] **Grant Global Visibility**: Give them Read-Only access to the relevant Primary Workspaces and the Global Taxonomy workspace on Day 1. 

* [ ] **Establish the Handoff**: How does their work "feed" the relevant Primary Workspaces? (e.g., via a Global Record Type or a specific lookup). 