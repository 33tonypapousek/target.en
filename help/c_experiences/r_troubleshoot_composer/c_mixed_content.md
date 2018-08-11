---
description: Some browsers block the display of a page if secure content is mixed with insecure content.
keywords: mixed content;secure;insecure;chomre;troubleshooting;vec;visual experience composer;unsecure
seo-description: Some browsers block the display of a page if secure content is mixed with insecure content.
seo-title: Enabling Mixed Content in Your Browser
solution: Target
title: Enabling Mixed Content in Your Browser
topic: Advanced,Standard,Classic
uuid: 4d702cf3-201d-4151-836e-1b75351c6fe6
index: y
internal: n
snippet: y
translate: y
---

# Enabling Mixed Content in Your Browser

## Enabling Mixed Content in Your Browser {#concept_46D022D50280468C9EF6D5DF6EFC911C}
>Some browsers block the display of a page if secure content is mixed with insecure content.If the Visual Experience Composer (VEC) tries to open a page containing mixed (secure and insecure) content, a message displays showing how to disable blocking in your browser so you can open an HTTP site or a site that has mixed calls (HTTPS and HTTP). 

![](../../assets/mixed_content_warning.gif) 

Previously, when mixed content was not allowed, you could still perform some actions in Step 1 of the three-step guided workflow when creating activities. Target now blocks actions in Step 1. When this message displays, you must enable mixed content before continuing. 

Your browser's security settings might block mixed content or insecure (HTTP) content being loaded into a secure (HTTPS) page or frame (such as the VEC). If you don't want to disable your browser's security settings, you need to have an HTTPS website. 

If you website is running on an insecure (HTTP) domain, you are required to allow the VEC to load active mixed content. 


>[!NOTE]
>
>Allowing mixed content affects the VEC only and not your live website.



For more information, see [ Mixed Content](https://developer.mozilla.org/en-US/docs/Web/Security/Mixed_content) on the *Mozilla Developer Network* (MDN) website. 
>## Enabling Mixed Content in Firefox {#task_5448763B8DC941FD80F84041AEF0A14D}
>By default, Firebox blocks pages that mix secure and insecure content. It is recommended that you permanently change this setting to use 
<keyword>
  Target
</keyword>. 
<draft-comment>
  target/t_mixed_content_firefox.xml 
</draft-comment>
>1. In Firefox, enter ` about:config` in the address bar.
>1. Acknowledge the warning message displayed by Firefox.
>1. In the search bar, type ` block_active`.
>1. Double-click ` ** [!UICONTROL  security.mixed_content.block_active_content] **` .

>## Enabling Mixed Content in Internet Explorer {#task_59E7D13C04DF486C92CD78D0C63DDDE8}
>By default, Internet Explorer blocks pages that mix secure and insecure content. It is recommended that you permanently change this setting to use Target Standard. 
<draft-comment>
  target/t_mixed_content_ie.xml 
</draft-comment>
>1. In Internet Explorer, click the settings icon > ** [!UICONTROL  Internet Options] **.
>1. Open the [!UICONTROL  Security] tab.
>1. Select ** [!UICONTROL  Internet] **, then click ** [!UICONTROL  Custom Level] **.
>1. Select ** [!UICONTROL  Miscellaneous] **.
>1. Under [!UICONTROL  Miscellaneous], enable ** [!UICONTROL  Display Mixed Content] **.
>1. Click ** [!UICONTROL  OK] ** > ** [!UICONTROL  Yes] ** > ** [!UICONTROL  Apply] **.
>## Enabling Mixed Content in Chrome {#task_FF297A08F66E47A588C14FD67C037B3A}
>If you're visiting a site via a secure connection, Google Chrome will verify that the content on the web page has been transmitted safely. 
<draft-comment>
  target/t_mixed_content_chrome.xml 
</draft-comment>See [ This page has insecure content](https://support.google.com/chrome/answer/1342714?hl=en) in Google Chrome Help. 
