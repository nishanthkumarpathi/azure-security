---
title: "104.4 Application Rule"
date: 2021-02-03T11:22:44+03:00
---





#### Task 4: Configure an application rule

In this task you will create an application rule that allows outbound access to `www.bing.com`.

1. In the Azure portal, navigate back to the **Test-FW01** firewall.

1. On the **Test-FW01** blade, in the **Settings** section, click **Rules**.

1. On the **Test-FW01 \| Rules** blade, click the **Application rule collection** tab, and then click **+ Add application rule collection**.

1. On the **Add application rule collection** blade, specify the following settings (leave others with their default values):

   |Setting|Value|
   |---|---|
   |Name|**App-Coll01**|
   |Priority|**200**|
   |Action|**Allow**|

1. On the **Add application rule collection** blade, create a new entry in the **Target FQDNs** section with the following settings (leave others with their default values):

   |Setting|Value|
   |---|---|
   |name|**AllowGH**|
   |Source type|**IP Address**|
   |Source|**10.0.2.0/24**|
   |Protocol port|**http:80, https:443**|
   |Target FQDNS|**www.bing.com**|

1. Click **Add** to add the Target FQDNs-based application rule.

    >**Note**: Azure Firewall includes a built-in rule collection for infrastructure FQDNs that are allowed by default. These FQDNs are specific for the platform and can't be used for other purposes. 