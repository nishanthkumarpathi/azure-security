---
title: "104.2 Azure Firewall"
date: 2021-02-03T11:22:25+03:00
---


#### Task 2: Deploy the Azure firewall

In this task you will deploy the Azure firewall into the virtual network. 

1. In the Azure portal, in the **Search resources, services, and docs** text box at the top of the Azure portal page, type **Firewalls** and press the **Enter** key.

1. On the **Firewalls** blade, click **+ Add**.

1. On the **Basics** tab of the **Create a firewall** blade, specify the following settings (leave others with their default values):

   |Setting|Value|
   |---|---|
   |Resource group|**AZ500LAB08**|
   |Name|**Test-FW01**|
   |Region|**(US) East US**|
   |Choose a virtual network|click the **Use existing** option and, in the drop-down list, select **Test-FW-VN**|
   |Public IP address|clck **Add new** and type the name **TEST-FW-PIP** and click **OK**|

1. Click **Review + create** and then click **Create**. 

    >**Note**: Wait for the deployment to complete. This should take about 5 minutes. 

1. In the Azure portal, in the **Search resources, services, and docs** text box at the top of the Azure portal page, type **Resource groups** and press the **Enter** key.

1. On the **Resource groups** blade, in the list of resource group, click the **AZ500LAB08** entry.

    >**Note**: On the **AZ500LAB08** resource group blade, review the list of resources. You can sort by **Type**.

1. In the list of resources, click the entry representing the **Test-FW01** firewall.

1. On the **Test-FW01** blade, identify the **Private IP** address that was assigned to the firewall. 

    >**Note**: You will need this information in the next task.