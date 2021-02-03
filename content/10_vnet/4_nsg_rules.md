---
title: "10.4 NSG Rules"
date: 2021-02-03T11:14:56+03:00
weight: 40
---



#### Task 4: Create inbound NSG security rules to all traffic to web servers and RDP to the management servers. 

1. On the **myNsg** blade, in the **Settings** section, click **Inbound security rules**.

1. Review the default inbound security rules and then click **+ Add**.

1. On the **Add inbound security rule** blade, specify the following settings to allow TCP ports 80 and 443 to the **myAsgWebServers** application security group (leave all other values with their default values): 

    |Setting|Value|
    |---|---|
    |Destination|in the drop-down list, select **Application security group** and then click **myAsgWebServers**|
    |Destination port ranges|**80,443**|
    |Protocol|**TCP**|
    |Priority|**100**|                                                    
    |Name|**Allow-Web-All**|

1. On the **Add inbound security rule** blade, click **Add** to create the new inbound rule. 

1. On the **myNsg** blade, in the **Settings** section, click **Inbound security rules**, and then click **+ Add**.

1. On the **Add inbound security rule** blade, specify the following settings to allow the RDP port (TCP 3389) to the **myAsgMgmtServers** application security group (leave all other values with their default values): 

    |Setting|Value|
    |---|---|
    |Destination|in the drop-down list, select **Application security group** and then click **myAsgMgmtServers**|
    |Destination port ranges|**3389**|
    |Protocol|**TCP**|
    |Priority|**110**|                                                    
    |Name|**Allow-RDP-All**|

1. On the **Add inbound security rule** blade, click **Add** to create the new inbound rule. 

> Result: You have deployed a virtual network, network security with inbound security rules, and two application security groups. 
