---
title: "102.2 Application security groups"
date: 2021-02-03T11:12:55+03:00
---



#### Task 2:  Create application security groups

In this task, you will create an application security group.

1. In the Azure portal, in the **Search resources, services, and docs** text box at the top of the Azure portal page, type **Application security groups** and press the **Enter** key.

1. On the **Application security groups** blade, click **+ Add**.

1. On the **Basics** tab of the **Create an application security group** blade, specify the following settings: 

    |Setting|Value|
    |---|---|
    |Resource group|**AZ500LAB07**|
    |Name|**myAsgWebServers**|
    |Region|**East US**|

    >**Note**: This group will be for the web servers.

1. Click **Review + create** and then click **Create**.

1. Navigate back to the **Application security groups** blade and click **+ Add**.

1. On the **Basics** tab of the **Create an application security group** blade, specify the following settings: 

    |Setting|Value|
    |---|---|
    |Resource group|**AZ500LAB07**|
    |Name|**myAsgMgmtServers**|
    |Region|**East US**|

    >**Note**: This group will be for the management servers.

1. Click **Review + create** and then click **Create**.