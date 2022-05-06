---
filename: configure-branded-domain-in-wp
product: workfront-proof
product-area: documents;system-administration
navigation-topic: branding-workfront-proof
title: Configure a branded domain in Workfront Proof
description: All Workfront Proof plans allow you to configure a branded sub-domain on your account. This means that you can customize your account URL to include your brand name.
hidefromtoc: true
---

# Configure a branded domain in Workfront Proof

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

All Workfront Proof plans allow you to configure a branded sub-domain on your account. This means that you can customize your account URL to include your brand name.

For example, if you set your sub-domain to be kattest, your URL would look like this:

**https://kattest.proofhq.com/dashboard**

Setting a custom sub-domain also means that all links in your notification emails will include your customized sub-domain. For example: http://kattest.proofhq.com/proof/review/id/123456.

You can create a branded sub-domain or a fully branded domain.

## Configuring a Branded Sub-Domain

1. Log in to Workfront Proof as the Workfront Proof administrator.
1. Click **Account settings** in the upper-right corner of the Workfront Proof interface.
1. Click the **Settings** tab.
1. In the **Customized Sub-Domain** section, click **Setup**.

1. Enter your brand name. Do not enter the whole URL (e.g. www.kattest.com) only enter the brand name, e.g. kattest.
1. Click **Save**.

![branded_subdomain_setup.png](assets/branded-subdomain-setup-350x59.png)

Only users with [Proof Permissions Profiles in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) or&nbsp; [Proof Permissions Profiles in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) rights can set up a branded sub-domain.

(Please see [Proof Permissions Profiles in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) for reference.)

>[!NOTE]
>
>&nbsp;Once you have set up your sub-domain it will not be editable. If you wish to change it please contact Workfront Proof Support.

## Configuring a Fully Branded Domain

You can have a fully customized domain. For example, http://proofing.<yourbrand>.com.

To set up your custom domain or branding, you must complete the following steps:

1. As a first step, it is important to determine what type of SSL certificate is required for your white label URL:

   * If you plan to have only one Workfront Proof account, a standard SSL certificate with Single domain should be purchased.
   * If you plan on having multiple Workfront Proof account (e.g., Satellite accounts), a Wildcard SSL certificate should be purchased.  
     For general information about SSL certificates, see [Understanding Certificate Signing Requests (CSR) and SSL Certificates](#understanding-certificate-signing-requests-csr-and-ssl-certificates).

1. A Certificate Signing Request (CSR) must be created by Workfront Proof. For general information about CSRs, see [Understanding Certificate Signing Requests (CSR) and SSL Certificates](#understanding-certificate-signing-requests-csr-and-ssl-certificates).  
   In order for us to create the CSR, we need the following information:

   >[!IMPORTANT]
   >
   >The CSR cannot be modified after it is generated. Ensure that the following information is correct.&nbsp;

   * **Common Name/Fully Qualified Domain Name** (Everything after http://. This must match exactly what you type in your browser, e.g. www.yourdomain.com or proofing.yourdomain.com.
   * **Will you be using this domain for multiple Workfront Proof accounts**? If you require multiple Workfront Proof accounts to use this domain, please specify this using the wildcard e.g., &#42;.yourdomain.com.)
   * **Organization Name** (Legal name of your Organization. This must not be abbreviated or include any suffixes e.g. Corp., Inc., Ltd.)
   * **Organizational Unit** (The department in your organisation handling the Certificate. This could be "IT" or even "General".)
   * **City** (City where your organization is located)
   * **State** (State where your organization is located)
   * **Country code** (2-letter ISO code for the country where your organization is located, e.g., US, GB.)

1. After the information in step 2 is received, we create the CSR and send it to you along with the CNAME URL&nbsp;to point the domain to.
1. Give the CSR to a SSL Certificate Provider (Certificate Authority) who will create the SSL Certificate and Key chain for you.
1. Point the domain to the CNAME URL we provided (see step 3 above).
1. Send the SSL Certificate and Key chain to Workfront Proof.

## Understanding Certificate Signing Requests (CSR) and SSL Certificates {#understanding-certificate-signing-requests-csr-and-ssl-certificates}

### A Certificate Signing Request (CSR)

A CSR&nbsp;is a block of encrypted text that is generated on the server that the certificate will be used on. It contains information that will be included in your certificate, e.g. common name, organization name, as above. It also contains the public key that will be included in your certificate. (A private key is normally created at the same time.)

### SSL Certificate

SSL stands for Secure Sockets Layer Certificate. This provides a means by which your identity can be proven to web browsers, allowing a secure site to communicate privately with the you.

The type of SSL Certificate required is a standard SSL Certificate with a Single domain is all that is required. A multi-year SSL certificate is best, as this will prevent you from having to go through this process again in 12 months, but a single year SSL certificate is also fine.

When the SSL Certificate Provider creates the SSL Certificate, they will also provide you with the Key chain. The Key Chain allows web browsers to recognize your SSL certificate as a trusted certificate.
