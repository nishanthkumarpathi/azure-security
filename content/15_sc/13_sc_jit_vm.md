---
title: "15.3 SC JIT VM"
weight: 13
---


#### Task 3: Implement the Security Center recommendation to enable Just in time VM Access

In this task, you will implement the Security Center recommendation to enable Just in time VM Access on the virtual machine. 

1. In the Azure portal, navigate back to the **Security Center \| Overview** blade. 

1. On the **Cloud Security \| Azure Defender** blade, click the **Just-in-time- VM access** tab, select **Not Configured** and then click the **myVM** entry.

1. Select **Enable JIT on 1 VM**.

1. On the **JIT VM access configuration** blade, on the far right of the row referencing the port **22**, click the ellipsis button and then click **Delete**.

1. On the **JIT VM access configuration** blade, click **Save**.

    >**Note**: Monitor the progress of configuration by clicking on the **Notifications** icon in the toolbar and viewing the **Notifications** blade. 

    >**Note**: It can take some time for the implementation of recommendations in this lab to be reflected by Secure Score. Periodically check the Secure Score to determine the impact of implementing these features. 

> Results: You have on-boarded Security Center and implemented virtual machine recommendations. 


>**Note**: Do not remove the resources from this lab as they are needed for the Azure Sentinel lab.

