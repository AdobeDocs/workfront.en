---
filename: example-connect-email-text-parser-gsheets
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Scenario example: Connect email, Text Parser, and Google Sheets
description: This scenario helps you create a log of all email messages and tag them for further action in a spreadsheet. It captures an email body in two separate tables in a spreadsheet using Regular Expressions (Regex) as search patterns. The first pattern searches for a phrase and the second searches for the same phrase and an email address.
---

# Scenario example: Connect email, Text Parser, and Google Sheets

This scenario helps you create a log of all email messages and tag them for further action in a spreadsheet. It captures an email body in two separate tables in a spreadsheet using Regular Expressions (Regex) as search patterns. The first pattern searches for a phrase and the second searches for the same phrase and an email address.

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p><span>Pro</span> or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront Fusion</span> license**</td> 
   <td> <p><span>Workfront Fusion for Work Automation and Integration</span> </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <span>Adobe Workfront Fusion</span> as well as <span>Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

&#42;&#42;For information on `Adobe Workfront Fusion` licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

This tutorial requires basic knowledge of regular expressions. To learn about Regex, visit [https://regexone.com](https://regexone.com/).

## Task 1: Add the first module and configure it

<ol> 
 <li value="1"> <p>Search for Email and choose <span class="bold">Watch emails</span> as the Trigger.</p> <note type="note">
   While you can connect a Google account using the Email module, you can also use the inbuilt Gmail module instead.
  </note> </li> 
 <li value="2">Connect either a Google account or any other IMAP based email client (such as Outlook). </li> 
 <li value="3">Once connected, select a Folder whose incoming emails you want to watch, such as Inbox.</li> 
 <li value="4"> <p>Under Criteria, choose All email (or narrow it down to read or unread emails).</p> <p>You can also choose to mark fetched emails as read or unread.</p> </li> 
 <li value="5"> <p>Set the Maximum number of results to 1.</p> <p> <img src="assets/save-max-as-1-350x304.png" style="width: 350;height: 304;"> </p> <p>You can change this based on the volume of messages you receive. However, it’s recommended to set a low value and run the scenario more often.</p> </li> 
 <li value="6"> <p>Now click <span class="bold">Show advanced settings</span> at the bottom to see these filters:</p> <p> <img src="assets/show-adv-settings-350x332.png" style="width: 350;height: 332;"> </p> </li> 
 <li value="7"> <p>Filter emails by the Sender address, Subject and Phrase.</p> <p>This gives you the ability to watch only relevant emails. In this example, we have added only a Subject filter and left the other 2 blank.</p> <note type="note">
   We will add a router to look for phrases in an email using the Match Pattern iterator and a Regular Expression (Regex) as a search pattern. This also enables us to build a multi-utility scenario.
  </note> </li> 
 <li value="8"> <p>Once the configuration is done, and you are prompted to specify where to start watching your emails, click <span class="bold">From now on</span>.</p> <p> <img src="assets/from-now-on-350x236.png" style="width: 350;height: 236;"> </p> </li> 
 <li value="9">Continue to <a href="#search" class="MCXref xref">Task 2: Search for Flow Control and add a Router</a></li> 
</ol>

## Task 2: Search for Flow Control and add a Router

<ol> 
 <li value="1"> <p>Add a router after any module to split or duplicate the data before sending it to the next module. </p> <p>Here, we have used a Router to send the Email body text to 2 separate tables in a Google Sheet. More on that in the next step.</p> <p> <img src="assets/search-for-flow-control-350x220.png" style="width: 350;height: 220;"> </p> </li> 
</ol>

## Task 3: Use the Text Parser Module

<ol> 
 <li value="1"> <p> Add a Match Pattern transformer to search for a phrase in an email. </p> <p>We will search for the phrase “text parser module” in all incoming emails to capture the body text and sender’s name of the ones that match that phrase.</p> 
  <ol> 
   <li value="1"> <p>Write the Pattern as a Regular Expression:</p> <p>text\sparser\smodule</p> </li> 
   <li value="2"> <p>(Optional) Use any of the other Patter options. </p> <p> <img src="assets/pattern-350x318.png" style="width: 350;height: 318;"> </p> <p>Multiline is useful if your text contains several lines and you need to search for the pattern in each line. For this tutorial we need to search for the pattern in the entire email body text, hence we will leave it unchecked.</p> </li> 
   <li value="3"> <p>In the Text field, click the attribute <span class="bold">Text content</span> in the list. </p> <p> <img src="assets/text-content-350x264.png" style="width: 350;height: 264;"> </p> <p>This is the attribute that stores the text from the email body in which we will search for the pattern.</p> </li> 
  </ol> </li> 
 <li value="2"> <p>Add another Match Pattern that searches for the same phrase and an email address. </p> <p>This is particularly useful if you have customer accounts with multiple users. To save time, you can clone the Text Parser module you just created and link it to the Router.</p> <p> <img src="assets/clone.png"> </p> </li> 
 <li value="3"> <p>Now edit the pattern as follows:</p> <p>text\sparser\smodule.+\s([\w.-]+@[\w.-]+)</p> <p> <img src="assets/text-parser-350x202.png" style="width: 350;height: 202;"> </p> <p>This pattern searches for the phrase “text parser module” and an email address like jim.morrison@gmail.com and returns only the email address.</p> <note type="note">
   While it’s important to write your regex in accordance with the specification of the email addresses you accept, the one above takes care of most standard email addresses.
  </note> 
  <ul> 
   <li> <p>If you’d like to search only for email address, you can use the regex below:</p> <p>([\w.-]+@[\w.-]+)</p> </li> 
   <li> <p>You may also search only for phone numbers using the regex below:</p> <p>^[+]?\(?(\d{1,3})\)?[\s-]?\(?(\d{3})\)?[\s-]?\d{3}[\s-]?\d{3,4}</p> </li> 
  </ul> <p>The above pattern covers most common formats in which a phone number is written.</p> <p>To test your patterns, we recommend using <a href="https://regex101.com/">https://regex101.com</a> with javascript as the Flavor.</p> <p>The rest of the configuration remains the same as the one before.</p> </li> 
</ol>

## Task 4: Add the Google Sheets modules

Instead of Google Sheets, you can use another app like Airtable or a CRM such as InfusionSoft. For Sheets, we need to first create a spreadsheet with the requisite headers.

<ol> 
 <li value="1"> <p>Create a spreadsheet with the columns under which you’d like to capture the user data. (Feel free to use an existing file too).</p> <p>For example, create one called “Email Data: Support Ticket” with Sender Name, Sender Email and Email Content as columns. Name the worksheet "contains: text parser module."</p> </li> 
 <li value="2"> <p>Add the Google Sheets module with <span class="bold">Add a row</span> as the action.</p> <p> <img src="assets/add-a-row-350x174.png" style="width: 350;height: 174;"> </p> </li> 
 <li value="3"> <p>Connect your Google account (if you haven’t already). Choose the File you created earlier, followed by choosing the Worksheet in which you’re capturing the data. </p> <p>Your setup should look like this:</p> <p> <img src="assets/connect-google-acct-350x279.png" style="width: 350;height: 279;"> </p> </li> 
 <li value="4"> <p>Map the attributes in the relevant fields (columns) to finish the module setup.</p> <p> <img src="assets/map-attributes-350x282.png" style="width: 350;height: 282;"> </p> </li> 
 <li value="5">Clone the module you just created and link it to the second Text Parser module.
  <ol>
   <li value="1"><p>Go to your Spreadsheet, duplicate the worksheet you created earlier and give it a name. </p><p>For example, name it "contains: text parser module and email."</p></li>
   <li value="2"><p>Add another column to store the email address that the email body contains. </p><p>For example, name it "Email Address Shared."</p></li>
   <li value="3">Click the cloned Google Sheets module to configure the setup.</li>
   <li value="4">Change the worksheet to the new one you just created.</li>
   <li value="5"><p>Map the output from the Match Pattern module ($1) to the column where you want to store the email address (Email Address Shared).</p><p><img src="assets/map-the-output.png"></p><p><img src="assets/sender-name-350x411.png" style="width: 350;height: 411;"></p></li>
   <li value="6"><p>Click <span class="bold">OK</span>, save the scenario, and take it for a test run.</p><p>You will need to send two separate emails to the connected email address as follows:</p>
    <ul>
     <li><p>Containing the phrase “text parser module” (and no email address)</p><p><img src="assets/text-parser-module-350x103.png" style="width: 350;height: 103;"></p></li>
     <li><p>Containing the above phrase and an email address</p><p><img src="assets/above-phrase-and-email-350x106.png" style="width: 350;height: 106;"></p><p>If there are no errors in your setup, you will see that the first worksheet captures all emails containing the phrase “text parser module” while the second worksheet captures only those that contain the phrase “text parser module” and an email address. You may refer to the screenshots below.</p><p>Worksheet 1:</p><p><img src="assets/worksheet-1-350x57.png" style="width: 350;height: 57;"></p><p>Worksheet 2:</p><p><img src="assets/worksheet-2-350x41.png" style="width: 350;height: 41;"></p></li>
    </ul></li>
  </ol></li> 
</ol>

## Resources

* [Free exercises](https://regexone.com/) to learn about Regular Expressions
* [Learn about Phone Number Matching](https://regexone.com/problem/matching_phone_numbers) using Regex
* [Learn about Email Matching](https://regexone.com/problem/matching_emails) using Regex
* [Test your Regular Expressions](https://regex101.com/)

