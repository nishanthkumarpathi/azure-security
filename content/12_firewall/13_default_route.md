---
title: "12.3 Default Route"
date: 2021-02-03T11:22:36+03:00
weight: 30
---



#### Task 3: Create a default route

In this task, you will create a default route for the **Workload-SN** subnet. This route will configure outbound traffic through the firewall.

1. In the Azure portal, in the **Search resources, services, and docs** text box at the top of the Azure portal page, type **Route tables** and press the **Enter** key.

1. On the **Route tables** blade, click **+ Add**.

1. On the **Create route table** blade, specify the following settings:

   |Setting|Value|
   |---|---|
   |Name|**Firewall-route**|
   |Resource group|**AZ500LAB08**|
   |Region| **East US**|

1. Click **Review + create**, then click **Create**, and wait for the provisioning to complete. 

1. On the **Route tables** blade, click **Refresh**, and, in the list of route tables, click the **Firewall-route** entry.

1. On the **Firewall-route** blade, in the **Settings** section, click **Subnets** and then, on the **Firewall-route \| Subnets** blade, click **+ Associate**.

1. On the **Associate subnet** blade, specify the following settings:

   |Setting|Value|
   |---|---|
   |Virtual network|**Test-FW-VN**|
   |Subnet|**Workload-SN**|

    >**Note**: Ensure the **Workload-SN** subnet is selected for this route, otherwise the firewall won't work correctly.

1. Click **OK** to associate the firewall to the virtual network subnet. 

1. Back on the **Firewall-route** blade, in the **Settings** section, click **Routes** and then click **+ Add**. 

1. On the **Add route** blade, specify the following settings:  

   |Setting|Value|
   |---|---|
   |Route name|**FW-DG**|
   |Address prefix|**0.0.0.0/0**
   |Next hop type|**Virtual appliance**|
   |Next hop address|the private IP address of the firewall that you identified in the previous task|

    >**Note**: Azure Firewall is actually a managed service, but virtual appliance works in this situation.
	
1.  Click **OK** to add the route. 
