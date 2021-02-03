---
title: "103.1 Webserver"
date: 2021-02-03T11:19:02+03:00
---


#### Task 1: Create a virtual machine to use as a web server.

In this task, you will create a virtual machine to use as a web server.

1. In the Azure portal, in the **Search resources, services, and docs** text box at the top of the Azure portal page, type **Virtual machines** and press the **Enter** key.

1. On the **Virtual machines** blade, click **+ Add** and, in the dropdown list, click **+ Virtual machine**.

1. On the **Basics** tab of the **Create a virtual machine** blade, specify the following settings (leave others with their default values):

   |Setting|Value|
   |---|---|
   |Subscription|the name of the Azure subscription you will be using in this lab|
   |Resource group|**AZ500LAB07**|
   |Virtual machine name|**myVmWeb**|
   |Region|**(US)East US**|
   |Image|**Windows Server 2019 Datacenter Gen 1**|
   |Size|**Standard D2s v3**|
   |Username|**Student**|
   |Password|**Pa55w.rd1234**|
   |Public inbound ports|**None**|
   |Already have a Windows Server license|**No**|

    >**Note**: For public inbound ports, we will rely on the precreated NSG. 

1. Click **Next: Disks >** and, on the **Disks** tab of the **Create a virtual machine** blade, set the **OS disk type** to **Standard HDD** and click **Next: Networking >**.

1. On the **Networking** tab of the **Create a virtual machine** blade, select the previously created network **myVirtualNetwork**.

1. Under **NIC network security group** select **None**.

1. Click **Next: Management >**, on the **Management** tab of the **Create a virtual machine** blade, specify the following settings

   |Setting|Value|
   |---|---|
   |Boot diagnostics|**Enabled with managed storage account (recommended)**|
   |Diagnostics storage account|the default value|

1. Click **Review + create**, on the **Review + create** blade, ensure that validation was successful and click **Create**.