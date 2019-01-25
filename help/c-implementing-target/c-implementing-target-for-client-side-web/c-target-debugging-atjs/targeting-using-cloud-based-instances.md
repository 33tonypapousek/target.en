---
description: Information about issues customers face when using cloud-based instances to test Adobe Target.
keywords: cloud instances;public suffix list;public suffix;cookie;first-party cookie;1st-party cookie;azurewebsites.net;cloudapp.net;amazonaws.com;cloudfront.net;herokuapp.com;firebaseapp.com;targetGlobalSettings;cookieDomain
seo-description: Information about issues customers face when using cloud-based instances to test Adobe Target.
seo-title: Use cloud-based instances with Target
solution: Target
title: Use cloud-based instances with Target
uuid: dcaba49e-7567-4970-bb9a-19377aff7d38
---

# Use cloud-based instances with Target{#use-cloud-based-instances-with-target}

Information about issues customers face when using cloud-based instances to test Adobe Target.

Target customers sometimes use cloud-based instances with [!DNL Target] for testing or simple proof-of-concept purposes. These instances might include the following domains: 

`azurewebsites.net`, `cloudapp.net`, `amazonaws.com`, `cloudfront.net`, `herokuapp.com`, or `firebaseapp.com`

These domains, and many others, are part of the [Public Suffix List](https://publicsuffix.org/list/public_suffix_list.dat).

**Issue:** Modern browsers won't save cookies if you are using these domains.

The [!DNL at.js] and [!DNL mbox.js] JavaScript libraries use cookies to track users to ensure that [!DNL Target] always presents a consistent experience. If the [!DNL Target] JavaScript libraries can't save cookies, [!DNL Target] requests are disabled.

**Solution:** As best practice, if you intend to use cloud-based instances with domains included on the Public Suffix List, make sure that you customize the `cookieDomain` setting. For more information, see [targetGlobalSettings()](../../../c-implementing-target/c-implementing-target-for-client-side-web/cmp-at.js-functions.md#concept_8DACBC47ABDE4279BB102B42609FE506). 
