---
filename: set-up-taxonomy-metadata
product: workfront-library
product-area: documents
navigation-topic: metadata
title: Set up taxonomy metadata for Workfront Library
description: As a Workfront Library administrator, you can set up your organization's taxonomy to gather the information your users search for and to track content. For more information about the different types of taxonomy you can collect, see Overview of taxonomy metadata in Workfront Library.
---

# Set up taxonomy metadata for *Workfront Library*

As a *Workfront Library administrator*, you can set up your organization's taxonomy to gather the information your users search for and to track content. For more information about the different types of taxonomy you can collect, see [Overview of taxonomy metadata in Workfront Library](../../../workfront-library/administration-and-setup/metadata/taxonomy-metadata-overview.md).

<ol> 
 <li value="1"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In <em>Workfront</em>, click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png">, then select <span class="bold">Library</span> to open <em>Workfront Library</em> in a new browser tab.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In <em>Workfront</em>, click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png">, then select <span class="bold">Library</span> to open <em>Workfront Library</em> in a new browser tab.</p> </li> 
 <li value="2"> <p>In the upper-left corner of <em>Workfront Library</em>, click the <span class="bold">Menu</span> icon <img src="assets/library-menu-icon.png">.</p> </li> 
 <li value="3"> <p>In the left panel, click <span class="bold">Setup</span> > <span class="bold">Taxonomy</span>.</p> </li> 
 <li value="4"> <p>Click <span class="bold">Add Field</span>, then select the type of field you want to add to your taxonomy.</p> <p>You can choose from the following field types:</p> 
  <ul> 
   <li>Custom</li> 
   <li>Attribute</li> 
   <li>EXIF</li> 
   <li>XMP</li> 
  </ul> </li> 
</ol>

### Custom

Use custom taxonomy to gather information tailored to your organization, such as campaign, department, or location.

<ol> 
 <li value="1"> <p>In the <span class="bold">Field Type</span> drop-down list, select the type of field you want to configure.</p> <p>You can choose from the following field types:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Date</td> 
     <td>Allows users to manually enter a date or select a date from a date picker</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Multi-select</td> 
     <td>Lists multiple options in a picklist from which users can choose several options</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Single-select</td> 
     <td>Lists multiple options in a picklist from which users can choose one option</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Text field</td> 
     <td>Allows users to freely enter<draft-comment>
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         up to X characters of [FOLLOW&nbsp;UP&nbsp;WITH&nbsp;CLINT]
       </MadCap:conditionalText>
      </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        up to X characters of [FOLLOW&nbsp;UP&nbsp;WITH&nbsp;CLINT]
      </MadCap:conditionalText> text</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="2"> <p>(Conditional) If you are configuring a multi- or single-select custom field, enter the <span class="bold">Value</span> and press <span class="bold">Enter</span>. You can list up to 100 different values in the picklist with names. These names can be up to 50 characters.</p> </li> 
 <li value="3"> <p>(Optional) To require users to complete this field when entering metadata, enable&nbsp;<span class="bold">Required Field</span>.</p> </li> 
 <li value="4"> <p>Click <span class="bold">Save</span>.</p> <p>The custom field is added to the taxonomy.</p> </li> 
</ol>

### Attribute

The metadata for attribute fields is derived from the device or application used to create the content.

1. In the `Name`&nbsp;drop-down menu, choose the attribute you want to add to the taxonomy.

   You can choose from the following attributes:

  * File Extension
  * Size
  * Modified Date
  * Created Date

1. Click `Save`.

### EXIF

Although some asset files contain large amounts of EXIF metadata, you can configure your taxonomy to collect only the EXIF metadata you need.&nbsp;If at a later date you decide to collect additional EXIF metadata, simply add the appropriate EXIF field to your taxonomy. *Workfront Library* then updates the EXIF metadata for all content embedded with the appropriate EXIF metadata.

To learn about the EXIF metadata that *Workfront Library* supports, see [Overview of taxonomy field types](../../../workfront-library/administration-and-setup/metadata/taxonomy-field-types-overview.md).

1. In the `EXIF Field` box, begin typing the EXIF tag you want to capture and select the tag when it displays in the drop-down list.
1. In the `Custom Label` box, enter a unique name for the field.  
   The field name becomes the label that displays in the Details panel for content.
1. Click `Save`.

### XMP

You can configure XMP taxonomy fields to embed specific types of metadata to content when it is uploaded to *Workfront Library*.

To learn about the XMP metadata that *Workfront Library* supports, see [Overview of taxonomy field types](../../../workfront-library/administration-and-setup/metadata/taxonomy-field-types-overview.md).

<ol> 
 <li value="1"> <p>In the <span class="bold">XMP Field</span>&nbsp;box, begin typing the XMP tag you want to capture in the taxonomy and select the tag when it displays in the drop-down list.</p> <note type="note">
   If your organization has not yet uploaded content to 
   <em>Workfront Library</em>, no options display in the XMP Field drop-down list. After you upload some content files with XMP data, 
   <em>Workfront Library</em> begins to recognize the type of XMP data your organization uses and lists the applicable XMP tags in the XMP Field drop-down list.
  </note> </li> 
 <li value="2"> <p>In the <span class="bold">Custom Label</span> box, enter a label for the field.</p> <p>The field name becomes the label that displays in the Details panel for content. </p> </li> 
 <li value="3"> <p>Click <span class="bold">Save</span>.</p> </li> 
</ol>

