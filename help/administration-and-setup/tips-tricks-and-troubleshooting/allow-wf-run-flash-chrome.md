---
filename: allow-wf-run-flash-chrome
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Allow Adobe Workfront to run flash on Google Chrome
description: Chrome has recently changed the way Flash is set up. Unfortunately, this means that even if you allowed Flash to run in the past, your setting will have reverted back to default, which can cause issues within Adobe Workfront. If you have pages that do not load, allowing Flash to run will likely resolve your issue.
---

# Allow `Adobe Workfront` to run flash on Google Chrome

Chrome has recently changed the way Flash is set up. Unfortunately, this means that even if you allowed Flash to run in the past, your setting will have reverted back to default, which can cause issues within `Adobe Workfront`. If you have pages that do not load, allowing Flash to run will likely resolve your issue.

## If you have the most recent version of Chrome

<ol> 
 <li value="1"> From the website that needs to allow Flash, click the lock icon in the URL next to the URL.<br><img src="assets/new-1-36x28.png" alt="new-1.png" style="width: 36;height: 28;"><br></li> 
 <li value="2"> Under Flash, select <span class="bold">Allow</span> from the drop-down list.<br><img src="assets/new-2-350x344.png" alt="new-2.png" style="width: 350;height: 344;"><br> OR <br>Click <span class="bold">Site settings</span>. Then u nder Flash, select <span class="bold">Allow</span> from the drop-down list.&nbsp; </li> 
 <li value="3"> Refresh the settings page.&nbsp; </li> 
 <li value="4"> Return to the original website and reload the page.<br><img src="assets/new-3-350x30.png" alt="new-3.png" style="width: 350;height: 30;"><br></li> 
</ol>

## If you have an older version of Chrome

<ol> 
 <li value="1"> Open your Chrome browser and click the three-dot icon next to your URL bar.<br><img src="assets/icon-35x30.png" alt="icon.png" style="width: 35;height: 30;"></li> 
 <li value="2">Select <span class="bold">Settings</span>.</li> 
 <li value="3"> Scroll to the bottom of the page and click <span class="bold">Advanced</span>.<br></li> 
 <li value="4"> Locate the <span class="bold">Privacy and Security</span>&nbsp;section and click <span class="bold">Content settings</span>.<br><img src="assets/3-content-settings-350x344.png" alt="3-content-settings.png" style="width: 350;height: 344;"><br></li> 
 <li value="5"> Click <span class="bold">Flash</span>.<br><img src="assets/4-flash-350x35.png" alt="4-flash.png" style="width: 350;height: 35;"><br></li> 
 <li value="6">Toggle the switch from <span class="bold">Block sites from running Flash</span> to <span class="bold">Ask first (recommended)</span>.<br><img src="assets/5-toggle-block-350x31.png" alt="5-toggle-block.png" style="width: 350;height: 31;"><br><img src="assets/6-toggle-ask-350x28.png" alt="6-toggle-ask.png" style="width: 350;height: 28;"></li> 
 <li value="7">To manage your exceptions, click <span class="bold">ADD</span> under the <span class="bold">Allow</span> section.<br><img src="assets/7-exceptions-350x119.png" alt="7-exceptions.png" style="width: 350;height: 119;"></li> 
 <li value="8"> Add&nbsp;exceptions for&nbsp;<span class="bold">[*.]workfront.com</span> and &nbsp;for<span class="bold">&nbsp;[*.]proofhq.com</span>. 
  <ul>
   <li>You may also want to add exceptions for your sandbox environments:
    <ul>
     <li>Preview:&nbsp;<span class="bold">[*.]preview.workfront.com</span></li>
     <li>SB01: <span class="bold">[*.]sb01.workfront.com</span><br><img src="assets/8-last-350x157.png" alt="8-last.png" style="width: 350;height: 157;"><br></li>
    </ul></li>
  </ul></li> 
</ol>

