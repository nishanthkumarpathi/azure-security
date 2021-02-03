---
title: "2.3 Verify Allowed Locations Policy"
date: 2021-01-29T15:18:39+03:00
weight: 30
tags: ["Azure Policy","Resource Group","Policy Assignments","Allowed Locations"]
---


#### Task 3: Test the Allowed Locations policy assignment

In this task, you will test the Allowed Locations policy assignment. 

1. In the Azure portal, in the **Search resources, services, and docs** text box at the top of the Azure portal page, type **Virtual networks** and press the **Enter** key.

1. On the **Virtual Networks** blade, click **+ Add**.

   >**Note**: First, you will try to create a virtual network in East US. Since this is not an allowed location, the request should be blocked. 

1. On the **Basics** tab of the **Create virtual network** blade, specify the following settings (leave others with their defualt values):

    |Setting|Value|
    |---|---|
    |Resource group|**AZ500LAB02**|
    |Name|**myVnet**|
    |Region|**(US) East US**|

1. Click **Review + create**. 

1. On the **Review + create** tab of the **Create virtual network** blade note the **Validation failed** message. 

    > **Note**: If the **Validation Failed** warning does not appear, click **Previous** and wait a few more minutes.

1. Click the error message to open the **Errors** blade. You will see the detailed error message stating that the deployment of the resource **myVnet** was disallowed by policy.

1. Close the **Errors** blade, on the **Create virtual network** blade, click the **Basics** tab, and, in the **Region** drop-down list, select **(Europe) UK South**.

1. Click **Review + create**, verify that validation passed, click **Create**, and verify that the virtual network was created successfully. 

> Exercise results: In this exercise, you learned to apply an Azure policy by selecting a built-in policy definitions and assigning it to a resource group.
