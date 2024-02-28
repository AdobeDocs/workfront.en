---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Generate a module using AI 
description: You can enter a text prompt to create an HTTP module configured to the prompt.
author: Becky
feature: Workfront Fusion
---
# Generate a module using AI 

You can use AI to enter a text prompt describing what you need a module to do. Fusion will then generate an HTTP module that will connect to the correct endpoint of the desired API.

As with anything generated from AI, we recommend that you double check and test the generated module to ensure that it is performing as intended.

## Currently supported AI module applications

The Fusion AI can currently generate modules that connect to the following applciations:

* Adobe Maestro
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

## Generate a module

1. Add a module and select **Generate with AI** from the list of applications.

   Or

   Right click on a blank area of the scenario editor, then select **Generate with AI**.
1. Enter a text prompt into the box. 

   For tips on prompts, see [Tips for creating text prompts](#tips-for-creating-text-prompts) in this article.
1. Add your API token for the application into the module. 
1. Check the module to ensure that it appears to be configured for the appropriate application and action.
1. (Conditional) If the module is not attached to your scenario, drag it into place.

We recommend testing the module to ensure that the generated module is performing as intended.

## Tips for creating text prompts

Text prompts should include the following information at a minimum:

* The application that you are connecting to
* The action that you want to perform

>[!INFO]
>
>**Examples**:
>
>* `Retrieve a list of my calendars from Google Calendar`
>
>   This includes the application `Google Calendar` and the action `Retrieve a list of my calendars`.
>
>* `Retrieve popular songs from Spotify`
>
>   This includes the application `Spotify` and the action `Retrieve popular songs`.

Consider the following when creating text prompts:

* Because each Fusion module performs a single action, your text prompt should describe one specific action. 
* Use direct, simple language.
* Check and test your module. If it does not perform as expected, refine your prompt and try again.



