---
content-type: reference
navigation-topic: get-started-with-workfront
title: HIPAA Readiness for Workfront
description: A Workfront customer who is, as defined in HIPAA, a Business Associate and/or the Covered Entity on whose behalf the Business Associate provides Adobe Workfront should use the following guidelines to configure Workfront for HIPAA-ready use.
feature: Get Started with Workfront
author: Courtney
hide: yes
hidefromtoc: yes
exl-id: e3cdaa03-d523-46a4-954b-8456d5f190e4
---
# HIPAA Readiness for Workfront

A Workfront customer who is, as defined in HIPAA, a Business Associate and/or the Covered Entity on whose behalf the Business Associate provides Adobe Workfront should use the following guidelines to configure Workfront for HIPAA-ready use:


## Password requirements

| **Security Setting** | **What Is It?** | **Requirement** |
|----------------------|------------------|------------------|
| Minimum password strength for agreements | What is the minimum strength for agreement passwords? | No less than 8 characters |
| Minimum password strength for user passwords | What is the minimum strength for users' passwords? | Characters from three of the following categories:<br>* Uppercase letters (Latin alphabet)<br>* Lowercase letters (Latin alphabet)<br>* Base 10 digits<br>* Non-alphanumeric characters |
| Password Duration | How long should passwords be allowed to remain unchanged? | Passwords should be changed at least every 90 days |
| Password History | How many past passwords should be remembered and disallowed? | Not less than 5 |


## Login requirements

| **Security Setting** | **What Is It?** | **Requirement** |
|----------------------|------------------|------------------|
| Maximum Login Failures | How many failed login attempts cause the user to be locked out? | Not more than 5 attempts within a 5-minute period; retry allowed after 30 minutes |
| Maximum SSO Verification Failures | How many failed SSO verification attempts cause a lockout? | Not more than 5 (applies only to customers using SSO) |


## Session requirements

| **Security Setting** | **What Is It?** | **Requirement** |
|----------------------|------------------|------------------|
| Session Timeout | How many minutes of inactivity cause a logout? | Not more than 15 minutes |

## Customer responsibilities

Ensure all that all employees, representatives, and/or agents are aware of and understand the terms in the licensing and/or service agreement(s) signed between the parties, as applicable, relevant to the use of data with Workfront.

In particular, the following responsibilities and obligations should be reviewed and communicated: 

* The customer is responsible for the use of the Workfront Service by all of its users. 

* The customer is required to comply with all terms of its agreement with Adobe that includes prohibited data elements from being uploaded into Workfront. 

* Any sensitive data, including, but not limited to ePHI, is uploaded at the customer's own risk.  The customer is at all times responsible for all customer data. 


## Data protection and compliance

>[!IMPORTANT]
>
>Workfront is not designed to be a repository for electronic health records (EHRs). ePHI may only be processed if expressly authorized by Adobe in writing. 

* For any Workfront database where ePHI might be accessible, ensure **Encryption at Rest (EAR)** is enabled.
    * Contact your Account Executive (AE) to verify EAR is included in your Workfront purchase.
    * Configure systems/databases accessible via Workfront to meet compliance obligations.
* Ensure ePHI is not transferred, linked, or shared with other Adobe solutions.
* Ensure patient photographs processed via Workfront are stored securely and not publicly accessible.
