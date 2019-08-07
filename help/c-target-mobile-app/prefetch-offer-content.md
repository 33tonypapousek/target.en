---
description: The Adobe Target prefetch feature uses the iOS and Android Mobile SDKs to fetch offer content as few times as possible by caching the server responses.
keywords: offer;prefetch;iOS;android;sdk;mobile;mobile sdk
seo-description: The Adobe Target prefetch feature uses the iOS and Android Mobile SDKs to fetch offer content as few times as possible by caching the server responses.
seo-title: Prefetch offer content
solution: Target
title: Prefetch offer content
topic: Advanced,Standard,Classic
uuid: 715e0e77-bfd9-437b-b42c-899d66f2890c
---

# Prefetch offer content{#prefetch-offer-content}

The [!DNL Target] prefetch feature uses the iOS and Android Mobile SDKs to fetch offer content as few times as possible by caching the server responses.

This process reduces the load time, prevents multiple network calls, and allows [!DNL Target] to be notified which mbox was visited by the mobile app user. All content is retrieved and cached during the prefetch call, and this content is retrieved from the cache for all future calls that contain cached content for the specified mbox name.

Consider the following when uses in prefetch method with the iOS and Android Mobile SDKs:

* Prefetch content does not persist across launches. The prefetch content is cached as long as the application lives or until the `clearPrefetchCache()` method is called.
* Prefetch functionality in the iOs and Android Mobile SDKs is not supported for Auto Target, Auto Allocate, and Automated Personalization activity types.

For more information, including prefetch methods, public classes, and code samples, see:

* **iOS:**  [Prefetch Offer Content in iOS](https://marketing.adobe.com/resources/help/en_US/mobile/ios/c_mob_target-prefetch_ios.html) in the *iOS SDK 4.x for Experience Cloud Solutions* guide. 
* **Android:**  [Prefetch Offer Content in Android](https://marketing.adobe.com/resources/help/en_US/mobile/android/c_mob_target-prefetch_android.html) in the *Android SDK 4.x for Experience Cloud Solutions* guide.
