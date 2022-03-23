---
filename: allow-wf-run-flash-chrome
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Allow Adobe Workfront to run flash on Google Chrome
description: Chrome has recently changed the way Flash is set up. Unfortunately, this means that even if you allowed Flash to run in the past, your setting will have reverted back to default, which can cause issues within Adobe Workfront. If you have pages that do not load, allowing Flash to run will likely resolve your issue.
hidefromtoc: true
---

# Allow Adobe Workfront to run flash on Google Chrome

Chrome has recently changed the way Flash is set up. Unfortunately, this means that even if you allowed Flash to run in the past, your setting will have reverted back to default, which can cause issues within Adobe Workfront. If you have pages that do not load, allowing Flash to run will likely resolve your issue.

## If you have the most recent version of Chrome

1. From the website that needs to allow Flash, click the lock icon in the URL next to the URL.  
   ![new-1.png](assets/new-1-36x28.png)  

1. Under Flash, select **Allow** from the drop-down list.  
   ![new-2.png](assets/new-2-350x344.png)  
   OR   
   Click **Site settings**. Then u nder Flash, select **Allow** from the drop-down list.&nbsp; 

1. Refresh the settings page.&nbsp; 
1. Return to the original website and reload the page.  
   ![new-3.png](assets/new-3-350x30.png)

## If you have an older version of Chrome

1. Open your Chrome browser and click the three-dot icon next to your URL bar.  
   ![icon.png](assets/icon-35x30.png)

1. Select **Settings**.
1. Scroll to the bottom of the page and click **Advanced**.  

1. Locate the **Privacy and Security**&nbsp;section and click **Content settings**.  
   ![3-content-settings.png](assets/3-content-settings-350x344.png)  

1. Click **Flash**.  
   ![4-flash.png](assets/4-flash-350x35.png)  

1. Toggle the switch from **Block sites from running Flash** to **Ask first (recommended)**.  
   ![5-toggle-block.png](assets/5-toggle-block-350x31.png)  
   ![6-toggle-ask.png](assets/6-toggle-ask-350x28.png)

1. To manage your exceptions, click **ADD** under the **Allow** section.  
   ![7-exceptions.png](assets/7-exceptions-350x119.png)

1. Add&nbsp;exceptions for&nbsp;**[&#42;.]workfront.com** and &nbsp;for**[&#42;.]proofhq.com**.

  * You may also want to add exceptions for your sandbox environments:

    * Preview:&nbsp;**[&#42;.]preview.workfront.com**
    * SB01: **[&#42;.]sb01.workfront.com** 
      ![8-last.png](assets/8-last-350x157.png)

