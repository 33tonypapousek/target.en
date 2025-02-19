---
keywords: partial data;partial-data;A4T;discrepancies;analytics for target;orphaned;virtual report suite;phantom;troubleshooting;unstitched;inflated;unspecified
description: Learn how to minimize the effects of inflated Visit and Visitor counts when using Analytics for Target (A4t). Learn what "partial data" is and how to reduce it.
title: How Do I Minimize Inflated Visit and Visitor Counts in A4T?
feature: Analytics for Target (A4T)
---

# Minimizing inflated visit and visitor counts in A4T{#minimizing-inflated-visit-and-visitor-counts-in-a-t}

Information to help you minimize the effects of inflated Visit and Visitor counts when using [!DNL Adobe Analytics] as the reporting source for [!DNL Adobe Target] (A4T).

>[!IMPORTANT]
>On November 14, 2016, Adobe Analytics changed the way some data is processed for customers using Analytics reporting for Target (A4T). These changes bring Adobe Target data into better alignment with the data model for Adobe Analytics . These changes were rolled out for all customers using A4T. These changes specifically address an issue where some customers have noticed an inflated visitor count when Target activities are running.
>
>This change is not retroactive. If your historical reports show inflated counts, and you would like to exclude them from your reports, you can create a virtual report suite, as explained below.
>
>Also, several JavaScript libraries have been updated to help minimize inflated counts. Adobe recommends that you upgrade to the following library versions (or newer):
>
>* Experience Cloud Visitor ID Service: visitorAPI.js version 2.3.0 or later.
>* Adobe Analytics: appMeasurement.js version 2.1.
>* Adobe Target: at.js version 0.9.6 or later (except version 1.1.0 if using redirect offers with A4T).
>
>  The mbox.js library does not support redirect offers with A4T. Your implementation must use at.js.

## What changed? {#section_9CCF45F5D66D48EBA88F3A178B27D986}

When [!DNL Adobe Analytics] is used to measure [!DNL Target] activities (called A4T), [!DNL Analytics] collects extra data that is not available when there is no [!DNL Target] activity on the page. The [!DNL Target] activity fires a call at the top of the page, but [!DNL Analytics] typically fires its data collection calls at the bottom of the page. In the implementation of A4T to date, Adobe includes this additional data whenever a [!DNL Target] activity was active. Going forward, Adobe includes this additional data only when both the [!DNL Target] and [!DNL Analytics] tags have fired.

## Why did Adobe make this change? {#section_92380A4BD69E4B8886692DD27540C92A}

Adobe prides itself on data accuracy and quality. When the [!DNL Target] tag fires, but the [!DNL Analytics] tag does not, Analytics records “partial data” (sometimes called "unstitched hits"). These unstitched hits would not be captured by [!DNL Analytics] if there was no [!DNL Target] activity. Although including this partial data in [!DNL Analytics] reporting provides additional information, it also creates inconsistency with historical data from periods when there were no [!DNL Target] activities running. This situation can cause problems for [!DNL Analytics] users who are analyzing trends over time. In the interest of ensuring data consistency in [!DNL Analytics], Adobe excludes all partial data.

## What contributes to partial data? {#section_C9C906BEAA7D44DAB9D3C03932A2FEB8}

Adobe has encountered some customers with high rates of partial data in [!DNL Analytics]. High rates of partial data can result from improper implementation, but there are legitimate causes as well.

The identified causes of partial data include the following:

