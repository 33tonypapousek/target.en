---
description: Information to use at.js 2.0 to implement Single Page Applications (SPAs).
keywords: single page application implementation;implement single page application;spa;at.js 2.0
seo-description: Information to use Adobe Target at.js 2.0 to implement Single Page Applications (SPAs).
seo-title: Single Page Application implementation
solution: Target
title: Single Page Application implementation
topic: standard
uuid: 5887ec53-e5b1-40f9-b469-33685f5c6cd6
---

# Single Page Application implementation{#single-page-application-implementation}

Traditional websites worked on "Page-to-Page" navigation models, otherwise known as Multi Page Applications where website designs were tightly coupled to URLs and transitions from one webpage to another required a page load. Modern web applications, such as Single Page Applications (SPAs), instead adopt a model that propels rapid use of browser UI rendering, which is often independent of page reloads. These experiences are often triggered by customer interactions such as scrolls, clicks, and cursor movements. As the paradigms of the modern web have evolved, the relevance of traditional generic events, such as page load, to deploy personalization and experimentation no longer work.

![Traditional page lifecycle vs. SPA lifecycle](/help/c-experiences/assets/trad-vs-spa.png)

The newest version of at.js 2.0 provides rich features that equip your business to execute personalization on next generation client-side technologies. This version is focused on improving at.js to have harmonious interactions with Single Page Applications. 

Here are some benefits to using at.js 2.0 that are not available in previous versions:

* Ability to cache all offers on page load to reduce multiple server calls to a single server call. 
* Tremendously improve your end-user’s experience on your site since offers are shown immediately via the cache without lag time introduced by traditional server calls.
* A simple one-line of code and one-time developer setup to enable your marketers to create and run A/B & Experience Targeting activities via the Visual Experience Composer (VEC) on your SPA. 

## Adobe Target Views and Single Page Applications

The Adobe Target VEC for SPAs takes advantage of a new concept called Views: a logical group of visual elements that together make up an SPA experience. A SPA can, therefore, be considered as transitioning through views, instead of URLs, based on user interactions. A View can typically represent a whole site, or grouped visual elements within a site.

To explain further about what Views are, let’s navigate this fake online e-commerce site implemented in React called AShop and explore some example Views.

**Home Site**: `http://www.adobeshop.com/home`

![home site](/help/c-experiences/assets/home.png)

When we navigate to the home site of the AShop, we can immediately see a hero image that promotes an Easter sale as well as the newest products that AShop is selling on its site. In this case, a View can be defined as the entire home site. We can name this View as home just like the path name in `www.adobshop.com/home`. This is handy to note as we will expand on this more in the Implementing Adobe Target Views section below.

**Product Site**: `http://www.adobeshop.com/products`

![product site](/help/c-experiences/assets/product-site.png)

As we become more interested in the products that AShop is selling, we decide to click the Products link. Similar to the home site, the entirety of the products site can be defined as a View. We can name this View as products just like the path name in `www.adobshop.com/products`.

![product site 2](/help/c-experiences/assets/product-site-2.png)

In the beginning of this section, we defined Views as the whole site or even a group of visual elements on the site. As shown above, the four products shown on the site can also be grouped and considered as a View. If we wanted to name this View, we can name it to be Products.

![product site 3](/help/c-experiences/assets/product-site-3.png)

We decide to click on the Load More button to explore more products on the site. The website URL does not change in this case. But a View here can represent only the second row of products shown above. The View name can be called PRODUCTS-PAGE-2.

**Checkout**: `http://www.adobeshop.com/checkout`

![check-out page](/help/c-experiences/assets/checkout.png)

Because we liked some products shown in AShop, we decided to buy a couple. Now, on the checkout site we are given some options to choose normal delivery or express delivery. Because a View can be any group of visual elements on a site, we can name this View Delivery Preferences. 

Furthermore, the Views concept can be extended much further than this. If AShop wants to personalize content on the site depending on which delivery preference is selected, a View can be created for each delivery preference. In this case, when we select Normal Delivery, the View can be named Normal Delivery. If Express Delivery is selected, the View can be named Express Delivery. 

Now, AShop may want to run an A/B Test to see whether changing the color from blue to red when Express Delivery is selected can boost conversions as opposed to keeping the button color blue for both delivery options. 

## Implementing Adobe Target Views

Now that we have covered what Adobe Target Views are, we can leverage this concept in Target to empower marketers to run A/B and XT tests on Single Page Applications via the Visual Experience Composer. This will require a one-time developer setup. Let’s go through the steps to set this up.

1. Install at.js 2.0.

   First, we need to install at.js 2.0. The newest version of at.js 2.0 was developed with Single Page Applications in mind. Previous versions of at.js and mbox.js do not support Adobe Target Views and the VEC for SPA.

   ![Implementations Details dialog box](/help/c-experiences/assets/implement-atjs-2.png)

   Download the at.js 2.0 via the Adobe Target UI located in [!UICONTROL Setup > Implementation]. at.js 2.0 can also be deployed via Adobe Launch. However, the Adobe Target Extensions are not up to date and supported.

