---
title: Access Needed to Use The Ideation Space 
description: Adobe Workfront Planning now offers an additional capability to ideate before you launch your campaigns. Leverage the power of AI to transform data and direct inputs into tangible plans and give teams an informed starting point instead of a blank page. 
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
---

# Access needed to use The Ideation space

<!--add to TOC-->

From Claude:

The permissions and entitlement model below reflects what was documented and confirmed as of the Closed Beta (through Aug 2026). Internal teams were still finalizing a formal access-model document and access-level definitions at this time, so treat this as the current best understanding rather than a final spec — confirm against the latest internal documentation before publishing externally.

## Baseline product requirement

Catalyze is not a standalone purchase — it requires **Workfront Planning**. Customers can access it through either:
- Adobe Workfront Workflow package **with** a Workfront Planning package, or
- Adobe Workfront Planning as a **standalone** product

If an org has Workfront Planning, it will have Catalyze; Catalyze cannot exist without Planning.

For Closed/Open Beta specifically, Catalyze is only available to **Planning + GenStudio (GenS)** customers.

You must have Adobe Workfront Planning to access the Ideation space.

## Customer-level entry requirements (Closed Beta)

To participate in the Closed Beta, customers needed to meet these criteria:
- Active Adobe Customer Journey Analytics (CJA) deployment with campaign tracking in place
- Multi-channel campaigns with a repeatable planning process
- Active use of Workfront Planning for marketing operations
- At least one identified strategist/ideation user who will be the primary Catalyze user

## Org- and user-level enablement

- The Catalyze integration is surfaced to users when the **"strategic ideation" product** is enabled at the **org level**.
- A **user-level feature flag** additionally controls access during the closed beta, so org-level enablement alone isn't sufficient during this phase.
- For Open Beta, access is expected to move to an **opt-in model** (customers actively configure themselves in) rather than opt-out.

## Record-level permissions

Catalyze permissions are inherited from Workfront Planning record permissions — there is no separate permission system layered on top:

- **Rule:** If a user can create a record in Planning, they can also create a canvas in Catalyze — any Planning license is sufficient for this.
- **Read-only users:** A user with read-only access to a record has **read-only access** to the canvas connected to that record.
- **View-only records:** If a user only has *view* access to an existing record, they **cannot open Ideation** from it at all (this was confirmed as a known behavior, with an "Insufficient permissions" state surfaced to the user).
- A canvas is always related to exactly **one** record.

As of Aug 2026, the team was actively defining discrete access levels for Ideation/Catalyze, expected to include at minimum:
- Can read
- Can view
- Can create

## Org/IMS-level entitlements

Beyond Planning access itself, a customer's IMS Org needs specific entitlements for the full Catalyze experience to work:

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use Catalyze |
| Fonts entitlement | Entitlement | Missing entitlement can block the full Catalyze experience |
| Adobe Cloud Platform / document storage entitlement | Entitlement | Existing documentation indicates users may be able to reach ideation entry points but fail during actual usage if storage-related entitlements are missing |

Historically, some customer teams relied on GenStudio (GenS) provisioning without realizing they could use Catalyze directly — provisioning conversations should confirm both Planning and GenStudio PEM entitlements are explicitly set up for Catalyze, not just assumed via GenS.

## Content-sharing and abuse controls

Because Catalyze lets users create content and share it with other users through Adobe systems, a **"Report Abuse"** capability is planned as a requirement before General Availability (needed roughly one month ahead of GA to support Adobe's platform license agreement process). This may reuse existing Report Abuse functionality from another Adobe product (Horizon) rather than being built from scratch.

## Coworker (conversational AI) access — separate consideration

Access to the **Coworker** integration inside Catalyze (the conversational right-rail assistant) is being rolled out separately from core Catalyze/Planning access:
- As of mid-Aug 2026, Coworker access was not yet generally available for customer testing.
- By Aug 17, 2026, Coworker was available inside Catalyze for internal use but still being refined.
- If you are documenting or testing Coworker-in-Catalyze specifically, verify current availability separately from standard Planning/Catalyze provisioning — do not assume it's included automatically.

## Practical checklist for provisioning a customer

1. Confirm the customer has Workfront Planning (via Workflow+Planning or Planning standalone).
2. Confirm the customer's IMS Org has GenStudio PEM entitlements provisioned (not just assumed).
3. Confirm font and document-storage entitlements are active — test actual usage, not just entry-point visibility.
4. Confirm the "strategic ideation" product is enabled at the org level.
5. During Closed Beta, confirm the user-level feature flag is set for named ideation users.
6. Confirm the target users have **create** (not just view) access to the records they need to ideate on.
7. If Coworker-in-Catalyze is in scope, verify its availability separately.

## Packaging

| Detail | Description |
|---|---|
| Included with Workfront Planning | Yes |
| Standalone option | Can also be launched as its own surface |
| Agent platform | Runs within the Adobe Agent Orchestrator |
| Billing | Monetized through Adobe's AI-credits framework |