* **Misaligned report suite IDs (Implementation):** The report suite specified during activity setup does not match the report suite on the page where the test is delivered. The data cannot be reconciled on [!DNL Analytics] servers, so it looks like partial data. 
* **Slow pages:** [!DNL Target] calls are at the top of the page and [!DNL Analytics] calls are typically at the bottom of the page. If the page loads slowly, it increases the likelihood of a visitor leaving the page after the [!DNL Target] call fires, but before the [!DNL Analytics] call. Slow pages can be especially problematic on mobile web sites where connections are often slower. 
* **Page errors:** If there are JavaScript errors or other scenarios where each of the touchpoints do not fire (Experience Cloud ID service, Target, and Analytics), partial data results. 
* **Redirect offers in [!DNL Target] activity:** For redirect offers in activities using A4T, your implementation must meet certain minimum requirements. In addition, there is important information that you must know. For more information, see [Redirect Offers - A4T FAQ](/help/c-integrating-target-with-mac/a4t/r-a4t-faq/a4t-faq-redirect-offers.md#section_FA9384C2AA9D41EDBCE263FFFD1D9B58).
* **Old versions of the libraries:** Over the past year Adobe has made several improvements to the JavaScript libraries ( [!DNL appMeasurement.js], `at.js/mbox.js`, and `visitorAPI.js`) to make sure that data is sent as efficiently as possible. To learn more about implementation requirements, see [Before You Implement](/help/c-integrating-target-with-mac/a4t/before-implement.md#concept_046BC89C03044417A30B63CE34C22543).

## What are the best practices to reduce partial data? {#section_065C38501527451C8058278054A1818D}

Review the following steps to reduce partial data collection:

| Step | Task |
| --- | --- |
| ![Step 1](assets/step1_icon.png) | Ensure that the report suite selected in [!DNL Target] is the same as the one on the pages where the activity is presented.|
| ![Step 2](assets/step2_icon.png) | Ensure that the visitorAPI.js, appMeasurement.js, at.js / mbox.js libraries are on A4T-compatible versions. To learn more about implementation requirements, see [Before You Implement](/help/c-integrating-target-with-mac/a4t/before-implement.md). |
| ![Step 3](assets/step3_icon.png) | Ensure that the SDID is getting set on all [!DNL Target] and [!DNL Analytics] calls leaving the page and that they match.<br/>Use a network analyzer or debugging tool to ensure that the `mboxMCSDID` parameter on [!DNL Target] calls matches the SDID parameter in the [!DNL Analytics] call. |
| ![Step 4](assets/step4_icon.png) | Confirm that the implementation libraries load in the correct order on your sites. For more information, see [Analytics for Target Implementation](/help/c-integrating-target-with-mac/a4t/a4timplementation.md).|

## How can I see how much partial data I have? {#section_89B663E2824A4805AB934153508A0F4B}

Although this information is not available directly in [!DNL Analytics], you can contact Adobe Customer Care to retrieve a Partial Data report. This report is intended to aid in debugging.

## How can I view historical trends without partial data? {#section_4C9DED560FAD4428B362DDA2064897C3}

This processing change affects data only after the release date (November 14, 2016). If you want to adjust your historical metrics to match, Adobe recommends that you create a segment to exclude partial data.

The following information relating to this change includes instructions to help you define the segment and apply it to a virtual report suite so that this segment is always applied to your [!DNL Analytics] views.

In most situations, a [!DNL Target] hit is stitched with an  [!DNL Analytics] hit on each webpage. This stitching happens if there is a consistent SDID in both the  [!DNL Target] and [!DNL Analytics] call and a [!DNL Experience Cloud ID] (MCID) in the  [!DNL Analytics] call on the same page. [!DNL Target] typically has the MCID as well, but if the call to [!DNL Target] happens before the visitor ID returns, the hit is still stitched because of the SDID. Also, the user must remain on the page long enough to fire an  [!DNL Analytics] call after a  [!DNL Target]&nbsp;call was fired. This scenario is ideal.

**Partial-data hits:** Users sometimes don't remain on a page long enough to send an [!DNL Analytics] call, but [!DNL Target] has a proper MCID. This scenario results in partial-data hits (hits with no [!DNL Analytics] page view). If these users come back to your site and view a page containing [!DNL Analytics] code, they are properly counted as returning visitors. These hits would have been lost if you had only [!DNL Analytics] code on the page. Some clients don't want data for these hits because they inflate certain metrics (visits) and deflate other metrics (page views per visit, time per visit, and so forth). You also see visits without any page views. However, there are still valid reasons for keeping this data.

To minimize partial-data hits, you can make your page load faster, update to the latest versions of the libraries, or create a [virtual report suite](https://experienceleague.adobe.com/docs/analytics/components/virtual-report-suites/vrs-workflow/vrs-create.html) that excludes those hits. For step-by-step instructions, see [Create virtual report suites](https://experienceleague.adobe.com/docs/analytics/components/virtual-report-suites/vrs-workflow/vrs-create.html) in the *Analytics Components Guide*.

The following illustration shows for the segment definition for the virtual report suite:

![](assets/ts_a4t.png)

When creating the virtual report suite, specify the following configuration for the segment definition (as shown in the above illustration):

*   **Show Hit:**
*   Analytics for Target: Exists
*   And
*   Page Views: Does not exist
*   And
*   Custom Link Instances: Does not exist
*   And
*   Download Link Instances: Does not exist
*   And
*   Exit Link Instances: Does not exist

**Orphaned hits:&nbsp;** In fewer situations, users don't remain on the page long enough for an Analytics call and Target didn't get a proper MCID. These hits are what Adobe defines as "orphaned" hits. These hits represent customers that rarely return and they inflate visit and visitor counts inappropriately.

To minimize these "orphaned" hits, you can create a [virtual report suite](https://experienceleague.adobe.com/docs/analytics/components/virtual-report-suites/vrs-workflow/vrs-create.html) that excludes those hits, as explained above.

## What does this mean for my [!DNL Target] reporting? {#section_AAD354C722BE46D4875507F0FCBA5E36}

Once this change occurs, you might see a decrease in new visitors and visits to live tests because [!DNL Adobe] does not process incoming partial data. Conversions and hits to other [!DNL Analytics] metrics will not change. 