1. Implement at.js 2.0’s newest function, `triggerView()` on your sites.

   After defining the Views of your SPA where you want to run an A/B or XT test, implement at.js 2.0’s `triggerView()` function with the Views passed in as a parameter. This allows marketers to use the VEC to design and run the A/B and XT tests for those Views defined. If the `triggerView()` function is not defined for those Views, the VEC will not detect the Views and thus marketers cannot use the VEC to design and run A/B and XT tests.

   adobe.target.triggerView(viewName, options)

   |Parameter|Type|Required?|Validation|Description|
   | --- | --- | --- | --- | --- |
   |viewName|String|Yes|1. No trailing spaces<br>2. Cannot be empty<br>3. View name should be unique for all pages.<br>4. Warning: View name should not start or end with '`/`'. This is because the customer would generally extract view name from URL path and for us "home" and "`/home`" are different.<br>5. Warning: Same view should not be consecutively triggered multiple times with the  `{page: true}` option.|Pass in any name as a string type that you want to represent your View. This View name displays in the [!UICONTROL Modifications] panel of the VEC for marketers to create actions and run their A/B and XT activities.|
   |options|Object|No|||
   |options > page|Boolean|No||**TRUE**: Default value of page is true. When `page=true`, notifications will be sent to the Edge servers for incrementing impression count.<br>**FALSE**: When `page=false`, notifications will not be sent for incrementing impression count. This should be used when you want to only re-render a component on a page with an offer.|

   Now let’s go through some example use cases on how to invoke the `triggerView()` function in React for our hypothetical AShop e-commerce SPA:

   **Home Site**: `http://www.adobeshop.com/home`

   ![home-react-1](/help/c-experiences/assets/react1.png)

   ![home-react-2](/help/c-experiences/assets/react2.png)

   ![home-react-3](/help/c-experiences/assets/react3.png)

   As AShop marketers, if we want to run A/B tests on the whole home site, then we might want to name the view as home that can be extracted from the URL:

   `[Insert Code Here]`

   **Products Site**: `http://www.adobeshop.com/products`

   Now, let’s look at an example that is a little bit more complicated. Let’s say as AShop marketers, we would like to personalize the second row of the products by changing the price label color to red after a user clicked on the Load More button.

   ![react products](/help/c-experiences/assets/react4.png)

   `[Insert Code Here]`

   **Checkout**: `http://www.adobeshop.com/checkout`

   ![react checkout](/Checkout: http://www.adobeshop.com/checkout)

   ![react checkout](/help/c-experiences/assets/react6.png)

   If AShop wants to personalize content on the site depending on which delivery preference is selected, a View can be created for each delivery preference. In this case, when we select Normal Delivery, the View can be named as Normal Delivery. If Express Delivery is selected, the View can be named as Express Delivery. 

   Now, AShop might want to run an A/B test to see whether changing the color from blue to red when Express Delivery is selected can boost conversions as opposed to keeping the button color blue for both delivery options.  

   `[INSERT CODE HERE]`

## at.js 2.0 system diagrams

The following diagrams help you understand the workflow of at.js 2.0 with Views and how this enhances the SPA integration. To get a better introduction of the concepts used in at.js 2.0, see [Single Page Application implementation](/help/c-implementing-target/c-implementing-target-for-client-side-web/how-to-deployatjs/target-atjs-single-page-application.md).

![Target flow with at.js 2.0](/help/c-implementing-target/c-implementing-target-for-client-side-web/assets/system-diagram-atjs-20.png)

|Call|Details|
| --- | --- |
|1|Call returns the [!DNL Experience Cloud ID] if the user is authenticated; another call syncs the customer ID.|
|2|The at.js library loads synchronously and hides the document body.<br>at.js can also be loaded asynchronously with an option prehiding snippet implemented on the page.|
|3|A page load request is made including all configured parameters (MCID, SDID, and customer ID).|
|4|Profile scripts execute and then feed into the Profile Store. The Store requests qualified audiences from the Audience Library (for example, audiences shared from Adobe Analytics, Audience Management, etc.).<br>Customer attributes are sent to the Profile Store in a batch process.|
|5|Based on URL request parameters and profile data, [!DNL Target] decides which activities and experiences to return to the visitor for the current page and future views.|
|6|Targeted content is sent back to the page, optionally including profile values for additional personalization.<br>Targeted content on the current page is revealed as quickly as possible without flicker of default content.<br>Targeted content for views that are shown as a result to user actions in a SPA that is cached in the browser so it can be instantly applied without an additional server call when the views are triggered through `triggerView()`.|
|7|Analytics data is sent to Data Collection servers.|
|8|Targeted data is matched to Analytics data via the SDID and is processed into the Analytics reporting storage.<br>Analytics data can then be viewed in both Analytics and Target via Analytics for Target (A4T) reports.|

Now, wherever `triggerView()` is implemented on your SPA, the Views and actions are retrieved from cache and shown to the user without a server call. `triggerView()` also makes a notifications request to the [!DNL Target] backend in order to increment and record impression counts.

![Target flow at.js 2.0 triggerView](/help/c-implementing-target/c-implementing-target-for-client-side-web/assets/atjs-20-triggerview.png)

|Call|Details|
| --- | --- |
|1|`triggerView()` is called in the SPA to render the View and apply actions to modify visual elements.|
|2|Targeted content for the view is read from the cache.|
|3|Targeted content is revealed as quickly as possible without flicker of default content.|
|4|Notification request is sent to the [!DNL Target] Profile Store to count the visitor in the activity and increment metrics.|
|5|Analytics data sent to Data Collection Servers.|
|6|Target data is matched to Analytics data via the SDID and is processed into the Analytics reporting storage. Analytics data can then be viewed in both Analytics and Target via A4T reports.|

## Single Page App Visual Experience Composer

After you have completed installing at.js 2.0 and adding `triggerView()` to your site, use the VEC to run A/B and XT activities. For more information, see [Single Page App (SPA) Visual Experience Composer](/help/c-experiences/spa-visual-experience-composer.md).