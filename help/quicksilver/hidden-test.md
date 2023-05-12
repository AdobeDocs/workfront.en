---
title: Hidden test file
author: Bob
description: Hidden from search and from the left nav
hidefromtoc: yes
hide: yes
exl-id: b6b0f429-b619-4b8e-ab81-ad190dae5a0b
---

# Hidden test file - FEATURE BRANCH TEST

This file is hidden from search (`hide: yes`) and from the left nav (`hidefromtoc: yes`).

<span class="preview">This file is **hidden** from search (`hide: yes`) and from the left nav (`hidefromtoc: yes`).</span>

<p class="preview">This file is **hidden** from search (`hide: yes`) and from the left nav (`hidefromtoc: yes`).</p>

## Image test

![image test](assets/get-started.png){width="50" align="center"}

## Test of preview highlighting

**Use DIV for blocks of components.**

DIV starts below.

<div class="preview">

Start of DIV.

>[!NOTE]
>
>This is a note.
>
>I have a request to highlight the note's background.

![image](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/assets/add-admin-1.png)

Last highlighted item.

</div>

DIV ends above.

**Use SPAN for paragraphs or phrases**

This is a paragraph. <span class="preview">I am yellow text.</span> Remember to close your syntax properly, or the page might render oddly.

DIV and SPAN are also useful in HTML tables.

**Other supported HTML elements**

You can also specify the `class="preview"` syntax in `<p>`, `<td>`, `<tr>`, and so on. Make sure you test on preview.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr class="preview"> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront plan</a>*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"></td> 
   <td> <p class="preview">Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira access</td> 
   <td> <p><span class="preview">System administrator access</p> <p>Important:  We recommend that you create separate system administrator accounts in Jira and Workfront to dedicate to this integration, rather than using existing ones that might be attached to users. </span></p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a Workfront administrator. For information on Workfront administrators, see .</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Video with quality = 12

>[!VIDEO](https://video.tv.adobe.com/v/3413544/?quality=12)

Video with quality = 6

>[!VIDEO](https://video.tv.adobe.com/v/3413544/?quality=6)

Video inside HTML table

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  </tr> 
  <tr> 
   <td role="rowheader">Does this video work?</td> 
   <td>No it does not </td> 
  </tr> 
 </tbody> 
</table>

Video inside markdown table

|Column1|Column2|
|---|---|
|Does this work?|Also no|


