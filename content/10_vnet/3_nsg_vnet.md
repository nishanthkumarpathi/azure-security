---
title: "10.3 ASG with Subnet"
date: 2021-02-03T11:14:44+03:00
weight: 30
---


#### Task 3:  Create a network security group and associate the NSG to the subnet

In this task, you will create a network security group. 

1. In the Azure portal, in the **Search resources, services, and docs** text box at the top of the Azure portal page, type **Network security groups** and press the **Enter** key.

1. On the **Network security groups** blade, click **+ Add**.

1. On the **Basics** tab of the **Create network security group** blade, specify the following settings: 

    |Setting|Value|
    |---|---|
    |Subscription|the name of the Azure subscription you are using in this lab|
    |Resource group|**AZ500LAB07**|
    |Name|**myNsg**|
    |Region|**East US**|

1. Click **Review + create** and then click **Create**.

1. In the Azure portal, navigate back to the **Network security groups** blade and click the **myNsg** entry.

1. On the **myNsg** blade, in the **Settings** section, click **Subnets** and then click **+ Associate**. 

1. On the **Associate subnet** blade, specify the following settings and click **OK**:

    |Setting|Value|
    |---|---|
    |Virtual network|**myVirtualNetwork**|
    |Subnet|**default**|