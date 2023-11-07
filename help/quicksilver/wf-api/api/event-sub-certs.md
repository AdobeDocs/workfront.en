---
content-type: api
navigation-topic: api-navigation-topic
title: Event subscription certificates
description: Event subscription certificates
author: Becky
feature: Workfront API
role: Developer
exl-id: 3606b6c3-b373-47ea-9cb5-813bd3af8da7
---
# Configure Client TLS for Event Subscription

<!--Configuring Client TLS for Event Subscription
Steps to Verify Workfront's Client Certificate
Examples for Server configuration
NGINX
Apache
Certificate to Environment Mapping
Certificates
Production
Preview
Sandbox 1
Sandbox 2
-->

Client TLS allows you to verify that the event subscription message you receive actually came from Adobe Workfront. To enable this functionality, your server must be configured to request and validate Workfront's x509 certificate. 


## Verify Workfront's client certificate

This procedure assumes your server is configured to accept TLS connections. Workfront does not support self-signed certificates.

In general, these are the steps needed to turn on client authentication for your server:

1. Download the PEM version of the DigiCert Global Root CA certificate.
1. Turn on client certificate verification.

   Specify the CA certificate from step 1 as trusted.

1. Set the verification depth to 2 since our certificate is actually signed by the DigiCert SHA2 Secure Server CA which is an intermediate CA under DigiCert Global Root CA.
1. Verify the client certificate is actually from Workfront by inspecting its Subject Domain Name.

## Examples for Server configuration

### NGINX

```
server {

    listen 443 ssl default_server;
    # ... existing SSL configuration for server authentication ...

    ssl_verify_client on;
    ssl_client_certificate /path/to/DigiCert_Global_Root_CA.pem;
    ssl_verify_depth 2;

        # ... existing location configuration ...
    }
}
```

For more information, see the [NGiNX documentation for ngx_http_ssl_module](http://nginx.org/en/docs/http/ngx_http_ssl_module.html). 

### Apache

```
Listen 443
<VirtualHost *:443>
    # ... existing SSL configuration for server authentication ...

    SSLVerifyClient require
    SSLCACertificateFile "/path/to/DigiCert_Global_Root_CA.pem"
    SSLVerifyDepth 2
</VirtualHost>

<Directory /var/www/>
    Require expr "%{SSL_CLIENT_S_DN_CN} == <>"

    # ... existing directory configuration ...
</Directory>
```

For more information, see 

* [Client Authentication and Access Control](https://httpd.apache.org/docs/2.4/ssl/ssl_howto.html#accesscontrol)
* [Apache Module mod_ssl](https://httpd.apache.org/docs/2.4/mod/mod_ssl.html) 
 

## Certificate to Environment Mapping

| WF Environment | Certificate Common Name | Certificate Subject (DN) |
| -- | -- | -- |
| Production | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.prod.eventsubscriptions.workfront.com|
| Preview | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.preview.eventsubscriptions.workfront.com |
| Sandbox 1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |
| Sandbox 2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |

## Download certificates

Click the following links to download the client certificates.

* [Client certificate - Production environment](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_production.crt)
* [Client certificate - Preview environment](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_preview.crt)
* [Client certificate - Sandbox environment](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_sandboxes.crt)

>[!NOTE]
>
>You can use the same client certificate for both Sandbox environments.
