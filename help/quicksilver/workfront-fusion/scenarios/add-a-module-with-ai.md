---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Generate a scenario segment using AI
description: You can enter a text prompt to create an HTTP module configured to the prompt.
author: Becky
feature: Workfront Fusion
hide: yes
hidefromtoc: yes
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
---
# Generate a scenario segment using AI 

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>Because this feature is in Beta, it is available only to some Workfront users.

You can use AI to enter a text prompt describing what you need a section of your scenario to do. Fusion will then generate modules that will perform those actions, which you can use in your scenario.

As with anything generated from AI, we recommend that you double check and test the generated modules to ensure that they are  performing as intended.

## Currently supported AI module applications

The Fusion AI can currently generate modules that connect to the following applications:

* Adobe Firefly
* Azure OpenAI
* Microsoft Graph 
* Adobe Workfront Planning
* Adobe Analytics
* Adobe PDF Services
* Adobe Marketo
* Adobe Frame.io
* Dropbox
* NetSuite
* Google Calendar
* Atlassian Jira
* GitLab
* Spotify
* Bitbucket
* OpenAI
* Slack

## Generate modules

1. Begin adding a module and select **Generate with AI** from the list of applications.

   Or

   Click the Generate with AI icon ![Generate with AI](assets/generate-with-ai-icon-beta.png) near the bottom of the scenario editor page.

     That AI Assistant panel opens.
1. Enter a text prompt into the box. 

   For tips on prompts, see [Tips for creating text prompts](#tips-for-creating-text-prompts) in this article.

   The module or set of modules is generated.
1. (Conditional) If necessary, add your API token for the application into the modules. 
1. Check the modules to ensure that they are to be configured for the appropriate application and action.
1. (Conditional) If the generated scenario section is not attached to your scenario, drag it into place.

We recommend testing the modules to ensure that they are performing as intended.

## Tips for creating text prompts

Text prompts should include the following information at a minimum:

* The application that you are connecting to
* The action or actions that you want to perform

>[!IMPORTANT]
>
>You can generate more than one module at a time, but can only generate modules for one application at a time.  

>[!INFO]
>
>**Examples**:
>
>* `Delete the records 'xyz-123', 'xyz-456', 'xyz-789' from Adobe Workfront Planning`
>This includes the application `Workfront Planning` and the action `delete records`. This prompt creates three modules, one for each record that will be deleted.
>* `Change campaign summary of the record 'xyz-123' from Adobe Workfront Planning`
>This includes the application `Workfront Planning` and the action `change campaign summary`.
>* `Get all field details in the record type with ID 'test-record' from Adobe Workfront Planning`
>This includes the application `Workfront Planning` and the action `get field details`.
>
>The following example is NOT correct:
>
>* `Generate an image in Adobe Firefly and upload it to Dropbox`
>
>    This example is incorrect because it includes more than one application

Consider the following when creating text prompts:

* Use direct, simple language.
* Check and test your modules. If it does not perform as expected, refine your prompt and try again.
