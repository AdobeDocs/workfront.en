

# `Workfront Tools for AEM User Guide : Content Fragments`

This workflow step will allow a user to map *Adobe Workfront* metadata fields to an AEM Content Fragment Model.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p><em>Pro</em> or higher</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
    <td> <p><em>Review</em> or higher</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Review</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>You must have a license to Adobe Experience Manager</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Prerequisites

* You must install Workfront Tools for Adobe Experience Manager before you can use it to map metadata.

  For instructions, see [Workfront Tools for AEM User Guide: Installation Guide 1.x.x](../../workfront-integrations-and-apps/workfront-integration-for-aem/installation-guide.md)

## Create the event subscription

<ol> 
 <li value="1"> <p>Navigate to <span class="uitext">Tools → Cloud Services → Workfront Tools Configuration</span>. Select the configuration and click <span class="uitext">Properties</span>.<br></p> <p> <img src="assets/tools-config-350x280.png" style="width: 350;height: 280;"> </p> <p> <img src="assets/wf-tools-350x286.png" style="width: 350;height: 286;"> </p> </li> 
 <li value="2"> <p>Select the <span class="uitext">Event Subscriptions</span> tab. Under the <span class="uitext">Create a new event subscription</span> menu, select <span class="uitext">update </span>from the Event dropdown and under the Object dropdown select <span class="uitext">task </span>if you want to create content fragments from a task custom form or select <span class="uitext">issue </span>if you want to create content fragments from an issue custom form.</p> <p> <img src="assets/event-sub--objects-350x254.png" style="width: 350;height: 254;"> </p> </li> 
 <li value="3"> <p>Next, navigate back to <span class="uitext">Tools → Assets → Content Fragment Models</span>. Select an existing Content Fragment Model or create a new model.</p> <p> <img src="assets/contelt-frag-models-350x297.png" style="width: 350;height: 297;"> </p> </li> 
 <li value="4"> <p>Select an existing data field or add a new field. With the field selected, navigate to the <em>Workfront</em> Custom Form Field drop-down menu and select the custom form field you’d like to map.</p> <p> <img src="assets/form-example-350x286.png" style="width: 350;height: 286;"> </p> </li> 
 <li value="5"> <p>After you’ve mapped your desired fields, return to the <span class="uitext">Tools → Cloud Services → Workfront Tools Configuration</span>.</p> <p> <img src="assets/tools-config-350x280.png" style="width: 350;height: 280;"> </p> </li> 
</ol>

