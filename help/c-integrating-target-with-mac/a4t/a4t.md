---
keywords: a4t;analytics;analytics for target;analytics reporting source;adobe analytics as the reporting source for target
description: Use Analytics for Target (A4T) to create activities based on Analytics conversion metrics and audience segments and use Analytics reports to examine results.
title: What is Analytics for Target (A4T)?
feature: Analytics for Target (A4T)
---

# Adobe Analytics as the reporting source for Adobe Target (A4T)

[!DNL Adobe Analytics for Target] (A4T) is a cross-solution integration that lets you create activities based on [!DNL Analytics] conversion metrics and audience segments. The A4T integration lets you use [!DNL Analytics] reports to examine your results. If you use [!DNL Analytics] as the reporting source for an activity, all reporting and segmentation for that activity is based on [!DNL Analytics] data collection.

## A4T overview {#section_92B66069210C40DBA937790E8CC596CF}

The [!DNL Analytics for Target] integration between [!DNL Analytics] and [!DNL Target] provides powerful analysis and timesaving tools for your optimization program.

The three primary benefits of using [!DNL Analytics] data in [!DNL Target] are:

* Marketers can dynamically apply [!DNL Analytics] success metrics or reporting segments to [!DNL Target] activity reports at any time. It is not required to specify everything before running the activity. 
* A single source of data eliminates the variance that occurs when collecting data in two separate systems. 
* Your existing [!DNL Analytics] implementation collects all required data. There is no need to implement mboxes on pages for the sole purpose of collecting data for reports. Adobe still recommends that you implement an order confirmation mbox for [Automated Personalization](/help/c-activities/t-automated-personalization/automated-personalization.md) (AP) activities.

