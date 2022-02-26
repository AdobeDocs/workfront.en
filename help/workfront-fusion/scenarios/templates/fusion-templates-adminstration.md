---
filename: fusion-templates-adminstration
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion Templates administration
description: If you are an administrator, you have permission to view, modify, rename, publish, approve, and delete templates created by others. You can perform these actions from the Templates page in the Adobe Workfront Fusion Administration area.
---

# *Adobe Workfront Fusion* Templates administration

If you are an administrator, you have permission to view, modify, rename, publish, approve, and delete templates created by others. You can perform these actions from the Templates page in the *Adobe Workfront Fusion* Administration area.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p><em>Pro</em> or higher</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
    <td> <p>Plan, Work</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront Fusion</em> license**</td> 
   <td> <p><em>Workfront Fusion for Work Automation and Integration</em>,</p> <draft-comment>
     <p data-mc-conditions="SnippetConditions.HIDE"><em>Workfront Fusion for Work Automation</em> </p>
    </draft-comment><p data-mc-conditions="SnippetConditions.HIDE"><em>Workfront Fusion for Work Automation</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <em>Adobe Workfront Fusion</em> as well as <em>Adobe Workfront</em> to use functionality described in this article.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <p>You must be a <em>Workfront Fusion</em> administrator for your organization.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a <em>Workfront Fusion</em> administrator for your organization.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**For information on <em>Adobe Workfront Fusion</em> licenses, see <a href="../../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">Adobe Workfront Fusion licenses</a></p>
-->

&#42;&#42;For information on *Adobe Workfront Fusion* licenses, see [Adobe Workfront Fusion licenses](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## View *Workfront Fusion* templates as an administrator

To view a table of all created templates and their statuses:

1. Click `Administration`in the left navigation panel to open the Administration area.
1. Click `Templates`in the left navigation panel.

There are three columns related to the templates publication status. A checkmark in a column indicates the following:

* `Published`: These templates are currently visible in the Team templates tab in the user interface.
* `Requested approval`: These templates are waiting for your approval. They are currently visible in the Team templates tab in the user interface.
* `Approved`: These templates have been approved. They are currently visible in the Public templates tab in the standard user interface.

>[!NOTE]
>
>Templates with the checkmark in both the Requested approval column and in the Approved column have been already approved and made public, but there is a newer version of them waiting for your approval.

## Edit *Workfront Fusion* templates as an administrator

1. Click `Administration`in the left navigation panel to open the Administration area.
1. Click `Templates`in the left navigation panel.
1. Click `Detail`to the right of the template you want to edit.

You can now edit the template, similar to editing a template as a non-admin user. However, in the Options in the top-right corner, there is one additional option - the SVG diagram that provides you with the SVG code. Also, the publishing process is the same as in the case of a standard user, refer to the Publishing and sharing templates section for more details.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To view the SVG&nbsp;code of the template, click Options in the upper-right corner and select SVG.</p>
-->

To view the SVG&nbsp;code of the template, click Options in the upper-right corner and select SVG.

For information about specific template options that you can edit, see [Create new templates in Adobe Workfront Fusion](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

For information about publishing templates, see [Publish and share Adobe Workfront Fusion templates](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## Approve or disapprove *Workfront Fusion* templates

Approving a template makes it visible in the Public templates tab and available to all users. Disapproving a template removes it from the Public templates tab and makes it available only to the team that created it.

1. Click `Administration`in the left navigation panel to open the Administration area.
1. Click `Templates`in the left navigation panel.
1. If you want to approve a template, click `Approve`to the right of the template.
1. If you want to disapprove a template, click `Disapprove`to the right of the template.

>[!NOTE]
>
>If you are approving the template that was previously approved and then edited, your second approval will overwrite the original template.

## Clone a scenario as a template

As an administrator, you have the ability to clone a scenario as a template.

For instructions on cloning a scenario as a template, see [Create new templates in Adobe Workfront Fusion](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create)in [Create new templates in Adobe Workfront Fusion](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
