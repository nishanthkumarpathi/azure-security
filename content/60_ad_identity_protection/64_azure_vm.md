---
title: "6.4 Azure VM"
date: 2021-02-03T10:56:10+03:00
---


#### Task 4: Deploy an Azure VM by using an Azure Resource Manager template

In this task, you will create a virtual machine by using an ARM template. This virtual machine will be used in the last exercise for this lab. 

1. Sign-in to the Azure portal **`https://portal.azure.com/`**.

    >**Note**: Sign in to the Azure portal using an account that has the Owner or Contributor role in the Azure subscription you are using for this lab and the Global Administrator role in the Azure AD tenant associated with that subscription.

1. In the Azure portal, in the **Search resources, services, and docs** text box at the top of the Azure portal page, type **custom template** and select **Deploy a custom template** under the list of **Services**.

    >**Note**: You can also select **Template Deployment (deploy using custom templates)** from the **Marketplace** list.

1. On the **Custom deployment** blade, click the **Build your own template in the editor** option.

1. On the **Edit template** blade, click **Load file**, locate the **az-500-04_azuredeploy.json** file and click **Open**.

    >**Note**: Review the content of the template and note that it deploys an Azure VM hosting Windows Server 2019 Datacenter.

1. On the **Edit template** blade, click **Save**.

1. Back on the **Custom deployment** blade, click **Edit parameters**.

1. On the **Edit parameters** blade, click **Load file**, locate the **az-500-04_azuredeploy.parameters.json** file and click **Open**.

    >**Note**: Review the content of the parameters file noting the adminUsername and adminPassword values.

1. On the **Edit parameters** blade, click **Save**.

1. On the **Custom deployment** blade, ensure that the following settings are configured (leave any others with their default values):

   |Setting|Value|
   |---|---|
   |Subscription|the name of the Azure subscription you will be using in this lab|
   |Resource group|click **Create new** and type the name **AZ500LAB04**|
   |Location|**(US) East US**|
   |Vm Size|**Standard_D2s_v3**|
   |Vm Name|**az500-04-vm1**|
   |Admin Username|**Student**|
   |Admin Password|**Pa55w.rd1234**|
   |Virtual Network Name|**az500-04-vnet1**|

    >**Note**: To identify Azure regions where you can provision Azure VMs, refer to [**https://azure.microsoft.com/en-us/regions/offers/**](https://azure.microsoft.com/en-us/regions/offers/)

1. Click **Review + create**, and then click **Create**.

    >**Note**: Do not wait for the deployment to complete but proceed to the next exercise. You will use the virtual machine included in this deployment in the last exercise of this lab.

> Result: You have initiated a template deployment of an Azure VM **az500-04-vm1** that you will use in the last exercise of this lab.
