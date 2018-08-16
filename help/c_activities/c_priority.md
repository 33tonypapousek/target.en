---
description: Target determines which activity (or activities) to deliver to a page differently depending on which Target interface and which activity creation function (Visual Experience Composer or Form Based composer) you're using.
keywords: settings;priority
seo-description: Target determines which activity (or activities) to deliver to a page differently depending on which Target interface and which activity creation function (Visual Experience Composer or Form Based composer) you're using.
seo-title: Priority
solution: Target
title: Priority
topic: Standard
uuid: c56b7ed5-c1c3-4843-8ab1-42de7c583a0b
index: y
internal: n
snippet: y
translate: y
---

# Priority

This page is separated into sections based on the setup for your company. 


<ul class="simplelist"> 
 <li> <a href="../c_activities/c_priority.md#section_4A0A317DFED345649B58B0CB5B410C8B" format="dita" scope="local"> Target Standard/Premium Visual Experience Composer Only</a> </li> 
 <li> <a href="../c_activities/c_priority.md#section_4620253E1CE942DD830724C7822B175F" format="dita" scope="local"> Target Standard/Premium Form-Based Composer and Target Standard/Premium Visual Experience Composer</a> </li> 
 <li> <a href="../c_activities/c_priority.md#section_C3F5F09B0B2D4EF795C5929D5C426A8C" format="dita" scope="local"> Target Standard/Premium Form-Based Composer with Non-Global Mboxes</a> </li> 
 <li> <a href="../c_activities/c_priority.md#section_F6A788AAC3884A2FA03E47F0557A1213" format="dita" scope="local"> Use Cases </a> </li> 
</ul>




