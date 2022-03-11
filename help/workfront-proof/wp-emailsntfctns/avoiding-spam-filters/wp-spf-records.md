---
filename: wp-spf-records
product: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Workfront Proof SPF records
description: Workfront Proof sends email notifications to your reviewers from a Workfront Proof email address such as notification@proofing.yourdomain.com. In order to ensure that your recipients' mail servers trust all Workfront Proof email notifications, you need to set up a Sender Policy Framework (SPF) record for your customized domain connected to the Workfront Proof account (for example, proofing.yourdomain.com).
---

# Workfront Proof SPF records

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Workfront Proof sends email notifications to your reviewers from a Workfront Proof email address such as notification@proofing.yourdomain.com. In order to ensure that your recipients' mail servers trust all Workfront Proof email notifications, you need to set up a Sender Policy Framework (SPF) record for your customized domain connected to the Workfront Proof account (for example, `proofing.yourdomain.com`).

To set up an SPF record, you will need to include the SPF record used for our primary domain.

<ol> 
 <li value="1"> <p>Add a&nbsp;<span class="bold">DNS TXT</span> entry for your domain with the following value:</p> <p>v=spf1 a:mx.proofhq.com -all</p> <p>Your email administrator or IT personnel can help you set this up.<br></p> <note type="tip">
   You can use the free tool at 
   <a href="https://mxtoolbox.com/spf.aspx">https://mxtoolbox.com/spf.aspx</a> to review Workfront SPF records.
   <br>
  </note> </li> 
</ol>

