---
filename: text-parser-troubleshooting
content-type: tips-tricks-troubleshooting
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Text parser troubleshooting
description: Use this information if you can not get text parser to produce any output.
---

# Text parser troubleshooting

Use this information if you can not get text parser to produce any output.

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Troubleshooting

Case scenario example, you would like to parse the filetype of a file document "filename.docx" and the extension of the filename always varies from DOCX to PDF to CSV.

The expression that you may choose to use in this case is \..+

If you were to use this on regex expression on regex101.com you will rightly find that you will get a full match.

![](assets/regex-expression-350x130.png)

As you will notice on the image above, the file extension was correctly matched. If you take this and try to implement it in your text parser:

![](assets/text-parser-350x602.png)

you will not get a match:

![](assets/text-parser-you-don't-get-a-match-350x365.png)

The reason for this is that the "i" shows only the number of matches per match so in this case, we have 2 matches henceforth after the "i" there is a numerical value 1 and 2. The use case for this is that should you ever need to match or pass data through a filter only the second matched value you can specify which value that is represented by the numerical value.

![](assets/text-parser-matches-350x355.png)

To be able to get the match values that you require to add brackets to the part that you want to parse (for example, to extract from "filename.docx" - "docx" only), then, according to the regex expression we are using for this case scenario, the brackets should be applied on \.(.+)

This captures the DOCX, places it in a group, and leave the "." out of it.

![](assets/text-parser-get-matches-350x592.png)

The output shown in the picture below, you will notice that the capturing group will match any character (except for line terminators)

![](assets/text-parser-output-350x389.png)

Another workaround that also incorporates regex is using the replace function

{{replace("abcdefghijklmno pqr stuvw xyz.docx"; "/.&#42;\./"; ".")}}

Then replace abcdefghijklmno pqr stuvw xyz.docx with your actual filename variable.
