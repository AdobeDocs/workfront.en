---
filename: fusion-security-standards
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion Security Standards
description: Adobe Workfront Fusion enforces several best-practice security standards to ensure that data is:
---

# Adobe Workfront Fusion Security Standards

Adobe Workfront Fusion enforces several best-practice security standards to ensure that data is:

* Appropriately scoped to the most limited set of required uses
* Maintained and transferred securely
* Safe from external threats

Security mechanisms include, but are not limited to, the following.

## Connector Authentication

Workfront Fusion includes a set of application connectors that enable administrators to connect to other applications without coding. Each connector is built to ensure that it connects in the most secure way that is supported by the given service. In some cases (such as FTP, databases, etc.) you have the option to set the security level manually.

Workfront Fusion uses AES encryption (PBKDF2-SHA512 with 200k iterations) to save credentials securely. Best practice authentication mechanisms include the use of OAuth2. When using OAuth2, usernames and passwords are never stored in Workfront Fusion.

Connected applications that support OAuth2 can revoke Workfront Fusion’s access at any time without having access to Workfront Fusion. Additionally, Workfront Fusion users can also revoke Workfront Fusion’s access to the connected application at any time.

Administrators using Workfront Fusion can never retrieve any information related to credentials (such as usernames or the target URL of other systems).

##  Connector Authorization

Workfront Fusion uses the connected application's own authorization mechanisms to ensure that users have access only to the information and actions for which they are authorized. If a user’s credentials do not allow them to access information in the connecting application, they cannot access that information within Workfront Fusion.

## IP Allowlist

Workfront Fusion IP Addresses are shared Virtual Private Cloud (VPC) IPs and are static for IPs for Workfront Fusion traffic. Workfront Fusion uses static IP addresses so that organizations can limit access or make tunnels.

Add the following IP addresses to your allowlist to enable Workfront Fusion to access your system:

* 35.160.0.242
* 34.213.36.118
* 3.209.27.146
* 18.205.251.4

If your organization uses outbound network filtering, add the following domain to your allowlist to enable your system to access Workfront Fusion.

>[!NOTE]
>
>Outbound network filtering is uncommon. Check with your network administrator to see if you need to update your allowlist to accommodate for it.

* 

  ```
  hook.app.workfrontfusion.com
  ```

## Data Encryption

Workfront Fusion interacts with connectors through the highest level of security offered by the connected solution. At a minimum, data is encrypted in transit over a TLS 1.2 connection. Mutual TLS is also available.

For more information on Mutual TLS in Workfront Fusion, see [Use Mutual TLS in HTTP modules](../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md).

## Role-Based Access

Workfront Fusion has multiple roles and authorization controls that ensure that Workfront Fusion users only have access to their own flows and connections, and those flows and connections that have been explicitly shared with them.

## Intrusion Prevention

Workfront Fusion, like Adobe Workfront, follows best practices in preventing unauthorized access to the platform. Such best practices include those outlined in the Open Web Application Security Project (OWASP) and other common intrusion prevention mechanisms. This includes regular security testing.

## Fusion UI

The connection between Workfront Fusion and your browser is always encrypted (HTTPS).

## Other security measures:

* To protect our secure HTTPS website from downgrade attacks, we have implemented and use HTTP Strict Transport Security (HSTS), the web security policy mechanism.
* We have protection against CSRF/XSRF attacks.
* We use CSP protection to prevent XSS.
* Fusion is supported only on Chrome, which has the highest security standards of any browser.