>[!IMPORTANT]
>
>Before you can begin using A4T, you must request integration provisioning for your account. Use [this form](https://www.adobe.com/go/audiences) to request to be provisioned.
>
>The integration that enables [!DNL Analytics] as the data source for [!DNL Target] (A4T) represents the next generation of the Test&Target to SiteCatalyst plug-in. This plug-in has been deprecated, but is still supported for customers who already use it.

If you use [!DNL Analytics] as the reporting source for an activity, all reporting and segmentation for that activity is based on [!DNL Analytics].

All [!DNL Analytics] metrics, including calculated metrics, are available in [!DNL Target] and the [!UICONTROL Target Activities] report in [!DNL Analytics]. Likewise, any segment available in [!DNL Analytics] can be applied to both solutions. You can apply the metric or audience to the report in [!DNL Target] after the activity has started, or even after the activity has completed.

Every metric is included, including any custom or calculated metrics that are built-in in [!DNL Analytics].

After the classification period, data appears in these reports approximately an hour after it is collected from the website. All metrics, segments, and values in the reports come from the report suite you selected when you set up the activity.

Keep the following points in mind when considering using A4T:

* To use [!DNL Analytics] as the reporting source for [!DNL Target], both you and your company must have access to [!DNL Analytics] and to [!DNL Target]. [Contact your account representative](/help/cmp-resources-and-contact-information.md#concept_34A1CA16F2244D42930BB77846A5ABBB) if you need either solution. 
* The reporting source is set for each activity. [!DNL Target] continues to collect data to use in reporting and [!DNL Target] data is still available if you prefer to base an activity on data collected by [!DNL Target]. 
* Use one reporting source or the other. You cannot collect data for a single activity from both sources. 
* When using A4T, all success metrics available to your activities are [!DNL Analytics] metrics. However, your goal metric can be based on an mbox call. For example, you can use Target's out-of-the-box click-tracking capabilities with A4T instead of having to implement [!DNL Analytics] click-tracking code. 
* When viewing reporting of an A4T activity in the [!DNL Target] UI, you are viewing [!DNL Analytics] data. For example, if you use the [!UICONTROL Visitor] metric in [!DNL Target], you are using the [!DNL Analytics] [!UICONTROL Visitor] metric, not the [!DNL Target] [!UICONTROL Visitors] metric, which is now called [!UICONTROL Entrants]. This difference is especially important for basic traffic metrics ([!UICONTROL Visitors], [!UICONTROL Visits], [!UICONTROL Page Views]) and conversion metrics. 
* Any existing [!DNL Target] activities continue to use [!DNL Target] data collection and are not affected by enabling A4T. 
* Only one mbox-based metric is allowed when using [!DNL Analytics] as the reporting source. 
* A server-to-server call from [!DNL Target] to [!DNL Analytics] sends activity and experience information to [!DNL Analytics]. This integration does not result in more server calls for either [!DNL Target] or [!DNL Analytics]. 

  In some situations, the classifications from [!DNL Target] to [!DNL Analytics] fail and activities do not show data in [!DNL Analytics]. See [Troubleshoot the Analytics and Target integration (A4T)](/help/c-integrating-target-with-mac/a4t/c-a4t-troubleshooting/a4t-troubleshooting.md). You can also [contact Client Care](/help/cmp-resources-and-contact-information.md#concept_34A1CA16F2244D42930BB77846A5ABBB) for further assistance.

## Supported activity types {#section_F487896214BF4803AF78C552EF1669AA}

The following table shows you which activity types support [!DNL Analytics] as the reporting source in [!DNL Target] (A4T):

| Activity Types | A4T Compatible? | Notes, if applicable |
|--- |--- |--- |
|A/B activity with manual traffic split|Yes||
|A/B activity with Auto-Allocate|Yes|See [A4T support for Auto-Allocate and Auto-Target activities](/help/c-integrating-target-with-mac/a4t/a4t-at-aa.md)|
|A/B activity with Auto-Target|Yes|See [A4T support for Auto-Allocate and Auto-Target activities](/help/c-integrating-target-with-mac/a4t/a4t-at-aa.md).|
|Experience Targeting (XT)|Yes||
|Multivariate test (MVT)|Yes|Requires mbox-based goal metric goal to get the [!UICONTROL Element Contribution] report. The [!UICONTROL Element Contribution] report does not currently support [!DNL Analytics] metrics.|
|Automated Personalization (AP) activity|No||
|Recommendations activity|Yes||
|Mobile App|Yes|Supported with the Mobile Services SDK, version 4.13.1 or later. For more information, see the [Mobile Services documentation](https://experienceleague.adobe.com/docs/mobile-services/using/home.html).|
|Email|No||
|Server-Side Delivery API|Yes|For more information, see [Server Side: implement Target](/help/c-implementing-target/c-api-and-sdk-overview/api-and-sdk-overview.md).|
|NodeJS SDK|Yes|For more information, see [Server Side: implement Target](/help/c-implementing-target/c-api-and-sdk-overview/api-and-sdk-overview.md).|
|AEM 6.1 (or earlier) Cloud Service Integration|No||
|AEM 6.2 (or later) Cloud Service Integration|Yes|For more information, see [Integrating with Adobe Target](https://helpx.adobe.com/experience-manager/6-2/sites/administering/using/target.html) in the [!DNL Adobe Experience Manager] 6.2 documentation.|
|Any activity using a redirect offer|Yes|There are stricter minimum requirements for using redirect offers with A4T. For more information, see [Redirect Offers - A4T FAQ](/help/c-integrating-target-with-mac/a4t/r-a4t-faq/a4t-faq-redirect-offers.md).|
|Node.JS|Yes|For more information, see [Node.js SDK](https://adobetarget-sdks.gitbook.io/docs/sdk-reference-guides/nodejs-sdk) in the *Adobe Target SDKs* guide.|
|Java SDK|Yes|For more information, see [Java SDK](https://adobetarget-sdks.gitbook.io/docs/sdk-reference-guides/java-sdk) in the *Adobe Target* SDKs guide.|

Because all activity types do not yet support A4T, it is recommended that you keep or implement important conversion mboxes, such as the `orderConfirmPage` mbox.

## Examples of A4T reports {#section_F0A43A1CB2F04E8282B909E4D7034361}

To view A4T reports in [!DNL Target], click **[!UICONTROL Activities]**, click the desired activity from the list that uses [!DNL Analytics] as its reporting source, then click the **[!UICONTROL Reports]** tab.

>[!NOTE]
>
>You can use the [!UICONTROL Reporting Source] drop-down list at the top of the [!UICONTROL Activities] page to display only activities that use [!DNL Analytics] as the reporting source.

You can toggle between the [!UICONTROL Table View] and [!UICONTROL Graph View] of the report by clicking the appropriate icon at the top-right side of the report.

The following illustration shows the [!UICONTROL Graph View] of an A4T report with the [!UICONTROL Report Metric] drop-down list displaying the available [!DNL Analytics] goal metrics:

![](assets/a4t_report_graph1.png)

The following illustration shows the [!UICONTROL Graph View] of an A4T report with the [!UICONTROL Audience] drop-down list displaying the available [!DNL Analytics] audiences:

![](assets/a4t_report_graph2.png)

The following illustration shows the [!UICONTROL Table View] of an A4T report:

![](assets/a4t_report_table.png)

To view the report in [!DNL Analytics] rather than in [!DNL Target], click **[!UICONTROL View in Analytics]** along the top of the report. 

## Analytics & Target: Best Practices for Analysis Tutorial {#section_3438E6E77A464424B717A4FD333B84B2}

Open the [Analytics & Target: Best Practices for Analysis](https://spark.adobe.com/page/Lo3Spm4oBOvwF/) tutorial, provided by [!DNL Adobe Experience League].

## Training videos:

The following videos contain more information about the concepts discussed in this topic.

### Analytics for Target (A4T) (4:32) ![Overview badge](/help/assets/overview.png)

This video explains how to use [!DNL Analytics] as a reporting source in [!DNL Target] to drive the analysis of your optimization program.

* Explain what A4T is and why you would use it 
* Explain how A4T works 
* Understand the prerequisites needed before using A4T

>[!VIDEO](https://video.tv.adobe.com/v/17384)

### Analytics / Target Integration (A4T) (40:33) ![Tutorial badge](/help/assets/tutorial.png)

This video is a recording of " [Office Hours](/help/cmp-resources-and-contact-information.md#concept_58EA30379D3B48C4848BA2A8C464A5B7)," an initiative led by the Adobe Customer Care team.

* How to set up and validate that the integration is working 
* How the integration works 
* Learn about the ideal reports to use in Analytics 
* Answers to common questions about A4T

[Analytics/Target Integration (A4T) Office Hours](https://helpx.adobe.com/customer-care-office-hours/target/analytics-target-A4T-integration.html)
