---
title: "102.1 Virtual network with one subnet"
date: 2021-02-03T11:12:21+03:00
---



#### Task 1:  Create a virtual network

In this task, you will create a virtual network to use with the network and application security groups. 

1. Sign-in to the Azure portal **`https://portal.azure.com/`**.

    >**Note**: Sign in to the Azure portal using an account that has the Owner or Contributor role in the Azure subscription you are using for this lab.

1. In the Azure portal, in the **Search resources, services, and docs** text box at the top of the Azure portal page, type **Virtual networks** and press the **Enter** key.

1. On the **Virtual networks** blade, click **+ Add**.

1. On the **Basics** tab of the **Create virtual network** blade, specify the following settings (leave others with their default values) and click **Next: IP Addresses**:

    |Setting|Value|
    |---|---|
    |Subscription|the name of the Azure subscription you are using in this lab|
    |Resource group|click **Create new** and type the name **AZ500LAB07**|
    |Name|**myVirtualNetwork**|
    |Region|**East US**|

1. On the **IP addresses** tab of the **Create virtual network** blade, set the **IPv4 address space** to **10.0.0.0/16**, and, if needed, in the **Subnet name** column, click **default**, on the **Edit subnet** blade, specify the following settings and click **Save**:

    |Setting|Value|
    |---|---|
    |Subnet name|**default**|
    |Subnet address range|**10.0.0.0/24**|

1. Back on the **IP addresses** tab of the **Create virtual network** blade, click **Review + create**.

1. On the **Review + create** tab of the **Create virtual network** blade, click **Create**.