>[!NOTE]
>
>Target Classic is scheduled to be decommissioned. For more information, see[ Target Classic Help](https://marketing.adobe.com/resources/help/en_US/tnt/help/). 



**Activity Settings (3:02)** 

This video includes information about activity settings. 


* Enter an objective for your activity 

* Set the priority level of your activities 

* Schedule activity start and end times 

* Add audiences for reporting to create report filters 

* Enter notes for your activities 



>[!VIDEO](https://vimeo.com/6XNEM8tUADo) 

## Target Standard/Premium Visual Experience Composer Only or Form-Based Composer Using Global mbox Only {#section_4A0A317DFED345649B58B0CB5B410C8B}

If your company uses Target Standard/Premium and the Visual Experience Composer exclusively, then content from multiple activities can be returned for the same call. Activities are delivered using the following decision flow: 


1. The Target server call comes to Target with information about the URL. 

1. Target pulls every activity running on that URL. 

1. Target attempts to match the visitor into activities. 

   If the visitor is already in an A/B test or Multivariate Test, they will match into that test until they convert. If they were previously in an experience targeting activity, they must match into it again. If they meet the audience rules, then the visitor falls into those activities and into specific experiences. ([ How experience matching works](../c_target/c_target_rulebased/c_target_whoseeswhat.md#concept_014AB6795D2D4B6EB5E45A226A4FF7E9).) 

1. Content for all the activities and experiences the visitor matches is returned to the page. 

1. If the content for each activity references different [ CSS selectors](../c_experiences/c_vec_selectors.md#concept_4EB7663E255F439B8D24079D23479337), then all content is displayed. 

   If there is an overlap or a duplicated CSS selector, then the activity content with the highest priority is displayed. The results from all activities that run on the page are counted and reflected in the reports. 


   >[!IMPORTANT]
   >
   >Target returns the content for all activities on the page, beginning with the lowest-priority content, which is then overwritten by each activity, from lowest to highest priority. In most cases, this results in the highest priority content being displayed. However, if a lower-priority activity alters the structure of the DOM for the page, it is possible that the higher-priority activity will not recognize the page structure, so the lower-priority content will be displayed. The results from all activities that run on the page are counted and reflected in the reports.


1. If multiple activities share the same priority level, then there are two tiebreakers: 


    * If only one activity has audience targeting, that activity is displayed. 

    * If all or none have targeting, then the activity that was approved first is displayed. 





## Target Standard/Premium Form-Based Composer and Target Standard/Premium Visual Experience Composer {#section_4620253E1CE942DD830724C7822B175F}


>[!NOTE]
>
>This information also applies to any campaigns running that were created in Target Classic.



If your company uses the form-based composer in Target Standard/Premium and the Target Standard/Premium Visual Experience Composer, then content from multiple Visual Experience Composer activities can deliver, but only one activity from the form-based workflow. Activity delivery is determined using the following decision flow: 


1. Target server call comes to Target with information about the mbox and URL. 

1. Target Classic and Standard pull every activity running in that mbox. 

1. Target attempts to match the visitor into activities. 

   If the visitor is already in an A/B test or Multivariate Test, they will match into that test until they convert. If they were previously in an experience targeting activity, they must match into it again. If they meet the audience rules, then the visitor falls into those activities and into specific experiences. ([ Information about how experience matching works](../c_target/c_target_rulebased/c_target_whoseeswhat.md#concept_014AB6795D2D4B6EB5E45A226A4FF7E9).) 

1. If a form-based activity is the highest priority, then that activity content is returned along with all matching activity content from Visual Experience Composer activities. 

1. If a Visual Experience Composer activity is the highest priority, then content from all matching visual experience composer activities is returned, but no Target Classic or form-based activity content is returned. 

   The results from all activities that run on the page are counted and reflected in the reports. 



**Example** 

If you have two activities, one targeting the branded search keyword Nike and the second targeting the non-branded keyword sneakers, the priorities of both activities are checked. If the Nike activity has a higher priority, that content is displayed. If the sneakers activity has the higher priority, its content is displayed. 

If both targeted activities have the same priority, the activity that was most recently viewed is displayed. If the visitor is new to the page, the activity that was activated most recently is displayed. 

## Target Standard/Premium Form-Based Composer with Non-Global Mboxes {#section_C3F5F09B0B2D4EF795C5929D5C426A8C}


>[!NOTE]
>
>This information also applies to any campaigns running that were created in Target Classic.



If your company uses mboxes other than the global mbox in the form-based composer, content from only one activity can be returned per call. Activity delivery is determined using the following decision flow: 


1. The Target server call comes to Target with information about the mbox and URL. 

1. Target pulls every activity running in that mbox. 

1. Target attempts to match the visitor into the highest priority activity. 

   If the visitor is already in an A/B test or Multivariate Test, they will match into that test until they convert. If they were previously in an experience targeting activity, they must match into it again. If they meet the audience rules, then the visitor falls into those activities and into specific experiences. ([ Information about how experience matching works](../c_target/c_target_rulebased/c_target_whoseeswhat.md#concept_014AB6795D2D4B6EB5E45A226A4FF7E9).) 

1. If multiple activities share the same priority level, then there are two tiebreakers: 


    * If only one activity has audience targeting, that activity is displayed. 

    * If all or none have targeting, then the activity that was approved first is displayed. 





## Examples {#section_F6A788AAC3884A2FA03E47F0557A1213}


>[!NOTE]
>
>Depending on your settings, the priority values vary. You can use the legacy settings of Low, Medium, or High, or you can enable fine-grained priorities from 0 to 999. For more information, see[ Activity Settings](../c_activities/t_activity_settings.md#task_C6B2FF8374724933BE79A83549B9CD02). 



**Two Target Classic campaigns use non-global mboxes ** 


* Campaign 1: homePageHero, offer1, priority high 

* Campaign 2: homePageHero, offer2, priority low 



Response: offer1 

**Two activities use only offers created in the Visual Experience Composer for different selectors** 


* Activity 1: target-global-mbox, selector1, visualExpCompOffer1, priority low 

* Activity 2: target-global-mbox, selector2, visualExpCompOffer2, priority high 



Response: visualExpCompOffer1, visualExpCompOffer2 

**Two activities use only offers created in the Visual Experience Composer for same selector** 


* Activity 1: target-global-mbox, selector1, visualExpCompOffer1, priority low 

* Activity 2: target-global-mbox, selector1, visualExpCompOffer2, priority high 



Response: visualExpCompOffer1, visualExpCompOffer2 


>[!NOTE]
>
>This is the same response as in the second use case above because Target Classic does not handle selector collisions. Target Standard catches such behavior and other use cases when selectors might collide both in DOM and visually (usually done at experience editor level or in campaign simulation mode).



**Two activities use offers created in the Visual Experience Composer and two Target Classic campaigns** 


* Activity 1: target-global-mbox, selector1, visualExpCompOffer1, medium high 

* Activity 2: target-global-mbox, selector2, visualExpCompOffer2, priority low 

* Campaign 1: target-global-mbox, offer1, priority high 

* Campaign 2: target-global-mbox, offer2, priority low 



Response: offer1, visualExpCompOffer2, visualExpCompOffer1 


>[!NOTE]
>
>The order of combined responses is that classic content comes first (only one classic response will be serviced as in use case 1) and then Visual Experience Composer offer responses that are ordered by inverted priority.


