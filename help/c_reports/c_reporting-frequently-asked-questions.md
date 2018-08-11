---
description: List of frequently asked questions about reporting in Target.
keywords: troubleshooting;metric discrepancies;FAQ;reports
seo-description: List of frequently asked questions about reporting in Target.
seo-title: Reporting Frequently Asked Questions
solution: Target
title: Reporting Frequently Asked Questions
topic: Standard
uuid: 5c37faf1-f4ab-49ac-a7d4-6b9476b93456
index: y
internal: n
snippet: y
translate: y
---

# Reporting Frequently Asked Questions

This section contains the following information: 


* [ Why are the number of visits lower in Target than...](../c_reports/c_reporting-frequently-asked-questions.md#section_7E626FDB417E41B8B58BBF30FB207409)
* [ Why is there no data available for my activity's report?](../c_reports/c_reporting-frequently-asked-questions.md#section_E4722F6445884130951DF79981C8289B)


## Why are the number of visits lower in Target than in other Experience Cloud solutions? {#section_7E626FDB417E41B8B58BBF30FB207409}

Metric numbers, for example visits, reported by [!DNL  Target] will always be lower than the reported numbers in other [!DNL  Experience Cloud] solutions for a number of reasons: 


* [!DNL  Target] counts visits only for visitors that qualified for the activity. Other solutions count visits for visitors that display the page, regardless of which activity brought them to the page. 

* There might be situation where different activities compete for the same location (mutually exclusive). As a result, visitors see different content on a web page, which affects the metric numbers reported by [!DNL  Target]. 



## Why is there no data available for my activity's report? {#section_E4722F6445884130951DF79981C8289B}

If an activity's content was successfully delivered to users but its report contains no data, ensure that you have the correct environment (host group) selected in the report's settings. 

If you have a development environment selected, you might see the following error message: "There is no data available for the selected report settings." 

To change the environment for an activity's report: 


1. Click ** [!UICONTROL  Activities] **, click the desired activity from the list, then click the ** [!UICONTROL  Reports] ** tab. 

1. Click the [!UICONTROL  Settings] icon (  ![](../assets/icon_gear.png) ) to configure report settings. 

   ![](../assets/ab_settings_dialog.png) 


   >[!NOTE]
   >
   >The Settings icon ( ![](../assets/icon_gear.png) ) is not available for Automated Personalization reports. 


1. From the ** [!UICONTROL  Environment] ** drop-down list, select ** [!UICONTROL  Production] **. 

   Report data might not be available if you have a development environment selected. 

1. Click ** [!UICONTROL  Save Settings] **. 



For more information about environments, see [ Hosts](../c_seting_up_target/c_hosts.md#concept_516BB01EBFBD4449AB03940D31AEB66E). 
