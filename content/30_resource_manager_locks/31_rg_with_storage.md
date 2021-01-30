---
title: "3.1 Resource Group with Storage Account"
date: 2021-01-29T15:28:53+03:00
tags: ["Resource Manager","Storage Account","ReadOnly Lock","Delete Lock"]
---

#### Task 1: Create a resource group with a storage account.

In this task, you will create a resource group and storage account for the lab. 

1. Sign-in to the Azure portal **`https://portal.azure.com/`**.

    >**Note**: Sign in to the Azure portal using an account that has the Owner or Contributor role in the Azure subscription you are using for this lab.

1. Open the Cloud Shell by clicking the first icon in the top right of the Azure Portal. If prompted, select **PowerShell** and **Create storage**.

1. Ensure **PowerShell** is selected in the drop-down menu in the upper-left corner of the Cloud Shell pane.

1. In the PowerShell session within the Cloud Shell pane, run the following to create a resource group (verify with your instructor regarding the value of the location parameter):

    ```powershell
    New-AzResourceGroup -Name AZ500LAB03 -Location 'EastUS'
    ```

1. In the PowerShell session within the Cloud Shell pane, run the following to create a storage account in the newly created resource group:
    
    ```powershell
    New-AzStorageAccount -ResourceGroupName AZ500LAB03 -Name (Get-Random -Maximum 999999999999999) -Location  EastUS -SkuName Standard_LRS -Kind StorageV2 
    ```

   >**Note**:  Wait until the storage account is created. This might take a couple of minutes. 

1. Close the Cloud Shell pane.

