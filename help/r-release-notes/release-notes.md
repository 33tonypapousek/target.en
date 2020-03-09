---
keywords: Release notes;new features;releases;updates;update;release;enhancement;enhancements;fixes;bug fixes;updates
description: These release notes provide information about features, enhancements, fixes, and known issues for each Adobe Target Standard and Target Premium release.
title: Adobe Target release notes (current) 
topic: Recommendations
uuid: f6c3e64d-de1e-416c-a56f-2122a58b613e
---

# Target release notes (current){#target-release-notes-current}

These release notes provide information about features, enhancements, and fixes for each Target Standard and Target Premium release. In addition, release notes for Target APIs, SDKs, the JavaScript library (at.js), and other platform changes are also included, when applicable.

>[!NOTE]
>
>* **TLS support changes**: Starting on March 1, 2020, Target will disable support for TLS 1.1 and TLS 1.0 encryption. Transport Layer Security (TLS) is the most-widely deployed security protocol used today for web browsers and other applications that require data to be securely exchanged over a network. This change is needed to meet the generally accepted security compliance standard of TLS 1.2 or higher. Check which TLS version you are currently using. If your version is lower than 1.2, implement the required changes prior to March 1, 2020 in order to continue to use Target as expected.
>
>   For detailed information on the possible impact and the steps you might need to take to update your implementation, see [TLS (Transport Layer Security) encryption changes](/help/c-implementing-target/c-considerations-before-you-implement-target/tls-transport-layer-security-encryption.md).
>
>* **mbox.js deprecation**: On August 30, 2020, Adobe Target will no longer support the mbox.js library. Post August 30, 2020, all calls made from mbox.js will fail and impact your pages that have Target activities running. We recommend that all customers migrate to the most recent version of the at.js library before this date to avoid any potential issues with your sites. For more information, see [How At.js Works](/help/c-implementing-target/c-implementing-target-for-client-side-web/c-how-atjs-works/how-atjs-works.md).
>
>   Although, mbox.js is currently supported, we have not provided feature updates to this library since July 2017. The newer at.js provides many advantages over mbox.js. Among other benefits, at.js improves page load times for web implementations, improves security, and provides better implementation options for single page applications.
>
>   By moving all customers to at.js, our engineers and support staff will be able to provide you with new functionality and offer the support you have come to expect from Adobe.
>
>* The issue numbers in parentheses are for internal [!DNL Adobe] use.

## Target Standard/Premium 20.2.1 (To Be Determined)

Check back here for the exact date when that information becomes available.

>[!IMPORTANT]
>
>See the information above about the deprecation of mbox.js.

This release contains the following enhancements, fixes, and changes:

* Fixed an issue that prevented customers from selecting a collection when performing a catalog search. (TGT-36230)
* Fixed an issue in which a criteria created via API, but not referenced by an activity created in the Target UI, could be erroneously deleted from the UI. (TGT-35917)
* Implemented security improvements to the Content Security Policy (CSP). (TGT-36190)
* Fixed an issue that caused "NaN%" to display when sliding the Attribute Weighting percentage bar to the far left. (TGT-36211)
* Resolved localization issues so that UI text in various languages displays correctly.
* The following Adobe Analytics metrics are no longer supported for Analytics for Target (A4T) effective with the March 2020 Target release:
  * averagevisitdepth
  * bots
* The following metrics are no longer supported and are automatically converted to new versions of the metric the first time a user modifies an activity containing the metric:

  |Deprecated Metric|New Metric|
  |--- |--- |
  |`averagetimespentonpage`|`averagetimespentonsite` (note: measured in minutes rather than seconds)|
  |`instances`|`occurrences`|
  |`singleaccess`|`singlepagevisits`|
  |`uniquevisitors`|`visitors`|
  |`visitorsdaily`, `visitorshourly`, `visitorsmonthly`, `visitorsquarterly`, `visitorsweekly`, `visitorsyearly`|`visitors`|

## Adobe Experience Cloud navigation (February 22, 2019)

