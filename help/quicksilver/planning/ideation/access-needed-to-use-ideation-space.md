---
title: Access Needed to Use the Ideation Space 
description: Adobe Workfront Planning now offers an additional capability to ideate before you launch your campaigns. Leverage the power of AI to transform data and direct inputs into tangible plans and give teams an informed starting point instead of a blank page with Adobe Ideation space. 
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
---

# Access needed to use The Ideation space

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only as part of the **Ideation space Beta** program. </span>   

<span class="preview">For more information, see [Get started with the Ideation space for Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>


{{planning-important-intro}}

Adobe Workfront Planning now offers an additional capability to ideate before you launch your campaigns. Leverage the power of AI to transform data and direct inputs into tangible plans and give teams an informed starting point instead of a blank page with Adobe Ideation space. 

This article describes the access and permissions you must have to access the Ideation space from Workfront Planning. 

For general information about the Ideation space, see [Get started with The Ideation space for Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md). 

## Product requirements

The Ideation space is not a standalone product. It requires a Workfront Planning package and it is only accessible from Workfront Planning. It also requires additional products. 

Your organization must purchase a package for the following products to access the Ideation space: 

* An Adobe Workfront Workflow package in addition to a Planning package

    Or
    
    An Adobe Workfront Planning purchased as a standalone product. 
* An Adobe GenStudio for Performance Marketing license

    >[!TIP]
    >
    >GenStudio for Performance Marketing is needed to have access to the correct font entitlements. 


<!--only required for closed beta:* An Adobe Customer Journey Analytics license that includes campaign tracking-->

## Workfront Planning access level requirements

Ideation space access is configured in Workfront. 

Your Workfront access level must include the following to access Ideation space: 

* A Standard Workflow license, when your company purchased a Workflow package in addition to a Planning package. 
* A Standard Planning license, when your company purchased with a Workflow and a Planning package, or a Workfront Planning as a standalone product. 
* The Disable Ideation space setting in the Set additional restriction section of your access level must be unselected. <!--***********check the UI for this***********-->

## Workfront Planning permissions requirements

Each Planning record is connected to one brief in Ideation space. 

Ideation space brief permissions are inherited from Workfront Planning record permissions. <!--not sure if this is right, because now you can share the ideation with others??-->

You must have Manage permissions for a record type in Planning to create records in order to create or edit a record in the ideation space.

Planning users with View permissions on records can view the ideation space of a record. 

The following table shows the connection between Workfront Planning record permissions and Ideation space brief permissions:

| Planning record-level permission  | Ideation space brief-level permissions |
|---|---|
| Manage permissions to a record | Can create a brief in the Ideation space of the record|
| View permissions to a record | Can read the brief of that record in Ideation space, but cannot modify it|

## Ideation space permissions

<!--this is also duplicated in the intro of the Share an ideation space article-->

Planning permissions are transferred to the ideation space of a record. 

In addition, you can give other users permissions to use the ideation space and add ideas to it. 

Consider the following: 

* Creators of ideations always have Editor permissions on their own ideations. 

* You must have Editor permissions on an ideation space to create briefs and export them to other applications. 

The following are ideation space permissions and the capabilities they offer:  

| Ideation space permission  | Capabilities |
|---|---|
| Editor | Can edit, download and share the ideation space|
| Commenter | Can view and comment on the ideation space|
| Viewer | Can view the ideation space|

For more information about sharing an ideation space, see [Share an Ideation space](/help/quicksilver/planning/ideation/share-the-ideation-space.md). 

<!--there is no additional setup for Workfront layout template assignment because Contributors an below cannot access Ideation space; only Standard users-->


<!-- 
Not sure if this is needed. Maybe all orgs have IMS for all Adobe?? - asking Becky: 

## Org/IMS-level entitlements

Beyond Planning access itself, a customer's IMS Org needs specific entitlements for the full Ideation space experience to work:

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | Missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform / document storage entitlement | Entitlement | Existing documentation indicates users may be able to reach ideation entry points but fail during actual usage if storage-related entitlements are missing |

Historically, some customer teams relied on GenStudio (GenS) provisioning without realizing they could use the Ideation space directly — provisioning conversations should confirm both Planning and GenStudio PEM entitlements are explicitly set up for the Ideation space, not just assumed via GenS.
-->



<!--
From Claude: Internal information, not customer-facing: 

The permissions and entitlement model below reflects what was documented and confirmed as of the Closed Beta (through Aug 2026). Internal teams were still finalizing a formal access-model document and access-level definitions at this time, so treat this as the current best understanding rather than a final spec — confirm against the latest internal documentation before publishing externally.

## Practical checklist for provisioning a customer

1. Confirm the customer has Workfront Planning (via Workflow+Planning or Planning standalone).
2. Confirm the customer's IMS Org has GenStudio PEM entitlements provisioned (not just assumed).
3. Confirm font and document-storage entitlements are active — test actual usage, not just entry-point visibility.
4. Confirm the "strategic ideation" product is enabled at the org level.
5. During Closed Beta, confirm the user-level feature flag is set for named ideation users.
6. Confirm the target users have **create** (not just view) access to the records they need to ideate on.
7. If the Coworker integration inside the Ideation space is in scope, verify its availability separately.

## Packaging

| Detail | Description |
|---|---|
| Included with Workfront Planning | Yes |
| Standalone option | Can also be launched as its own surface |
| Agent platform | Runs within the Adobe Agent Orchestrator |
| Billing | Monetized through Adobe's AI-credits framework |
-->

<!--

Original Claude write-up, in addition to the info above:

## Baseline product requirement

The Ideation space isn't a standalone purchase — you need **Workfront Planning** to access it, through either:

- Adobe Workfront Workflow with a Workfront Planning package, or
- Adobe Workfront Planning as a standalone product

If your org has Workfront Planning, it has the Ideation space too. The Ideation space can't exist without Planning.

For the Closed Beta and Open Beta, the Ideation space is available only to Planning and GenStudio (GenS) customers.

## Customer-level entry requirements (Closed Beta)

To participate in the Closed Beta, customers needed to meet these criteria:

- An active Adobe Customer Journey Analytics (CJA) deployment with campaign tracking in place
- Multi-channel campaigns with a repeatable planning process
- Active use of Workfront Planning for marketing operations
- At least one identified strategist or ideation user who will be the primary Ideation space user

## Org- and user-level enablement

- Workfront surfaces the Ideation space integration to users only after a Workfront administrator enables the **strategic ideation** product at the org level.
- During the Closed Beta, a user-level feature flag also controls access, so org-level enablement alone isn't enough.
- For Open Beta, access is expected to move to an opt-in model, where customers actively configure themselves in, rather than opt-out.

## Record-level permissions

Your Ideation space permissions come from your Workfront Planning record permissions — there's no separate permission system layered on top:

- If you can create a record in Planning, you can also create a canvas in the Ideation space. Any Planning license is sufficient for this.
- If you have read-only access to a record, you have read-only access to the canvas connected to that record.
- If you only have view access to an existing record, you can't open the Ideation space from it. Workfront shows an "Insufficient permissions" message instead.
- Each canvas is related to exactly one record.

>[!NOTE]
>As of August 2026, the team was still defining discrete access levels for the Ideation space. These are expected to include, at minimum, Can read, Can view, and Can create.

## Org and IMS-level entitlements

Beyond Planning access, your organization's IMS Org needs specific entitlements for the Ideation space to work fully.

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | A missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform or document storage entitlement | Entitlement | Users may be able to reach Ideation space entry points but fail during actual use if storage-related entitlements are missing |

>[!IMPORTANT]
>When you provision a customer, confirm that both the Planning and GenStudio PEM entitlements are set up specifically for the Ideation space. Don't assume that GenStudio (GenS) provisioning alone includes Ideation space access.

## Content-sharing and abuse controls

Because the Ideation space lets you create content and share it with other users through Adobe systems, a **Report Abuse** capability is planned as a requirement before General Availability (GA). Workfront needs this roughly one month ahead of GA to support Adobe's platform license agreement process. This capability may reuse the existing Report Abuse functionality from Adobe Horizon rather than being built from scratch.

## Coworker (conversational AI) access

Access to the **Coworker** integration inside the Ideation space, the conversational right-rail assistant, is being rolled out separately from core Ideation space and Planning access:

- As of mid-August 2026, Coworker access wasn't yet generally available for customer testing.
- By August 17, 2026, Coworker was available inside the Ideation space for internal use, but still being refined.
- If you're documenting or testing the Coworker integration inside the Ideation space specifically, verify current availability separately. Don't assume it's included automatically with standard Planning or Ideation space provisioning.

For more information, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

-->
