---
filename: new-proof-email
content-type: reference
product: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
---



# New proof email {#new-proof-email}



>[!IMPORTANT] {type="important"}
>
>This article refers to functionality in the standalone product *`Workfront Proof`*. For information on proofing inside *`Adobe Workfront`*, see [Proofing](_proofing.md).


When you are creating a new *`proof`* or a new version of a *`proof`*, adding new people to a *`proof`*, or adding a workflow to a *`proof`*, you can decide if you want to email the reviewers, as explained in these articles:



* [Create an advanced proof with an Automated workflow](create-automated-proof-workflow.md) 
* [Generate Proofs in Workfront Proof](generate-proofs.md) 


The email your recipients receive is called the New Proof email. Only the *`proof`* creator and users authorized to add reviewers to a *`proof`* can control this email. Recipients cannot disable it.


The New *`proof`* email contains:



* Your personal message (if you choose to include one)  
*  If you always send the same custom message to your reviewers, it might be a good idea to save it in your Personal settings under the Proofing defaults tab. For more information, see [Configure proof settings for your organization](configure-proofing-organization.md).
* Personal link to the *`proof`*
* `View details` link that takes you to the associated *`Workfront`* object (such as a project, task, or issue)

* Thumbnail of the *`proof`* image
* The following *`proof`* details:
*  `<li>Proof name</li>` `<li> <p>Version number</p> <p>For more information, see .</p> </li>` `<li>List of the reviewers and their progress on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span></li>` `<li> <p>A link to share the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> with someone else</p> <p>This allows you to share the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> URL and/or the download link for the original file. This does not allow you to explicitly add reviewers to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>, you will only be sharing the public <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> URL, and the recipient will receive read only access to the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.<br></p> <p>See <a href="share-proof.md" class="MCXref xref">Share a Proof in Workfront Proof</a> for more information.<br></p> <p>If you don't want this link to appear on your recipient's email, you can disable the Public Sharing settings on the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> </p> <p>(Download original file and Public URL). See <a href="manage-proof-details.md" class="MCXref xref">Manage Proof Details in Workfront Proof</a> for more information.</p> </li>` 





## The Activity Log {#the-activity-log}

Sending a New Proof email to a reviewer is logged in the Activity section of Proof details page. See  [Manage Proof Details in Workfront Proof](manage-proof-details.md) for more information. You can check if the New Proof email was enabled at the time of creating a *`proof`*.


![New_Verison_email_-_acitivity_log.png](assets/new-verison-email---acitivity-log-350x44.png)




>[!NOTE]
>
>
>
>
>* If the Creator or Owner of the *`proof`* has Proof Made emails disabled by default (in their personal settings), they won't receive any Proof made or New *`proof`* emails even if the Notify people by email box is checked on the New *`proof`* page. For more information, see [Configure proof settings for your organization](configure-proofing-organization.md).
>
>* If the email notifications are disabled as a default in the Account settings the Creator / Owner of the *`proof`* won't receive any Proof made or New *`proof`* emails even if this is enabled in their personal settings and the Notify people by email box is checked on the New *`proof`* page.&nbsp;For more information, [The Proof Made email](proof-made-email.md) and see [Configure proof settings for your organization](configure-proofing-organization.md).
>
>
>





## Enable the New Proof email and include a custom message {#enable-the-new-proof-email-and-include-a-custom-message}

You can specify whether you want to send an email alert to the reviewers on a *`proof`* when you create it or when you add someone to it.



* [When you create a proof](#when-you-create-a-proof) 
* [When you add a reviewer to a proof](#when-you-add-a-reviewer-to-a-proof) 




### When you create a *`proof`* {#when-you-create-a-proof}

When you are creating a new *`proof`* in the New *`proof`* page, under the `Share` section, you can select whether to send email alerts:



* Here you can decide if you want to Notify people by email (1). If you deselect this option, none of your reviewers receive an email to let them know that the *`proof`* is ready for their review.
* You can also include a Custom message in the email notification (2).
* If you decide to add your own custom message you will be able to put in a customized subject line (3) and a message in the body of the email (4).
*  To discard the custom message simply click on the link (5).


  >[!NOTE]
  >
  >If you always send the same custom message to your reviewers, it might be a good idea to save it in your Personal settings under the Proofing defaults tab. For more information, see [Configure proof settings for your organization](configure-proofing-organization.md).





![New_Proof_page_1.png](assets/new-proof-page-1-350x186.png)



![New_Proof_page_2.png](assets/new-proof-page-2-350x283.png)



### When you add a reviewer to a *`proof`* {#when-you-add-a-reviewer-to-a-proof}

You can select if a new reviewer added to an existing *`proof`* will be notified of the *`proof`* (similar to above).



* First, add new reviewers by clicking the `Share this Version` button on the `Proof details` page (1).



![Proof_Details_page_1.png](assets/proof-details-page-1-350x118.png)





* A box appears in which you can add new reviewers. You can then decide if you want them to be notified by email (2) and choose to add a custom message to the email (3).


![Proof_Details_page_2.png](assets/proof-details-page-2-350x174.png)





* If you choose to add a custom message, the box expands and you will be able to put in a custom subject line (4) and custom text in the body of the email (5). You can also discard the custom message by clicking on the link (6).


![Proof_Details_page_3.png](assets/proof-details-page-3-350x258.png)


