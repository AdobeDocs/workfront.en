---
title: First Quarter 2027 release overview
description: This page provides information about functionality that is included in the First Quarter 2027 release. These enhancements are planned to become available in the Production environment throughout the quarter.
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
---

# First Quarter 2027 release overview

This page provides information about functionality that is included in the First Quarter 2027 release scheduled for January 2027.

The enhancements on this page are available in the Preview environment. This page will be updated with additional enhancements as the First Quarter 2027 release nears its planned Production release.

>[!IMPORTANT]
>
>
>Monthly and quarterly releases are planned to be available on the Thursday of the second full week of the month, unless otherwise specified.
>
>|Monthly release|Quarterly release|
>|----|----|
>|<ul><li>2026.11 (November 12, 2026)</li><li>2026.12 (December 17, 2026)</li><li>2027.01 (January 21, 2027)</li></ul>|<ul><li>2027.01 (January 21, 2027)</li></ul>|
>
>For more information on the fast release process, see [Enable or disable the fast release process](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront enhancements

* [Project enhancements](#project-enhancements)


### Project enhancements

<table>
    <tbody>
        <tr>
            <td><strong>Feature</strong>
            </td>
            <td><strong>Preview</strong></td>
            <td><strong>Fast release</strong></td>
            <td><strong>Quarterly</strong></td>
        </tr>
        <tr>
            <td>
                <p><a href="/help/quicksilver/product-announcements/product-releases/27-q1-release-activity/27-q1-projects.md">Pin threads to the top of updates</a></p>
                <p>You can now pin the most important threads at the top of the Updates area on a project, task, issue, or request so that key information stays visible for your team.</p>
            </td>
            <td><p>October 15, 2026</p></td>
            <td><p>November 12, 2026</p></td>
            <td><p>January 21, 2027</p></td>
        </tr>
    </tbody>
</table>

## Release notes for other areas

* [Adobe Workfront Fusion release activity](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).
* [Adobe Workfront Planning release activity](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

There are no updates for the following at this point in the release:

* Scenario Planner
* Proof
* Goals

## Announcements

### Deprecation of legacy billing and cost rate fields in job role list views

Over time, we have introduced enhanced rate management capabilities and dedicated Job Role experiences that provide a more complete and scalable approach to maintaining rate information. As a result, rate administration is moving toward these dedicated experiences rather than list-based management workflows.

With the January 2027 release, the legacy fields **Billing Per Hour** and **Cost Per Hour** will no longer be available in the Workfront API or in Job Role list views, including Filter / View / Grouping configurations (both direct references and text mode calculated columns).

As a replacement in reports, you can use the recommended Text Mode code (use `costRates` or `billingRates` as needed):

    ```
    displayname=Test
    listdelimiter=<br>
    listmethod=nested(costRates).lists
    type=iterate
    valueexpression=CONCAT({startDate}," - ",{endDate},": ",{value})
    valueformat=HTML
    ```

To manage and review job role rates, use the dedicated rate management experiences:

* Access and manage job role rates directly from the Job Role > Rates page.
* Use Rate Reports to review, analyze, and report on rate information across job roles.

No action is required to prepare for the change. However, administrators who currently display **Billing Per Hour** and **Cost Per Hour** fields in Job Role list views should update their workflows to use the recommended rate management experiences described above.

For information on job role rates, see [Create and manage job roles](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

<!--

### Workfront Maintenance Updates

For information about the maintenance updates made during the First Quarter 2027 release, see [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

-->

### Training updates

Explore the latest updates made to learning programs, learning paths, videos, and guides for each Adobe Workfront product release. For more information, see the "What's New" section of the [Workfront Tutorials page](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html).
