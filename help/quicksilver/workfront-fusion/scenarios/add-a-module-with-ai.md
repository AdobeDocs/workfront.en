---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Add a module to a scenario using AI 
description: You can enter a text prompt to create an HTTP module configured to the prompt.
author: Becky
feature: Workfront Fusion
---
# Add a module to a scenario using AI 

You can use AI to enter a text prompt describing what you need a module to do. Fusion will then generate an HTTP module that will connect to the correct endpoint of the desired API.

As with anything generated from AI, we recommend that you double check and test the generated module to ensure that it is performing as intended.

## Generate a module using AI

1. Add a module and select **Generate with AI** from the list of applications.

   Or

   Right click on a black area of the scenario editor, then select **Generate with AI**.
1. Enter a text prompt into the box. 

   For tips on prompts, see [] in this article.

1. (Conditional) If the module is not attached to your scenario, drag it into place.

1. Check the module to ensure that it appears to be configured for the appropriate application and action.


We recommend testing the module to ensure that it is performing as intended.

## Tips for creating text prompts

Text prompts should include the following information:

* The application that you are connecting to
* The action that you want to perform

>[!INFO]
>
>**Examples**:
>
>* `Get a list of my calendars from Google Calendar`
>
>   This includes the application `Google Calendar` and the action `Get a list of my calendars`.
>
>* `Get popular videos from YouTube`
>
>   This includes the application `YouTube` and the action `Get popular videos`.





