---
filename: sso-in-wp-adfs-configuration
product: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Single Sign-On in Workfront Proof: AD FS configuration
description: Important: This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see Proofing.
---

# Single Sign-On in *Workfront Proof*: AD FS configuration

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product *Workfront Proof*. For information on proofing inside *Adobe Workfront*, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

If you are an administrator on your AD server, you can install and configure AD FS.

## Installing and Configuring AD FS

<ol> 
 <li value="1">Download <a style="background-color: #ffffff;" href="http://www.microsoft.com/en-us/download/details.aspx?id=10909">AD FS 2.0</a>&nbsp;to your computer.&nbsp;</li> 
 <li value="2">Open&nbsp;the downloaded AdfsSetup.exe file to start the ADFS (Active Directory Federation Services) Installation Wizard.</li> 
 <li value="3">On the Server Role screen, select one of the options&nbsp;(you need at a minimum a Federation Server).<br></li> <note type="note">
  &nbsp;If you do not want&nbsp;to expose IIS on your AD server to the internet (ports 80 and 443 for HTTP and HTTPS), you can first set up a Federation Server behind the firewall, then build a second Federation Server Proxy&nbsp;that passes requests through the firewall to the Federation Server.
 </note> 
 <li value="4">Once you complete the&nbsp;AD FS setup, select <span class="bold">Start the AD FS 2.0 Management snap-in</span>&nbsp;, then click <span class="bold">Finish.<br></span>Once this is completed, the AD FS 2.0 Management window should open right away. If not, you can open it from&nbsp;<span class="bold">Start</span> > <span class="bold">Administrative Tools</span> > <span class="bold">AD FS 2.0 Management</span>. This is&nbsp;the main AD FS control application.</li> 
 <li value="5">Begin by clicking AD FS 2.0 Federation Server Configuration Wizard.<br>This will help you to configure&nbsp;AD FS and connect it&nbsp;to both the Internet via IIS and to AD.</li> 
 <li value="6">If you are configuring a new AD FS server, select <span class="bold">Create a new Federation Service</span>.</li> 
 <li value="7">Select <span class="bold">Stand-alone federation server</span>&nbsp;(for testing and evaluation purposes).<br></li> <note type="note">
  &nbsp;For high availability and load balancing, click New federation server farm.&nbsp;
 </note> 
 <li value="8">Specify your Federation Service name.<br>By default the&nbsp;configuration&nbsp;wizard retrieves the SSL certificate bound to the Default Web Site in IIS&nbsp;and will use the subject name specified there. If you use a wildcard certificate you will need to enter the Federation Service name.<br>If there is no SSL certificate configured in IIS, then the configuration wizard will search in the local computer certificate store for any valid certificates. These display in the SSL certificate drop-down. If there are no certificates found, you can&nbsp;use the&nbsp;Server Certificate Generator in IIS&nbsp;to create one.</li> 
 <li value="9">Continue with the configuration, and click <span class="bold">Close</span> once it is complete.</li> 
</ol>

## Configuring *Workfront Proof* Single Sign-On

