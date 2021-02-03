---
title: "104.5 Network Rule"
date: 2021-02-03T11:22:54+03:00
---



#### Task 5: Configure a network rule

In this task, you will create a network rule that allows outbound access to two IP addresses on port 53 (DNS).

1. In the Azure portal, navigate back to the **Test-FW01 \| Rules** blade.

1. On the **Test-FW01 \| Rules** blade, click the **Network rule collection** tab and then click **+ Add network rule collection**.

1. On the **Add network rule collection** blade, specify the following settings (leave others with their default values):

   |Setting|Value|
   |---|---|
   |Name|**Net-Coll01**|
   |Priority|**200**|
   |Action|**Allow**|

1. On the **Add network rule collection** blade, create a new entry in the **IP Addresses** section with the following settings (leave others with their default values):

   |Setting|Value|
   |---|---|
   |Name|**AllowDNS**|
   |Protocol|**UDP**|
   |Source type|**IP address**|
   |Source Addresses|**10.0.2.0/24**|
   |Destination type|**IP address**|
   |Destination Address|**209.244.0.3,209.244.0.4**|
   |Destination Ports|**53**|

1. Click **Add** to add the network rule.

    >**Note**: The destination addresses used in this case are known public DNS servers. 