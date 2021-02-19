---
title: "13.2 KeyVault Configuration"
weight: 12
---


#### Task 2: Create and configure a Key Vault

In this task, you will create an Azure Key Vault resource. You will also configure the Azure Key Vault permissions.

1. Open the Cloud Shell by clicking the first icon (next to the search bar) at the top right of the Azure portal. If prompted, select **PowerShell** and **Create storage**.

1. Ensure **PowerShell** is selected in the drop-down menu in the upper-left corner of the Cloud Shell pane.

1. In the PowerShell session within the Cloud Shell pane, run the following to create an Azure Key Vault in the resource group **AZ500LAB10**. (If you chose another name for this lab's Resource Group out of Task 1, use that name for this task as well). The Key Vault name must be unique. Remember the name you have chosen. You will need it throughout this lab.  

    ```powershell
    $kvName = 'az500kv' + $(Get-Random)

    $location = (Get-AzResourceGroup -ResourceGroupName 'AZ500LAB10').Location

    New-AzKeyVault -VaultName $kvName -ResourceGroupName 'AZ500LAB10' -Location $location
    ```

    >**Note**: The output of the last command will display the vault name and the vault URI. The vault URI is in the format `https://<vault_name>.vault.azure.net/`

1. Close the Cloud Shell pane. 

1. In the Azure portal, in the **Search resources, services, and docs** text box at the top of the Azure portal page, type **Resource groups** and press the **Enter** key.

1. On the **Resource groups** blade, in the list of resource group, click the **AZ500LAB10** (or other name you chose earlier for the resource group) entry.

1. On the Resource Group blade, click the entry representing the newly created Key Vault. 

1. On the Key Vault blade, in the **Settings** section, click **Access Policies** and then click **+ Add Access Policy**.

1. On the **Add access policy** blade, specify the following settings (leave all others with their default values): 

    |Setting|Value|
    |----|----|
    |Configure from template (optional)|**Key, Secret, & Certificate Management**|
    |Key permissions|click **Select all** resulting in **16 selected** permissions|
    |Secret permissions|click **Select all** resulting in total of **8 selected** permissions|
    |Certification permissions|click **Select all** resulting in total of **16 selected** permissions|
    |Select principal|click **None selected**, on the **Principal** blade, select your user account, and click **Select**|

1. Back on the **Add access policy** blade, click **Add** to add the access policy and, back on the access policies blade of the Key Vault, click **Save** to your changes. 

