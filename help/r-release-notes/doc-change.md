---
description: This page lists important changes made to the Target documentation.
keywords: target documentation change log;documentation updates
seo-description: This page lists important changes made to the Target documentation.
seo-title: Documentation changes
solution: Target
title: Documentation changes
topic: Standard
uuid: 6fba75e2-0a93-488d-9010-fffa423600c0
---

# Documentation changes{#documentation-changes}

This page lists important changes made to the [!DNL Adobe Target] documentation.

## Adobe Target Standard/Premium 19.3.1 (March 29, 2019) {#section-19-3-1}

|Date|Topic|Changes|
| --- | --- | --- |
|April 15, 2019|[Initial provisioning - A4T FAQ](/help/c-integrating-target-with-mac/a4t/r-a4t-faq/a4t-faq-initial-provisioning.md)|Added new FAQ: "How can I capture Analytics events across multiple pages and associate them with an A4T activity in Target?"|
||[User permission requirements](/help/c-integrating-target-with-mac/a4t/account-reqs.md)|Updated topic.|
|April 11, 2019|[adobe.target.getOffers(options) - at.js 2.x](/help/c-implementing-target/c-implementing-target-for-client-side-web/adobe-target-getoffers-atjs-2.md)|Updated code samples.|
||[Visual Experience Composer helper extension](/help/c-experiences/c-visual-experience-composer/r-troubleshoot-composer/vec-helper-browser-extension.md)|Added screenshots.|
||[Auto-Allocate](/help/c-activities/automated-traffic-allocation/automated-traffic-allocation.md)|Added the following FAQ: "Should I remove an underperforming experience from an Auto-Allocate activity to speed the process of determining a winner?"|
|April 10, 2019|[Before you implement](/help/c-integrating-target-with-mac/a4t/before-implement.md)|Minor text updates to the "Implementation requirements" section (requirements reordered).|
||[adobe.target.triggerView (viewName, options) - at.js 2.x](/help/c-implementing-target/c-implementing-target-for-client-side-web/adobe-target-triggerview-atjs-2.md)|Updated text for the "options > page" parameter.|
|April 8, 2019|[Expected data variances between Target and Analytics when using and not using A4T](/help/c-integrating-target-with-mac/a4t/understanding-expected-data-variances.md)|Updated [Expected data variance when using A4T](/help/c-integrating-target-with-mac/a4t/understanding-expected-data-variances.md#expected-using-a4t). |
||[Minimizing inflated visit and visitor counts in A4T](/help/c-integrating-target-with-mac/a4t/c-a4t-troubleshooting/minimizing-inflated-visit-and-visitor-counts-a4t.md)|Updated information about A4T and redirects under [What contributes to partial data?](/help/c-integrating-target-with-mac/a4t/c-a4t-troubleshooting/minimizing-inflated-visit-and-visitor-counts-a4t.md#section_C9C906BEAA7D44DAB9D3C03932A2FEB8)|
||[Before you implement](/help/c-integrating-target-with-mac/a4t/before-implement.md#section_A0D2EF18033D4C3997B08A6EBB34C17A)|Updated the mininum requirements to use A4T with redirects (at.js version 1.6.2).|
||[Redirect offers - A4T FAQ](/help/c-integrating-target-with-mac/a4t/r-a4t-faq/a4t-faq-redirect-offers.md#section_FA9384C2AA9D41EDBCE263FFFD1D9B58)|<ul><li>Updated the mininum requirements to use A4T with redirects (at.js version 1.6.2).</li><li>Added information describing how data metrics are counted when a Target hit occurs, but no Analytics hit occurs. </li>|
||[Limits](/help/r-troubleshooting-target/target-limits.md#excludedid)|Added information about the limits for the `excludedIDs` mbox parameter.|
||[Upgrading from at.js 1.x to at.js 2.x](/help/c-implementing-target/c-implementing-target-for-client-side-web/upgrading-from-atjs-1x-to-atjs-20.md#response-tokens)|Added new section: Response tokens.|
|April 5, 2019|[Adobe Target Basics Webinar: Introduction to Recommendations](/help/c-recommendations/recommendations.md#intro-to-recs)|Added link to the "Introduction to Recommendations" webinar recording.|
||[Activity QA bookmarklet](/help/c-activities/c-activity-qa/activity-qa-bookmark.md)|Updated JavaScript code for the activity QA bookmarklet.|
||[Target release notes (prerelease)](/help/r-release-notes/target-release-notes.md)|Updated the preliminary release notes for the Target 19.4.1 and Target 19.4.2 releases, both scheduled for April 2019.|
|April 4, 2019|[Target release notes (prerelease)](/help/r-release-notes/target-release-notes.md) |Added preliminary release notes for the Target 19.4.1 and Target 19.4.2 releases, both scheduled for April 2019.|
|March 30, 2019|[Limits](/help/r-troubleshooting-target/target-limits.md#excludedid)|Added information about the limits for the `excludedID` mbox parameter.|
|March 29, 2019|[Known issues and resolved issues](/help/r-release-notes/known-issues-resolved-issues.md)|Added the following known issue: "For the Single Page Application (SPA) websites, cancelling loading does not allow you to edit actions under the [!UICONTROL Modifications] panel."<br>Moved the following known issue to the Resolved Issues section: "v1 version of the Offer APIs on Adobe I/O treats all offers created through Target to be in the default workspace."|
|March 28, 2019|[Visual Experience Composer (VEC)](/help/c-experiences/c-visual-experience-composer/visual-experience-composer.md)|Added the following new sections:<ul><li>[Cancel loading of a page within the VEC.](/help/c-experiences/c-visual-experience-composer/visual-experience-composer.md#cancel-loading)</li><li>[Edit a page while the page is loading or after the page fails to load](/help/c-experiences/c-visual-experience-composer/visual-experience-composer.md#loading).</li></ul>|
||[Visual Experience Composer options](/help/c-experiences/c-visual-experience-composer/viztarget-options.md)|New section: "[Navigate elements using the DOM path](/help/c-experiences/c-visual-experience-composer/viztarget-options.md#dom-path)."|
||[Known issues and resolved issues](/help/r-release-notes/known-issues-resolved-issues.md#cancel)|Added a current known issue about when you cancel loading of a page within the VEC.|
||[Release Notes](/help/r-release-notes/release-notes.md): 19.3.1|This release includes enhancements and fixes. You can read about them and link to the documentation from the Release Notes. This release also includes many documentation updates throughout the help.|

## Adobe Target Standard/Premium 19.2.1 (February 19, 2019) {#section-19-2-1}

|Date|Topic|Changes|
| --- | --- | --- |
|March 20, 2019|[at.js Frequently Asked Questions](/help/c-implementing-target/c-implementing-target-for-client-side-web/c-target-atjs-faq/target-atjs-faq.md)|Updated the following FAQ: "[Can I load the Target library asynchronously?](/help/c-implementing-target/c-implementing-target-for-client-side-web/c-target-atjs-faq/target-atjs-faq.md#section_AB9A0CA30C5440C693413F1455841470)"|
||[Real-time profile syncing for mbox3rdPartyID](/help/c-target/c-visitor-profile/3rd-party-id.md)|Added note at the bottom of the page.|
||[Limits](/help/r-troubleshooting-target/target-limits.md)<br>[Custom entity attributes](/help/c-recommendations/c-products/custom-entity-attributes.md#limits)|Added information about "entity custom attribute" limits.|
||[Targets and audiences FAQ](/help/c-target/c-troubleshooting-targets-and-audiences/troubleshooting-targets-and-audiences.md#strings-that-represent-numbers)|Updated text.|
||[Create new criteria](/help/c-recommendations/c-algorithms/create-new-algorithm.md#custom)|Added new section that explains how to create profile-based groupings for popularity algorithms: "Use a custom recommendations key."|
|March 19, 2019|[Target release notes (current)](/help/r-release-notes/release-notes.md)|Added information about at.js versions 2.0.1 and 1.7.1.|
||[View reports - A4T FAQ](/help/c-integrating-target-with-mac/a4t/r-a4t-faq/a4t-faq-viewing-reports.md)|Added the following FAQ: "Does A4T support virtual report suites?"|
|March 18, 2019|[Target release notes (prerelease)](/help/r-release-notes/target-release-notes.md) and [at.js version details](/help/c-implementing-target/c-implementing-target-for-client-side-web/target-atjs-versions.md)|Added information about at.js versions 2.0.1 and 1.7.1.|
||[Methods to get data into Target](/help/c-implementing-target/c-considerations-before-you-implement-target/c-methods-to-get-data-into-target/methods-to-get-data-into-target.md#section_92AB4820A5624C669D9A1F1B6220D4FA) and [Customer attributes](/help/c-target/c-visitor-profile/working-with-customer-attributes.md)|Added: You cannot send the following characters in `mbox3rdPartyID`: plus sign (+) and forward slash (/).|
|March 15, 2019|[Before you implement](/help/c-implementing-target/c-considerations-before-you-implement-target/considerations-before-you-implement-target.md)|Added important note: Modifications to at.js or mbox.js will not be supported by Adobe Customer Care.|
|March 14, 2019|[Target release notes (prerelease)](/help/r-release-notes/target-release-notes.md)|Changed the date of the Target Standard/Premium 19.3.1 release to March 29, 2019.|
|March 13, 2019|[Create an Automated Personalization activity](/help/c-activities/t-automated-personalization/create-ap-activity.md)|Updated the text in the Conversion Metric row.|
||[Profile attributes](/help/c-target/c-visitor-profile/profile-parameters.md)|Added new section: "JavaScript reference for script profile parameters."|
||[at.js functions](/help/c-implementing-target/c-implementing-target-for-client-side-web/cmp-atjs-functions.md)|Restructured page and created new pages for each at.js function to make accessing information easier.|
||[How at.js works](/help/c-implementing-target/c-implementing-target-for-client-side-web/c-how-atjs-works/how-atjs-works.md)|Added introductory paragraph to explain a client-side implementation.|
||[Recommendations FAQ](/help/c-recommendations/c-recommendations-faq/recommendations-faq.md)|Added following FAQ: "Can I dynamically exclude an entity?"|
|March 12, 2019|[Upgrading from at.js 1.x to at.js 2.x](/help/c-implementing-target/c-implementing-target-for-client-side-web/upgrading-from-atjs-1x-to-atjs-20.md) and [Debug at.js using the Adobe Experience Cloud Debugger](/help/c-implementing-target/c-implementing-target-for-client-side-web/c-target-debugging-atjs/target-debugging-atjs.md)|The Debugger is now a supported integration with at.js 2.x.|
|March 11, 2019|[Target release notes (current)](/help/r-release-notes/release-notes.md),<br>[Target release notes (prerelease)](/help/r-release-notes/target-release-notes.md), and <br>[TLS (Transport Layer Security) encryption changes](/help/c-implementing-target/c-considerations-before-you-implement-target/tls-transport-layer-security-encryption.md)|Updated text to indicate that TLS changes will occur on **April 1, 2019**.|
||[adobe.target.getOffers](/help/c-implementing-target/c-implementing-target-for-client-side-web/adobe-target-getoffers-atjs-2.md)|Added the following section: "Fetch and render data from multiple mboxes via getOffers() and applyOffers()."|
|March 6, 2019|[Upgrading from at.js 1.x to at.js 2.x](/help/c-implementing-target/c-implementing-target-for-client-side-web/upgrading-from-atjs-1x-to-atjs-20.md)|Added at_property row to the  "at.js 1.x parameters to at.js 2.x payload mapping" table.|
||[Single Page Application implementation](/help/c-implementing-target/c-implementing-target-for-client-side-web/how-to-deployatjs/target-atjs-single-page-application.md)|Added new section: "Use TriggerView to ensure that A4T works correctly with at.js 2.x and SPAs."|
|March 4, 2019|[Recommendations Classic documentation](/help/c-recommendations/recommendations-classic-documentaton.md)|New topic.|
||[Recommendations Classic versus Recommendations activities in Target Premium](/help/c-recommendations/c-recommendations-faq/recommendations-classic-versus-recommendations-activities-target-premium.md)|Added information about Recommendations as an offer.|
|February 28, 2019|[Activities](/help/c-activities/activities.md)|Updated text and images.|
||[Introduction to Target](/help/c-intro/intro.md)|Added "Recommendations as an offer" under "Target Premium."|
||[Target key concepts](/help/c-intro/target-key-concepts.md)|Updated "Activity Types" table.|
|February 26, 2019|[Known issues and resolved issues](/help/r-release-notes/known-issues-resolved-issues.md)|Added a known issue about Enterprise Permissions support in Target APIs.|
|February 25, 2019|[Target release notes (current)](/help/r-release-notes/release-notes.md), <br>[Target release notes (prerelease)](/help/r-release-notes/target-release-notes.md), and <br>[TLS (Transport Layer Security) encryption changes](/help/c-implementing-target/c-considerations-before-you-implement-target/tls-transport-layer-security-encryption.md)|Updated the following information:<br>On February 20, 2019, Adobe Target infrastructure was upgraded in the EMEA, Japan, and APAC regions to no longer collect data from end users with older devices or web browsers that do not support TLS 1.1 or later. This same upgrade is planned for the North America region on **March 4, 2019**. Migrating to TLS 1.2 provides improved security. It is important that you go through the specifics and plan out the changes for a smooth transition. |
||[Upgrading from at.js 1.x to at.js 2.x](/help/c-implementing-target/c-implementing-target-for-client-side-web/upgrading-from-atjs-1x-to-atjs-20.md#payload-mapping)|New section: "at.js 1.x parameters to at.js 2.x payload mapping."|
||[Troubleshooting Issues Related to the Enhanced Experience Composer](/help/c-experiences/c-visual-experience-composer/r-troubleshoot-composer/troubleshooting-issues-related-to-the-enhanced-experience-composer-eec.md)|Added "Hostnames" column to the IP addresses to whitelist.|
|February 22, 2019|[Configure enterprise permissions](/help/administrating-target/c-user-management/property-channel/properties-overview.md)|Added "Obtain your Workspace ID" section.|
|February 20, 2019|[Category affinity](/help/c-target/c-visitor-profile/category-affinity.md)|Updated "Category affinity algorithm" section.|
|February 19, 2019|[Single Page App (SPA) Visual Experience Composer](/help/c-experiences/spa-visual-experience-composer.md)|New topic and training videos.|
||[Single Page Application implementation](/help/c-implementing-target/c-implementing-target-for-client-side-web/how-to-deployatjs/target-atjs-single-page-application.md)|New topic and training videos.|
||[at.js version details](/help/c-implementing-target/c-implementing-target-for-client-side-web/target-atjs-versions.md)|Added information about at.js versions 1.7.0 and 2.0.0.|
||[Upgrading from at.js 1.x to at.js 2.x](/help/c-implementing-target/c-implementing-target-for-client-side-web/upgrading-from-atjs-1x-to-atjs-20.md)|New topic and training video.|
||[at.js functions](/help/c-implementing-target/c-implementing-target-for-client-side-web/cmp-atjs-functions.md)|Updated topic to reflect changes with the introduction of at.js 2.x.<br>There are three new fuctions available for at.js 2.x.<ul><li>adobe.target.getOffers(options)</li><li>adobe.target.applyOffers(options)</li><li>adobe.target.triggerView (viewName, options)</li></ul>|
||[How at.js works](/help/c-implementing-target/c-implementing-target-for-client-side-web/c-how-atjs-works/how-atjs-works.md)|Updated topic to reflect changes with the introduction of at.js 2.x. and added training video.|
||[How at.js manages flicker](/help/c-implementing-target/c-implementing-target-for-client-side-web/c-how-atjs-works/manage-flicker-with-atjs.md)|Updated topic to reflect changes with the introduction of at.js 2.x.|
||[at.js Frequently Asked Questions](/help/c-implementing-target/c-implementing-target-for-client-side-web/c-target-atjs-faq/target-atjs-faq.md)|Updated topic to reflect changes with the introduction of at.js 2.x.|
||[Debug at.js using the Adobe Experience Cloud Debugger](/help/c-implementing-target/c-implementing-target-for-client-side-web/c-target-debugging-atjs/target-debugging-atjs.md)|Added note explaining that the Adobe Experience Cloud Debugger Network Request and Mbox Trace features are not yet supported for at.js 2.x.|
||[at.js cookies](/help/c-implementing-target/c-implementing-target-for-client-side-web/atjs-cookies.md)|New topic.|
||[Recommendations as an offer](/help/c-recommendations/recommendations-as-an-offer.md)|New topic.|
||[Visual Experience Composer Options](/help/c-experiences/c-visual-experience-composer/viztarget-options.md)|<ul><li>Added information about using the [!UICONTROL Insert Before, Insert After, or Replace With] action to add recommendations to an experience in an A/B Test or Experience Targeting activity.</li><li>Added information about using the [!UICONTROL Insert Before or Insert After] action to add AEM Experience Fragments to an experience.</li></ul>|
||[Visual Experience Composer helper extension](/help/c-experiences/c-visual-experience-composer/r-troubleshoot-composer/vec-helper-browser-extension.md)|New topic.|
||[Privacy and General Data Protection Regulation](/help/c-implementing-target/c-considerations-before-you-implement-target/c-privacy/cmp-privacy-and-general-data-protection-regulation.md) (GDPR)|Minor edits and information about Opt-in functionality and at.js 1.7.0 and at.js 2.x. |
||[Known issues and resolved issues](/help/r-release-notes/known-issues-resolved-issues.md)|Added known issues about Target APIs.|
||[Entity attributes](/help/c-recommendations/c-products/entity-attributes.md)|Added note that provided entity attribute values expire after 61 days.|
||[Release Notes](/help/r-release-notes/release-notes.md): 19.2.1|This release includes enhancements and fixes. You can read about them and link to the documentation from the Release Notes. This release also includes many documentation updates throughout the help.|

## Adobe Target Standard/Premium 19.1.1 (January 22, 2019) {#section-19-1-1}

|Date|Topic|Changes|
| --- | --- | --- |
|February 2, 2019|[Target release notes](/help/r-release-notes/target-release-notes.md) (prerelease)|Updated prerelease notes for the [!DNL Target] 19.2.1 (February 19, 2019) release.|
|January 30, 2019|[Targets and audiences](/help/c-target/c-troubleshooting-targets-and-audiences/troubleshooting-targets-and-audiences.md)|Added new FAQ: Strings that represent numbers (floating point numbers are supported as well) are compared as numbers.|
||[Troubleshoot the Analytics and Target integration](/help/c-integrating-target-with-mac/a4t/c-a4t-troubleshooting/a4t-troubleshooting.md) (A4T)|Added new troubleshooting section: How should I implement the [!DNL Target] and [!DNL Analytics] JavaScript libraries to capture events across multiple pages and associate them with an A4T activity in [!DNL Target].|
|January 29, 2019|[Target release notes (current)](/help/r-release-notes/release-notes.md)|Enterprise Permissions support in Target APIs availability date updated to February 21, 2019.|
||[System status updates and proactive notifications](/help/r-release-notes/system-status-updates.md)|Added Proactive notifications section.|
|January 22, 2019|[Collections](/help/c-recommendations/c-products/collections.md)<br>[Exclusions](/help/c-recommendations/c-products/exclusions.md)<br>[Catalog search](/help/c-recommendations/c-products/catalog-search.md)<br>[Settings](/help/c-recommendations/plan-implement.md#concept_C1E1E2351413468692D6C21145EF0B84)<br>[Recommendations: filter collections and exclusions by environment (host group)](/help/administrating-target/hosts.md)|Added information about filtering collections and exclusions by environment (host group).|
||[Limits](/help/r-troubleshooting-target/target-limits.md)|Updated information in the Profile Script Value row.|
||[Release Notes](/help/r-release-notes/release-notes.md): 19.1.1|This release includes enhancements and fixes. You can read about them and link to the documentation from the Release Notes. This release also includes many documentation updates throughout the help.|

## Adobe Target Standard/Premium 18.11.1 (November 12, 2018) {#section_4AD10E8B7EB04F96807FFDB763F31703}

| Date | Topic | Changes |
|--- |--- |--- |
|January 16, 2019|[Target Release Notes (current)](/help/r-release-notes/release-notes.md)<br>[Target Release Notes (prerelease)](/help/r-release-notes/target-release-notes.md)<br>[at.js version details](/help/c-implementing-target/c-implementing-target-for-client-side-web/target-atjs-versions.md)|Added information about at.js version 1.6.4.|
|January 10, 2019|[Target Release Notes (current)](/help/r-release-notes/release-notes.md)<br>[Target Release Notes (prerelease)](/help/r-release-notes/target-release-notes.md)<br>[TLS (Transport Layer Security) encryption changes](/help/c-implementing-target/c-considerations-before-you-implement-target/tls-transport-layer-security-encryption.md)|Added the date when Target will completely phase out support for TLS 1.0 encryption: February 20, 2019.|
|January 9, 2019|[Visual Experience Composer Options](/help/c-experiences/c-visual-experience-composer/viztarget-options.md)|Added information regarding Recommendations to Insert Before, Insert After, and Replace With rows.|
||[Target Release Notes (current)](/help/r-release-notes/release-notes.md)<br>[Target Release Notes (prerelease)](/help/r-release-notes/target-release-notes.md)<br>[Supported Browsers](/help/c-implementing-target/c-considerations-before-you-implement-target/supported-browsers.md)|Added information about Target and the Adobe Marketing Cloud dropping support for Microsoft Internet Explorer 11 starting in March 2019.|
||[Target Release Notes (prerelease)](/help/r-release-notes/target-release-notes.md)|Added information for Target 19.1.1 and at.js 1.6.4 releases.|
||[at.js version details](/help/c-implementing-target/c-implementing-target-for-client-side-web/target-atjs-versions.md)|Added information for at.js 1.6.4 release.|
||[Minimizing inlated visit and visitor counts in A4T](/help/c-integrating-target-with-mac/a4t/c-a4t-troubleshooting/minimizing-inflated-visit-and-visitor-counts-a4t.md)|Removed note stating that after November 14, 2016, customers will no longer be able to create A4T activities with redirect offers.|
||[Redirect offers - A4T FAQ](/help/c-integrating-target-with-mac/a4t/r-a4t-faq/a4t-faq-redirect-offers.md)|Added note under "Why are page views on the original page and on the redirect page sometimes counted?"|
|December 20, 2018|[Server Side implement Target](../c-implementing-target/c-api-and-sdk-overview/api-and-sdk-overview.md)|Added note about CORS.|
|December 14, 2018|[Implement Target using Adobe Launch](../c-implementing-target/c-implementing-target-for-client-side-web/how-to-deployatjs/cmp-implementing-target-using-adobe-launch.md)|Added link to a new training video: Implementing Target with the Adobe Launch Tutorial.|
||[Personalization Insights reports](../c-reports/c-personalization-insights-reports/personalization-insights-reports.md)|Added link to training video.|
|December 13, 2018|[Form-based Experience Composer](../c-experiences/form-experience-composer.md)|Updated text and image.|
||[Known issues and resolved issues](known-issues-resolved-issues.md)|Added known issue that the Recommendations feed index can show "Waiting for index" if the items in the feed are the same as in the previous run.|
||[Select audience](../c-activities/t-test-ab/t-test-create-ab/ab-audience.md)|Updated images.|
||[Add experience](../c-activities/t-test-ab/t-test-create-ab/ab-add-experience.md)|Updated image.|
||[Create an A/B Test](../c-activities/t-test-ab/t-test-create-ab/test-create-ab.md)|Updated images.|
||[Test summary](../c-activities/c-multivariate-testing/t-create-multivariate-test/test-summary.md)|Updated image.|
||[Preview experiences for a Multivariate Test](../c-activities/c-multivariate-testing/t-create-multivariate-test/preview-experiences.md)|Updated image.|
||[Create combinations](../c-activities/c-multivariate-testing/t-create-multivariate-test/add-offers.md)|Updated text and images.|
||[Create a Multivariate Test](../c-activities/c-multivariate-testing/t-create-multivariate-test/create-multivariate-test.md)|Updated text and images.|
|December 11, 2018|[targetGlobalSettings](/help/c-implementing-target/c-implementing-target-for-client-side-web/targetgobalsettings.md)|Added that the default value for overrideMboxEdgeServer is "true" beginning with at.js version 1.6.2.|
|December 7, 2018|[ Known Issues and Resolved Issues ](known-issues-resolved-issues.md)|Moved the following from the Known Issues table to the Resolved Issues table: <ul><li>at.js: Mboxes not firing on Microsoft Explorer 11 browsers after upgrading to at.js version 1.0 due to the interaction between at.js and Visitor API 2.2.0.0.</li><li>Geo targeting: Searching for a string that contains special characters (such as a space or a comma) is currently not working when creating geo-targeting audiences.</li></ul>|
|December 5, 2018|[ Personalization Insights reports ](../c-reports/c-personalization-insights-reports/personalization-insights-reports.md)|Added note that the Personalization Insights reports are available in the default environment only.|
||[ Adobe Analytics as the reporting source for Adobe Target (AT) ](../c-integrating-target-with-mac/a4t/a4t.md)|Updated table to indicate that A4T supports server-side deployments.|
|November 29, 2018|[ Estimate the traffic required for a successful test](../c-activities/c-multivariate-testing/t-create-multivariate-test/traffic-estimator.md)|Minor text updates and updated images.|
|November 27, 2018|[ Activities ](../c-activities/activities.md#concept_D317A95A1AB54674BA7AB65C7985BA03)|Updated text and images.|
||[ Profile Script Attributes ](../c-target/c-visitor-profile/profile-parameters.md#concept_8C07AEAB0A144FECA8B4FEB091AED4D2)|Added note that  Target  has a limit of 1,000 profile scripts per account.|
|November 15, 2018|[ Target release notes (current) ](../r-release-notes/release-notes.md#reference_8FE40B43A5A34DDF8F26A53D55EE036A)<br>[ Target release notes (prerelease) ](../r-release-notes/target-release-notes.md#reference_4A966062C61048D1A81412E2DDB16E34)<br>[ at.js version details ](../c-implementing-target/c-implementing-target-for-client-side-web/target-atjs-versions.md#reference_DBB5EDB79EC44E558F9E08D4774A0F7A)|Added information about at.js version 1.6.3.|
||[ Personalization Insights reports ](../c-reports/c-personalization-insights-reports/personalization-insights-reports.md#concept_A897070E1EDC403EB84CFB7A6ECAD767)|Added new topics for the new  Personalization Insights  reports:  Automated Segments  and  Important Attributes .|
|November 14, 2018|Release 18.11.1 [ Target release notes (current) ](../r-release-notes/release-notes.md#reference_8FE40B43A5A34DDF8F26A53D55EE036A)|This release includes enhancements and fixes. You can read about them and link to the documentation from the Release Notes. This release also includes many documentation updates throughout the help.|

## Adobe Target Standard/Premium 18.10.1 (October 24, 2018) {#section_F3DB9A89D944428DBEE04634EB712601}

| Date | Topic | Changes |
|--- |--- |--- |
|November 8, 2018|[Adobe Analytics as the reporting source for Adobe Target (A4T)](../c-integrating-target-with-mac/a4t/a4t.md#concept_7540C8C04259434AB6EE33B09F47A1DE)|Added NodeJS SDK to the compatibility table.|
|November 7, 2018|[How long should you run an A/B Test?](../c-activities/t-test-ab/sample-size-determination.md#concept_2801F552DB874C20B8A17C1B774C0383)|Edited topic and added additional information.|
||[Target release notes (prerelease)](../r-release-notes/target-release-notes.md#reference_4A966062C61048D1A81412E2DDB16E34)|Added information about features in the Target 18.11.1 release.|
|November 5, 2018|[Integrate Recommendations with email](../c-recommendations/c-recommendations-faq/integrating-recs-email.md#reference_256B16C894864F24AF970E43DC174420)|Updated link in Option 3.|
||[Customer attributes](../c-target/c-visitor-profile/working-with-customer-attributes.md#concept_16C5C434D32D4EB1AD44A71821F3DEE8)|Added the following note:<br>**Important**: The data source name and the attribute name cannot contain a period.|
|October 31, 2018|[System status updates](../r-release-notes/system-status-updates.md#concept_5CBDF506BEFA40E483CC7DE0DA915EAD)|Updated topic.|
||[Target Basics Webinar Series](../cmp-resources-and-contact-information.md#concept_11902FAC95C64479AABE020557A7EEE4)|Added link to the Best Practices in Audience Segmentation recording.|
|October 29, 2018|[TLS (Transport Layer Security) encryption changes](../c-implementing-target/c-considerations-before-you-implement-target/tls-transport-layer-security-encryption.md#concept_CC1001E9D3AE4BABAF90B8311B0A6451)|Added new section: Expected Behavior with Browsers Supporting TLS 1.0 Only.|
|October 26, 2018|[Known Issues and Resolved Issues](../r-release-notes/known-issues-resolved-issues.md#concept_625C3A16B7F24D4B82EFF130F0945541)|<ul><li>Added a known issue about searching for strings containing special characters when creating geo-targeting audiences.</li><li>Moved at.js 1.6.0 redirect issue to Resolved Issues table.</li><li>Moved issue to the Resolved Issues table regarding activities in the default workspace deleted via API continuing to display in the Target UI</li></ul>|
|October 24, 2018|[Preferences](../administrating-target/r-target-account-preferences/target-account-preferences.md#reference_0CF97B1C2214412ABBC8222EA8A36D7E)|Added information to consider when choosing the reporting source for activities in Setup > Preferences or per activity.|
||[Create an Automated Personalization activity](../c-activities/t-automated-personalization/create-ap-activity.md#task_8AAF837796D74CF893CA2F88BA1491C9)|Added information about filtering for Unassigned Offers.|
||[Create Experience](../c-activities/t-experience-target/t-xt-create/xt-add-experience.md#task_454646F2895242D3B92DC395A0CE1A00)|Added information about duplicating experiences in XT activities.|
||[Add experience](../c-activities/t-test-ab/t-test-create-ab/ab-add-experience.md#task_454646F2895242D3B92DC395A0CE1A00)|Added information about duplicating experiences in A/B Tests.|
||[About audiences](../c-target/c-audiences/audiences.md#concept_65BE870D290E412D8BBF557EEA67C271)|Added information about the handling of audiences referenced in Target activities that have been deleted in Adobe Audience Manager (AAM).|
||[at.js integrations](../c-implementing-target/c-implementing-target-for-client-side-web/c-how-atjs-works/target-atjs-integrations.md#concept_C100BC4F073C4B57A608B309D0157B39)|Updated topic.|
||[Implement Target without a tag manager](../c-implementing-target/c-implementing-target-for-client-side-web/how-to-deployatjs/implementing-target-without-a-tag-manager.md#topic_397FFA3D6918456BBE02A9FBE9537894)|Updated all sections.  Added new section: at.js Implementation.|
||Release 18.10.1 [Release Notes](../r-release-notes/release-notes.md#reference_8FE40B43A5A34DDF8F26A53D55EE036A)|This release includes enhancements and fixes. You can read about them and link to the documentation from the Release Notes. This release also includes many documentation updates throughout the help.|

## Adobe Target Standard/Premium 18.9.1 (September 26, 2018) {#section_F7E74227BB9D467E9ABC0797EDC2FE0D}

<table id="table_0348AA29207D48A4BDFFA187F4F845B7"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Date </th> 
   <th colname="col2" class="entry"> Topic </th> 
   <th colname="col3" class="entry"> Changes </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> October 24, 2018 </td> 
   <td colname="col2"> <p> <a href="../r-release-notes/known-issues-resolved-issues.md#concept_625C3A16B7F24D4B82EFF130F0945541" format="dita" scope="local"> Known issues and resolved issues </a> </p> </td> 
   <td colname="col3"> <p>Added known issue about deleted activities via API in the default workspace persisting in the Target UI. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-reports/c-report-settings/average-lift-bounds-and-confidence-interval.md#topic_AFFDC672A8A34D028B100EF6BE5D8129" format="dita" scope="local"> Average Lift, Lift Bounds, and Confidence Interval </a> </p> </td> 
   <td colname="col3"> <p>Added a note explaining that minor variances between manual calculations using the listed formulas and the numbers displayed in the report are to be expected. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> October 22, 2018 </td> 
   <td colname="col2"> <p> <a href="../c-implementing-target/c-implementing-target-for-client-side-web/t-mbox-download/cookie-behavior.md#concept_4D8107E193B64168A3C0B85B51612991" format="dita" scope="local"> Target Cookie </a> </p> </td> 
   <td colname="col3"> <p>Added Important note at top of topic advising clients to not link sensitive information to mboxSession and mboxPC. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> October 21, 2018 </td> 
   <td colname="col2"> <p> <a href="../c-implementing-target/c-implementing-target-for-client-side-web/target-atjs-versions.md#reference_DBB5EDB79EC44E558F9E08D4774A0F7A" format="dita" scope="local"> at.js Version Details </a> </p> </td> 
   <td colname="col3"> <p>Added information about at.js Version 1.6.2. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-implementing-target/c-considerations-before-you-implement-target/c-privacy/cmp-privacy-and-general-data-protection-regulation.md#topic_6BCC0D0984184379A2A2EA6FFC948899" format="dita" scope="local"> Privacy and General Data Protection Regulation (GDPR) </a> </p> </td> 
   <td colname="col3"> <p>Added the "Adobe Target and Adobe Launch Opt-In" section. </p> <p>Updated the following FAQs: </p> <p> 
     <ul id="ul_BBF57B0E30A541E1BD1BCADD21A3D0F7"> 
      <li id="li_020DE613F4F340D8B68186465883A60C"> <p>How does Adobe Target handle consent management? </p> </li> 
      <li id="li_515B157F27B04342BB5664FD8E258FE2"> <p>What IDs are supported to help customers complete a GDPR access and deletion request for Target? </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-implementing-target/c-implementing-target-for-client-side-web/how-to-deployatjs/cmp-implementing-target-using-adobe-launch.md#topic_5234DDAEB0834333BD6BA1B05892FC25" format="dita" scope="local"> Implementing Target using Adobe Launch </a> </p> </td> 
   <td colname="col3"> <p>Updated link to the Adobe Target Extension. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> October 18, 2018 </td> 
   <td colname="col2"> <p> <a href="../c-recommendations/c-recommendations-faq/ip-addresses-marketing-cloud.md#concept_216F959FF18143D6A3BA0BE937918580" format="dita" scope="local"> IP Addresses Used by Recommendations Feed-Processing Servers </a> </p> </td> 
   <td colname="col3"> <p>Updated IP address range used by Target Recommendations activities. </p> <p>Added IP address range used by Target Recommendations APIs. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> October 12, 2018 </td> 
   <td colname="col2"> <p> <a href="../c-activities/c-activity-qa/activity-qa.md#concept_9329EF33DE7D41CA9815C8115DBC4E40" format="dita" scope="local"> Activity QA </a> </p> </td> 
   <td colname="col3"> <p>Edited the following paragraph under <span class="wintitle"> Considerations</span>: </p> <p>Activity QA does not display content for archived activities or activities that are past their end dates. If you deactivate an ended activity, you must save the activity again for Activity QA to work. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> October 10, 2018 </td> 
   <td colname="col2"> <p> <a href="../target-home.md#topic_74F655D8648E4586BCCFD789E60D13CE" format="dita" scope="local"> Adobe Target Product Documentation </a> </p> </td> 
   <td colname="col3"> <p>Updated the Adobe Target Product documentation in the following languages: German, Spanish, French, Italian, Japanese, and Portuguese (Brazil). </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> October 9, 2019 </td> 
   <td colname="col2"> <p> <a href="../c-target/c-visitor-profile/profile-parameters.md#concept_01A30B4762D64CD5946B3AA38DC8A201" format="dita" scope="local"> Profile Attributes </a> </p> </td> 
   <td colname="col3"> <p>Added Profile Scripts FAQ section. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-recommendations/c-recommendations-faq/ip-addresses-marketing-cloud.md#concept_216F959FF18143D6A3BA0BE937918580" format="dita" scope="local"> IP Addresses Used by Recommendations Feed-Processing Servers </a> </p> </td> 
   <td colname="col3"> <p>Edited text to indicate that <span class="wintitle"> Recommendations </span> activities use IP addresses located in the Oregon data center. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> October 8, 2018 </td> 
   <td colname="col2"> <p> <a href="../c-recommendations/c-recommendations-faq/ip-addresses-marketing-cloud.md#concept_216F959FF18143D6A3BA0BE937918580" format="dita" scope="local"> IP Addresses Used by Recommendations Feed-Processing Servers </a> </p> </td> 
   <td colname="col3"> <p>Added new IP address range for the CIDR Notation 192.243.242.0.0/24. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> October 5, 2018 </td> 
   <td colname="col2"> <p> <a href="../c-integrating-target-with-mac/a4t/r-a4t-faq/a4t-faq-viewing-reports.md#concept_72A95F6466A04B409FCD5989A6B6A554" format="dita" scope="local"> Viewing Reports - A4T FAQ </a> </p> </td> 
   <td colname="col3"> <p>Revised entire section: "Should I use visitors, activity impressions, or visits when viewing reports?" Reworded metric descriptions and added a list of considerations. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> October 4, 2018 </td> 
   <td colname="col2"> <p> <a href="../c-recommendations/c-algorithms/create-new-algorithm.md#task_8A9CB465F28D44899F69F38AD27352FE" format="dita" scope="local"> Creating Criteria </a> </p> </td> 
   <td colname="col3"> <p>Added "Expected Criteria Processing Time" section. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-activities/activities.md#concept_D317A95A1AB54674BA7AB65C7985BA03" format="dita" scope="local"> Activities </a> </p> </td> 
   <td colname="col3"> <p>Added information about how to disable the Tip of the Day. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> October 3, 2018 </td> 
   <td colname="col2"> <p> <a href="https://spark.adobe.com/page/Lo3Spm4oBOvwF/" format="https" scope="external"> Analytics &amp; Target: Best Practices for Analysis </a> </p> </td> 
   <td colname="col3"> <p>Check out the new Analytics for Target (A4t) tutorial. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-intro/how-target-works.md#concept_459AB4DEE7364A9290C2FD405DC29584" format="dita" scope="local"> How Adobe Target Works </a> </p> </td> 
   <td colname="col3"> <p>Updated entire topic. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-activities/t-test-ab/t-test-create-ab/test-create-ab.md#task_68C8079BF9FF4625A3BD6680D554BB72" format="dita" scope="local"> Create an A/B Test </a> </p> <p> <a href="../c-activities/t-automated-personalization/create-ap-activity.md#task_8AAF837796D74CF893CA2F88BA1491C9" format="dita" scope="local"> Creating an Automated Personalization Activity </a> </p> <p> <a href="../c-activities/t-experience-target/t-xt-create/xt-create.md#task_D6B3429AC31549E1A70EDF04B3DDC765" format="dita" scope="local"> Create an Experience Targeting Activity </a> </p> <p> <a href="../c-activities/c-multivariate-testing/t-create-multivariate-test/create-multivariate-test.md#task_BF870FA60A8245AB8F0B775BE32EA710" format="dita" scope="local"> Create a Multivariate Test </a> </p> <p> <a href="../c-recommendations/t-create-recs-activity/recs-activity-settings.md#reference_3FDA8388CEEC4159949151C1829E2FBB" format="dita" scope="local"> Recommendations Activity Settings </a> </p> <p> <a href="../c-activities/t-test-ab/t-test-create-ab/ab-add-experience.md#task_454646F2895242D3B92DC395A0CE1A00" format="dita" scope="local"> Add Experience </a> </p> <p> <a href="../c-activities/t-test-ab/t-test-create-ab/ab-set-metrics.md#task_A04AB66007C1467DA1C21A519A5C7BEB" format="dita" scope="local"> Set Metrics </a> </p>
   </td> 
   <td colname="col3"> <p>Updated the table listing characters not allowed in activity, experience, or metric names. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> October 2, 2018 </td> 
   <td colname="col2"> <p> <a href="../c-recommendations/c-products/collections.md#concept_671BEFFB997D4F1282665BF3CAC00AC5" format="dita" scope="local"> Collections </a> </p> </td> 
   <td colname="col3"> <p>Added note after Step 1. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-recommendations/c-products/exclusions.md#task_E79DA82BA402415FB41232976EDEF1CA" format="dita" scope="local"> Exclusions </a> </p> </td> 
   <td colname="col3"> <p>Added note after Step 1. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> September 27, 2018 </td> 
   <td colname="col2"> <p> <a href="../c-implementing-target/c-considerations-before-you-implement-target/c-methods-to-get-data-into-target/methods-to-get-data-into-target.md#concept_0069C0EFB56C4700BB33F2F35C2B9B17" format="dita" scope="local"> Methods to get Data into Target </a> </p> </td> 
   <td colname="col3"> <p>Added information about allowed characters in query stings. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../r-release-notes/known-issues-resolved-issues.md#concept_625C3A16B7F24D4B82EFF130F0945541" format="dita" scope="local"> Known Issues and Resolved Issues </a> </p> </td> 
   <td colname="col3"> <p>Moved known issue regarding offer-level reporting in AP activities to the Resolved Issues table. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> September 26, 2018 </td> 
   <td colname="col2"> <p> <a href="../c-experiences/c-visual-experience-composer/viztarget-options.md#reference_3BD1BEEAFA584A749ED2D08F14732E81" format="dita" scope="local"> Visual Experience Composer Options </a> </p> </td> 
   <td colname="col3"> <p>Added information about the <span class="wintitle"> Insert Before </span> option. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <a href="../c-activities/t-automated-personalization/create-ap-activity.md#task_8AAF837796D74CF893CA2F88BA1491C9" format="dita" scope="local"> Creating an Automated Personalization Activity </a> </td> 
   <td colname="col3"> <p>Added information about the Report Group list that lets you filter offers by reporting group. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-activities/t-automated-personalization/managing-exclusions.md#topic_30B4E4F89C914EB2B20B038C0299ED2E" format="dita" scope="local"> Manage Exclusions </a> </p> </td> 
   <td colname="col3"> <p>Added information about using multiple offers from the same location in an exclusion group. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../cmp-resources-and-contact-information.md#concept_11902FAC95C64479AABE020557A7EEE4" format="dita" scope="local"> Target Basics Webinar Series </a> </p> </td> 
   <td colname="col3"> <p>Added link to the Best Practices in Reporting &amp; Value Socialization session. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-recommendations/c-products/feeds.md#concept_1228B31E3D0B483B9DD42C5E2AE436E3" format="dita" scope="local"> Feeds </a> </p> </td> 
   <td colname="col3"> <p>Added following note: </p> <p> <p>Important:  Uploaded feeds expire after 61 days. This means that recommendations will no longer be returned if a feed file has not been processed in the last 60 days. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../r-release-notes/known-issues-resolved-issues.md#concept_625C3A16B7F24D4B82EFF130F0945541" format="dita" scope="local"> Known Issues and Resolved Issues </a> </p> </td> 
   <td colname="col3"> <p>Added known issue regarding offer-level reporting in AP activities. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-recommendations/c-recommendations-faq/integrating-recs-email.md#reference_256B16C894864F24AF970E43DC174420" format="dita" scope="local"> Integrating Recommendations with Email </a> </p> </td> 
   <td colname="col3"> <p>Updated note under "Option 1: Use the Delivery API." </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-recommendations/recommendations.md#concept_7556C8A4543942F2A77B13A29339C0C0" format="dita" scope="local"> Recommendations </a> </p> </td> 
   <td colname="col3"> <p>Reordered topics in entire section. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p>Release 18.9.1 <a href="../r-release-notes/release-notes.md#reference_8FE40B43A5A34DDF8F26A53D55EE036A" format="dita" scope="local"> Release Notes </a> </p> </td> 
   <td colname="col3"> <p>This release includes enhancements and fixes. You can read about them and link to the documentation from the Release Notes. This release also includes many documentation updates throughout the help. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Adobe Target Standard/Premium 18.8.1 (August 21, 2018) {#section_6A146EE91FFB49D1BA398B36817CD0A2}

<table id="table_F09AC99B587A4D6390B1F8AE54F5DC47"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Date </th> 
   <th colname="col2" class="entry"> Topic </th> 
   <th colname="col3" class="entry"> Changes </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> September 21, 2018 </td> 
   <td colname="col2"> <p> <a href="../c-implementing-target/c-implementing-target-for-client-side-web/c-target-debugging-atjs/target-debugging-atjs.md#concept_CAE591DA8C404C22917584ECD4F7494F" format="dita" scope="local"> Debugging at.js Using the Adobe Experience Cloud Debugger </a> </p> </td> 
   <td colname="col3"> <p>Revised entire topic and added training videos. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> September 20, 2018 </td> 
   <td colname="col2"> <p> <a href="../r-release-notes/release-notes.md#reference_8FE40B43A5A34DDF8F26A53D55EE036A" format="dita" scope="local"> Target Release Notes </a> </p> <p> <a href="../c-implementing-target/c-implementing-target-for-client-side-web/target-atjs-versions.md#reference_DBB5EDB79EC44E558F9E08D4774A0F7A" format="dita" scope="local"> at.js Version Details </a> </p> </td> 
   <td colname="col3"> <p>Added information about the at.js 1.6.1 release. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> September 19, 2018 </td> 
   <td colname="col2"> <p> <a href="../r-release-notes/known-issues-resolved-issues.md#concept_625C3A16B7F24D4B82EFF130F0945541" format="dita" scope="local"> Known Issues and Resolved Issues </a> </p> </td> 
   <td colname="col3"> Moved issue regarding the Code Editor from the Known Issues table to the Resolved Issues table. </td> 
  </tr> 
  <tr> 
   <td colname="col1"> September 18, 2018 </td> 
   <td colname="col2"> <p> <a href="../c-experiences/c-visual-experience-composer/c-vec-code-editor/experience-templates.md#concept_109BBD7EABC04DD39E6B7B1687786652" format="dita" scope="local"> Experience Templates </a> </p> </td> 
   <td colname="col3"> <p>New topic. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../cmp-resources-and-contact-information.md#concept_11902FAC95C64479AABE020557A7EEE4" format="dita" scope="local"> Target Basics Webinar Series </a> </p> </td> 
   <td colname="col3"> <p>Updated upcoming webinar dates. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> September 11, 2018 </td> 
   <td colname="col2"> <p> <a href="../c-activities/c-activity-qa/use-qa-mode-with-server-side-delivery.md#concept_54698C5CE8934F68B20961CD83FD6202" format="dita" scope="local"> Use Activity QA with Server-Side Delivery </a> </p> </td> 
   <td colname="col3"> <p>New topic. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-target/c-audiences/c-target-rules/custom-parameters.md#concept_C4C6E00D7C5A4BE9B72D471DB2E3027B" format="dita" scope="local"> Custom Parameters </a> </p> </td> 
   <td colname="col3"> <p>Added information about re-saving custom audiences created before the 18.5.1 release. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../r-release-notes/known-issues-resolved-issues.md#concept_625C3A16B7F24D4B82EFF130F0945541" format="dita" scope="local"> Known Issues and Resolved Issues </a> </p> </td> 
   <td colname="col3"> <p>Added known issue: Target activity impressions and conversions are currently counted incorrectly in Analysis Workspace. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-implementing-target/c-considerations-before-you-implement-target/c-privacy/cmp-privacy-and-general-data-protection-regulation.md#concept_41F88DE95D2943178BEC382736B5C038" format="dita" scope="local"> General Data Protection Regulation FAQ </a> </p> </td> 
   <td colname="col3"> <p>Updated code sample. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-recommendations/c-recommendations-faq/recommendations-faq.md#concept_EF272DE4AC6C47B19026BFBE816F5DB8" format="dita" scope="local"> Recommendations FAQ </a> </p> </td> 
   <td colname="col3"> <p>Changed the required Velocity version to 1.7.0. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> September 10, 2018 </td> 
   <td colname="col2"> <p> <a href="../r-release-notes/release-notes.md#reference_8FE40B43A5A34DDF8F26A53D55EE036A" format="dita" scope="local"> Target Release Notes </a> </p> <p> <a href="../c-implementing-target/c-considerations-before-you-implement-target/tls-transport-layer-security-encryption.md#concept_CC1001E9D3AE4BABAF90B8311B0A6451" format="dita" scope="local"> TLS (Transport Layer Security) Encryption Changes </a> </p> </td> 
   <td colname="col3"> <p>Changed the date when Adobe will phase out support for TLS 1.0 from September 12, 2018 to February 2019. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-reports/reports.md#concept_B5077F5503AA4C98901AA99EDCE6CDE6" format="dita" scope="local"> Reports </a> </p> </td> 
   <td colname="col3"> <p>Added information and link to help plan A/B Tests. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-recommendations/c-recommendations-faq/recommendations-faq.md#concept_EF272DE4AC6C47B19026BFBE816F5DB8" format="dita" scope="local"> Recommendations FAQ </a> </p> </td> 
   <td colname="col3"> <p>Added following FAQ: What is the maximum size of a CSV file for a feed upload? </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-target/c-audiences/c-target-rules/visitor-profile.md#concept_E972690B9A4C4372A34229FA37EDA38E" format="dita" scope="local"> Visitor Profile </a> </p> </td> 
   <td colname="col3"> <p>Added following paragraph: </p> <p>A visitor profile is created in the local edge memory for each mbox call with new <span class="codeph"> mboxPC </span>. After 30 minutes of inactivity, the profile is saved to the Target database and is accessible from other edges. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-activities/t-test-ab/t-test-create-ab/ab-activity-url.md#concept_D28549AAA0A14E3BB5F05F32BE8ABC90" format="dita" scope="local"> Activity URL </a> </p> </td> 
   <td colname="col3"> <p>Modified text and updated illustration. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> September 7, 2018 </td> 
   <td colname="col2"> <p> <a href="../c-recommendations/c-recommendations-faq/recommendations-faq.md#concept_EF272DE4AC6C47B19026BFBE816F5DB8" format="dita" scope="local"> Recommendations FAQ </a> </p> </td> 
   <td colname="col3"> <p>Added new FAQ: Why can't I save my legacy Recommendations activity after defining a new audience? </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> September 4, 2018 </td> 
   <td colname="col2"> <p> <a href="../c-implementing-target/c-implementing-target-for-client-side-web/cmp-atjs-functions.md#section_42725F3C837247D58AE1831EA330E44D" format="dita" scope="local"> Data Providers </a> </p> </td> 
   <td colname="col3"> <p>Updated code sample. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-implementing-target/c-considerations-before-you-implement-target/c-privacy/cmp-privacy-and-general-data-protection-regulation.md#concept_41F88DE95D2943178BEC382736B5C038" format="dita" scope="local"> General Data Protection Regulation FAQ </a> </p> </td> 
   <td colname="col3"> <p>Minor edits. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> August 30, 2018 </td> 
   <td colname="col2"> <p> <a href="../r-release-notes/known-issues-resolved-issues.md#concept_625C3A16B7F24D4B82EFF130F0945541" format="dita" scope="local"> Known Issues and Resolved Issues </a> </p> </td> 
   <td colname="col3"> Added following known issue: <p> 
     <ul id="ul_7AF527E5989D468BBC9472EA1C7F376D"> 
      <li id="li_7F53C6F01E1E471FB546AF98F1FF7F1E"> <p>When using <span class="codeph"> at.js </span> version 1.6.0, Analytics for Target (A4T) redirects occur, but without activity qualification. </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> August 28, 2018 </td> 
   <td colname="col2"> <p> <a href="../c-recommendations/c-products/entity-attributes.md#reference_3BCC1383FB3F44F4A2120BB36270387F" format="dita" scope="local"> Entity Attributes </a> </p> </td> 
   <td colname="col3"> <p>Updated the entity ID row. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-recommendations/c-algorithms/create-new-algorithm.md#concept_BC16005C7A1E4F1A87E33D16221F4A96" format="dita" scope="local"> Content Settings </a> </p> </td> 
   <td colname="col3"> <p>Clarified information about the <span class="wintitle"> Recommend Previously Purchased Items </span> option. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> August 21, 2018 </td> 
   <td colname="col2"> <p> <a href="../c-reports/c-personalization-insights-reports/personalization-insights-reports.md#concept_A897070E1EDC403EB84CFB7A6ECAD767" format="dita" scope="local"> Personalization Insights Reports </a> </p> </td> 
   <td colname="col3"> <p>New topic. </p> <p> <p>Note:  This feature will be available soon. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-experiences/c-visual-experience-composer/c-vec-code-editor/vec-code-editor.md#concept_B3A6E9EE3A60406DB640E205EA1745B5" format="dita" scope="local"> Modifications </a> </p> </td> 
   <td colname="col3"> <p>Added information about docking the Modifications panel. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-experiences/c-visual-experience-composer/viztarget-options.md#reference_3BD1BEEAFA584A749ED2D08F14732E81" format="dita" scope="local"> Visual Experience Composer Options </a> </p> </td> 
   <td colname="col3"> <p>Reorganized table to account for new groupings. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../cmp-resources-and-contact-information.md#concept_11902FAC95C64479AABE020557A7EEE4" format="dita" scope="local"> Target Basics Webinar Series </a> </p> </td> 
   <td colname="col3"> <p> 
     <ul id="ul_D5E4E05DFE7A4E45BF199395D7AC3CE1"> 
      <li id="li_7A4A621EC5C34E4AADD46AA294620D9C"> <p>Added information about upcoming webinars. </p> </li> 
      <li id="li_A77B214010EF45BEBD0E2CBB256AD67D"> <p>Added link to the recording for the second webinar: Steps to Add Automation &amp; More Sophisticated Activities. </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-activities/activities.md#concept_D317A95A1AB54674BA7AB65C7985BA03" format="dita" scope="local"> Activities </a> </p> </td> 
   <td colname="col3"> <p>Added the "Tips and Tricks" section. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../r-release-notes/known-issues-resolved-issues.md#concept_625C3A16B7F24D4B82EFF130F0945541" format="dita" scope="local"> Known Issues and Resolved Issues </a> </p> </td> 
   <td colname="col3"> <p>Rephrased issue regarding redirect activities in <span class="codeph"> at.js </span> implementations might cause the preview URL to enter into a loop. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p> <a href="../c-implementing-target/c-considerations-before-you-implement-target/tls-transport-layer-security-encryption.md#concept_CC1001E9D3AE4BABAF90B8311B0A6451" format="dita" scope="local"> TLS (Transport Layer Security) Encryption Changes </a> </p> </td> 
   <td colname="col3"> <p>Removed the previously proposed date when TLS 1.0 support would be phased out (September 12, 2018). </p> <p>The date when TLS 1.0 support will be removed will be announced at a later date; however, It is important that you go through the specifics and plan out the changes for a smooth transition. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> </td> 
   <td colname="col2"> <p>Release 18.8.1 <a href="../r-release-notes/release-notes.md#reference_8FE40B43A5A34DDF8F26A53D55EE036A" format="dita" scope="local"> Release Notes </a> </p> </td> 
   <td colname="col3"> <p>This release includes enhancements and fixes. You can read about them and link to the documentation from the Release Notes. This release also includes many documentation updates throughout the help. </p> </td> 
  </tr> 
 </tbody> 
</table>

