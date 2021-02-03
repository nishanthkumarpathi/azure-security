---
title: "2.1 Resource Group"
date: 2021-01-29T15:13:36+03:00
draft: false
weight: 10
tags: ["Azure Policy","Resource Group","Policy Assignments","Allowed Locations"]
---


#### Task 1: Create a resource group for the lab. 

In this task, you will create a resource group for the lab. 

1. Sign-in to the Azure portal **`https://portal.azure.com/`**.

    >**Note**: Sign in to the Azure portal using an account that has the Owner or Contributor role in the Azure subscription you are using for this lab.

1. Open the Cloud Shell by clicking the first icon in the top right of the Azure Portal. If prompted, select **PowerShell** and **Create storage**.

1. Ensure **PowerShell** is selected in the drop-down menu in the upper-left corner of the Cloud Shell pane.

1. In the PowerShell session within the Cloud Shell pane, run the following to create a resource group (verify with your instructor regarding the value of the location parameter):

    ```powershell
    New-AzResourceGroup -Name AZ500LAB02 -Location 'East US'
    ```

1. In the PowerShell session within the Cloud Shell pane, run the following to list resource groups to verify that the new resource group was created:

    ```powershell
    Get-AzResourceGroup | format-table
    ```

1. Close the **Cloud Shell**.
