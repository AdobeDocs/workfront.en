---
content-type: reference
navigation-topic: announcements
title: TLS 1.2 to be required in Adobe Workfront
description: In order to provide optimal security, Adobe Workfront is requiring that all browser connections and API integrations that rely on TLS 1.0 or earlier be upgraded to use TLS 1.2. In the Preview environment, TLS 1.0 is already disabled.
author: Luke
feature: Product Announcements
---

# TLS 1.2 to be required in Adobe Workfront

In order to provide optimal security, Adobe Workfront is&nbsp;requiring that all browser connections and API integrations that rely on TLS 1.0 or earlier be upgraded to use TLS 1.2.&nbsp;In the Preview environment, TLS 1.0 is already disabled.

Workfront officially ended support for TLS 1.0 in March&nbsp;2018. All integrations leveraging TLS 1.0 ceased to function as of January 9, 2019.&nbsp; TLS 1.1 will be disabled in Q4 of 2019.

The following sections provide more detail about these important milestones, as well as how you can prepare for this upgrade in your organization:

## Workfront ends official support of TLS 1.0 (March 5, 2018)

Workfront ended official support for TLS 1.0 in March 2018.

Browser connections and API integrations that leverage TLS 1.0 are still operational, but Workfront will not solve issues in the Workfront application that are related to TLS 1.0.

## Workfront integrations using TLS 1.0 disabled (January 9, 2019)

On January 9, 2019, all Workfront browser connections and API integrations that leverage TLS 1.0 must be upgraded to use TLS 1.1 or later. Browser connections and API integrations that continue leveraging TLS 1.0 (either inbound or outbound connections) will no longer be able to communicate with the Workfront application after this time.&nbsp;

## TLS 1.1 to be disabled in Q4 2019

In the Production environment, TLS 1.1 was disabled on October 21, 2019. After this time, all integrations using TLS 1.1 will no longer function.

This change will go into effect in the Preview and Sandbox environments on August 7 to help organizations prepare for the shut-off.

## Preparing for the TLS upgrade

* [When accessing Workfront via the browser](#when-accessing-workfront-via-the-browser) 
* [When connecting to Workfront via the API](#when-connecting-to-workfront-via-the-api)

### When accessing Workfront via the browser {#when-accessing-workfront-via-the-browser}

Ensure that users in your organization are accessing Workfront via a supported browser.&nbsp;(For information about supported browsers, see [Adobe Workfront browser requirements](../../workfront-basics/workfront-browser-requirements.md).)

All browsers supported by Workfront are compatible&nbsp;with TLS 1.2.

### When connecting to Workfront via the API {#when-connecting-to-workfront-via-the-api}

If you are integrating third-party applications to Workfront via the API (either inbound or outbound), ensure that TLS 1.2 (and the TLS 1.2 encryption protocols) are enabled in your integrations.
