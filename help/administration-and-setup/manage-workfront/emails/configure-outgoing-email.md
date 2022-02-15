---
filename: configure-outgoing-email
user-type: administrator
product-area: system-administration;setup
navigation-topic: emails-administration
---




# Configure outgoing email {#configure-outgoing-email}

You can configure the email address for emails sent from `Workfront`.



1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Setup** ![](assets/setup-gear-icon.png).

1. Click **Email** >** Setup.**






1.  In the **Outgoing Mail** section, in the **Email from `Workfront` will appear to come from** box, specify the email address users see when receiving email notifications from `Workfront`.  



   We recommend using  `Workfront`@YOURCOMPANY.com and adding the address to your safe sender list.

1. Select which server to use for sending emails and notifications from `Workfront`.
1.  `<col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" data-mc-conditions="">` `<col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" data-mc-conditions="">` `<tbody>  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray"><span class="WFVariablesProdNameWF">Workfront</span> Mail Server</td>   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>(Default)&nbsp;Select this option to use&nbsp;the <span class="WFVariablesProdNameWF">Workfront</span> Mail Server for sending email from <span class="WFVariablesProdNameWF">Workfront</span>. When using this option, no further configuration is required.</p> </td>  </tr>  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray">My Mail Server</td>   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <note type="important">    This functionality has been disabled for new configurations, but customers with SMTP configurations in place are still functional and working. Updates for this feature are planned for an upcoming 2020 release later this year.   </note> <p>Select this option to force <span class="WFVariablesProdNameWF">Workfront</span> emails to relay off an internal, trusted server.&nbsp;</p> <p>When using this option, specify the following information:</p>    <ul>     <li value="1"><b>User Name:</b> Specify&nbsp;the user name of the Simple Mail Transfer Protocol (SMTP) account as specified by your email administrator.</li>     <li value="2"> <p><b>Password:</b> Specify&nbsp;the password for the SMTP account.</p> <note type="note">      <span class="WFVariablesProdNameWF">Workfront</span> does not support 2-Step Verification for Gmail accounts.     </note> </li>     <li value="3"> <p><b>Outgoing SMTP server:</b> Assign the outgoing SMTP server.</p> <p>For example,&nbsp;smtp.nameofserver.com.</p> <note type="note">      <span class="WFVariablesProdNameWF">Workfront</span> does not support SMTP relay service.      <br>     </note> </li>     <li value="4"> <p><b>Port:</b>&nbsp;The default SMTP is 25. <br></p> <p>The default SMTP for secure (SSL) connections is 465. <br></p> <p>The default SMTP for secure (TLS) connections is 587.</p> </li>     <li value="5"><b>Use SSL to connect:</b>&nbsp;Select this option to connect over an SSL (Secure Socket Layer) secure connection. This&nbsp;establishes a secure connection between the <span class="WFVariablesProdNameWF">Workfront</span> application and your own configured mail server for outgoing email through the Secure Socket Layer (SSL) protocol.</li>     <li value="6"><b>Use TLS&nbsp;to connect:</b>&nbsp;Select this option to connect over a TLS (Transport Layer Security) secure connection.&nbsp;This&nbsp;establishes a secure connection between the <span class="WFVariablesProdNameWF">Workfront</span> application and your own configured mail server for outgoing email through theTransport Layer Security (TLS) protocol.</li>    </ul> </td>  </tr> </tbody>` 



