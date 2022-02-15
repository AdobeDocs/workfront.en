---
filename: item-data-types
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
---



# Item data types {#item-data-types}



## Access requirements {#access-requirements}

You must have the following access to use the functionality in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> license**</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFFusionIntegration variable varname">Workfront Fusion for Work Automation and Integration</span> </p> <p data-mc-conditions="SnippetConditions.HIDE"><span class="mc-variable WFVariables.WFFusionAutomation variable varname">Workfront Fusion for Work Automation</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Your organization must purchase <span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> as well as <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Item data types {#item-data-types-1}

You can contain the types of items listed below in a bundle.


For information on which types of items *`Workfront Fusion`* allows for conversion between one other, see [Type coercion](type-coercion.md).

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p><a name="Text"></a>Text</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The most common item type. For some text items, <span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> checks whether the maximum or minimum allowed length is met or whether the item performs format validation (email, URL or file name).</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>Number</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>For some numerical items, <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span> may validate the input for a specified range (the minimum or maximum allowed value).</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Boolean (Yes/No)</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>This type is used for items with only two possible values: true or false. </p> <p>When setting modules, the Boolean type can appear in two different forms:</p> 
    <ul> 
     <li> <p>The compulsory check box is shown in case the field is mandatory and must be filled in.</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>Optional fields that can be left blank are displayed as a selection box, allowing selection among three values: <code>Yes</code>, <code>No</code>, and <code>Not defined</code> (default).</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>You can click <span class="bold">Map</span> if you need to map the value to an item from another module.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p><a name="Date"></a>Date</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Dates are entered in the ISO 8601 date format, for example, <code>2015-09-18T11:58Z</code>. You can change the time zone in your profile settings, as explained in <a href="change-profile-settings.md" class="MCXref xref">Change profile settings</a>. </p> <p>If you click a field that requires a date, a pop-up calendar displays in the module settings. The time is not required for some items.</p> <p>Values of Date items are formatted using the local and Web timezone selected in your profile. You can display the ISO 8601 version of a date item's value by hovering over the item.</p> <p>Note: If the ISO value does not display, the item is probably text, not a date.</p> <p>The time is entered in the <code>hours:minutes:seconds</code> format, for example,<code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Buffer (binary data)</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>File content is usually sent as Buffer type content (image content, video file, and others). In some cases, text data is included in this type (for example, a text file). <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span> is able to automatically convert text data in binary code to text and text to text data in binary code. For more information, see <a href="about-mapping-files.md" class="MCXref xref">About mapping files</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>Collection</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>A collection is an item consisting of multiple sub-items. The Sender item in an email message is an example of a collection: it contains the sender name (text type) and the sender email address (text type).</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Select (menu)</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>When you configure the module settings as described in <a href="configure-a-modules-settings.md" class="MCXref xref">Configure a module's settings</a>, you can select from several items of the same type. An example is the folder select menu in the settings for the Dropbox modules. </p> <p>When setting modules, the select menu can appear in two forms:</p> <p> <p>If multiple selection is possible, several items with check boxes display.</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>If only one option is possible, a drop-down menu displays.</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>If you need to map an item from another module, use the <span class="bold">Map</span> button. This button opens a text field instead of the selection menu. For more information, see <a href="map-information-between-modules.md" class="MCXref xref">Map information from one module to another</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>Array</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>You can use the array type to work with several values of the same type, including collections. An example is the Email modules:&nbsp;they return an array of attachments and each attachment contains name, content, size, and so on. For more information, see <a href="map-an-array.md" class="MCXref xref">Map an array</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"> <p>Validation</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p><span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span> might perform validation on each type of item. If an item does not pass the validation, the module will stop processing because of a data error. For more information, see <a href="error-processing.md" class="MCXref xref">Error processing</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

