---
keywords: faq;frequently asked questions;analytics for target;a4T;activity setup
description: Find answers to questions about activity setup when using Analytics for Target (A4T). A4T lets you use Analytics reporting for Target activities.
title: Where Can I Find FAQs About Activity Settings with A4T?
feature: Analytics for Target (A4T)
docid: b9b849a5-c2ed-45c8-952e-9f2986a7a056
---

# Activity settings - A4T FAQ

This topic contains answers to questions that are frequently asked about activity setup and using [!DNL Analytics] as the reporting source for [!DNL Target] (A4T).

## Which activity types are support Analytics as the reporting source (A4T)? {#section_5E4F58CD25A5424E869E6FE0803968EF}

For a full list, see "Supported Activity Types" in [Adobe Analytics as the Reporting Source for Adobe Target (A4T)](/help/c-integrating-target-with-mac/a4t/a4t.md#concept_7540C8C04259434AB6EE33B09F47A1DE).

## While configuring my Goal Metics, why can't I access Advanced Settings?

For activities using [!DNL Analytics] as the reporting source (A4T), the the goal metric will always use the "[!UICONTROL Increment Count & Keep User in Activity]" and "[!UICONTROL On Every Impression]" settings. This is *not* configurable. 

For more information, see "While configuring my goal metics, why can't I access the Advanced Settings options?" in [Metric definitions - A4T FAQ](/help/c-integrating-target-with-mac/a4t/r-a4t-faq/a4t-faq-metric-definition.md).

## I just created an activity. Why don't I see any data coming in? {#section_9F8092BE4225442896F926540292F221}

When an activity is created, [!DNL Target] sends a classification file to [!DNL Analytics]. Although [!DNL Analytics] is capturing the and processing the data, it does not show in the reports until the classification file has been updated. This can take up to 24 hours. If after 48 hours you don't see your data, please [contact Client Care](/help/cmp-resources-and-contact-information.md#reference_ACA3391A00EF467B87930A450050077C). Alternately, if you know you will launch an activity, you can create the activity a few days beforehand and the classifications will be sent when the activity is saved. That way, data appears in the reports upon launch. Please note that it takes 45-90 minutes for data to be processed in [!DNL Analytics].

## Why can't I can't select Analytics as my reporting source when I create a new activity? {#section_9F4F69C3085F4C2480AF439127EB27CD}

You can change your [!UICONTROL Reporting Settings] options in [!UICONTROL Administration].

1. In [!DNL Target], click **[!UICONTROL Administration]**. 
1. In the **[!UICONTROL Experience Cloud solution used for reporting]** drop-down list, click **[!UICONTROL Select per Activity]**.

![](assets/select-per-activity.png)

The **[!UICONTROL Reporting Source]** drop-down list is enabled in the **[!UICONTROL Goal & Settings]** screen for creating and editing activities.

To always use [!DNL Analytics] as the reporting source, select **[!UICONTROL Adobe Analytics]** from the drop-down list in [!UICONTROL Administration]. 

## Can a visitor switch between targeted and controlled experiences in different visits in an Auto-Target activity that uses A4T?

The following is true assuming the visitorId does not change for a visitor between visits.

If the traffic-allocation percentage is adjusted mid-activity, it’s possible that a visitor could move between targeted and control experiences. 

If the percentages are not adjusted mid-activity, a visitor who initially sees the control will always be sent to control. A visitor that is sent to targeted experiences will always be sent to targeted experiences. 

* After being in the targeted “bucket” of traffic, the visitor can be sent to a different experience from visit to visit if the machine-learning models determine that a different experience is relevant for the new visit.
* After being assigned to the control "bucket" of traffic, a visitor will always see the same experience because experience assignment is based on a deterministic pseudo-random hash of the visitor's visitorId.