If you are a *Workfront Proof administrator*, you can configure Single Sign-On on the *Workfront Proof* side.&nbsp;For more information, see [Single Sign-On in Workfront Proof](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

<ol> 
 <li value="1">Click <span class="bold">Settings</span> > <span class="bold">Account Settings</span>, then open the&nbsp;<span class="bold">Single sign-on</span> tab.</li> 
 <li value="2">In the&nbsp;<span class="bold">SSO URL&nbsp;</span>box, paste your Entity ID.<br>The following is an example of an Entity ID:<br>http://<i><adfs.your-company.com></i>/adfs/services/trust<br>Your Entity ID can be found in your Federation Metadata XML file.<br><img src="assets/proofhq-configuration-02-350x80.png" alt="ProofHQ_configuration_02.png" style="width: 350;height: 80;"></li> <note type="note">
  &nbsp;Federation Metadata is&nbsp;found in the AD FS 2.0 snap-in > Service > Endpoints folder. In the Metadata section, locate the one with the Federation Metadata type. To view metadata, paste this endpoint in your browser. You can also go to this link directly:&nbsp;https://
  <i><adfs.your-company.com></i>/FederationMetadata/2007-06/FederationMetadata.xml after replacing the {adfs.your-company.com}&nbsp;with your own details.
 </note> 
 <li value="3">In the <span class="bold">Login URL</span> box, paste your SSO login.</li> 
 <p>The following is an example of an SSO login:</p> 
 <p>http://<i><adfs.your-company.com></i>/adfs/ls. </p> 
 <p>This link&nbsp;can be located&nbsp;in the Federation Metadata XML file.<br><img src="assets/proofhq-configuration-03-350x90.png" alt="ProofHQ_configuration_03.png" style="width: 350;height: 90;"></p> 
 <li value="4">In the&nbsp;<span class="bold">Logout URL</span> box, enter&nbsp;the link and save.<br>The following is an example of a Logout URL:<br>https://<i><adfs.your-company.com></i>/adfs/ls/?wa=wsignout1.0
  <ol>
   <li value="1">Go to your AD FS manager >&nbsp;Trust Relationships >&nbsp;Relying Party Trusts - ProofHQ&nbsp;properties.</li>
   <li value="2">Under the Endpoints, click Add and entry with the following details: 
    <ul>
     <li>Endpoint Type = SAML Logout</li>
     <li>Binding = POST</li>
     <li>URL = https://<i><adfs.your-company.com</i>>/adfs/ls/?wa=wsignout1.0</li><note type="note">
      This step can be completed after configuring the Relying Party Trust (see below) in your AD FS.
     </note>
    </ul></li>
   <li value="3">In the <span class="bold">Certificate fingerprint</span> box, enter the data from your certificate.</li>
   <li value="4">Go to your&nbsp;ADFS 2.0 snap-in&nbsp;navigate to Service > Certificates > Token-signing.</li>
   <li value="5">Right-click on this entry to view the certificate.</li>
   <li value="6">From the Certificate Details tab copy the Thumbprint, and paste it in the <span class="bold"><em>Workfront Proof</em> Single Sign-On</span> configuration tab.<br></li><note type="note">
    &nbsp;The fingerprint characters can be separated with colons or spaces, but we do recommend removing these. If you have any troubles with your Single Sign-On configuration, please contact the Customer Support team.
   </note>
  </ol></li> 
</ol>

## Adding a Relying Party Trust

Once configuration is complete, you need to work in the&nbsp;Relying Party Trusts section in your AD FS.

<ol> 
 <li value="1">Navigate to <span class="bold">Trust Relationships</span> > <span class="bold">Relying Party Trusts</span>&nbsp;folder, then click <span class="bold">Add a Relying Party Trust </span>to&nbsp;start the configuration wizard.</li> 
 <li value="2">Select your data source.<br>All metadata for your ProofHQ account is located under a link like this:<br>https://<i><yoursubdomain</i>>.proofhq.com/saml/module.php/saml/sp/metadata.php/phq<br>This will configures most of the Relying Party Trust.<br><note type="note">
   <ul>
    <li>If you're having any troubles with establishing the connection from the URL, save the metadata as a file and choose to import data from a file.</li>
    <li>When you have a full Custom domain (e.g., www.your-<em>proofing</em>.com) configured on your ProofHQ account replace the whole "{yoursubdomain}.proofhq.com" part with your own domain to create your ProofHQ metadata link.</li>
   </ul>
  </note></li> 
</ol>

## Configuring Claim Rules

Once your Relying Party Trust configuration is complete, you are ready to configure the claim rules to complete the set up. You will configure two claim rules for ProofHQ: E-mail and Name ID.

1. Open the `Edit Claim Rules` dialog box.
1. Go to `ProofHQ Relying Party Trust`, then click `Edit Claim Rules`&nbsp;(1).   
   The pop-up should automatically open if you selected this option at the end of configuring the trust.

1. Click `Add Rule` (2) to open the claim configuration window.

  * E-mail (Send LDAP Attributes as Claims rule template)
  * NameID (Transform an Incoming Claim rule template)

