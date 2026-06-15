---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Approver Decision shows a hyphen in the Proof Approval report
description: A hyphen in the Approver Decision field of the Proof Approval report indicates that a recipient is no longer in a decision-making role on the proof.
author: Courtney
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
---
# Approver Decision shows a hyphen in the Proof Approval report

## Problem

In the Proof Approval report, a recipient's Approver Decision field shows a hyphen (-) even though the Decision Date field shows a date and Awaiting Decision is False.

![Approver Decision shows a hyphen in the Proof Approval report](assets/approver-decision-hyphen.png)

## Cause

A hyphen in the Approver Decision field means that the recipient is no longer in a decision-making role on the proof. This can happen when:

* The recipient was added to the proof, made a decision, and was later removed from the workflow. If the recipient revisits the proof, the proofing system records the visit as a decision change. Because the recipient is no longer an approver, the system records the new decision as a hyphen.
* The recipient's proof role was changed to one that doesn't include approval rights, such as Reviewer. For information about the actions each role can take on a proof, see [Proof Roles overview](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md).
* The recipient's proof permission profile was downgraded after they made their decision.

## What this means in your reports

The hyphen is intentional. It tells you that the system isn't waiting on the recipient to approve the proof, and that the recipient no longer has a decision-making role on the proof.

The Decision Date field still shows the date of the recipient's most recent decision activity, but the recipient's decision is no longer counted in the report.

For information about creating and using the Proof Approval report, see [Use the proof approval report](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/proof-approval-report.md).