* When you log in to the [!DNL Adobe Experience Cloud], you will be taken to the new header navigation. It looks very similar to the previous navigation with the black bar at the top, but it provides the following improvements:

  * Easier switching between [!DNL Identity Management System] (IMS) organizations or to a different solution.
  * Improved user help: Search results include results from the [!DNL Target] product documentation, as well as community forums and more video content, giving you easier access to more content to help get the most out [!DNL Target]. We’ve also added a feedback mechanism right in the [!UICONTROL Help] menu, making it easier to report issues or to share your ideas.

  * Improved Net Promoter Score (NPS) feedback functionality, so the survey modal doesn’t disturb your flow of work.
  * Improved log-in flow. Previously, all [!DNL Target] customers landed on the Target landing page after clicking the [!DNL Target] icon in the header. This page then allowed customers to proceed forward with [!DNL Target Standard/Premium], [!DNL Search&Promote], or [!DNL Recommendations Classic],  as shown below:

    ![Landing page](/help/r-release-notes/assets/landing.png)
  
    We eliminated this landing page for all our customers. You are now always taken directly to the [!UICONTROL Activities List] page by clicking the [!DNL Target] icon in the new header navigation bar. 
    
    If you use [!DNL Recommendations Classic], you can either go directly to the solution or you can go from the short link created on the [!UICONTROL Recommendations] tab, as shown below:

    ![Recs Classic deep link](/help/r-release-notes/assets/recs-classic.png)
    
    If you use [!DNL Search&Promote], you need to go directly to the [Search&Promote URL](https://center.atomz.com/center/?ims=1) (https://center.atomz.com/center/?ims=1). The path to reach [!DNL Search&Promote] from inside of [!DNL Adobe Target] has been removed completely.
    
  * Notifications for [!DNL Target] are not currently available in the [!UICONTROL Notifications] drop-down in the header.

  >[!NOTE]
  >
  >As part of the rollout of the new navigation bar, you will also notice some URL changes. All previous bookmarked links continue to work but we encourage you to bookmark new links for faster opening.

## Additional release notes and version details

|Resource|Details|
|--- |--- |
|[Release notes - Target server-side APIs](/help/c-implementing-target/c-api-and-sdk-overview/releases-server-side.md)|Release notes related to Adobe Target's server-side APIs.|
|[Release notes - Target Node.js SDK](/help/c-implementing-target/c-api-and-sdk-overview/releases-nodejs.md)|Release notes related to Adobe Target's Node.js SDK.|
|[Release Notes - Target Java SDK](/help/c-implementing-target/c-api-and-sdk-overview/releases-target-java-sdk.md)|Release notes related to Adobe Target's Java SDK.|
|[at.js version details](/help/c-implementing-target/c-implementing-target-for-client-side-web/target-atjs-versions.md)|Details about changes in each version of the Adobe Target at.js JavaScript library.|
|[mbox.js version details](/help/c-implementing-target/c-implementing-target-for-client-side-web/t-mbox-download/mboxjs-change-log.md)|This page shows changes to each version of mbox.js.<br>Note that the mbox.js library is no longer being developed. All customers should migrate from mbox.js to at.js.|

## Documentation Changes, Past Release Notes, and Experience Cloud Release Notes {#section_1BC5F5208DA548E9B4344A0836E4B943}

In addition to the notes for each release, the following resources provide additional information:

|Resource|Details|
|--- |--- |
|Documentation changes|View detailed information about updates to this guide that might not be included in these release notes.<br>For more information, see [Documentation Changes](../r-release-notes/doc-change.md#reference_366123CF00994BACBBF9BBDF2C4D840C).|
|Release notes for previous releases|View information about new features and enhancements in previous releases of Target Standard and Target Premium.<br>For more information, see [Release notes for previous releases](../r-release-notes/release-notes-for-previous-releases.md).|
|Adobe Experience Cloud release notes|View the latest release notes for the Adobe Experience Cloud solutions.<br>For more information, see [Experience Cloud Release Notes](https://docs.adobe.com/content/help/en/release-notes/experience-cloud/current.html).|

## Prerelease Information {#section_5D588F0415A2435B851A4D0113ACA3A0}

The following resources let you see what's coming in the next Target release.

|Resource|Details|
|--- |--- |
|Adobe Priority Product Update list|To receive advance notifications about upcoming product enhancements to Target and other Adobe Experience Cloud solutions, sign up for the Adobe Priority Product Update:<br>[https://www.adobe.com/subscription/priority-product-update.html](https://www.adobe.com/subscription/priority-product-update.html)|
|Upcoming release notes|For information about the current month's Target releases, including prerelease information, see the [Target Release Notes - Prerelease](/help/r-release-notes/target-release-notes.md) page.|
