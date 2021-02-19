---
title: "15.1 Security Center Config"
weight: 11
---



#### Task 1: Configure Security Center

In this task, you will on-board and configure Security Center.

1. Sign-in to the Azure portal **`https://portal.azure.com/`**.

    >**Note**: Sign in to the Azure portal using an account that has the Owner or Contributor role in the Azure subscription you are using for this lab.

1. In the Azure portal, in the **Search resources, services, and docs** text box at the top of the Azure portal page, type **Security Center** and press the **Enter** key.

1. On the **Security Center \| Getting started** blade, click **Upgrade** and then click **Install agents**.
     
1. On the **Security Center \| Getting started** blade, in the vertical menu on the left side, in the **Management** section, click **Pricing & settings**.

1. On the **Security Center \| Pricing & settings** blade, click the entry representing your subscription and, on the **Settings \| Azure Defender Plans** blade, ensure that **Azure Defender on** is selected. 

    >**Note**: Review all the features that are available as part of Azure Defender tier and ensure that Azure Defender turned on for each resource type. 

1. If you made any changes, click **Save**.

1. On the **Settings \| Azure Defender plans** blade, in the vertical menu bar on the left side, click **Auto Provisioning**.

1. On the **Settings \| Auto Provisioning** blade, make sure that **Auto provisioning** is set to **On** for the first item **Log Analytics agent for Azure VMs**. 

1. On the **Settings \| Auto Provisioning** blade, for the first item **Log Analytics agent for Azure VMs** click the **Edit Configuration** link in the **Configuration** column. 

1. On the **Extension deployment configuration** blade, in the **Workspace configuration** section, select the **Connect Azure VMs to a different workspace** option and, in the drop-down list, select the Log Analytics workspace you created in the previous lab. 

1. On the **Extension deployment configuration** blade, click **Apply**, when prompted, select the **Existing and new VMs** option, and click **Apply** again.

1. Back on the **Settings \| Auto provisioning** blade, in the vertical menu on the left side, click **Workflow automation**.

1. On the **Settings \| Workflow automation** blade, click **+ Add workflow automation**.

1. On the **Add workflow automation** blade, review the available settings. 

    >**Note**: You can trigger actions based threat detection alerts and Security Center recommendations. You can also configure an action based on Logic apps. 

1. On the **Add workflow automation** blade, click **Cancel**.

    >**Note**: Security Center provides many insights into virtual machines including system update status, OS security configurations, and endpoint protection.

