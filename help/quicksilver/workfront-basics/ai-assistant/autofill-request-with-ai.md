---
title: Auto-fill a request using AI
content-type: reference
description: You can use AI to auto-fill request fields.
author: Becky
feature: Get Started with Workfront
hide: yes
hidefromtoc: yes
exl-id: d053e604-5a28-4fd3-8f89-4467b6e46f02
---
# Auto-fill a request using AI

AI can help you auto-fill request fields. It can suggest field values based on previous requests, or parse them from text such as emails. 

You can approve or reject these submissions before submitting the request.

Auto-fill does not overwrite any fields that you have already filled in.

## Get suggestions when filling out form 

Auto-fill can suggest field values while you are filling out the form. As you enter values into the request fields, Workfront compares those values with previous requests. If the entered value closely correlates with other field values in similar contexts in previous requests, Workfront suggests those values.

For example, if a clinic always uses the same billing code, Workfront would suggest that billing code in the appropriate field when the clinic name is entered.

To use suggestions based on previous requests:

1. Begin creating a request.

   For instructions, see [Create and submit requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Begin filling in fields.

   As you fill in fields, other fields may show suggestions.

1. For each field suggestion, select **Accept** or **Reject** below that field.

   Or

   Select **Accept all** or **Reject all** at the top of the page to accept or reject all suggestions. 

## Get suggestions from a text prompt

Auto-fill can suggest field values based on text such as emails. You paste in a text block, and Workfront processed the text to suggest field values based on the text.

For example, If the email includes "This is due on June 1," and the request form has a field for due date, Workfront would suggest June 1 for that field value.

This type of suggestion also checks previous requests for similar contexts. For example if the prompt mentions that the request is for a certain client, Workfront can locate and enter the billing address for that client automatically, based on previous requests.

You can paste in text to be applied to the entire form, or to a single section of the form.

To use suggestions based on a pasted text prompt:

1. Begin creating a request.

   For instructions, see [Create and submit requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. To apply the text prompt to the entire form, click **Auto-fill with AI** in the upper-right corner of the screen.

   Or

   To apply the text prompt for a single section, click the AI icon ![AI icon](assets/request-prompt-icon.png) next to the section name.

1. Paste the text into the prompt box.
1. Click **Fill the form**.

   Workfront generates suggestions for the form.
1. For each field suggestion, select **Accept** or **Reject** below that field.

   Or

   Select **Accept all** or **Reject all** at the top of the page to accept or reject all suggestions.
