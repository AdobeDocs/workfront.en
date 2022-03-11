---
filename: built-in-vs-api-vs-fusion
content-type: reference
product-area: workfront-integrations
keywords: native,ootb
navigation-topic: workfront-integrations-navigation-topic
title: Adobe Workfront integration methods
description: 
---

# `Adobe Workfront` integration methods

&nbsp;

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

You can integrate `Adobe Workfront` with third-party applications. These integrations can extend the utility of `Workfront` and tailor it to the needs of your organization. You can use any or all of these integrations, depending on which is most useful for a given task.

## Built-in integrations

`Workfront` provides various integrations that you can configure directly from `Workfront`, or from another application by installing the `Workfront` add-in for that application. These built-in integrations cover many common use case scenarios and focus on extending and connecting user experiences for end users.

`Workfront` built-in integrations largely focus on personal productivity and collaboration. These integrations reduce interruptions in an individual user's workflow, allowing them to receive `Workfront` notifications, access information, and act on `Workfront` work items without leaving the integrated application.

Advantages of built-in integrations may include the following:

* Many of these built-in integrations are available at no additional cost. (Others do require an additional purchase.)
* Built-in integrations cover many of the most common apps used by businesses, such as Slack, Google Drive, or Adobe products such as the Adobe Creative Cloud or Adobe Experience Manager Assets. If your company uses these apps already, the integration will go smoothly into your users' existing workflow. 
* Integrating Workfront with a frequently-used application can increase adoption among your users.

` `**Example: **`` With the `Workfront for Microsoft` integration, you can receive notifications in Microsoft Teams about your `Workfront` work items. Without leaving Microsoft Teams, you can perform actions like approving, commenting on, or changing the status of work items. Any changes you make to work items from Microsoft Teams are reflected in `Workfront` as well.
For more information about built-in integrations, including a list of currently available built-in integrations, see [Adobe Workfront built-in integrations overview](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## Custom OAuth2 applications

`Adobe Workfront administrators` can create OAuth2 applications for your instance of `Workfront`, which allow other applications to access `Workfront`. Your users can then give permission to those other applications to access their `Workfront` data. In this way, you can integrate `Workfront` with applications of your choice, including your own in-house applications.

>[!NOTE]
>
>In the context of OAuth2, "creating an app" refers to the process of creating this sort of access link between an app and a server such as `Workfront`.

Advantages of creating an OAuth2 application may include the following:

* Users can use these integrations directly in `Workfront`, similar to built-in integrations.
* Setting up or using an OAuth2 application does not require additional technical knowledge, such as familiarity with the `Workfront` API.
* Your organization may use software that is not offered as a `Workfront` built-in application. You can still integrate this software with `Workfront` by using an OAuth2 application, even if the software is proprietary to your organization.

For more information, see [Create OAuth2 applications for Workfront integrations](../administration-and-setup/configure-integrations/create-oauth-application.md).

## Workfront API

`Workfront` offers a public API (application programming interface) that enables you to extend and enhance your `Workfront` experience. The goal for the `Workfront` API is to simplify building your own integrations with `Workfront` by introducing a REST-ful architecture that operates over HTTP. The `Workfront` API does require some technical knowledge, but it is a very powerful tool for retrieving, creating, and modifying data. You can customize API calls to perform very specific functions.

In addition, `Workfront` offers an Event Subscription API. When an action occurs on a Workfront object that is supported by event subscriptions, you can configure Workfront to send a response to your desired endpoint. This means that third-party applications can receive updates from Workfront interactions via the Workfront API soon after they occur.

Advantages to using the Workfront API may include the following:

* You can use the Workfront API to connect to almost any other web service or app that offers a public API. It is therefore possible to integrate Workfront with nearly any web service or app that you want to use.
* The `Workfront` API's flexibility also extends to your business's proprietary software. You can use and modify `Workfront` data from inside your own software.
* Since APIs are so common to software, your in-house developers are likely familiar with them. `Workfront` uses a REST-ful API, the most common type of API, making it even easier for your developers to come up to speed quickly.

` `**Example: **`` The following API call puts a comment into the update stream of the task with the specified ID.

```
https://<your domain>.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
```

For more information about the Workfront API, see [API basics](../wf-api/general/api-basics.md).

For more information on event subscriptions, see [Event Subscription API](../wf-api/general/event-subs-api.md).

## `Adobe Workfront Fusion`

`Workfront Fusion` allows you to automate workflows across multiple apps and web services, creating scenarios where the apps work together to execute a task. A scenario is a visual representation of the task or workflow that is built using modules, which are discrete tasks like “Download a document” or “Create a project.” You chain modules together to define the workflow, and then the workflow executes automatically when a trigger condition is met.

Advantages to `Workfront Fusion` may include the following:

* `Workfront Fusion` doesn’t require as much technical knowledge as the API because the visual interface aids in understanding and setting up the workflow. This means that it can be used by individuals outside of a development team, which may save your organization time and money.
* Since `Workfront Fusion` works through the API, it can access most apps and web services. Many apps have modules to make API calls, or you can use the HTTP, SOAP, or JSON modules to interact with web services that don’t have a dedicated `Workfront Fusion` connector.

` `**Example: **`` The following Workfront module in `Workfront Fusion` is set up to add a comment to the selected project. After the module is executed, the comment is visible in the update stream of the project in `Workfront`.

![](assets/fusion-example-comment-350x416.png)

For more information about `Workfront Fusion`, see [Adobe Workfront Fusion](../workfront-fusion/workfront-fusion-2.md).
