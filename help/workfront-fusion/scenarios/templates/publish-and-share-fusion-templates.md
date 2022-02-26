---
filename: publish-and-share-fusion-templates
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Publish and share Adobe Workfront Fusion templates
description: When you create a template, your template becomes available for all your team members. If you want to share the template with someone outside of your team, you must publish it first.
---

# Publish and share *Adobe Workfront Fusion* templates

When you create a template, your template becomes available for all your team members. If you want to share the template with someone outside of your team, you must publish it first.

For information on creating a template, see [Create new templates in Adobe Workfront Fusion](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p><em>Pro</em> or higher</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
    <td> <p>Plan, Work</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront Fusion</em> license**</td> 
   <td> <p><em>Workfront Fusion for Work Automation and Integration</em> </p> <draft-comment>
     <p data-mc-conditions="SnippetConditions.HIDE"><em>Workfront Fusion for Work Automation</em> </p>
    </draft-comment><p data-mc-conditions="SnippetConditions.HIDE"><em>Workfront Fusion for Work Automation</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <em>Adobe Workfront Fusion</em> as well as <em>Adobe Workfront</em> to use functionality described in this article.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

&#42;&#42;For information on *Adobe Workfront Fusion* licenses, see [Adobe Workfront Fusion licenses](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

A template must be created before it can be shared.

## Publish an *Adobe Workfront Fusion* template

1. In the left navigation panel, click `Templates`.
1. Click the `Team templates` tab.
1. Click the name of your template.
1. Click the `Publish` button in the upper-right corner of the screen.

## Share a *Workfront Fusion* template

After you have published a template, you can share it.

<ol> 
 <li value="1"> <p>(Conditional) If you want a shareable link, click <span class="bold">Share public link</span>. </p> <note type="note">
   You can share this link with anyone you want. The template itself stays in the Team templates tab and is not public.
  </note> </li> 
 <li value="2"> <p>(Conditional) If you want the template to become public, send it to your administrator for approval by clicking Request Approval.</p> <note type="note"> 
   <ul> 
    <li> <p>Once the template is approved, it becomes public. Public templates are visible for all <em>Workfront Fusion</em>users, regardless of the organization or the team, in the Public templates tab. </p> </li> 
    <li> <p>Your administrator is not notified about receiving the template to review by email. If the approval is urgent, contact the administrator directly.</p> </li> 
   </ul> 
  </note> </li> 
</ol>

## Template statuses

You can check the status on your template page under the template name

The following statuses are available:

* `Private`: This template is visible only for the template author and their team.
* `Published`: This template is visible only for the template author and their team. You can send published templates for approval and copy a shareable link.
* `Approved`: This template is visible for all *Workfront Fusion* users in the Public templates tab. You can copy a shareable link by clicking Options in the upper-right corner of the screen.

You can also check the status from the Team templates tab. If a template is published, it will have an icon to the right of the template name.

* `Eye icon`: The template is published, it is visible only for the team, and the approval request was not sent.
* `Yellow checkmark icon`: The template is published, it is visible only for the team, and the approval request was sent.
* `Green checkmark icon`: The template is published and public. It is visible for any *Workfront Fusion* user in the Public templates tab. It is also still visible in the Team templates tab, and the template author or their team member can still edit it.

Templates without icons have Private status. They are not published and are visible only to the team.
