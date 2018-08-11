---
description: There are some differences between at.js and mbox.js. This section lists some of the differences and limitations, to help you be successful with at.js.
keywords: visual experience composer limitations;browser support;integrations;plugins;asynchronous considerations
seo-description: There are some differences between at.js and mbox.js. This section lists some of the differences and limitations, to help you be successful with at.js.
seo-title: at.js Limitations
solution: Target
title: at.js Limitations
topic: Premium
uuid: 7901f45c-1035-450f-b814-0449becd9af7
index: y
internal: n
snippet: y
translate: y
---

# at.js Limitations

This section contains the following information: 


* [ Known Visual Experience Composer Limitations ](c_target-atjs-limitations.md#section_4B63C97169DE4C93B22944E880FD3DF1)
* [ Integrations and Plugins ](c_target-atjs-limitations.md#section_D92E31170176406AAC7B5005F03D3425)
* [ Asynchronous Considerations ](c_target-atjs-limitations.md#section_B586360A3DD34E2995AE25A18E3FB953)


## Known Visual Experience Composer Limitations {#section_4B63C97169DE4C93B22944E880FD3DF1}


* Insert Element and Rearrange options in the Visual Experience Composer should be avoided in single-page apps. 

  Because the DOM is not cleared on page load events in single-page apps like it is with traditional websites, the Insert Element and Rearrange manipulations might be reapplied multiple times depending on how the visitor navigates the SPA. 



## Integrations and Plugins {#section_D92E31170176406AAC7B5005F03D3425}

Some functions within [!DNL  mbox.js] are not available in [!DNL  at.js]. Internal [ mbox.js objects and methods ](r_variables_profiles_parameters_methods.md#section_8C78059D15D9452F95636A5640188537) (such as ` mbox`, ` mboxCurrent`, ` mboxFactoryDefault`, ` mboxFactories`, and others) are no longer supported by [!DNL  at.js] (example: ` mboxFactoryDefault`). This is by design, intended to discourage you from "hacking" [!DNL  at.js] to develop unsupported functionality that over the long term can cripple an implementation and make it impossible to upgrade. The only exposed methods are covered in the API pages of this documentation. Because of this: 


* Legacy, page-based [ integrations ](c_target-atjs-integrations.md#concept_C100BC4F073C4B57A608B309D0157B39) with other Adobe solutions might not work and should be upgraded to newer, server-side integrations. 

* [ Custom plugins developed for mbox.js ](c_target-atjs-plugins.md#concept_F5D4C0A4DACF41409CC42FDD93B13FAF) might not work unless updated for [!DNL  at.js]. 

  Make sure you include any [ plugins ](c_target-atjs-plugins.md#concept_F5D4C0A4DACF41409CC42FDD93B13FAF) as part of your testing. 



## Asynchronous Considerations {#section_B586360A3DD34E2995AE25A18E3FB953}

Because all mboxes are now asynchronous, they won't block page rendering or return in the order in which they fired. 


* If you are using a global mbox in the [ Form-Based Experience Composer ](c_experiences.md#section_3643394BD424463C8768F2907DEBCC22), be aware that HTML offers should contain only ` &amp;lt;script&amp;gt;`, ` &amp;lt;style&amp;gt;`, and ` &amp;lt;link&amp;gt;` tags. 

  During delivery, [!DNL  at.js] filters out all the other HTML tags when applying global mbox offers. Global mbox offers are applied to HTML HEAD, which doesn't allow DIV, SPAN, and so forth. For example ` &amp;lt;div&amp;gt;test&amp;lt;/div&amp;gt;` cannot be applied because the ` &amp;lt;div&amp;gt;` tag can be used only inside HTML BODY. 

* Legacy page-based [!DNL  Target] to [!DNL  Analytics] integration will not work. 

  This integration requires that the [!DNL  Target] call is made before the [!DNL  Analytics] call. 

* Beware of JavaScript dependencies between your offer and the page. 

  You should not assume that the JavaScript in your offer is going to execute before the hardcoded JavaScript below the mbox. 

* Beware of JavaScript dependencies between multiple offers on the page. 

  You can no longer assume that the offer delivered by the first mbox is going to execute before the offer delivered by your second mbox. 

* DOM Manipulation and Redirect offers should be delivered through the auto-created global mbox in [!DNL  at.js] and delivered in the ` &amp;lt;head&amp;gt;`. 

  An ` mboxCreate()` function at the top of the ` &amp;lt;body&amp;gt;` will likely result in flicker of default content. 


