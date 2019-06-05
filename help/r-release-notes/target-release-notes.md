---
description: These release notes provide information about features, enhancements, fixes, and known issues for the latest or upcoming Target releases.
keywords: release notes
seo-description: These release notes provide information about features, enhancements, fixes, and known issues for the latest or upcoming Adobe Target releases
seo-title: Adobe Target release notes (prerelease)
solution: Target
title: Target release notes (prerelease)
topic: Standard
uuid: 35ecabbe-b8b4-479b-9266-4823c831d79a
---

# Target release notes (prerelease){#target-release-notes-prerelease}

These release notes provide information about features, enhancements, and fixes for the latest or upcoming [!DNL Adobe Target] releases.

**Last Updated: May 28, 2019**

>[!NOTE]
>
>These release notes contain prerelease information. Release dates, features, and other information are subject to change. To view information about the current release, see [Target Release Notes](release-notes.md). The information on these pages might be the same or it might differ, depending on the timing of releases.

## Target Standard/Premium 19.6.1 (June 25, 2019) {#tgt-19-6-1}

(The issue numbers in parentheses are for internal [!DNL Adobe] use.)

|Feature|Description|
| --- | --- |
|Visual Experience Composer (VEC)|**New VEC menu options**: When you click a page element in the VEC, a menu shows the options that are available for that element type. The following new menu options are available in this release: <ul><li>**Styles > Background**: You can now use the [!UICONTROL Styles > Background] option to change the background image and color for the selected element. (TGT-15001)</li><li>**[!UICONTROL Replace With > HTML] and [!UICONTROL Replace With > Experience Fragment]**: When you click an image then click [!UICONTROL Replace With], two new options display:<ul><li>**HTML**: You can replace an image with HTML to give you full control of the element without needing to select the parent element to access the HTML option.</li><li>**Experience Fragment**: You can replace an image with an Adobe Experience Manager (AEM) [experience fragment](/help/c-experiences/c-manage-content/aem-experience-fragments.md) to quickly insert elements created in AEM in Target activities. (TGT-34097)</li></ul></li></ul>**Click-tracking improvements**: We have improved the process for configuring click tracking within the VEC and the Single Page Application VEC.<ul><li>While selecting elements to use in click tracking, the names of all available elements display in the Modifications panel on the right side, making it quick and easy to select the desired elements.</li><li>The [!UICONTROL Goals & Settings] page of the three-part guided activity workflow displays a number representing the number of elements selected for click tracking. You can hover over this number to see the names of all selected elements. (TGT-33878)</li></ul>|
|Single Page App (SPA) Visual Experience Composer (VEC)|**Guided workflow**: A new guided workflow helps you understand how page-delivery-rule settings should be configured to execute and run an activity successfully for your Single Page App. (TGT-33718)<br>**Clone modifications**: You can now define a modification using the SPA VEC and then clone that modification for use in other views in your Single Page App. (TGT-33882)|
|Mobile Visual Experience Composer (VEC)|**Multiple app versions**: You can now author activities for multiple versions of your mobile app. This saves you time and effort when the versions are similar and you don't need to significantly change the app's UI. (TGT-34231)|
|![Premium badge](/help/assets/premium.png)<br>Automated Personalization (AP) & Auto-Target|**Specific experience as control**: You can select an experience to be used as control while creating an AP or Auto-Target activity. This feature lets you route the entire control traffic to a specific experience, based on the traffic allocation percentage configured in the activity. You can then evaluate the performance reports of the personalized traffic against control traffic to that one experience. The current control option (randomly served experiences) will continue to be available. (TGT-32801 & TGT-26572)|

### Enhancement, fixes, and changes

* The `<BODY>` tag now displays in the DOM path that displays at the bottom of the VEC when you click an element on the page, letting you perform actions on the `<BODY>` tag. (TGT-33736)

## Prerelease information {#section_7B9D4AAFC6A74388B9D7DEF0658D8B63}

To receive advance notifications about upcoming product enhancements to Target and other Adobe Experience Cloud solutions, sign up for the Adobe Priority Product Update:

[https://www.adobe.com/subscription/priority-product-update.html](https://www.adobe.com/subscription/priority-product-update.html) 
