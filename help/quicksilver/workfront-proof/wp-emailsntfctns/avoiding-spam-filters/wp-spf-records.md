---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Workfront Proof SPF records
description: Workfront Proof sends email notifications to your reviewers from a Workfront Proof email address such as notification@proofing.yourdomain.com. In order to ensure that your recipients' mail servers trust all Workfront Proof email notifications, you need to set up a [!DNL Sender Policy] Framework (SPF) record for your customized domain connected to the [!DNL Workfront Proof] account (for example, proofing.yourdomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
---
# Workfront Proof SPF records

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product [!DNL Workfront Proof]. For information on proofing inside [!DNL Adobe Workfront], see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] sends email notifications to your reviewers from a [!DNL Workfront Proof] email address such as notification@proofing.yourdomain.com. In order to ensure that your recipients' mail servers trust all [!DNL Workfront Proof] email notifications, you need to set up a [!UICONTROL Sender Policy Framework] (SPF) record for your customized domain connected to the [!DNL Workfront Proof] account (for example, **proofing.yourdomain.com**).

To set up an SPF record, you will need to include the SPF record used for our primary domain.

1. Add a **[!UICONTROL DNS TXT]** entry for your domain with the following value:

   `v=spf1 a:mx.proofhq.com -all`

   Your email administrator or IT personnel can help you set this up.

   >[!TIP]
   >
   >You can use the free tool at [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) to review [!DNL Workfront] SPF records.
