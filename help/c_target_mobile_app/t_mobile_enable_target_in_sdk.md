---
description: Add the Adobe Mobile Services SDK to your app.
keywords: mobile app;mobile app sdk;target mobile app;mobile target sdk;mobile app sdk;enable target in sdk
seo-description: Add the Adobe Mobile Services SDK to your app.
seo-title: Enable Target in the SDK
title: Enable Target in the SDK
topic: Target
uuid: 64fd2a63-60c7-4c48-8816-17bfe122f619
index: y
internal: n
snippet: y
translate: y
---

# Enable Target in the SDK


>1. If you haven't installed the Adobe Mobile Services SDK in your app, use your Analytics or Experience Cloud credentials and download the SDK from the [ Adobe Mobile Services ](https://mobilemarketing.adobe.com) website.

>1. Add the Adobe Mobile Services SDK to your app.

>       You can find the instructions under [ Core Implementation and Lifecycle ](https://marketing.adobe.com/resources/help/en_US/mobile/ios/dev_qs.html). 
>1. Add client code, timeout and enable SSL.

>       In the Experience Cloud, open Mobile Services, then go to **[!UICONTROL  Manage App Settings]** > **[!UICONTROL  SDK Target Options]**. 

>       Add your Target clientcode and timeout. The clientcode is unique to your account or company. The timeout is the time in number of seconds until which Target will wait for a response before showing the default content. Make sure the **[!UICONTROL  Use HTTPS]** option is checked in the Manage App Settings page in Adobe Mobile Services. If HTTPS isn't enabled, all calls in iOS9+ will be blocked unless you whitelist the Target server. 

>       ![](assets/mobile-clientcode.png) 
>1. After you’ve created/located your app, find the app settings and download the desired SDK.

>       ![](assets/download-sdk.png) 
