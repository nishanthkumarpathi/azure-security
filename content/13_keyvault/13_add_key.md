---
title: "13.3 Add Key to KV"
weight: 13
---


#### Task 3: Add a key to Key Vault

In this task, you will add a key to the Key Vault and view information about the key. 

1. In the Azure portal, open a PowerShell session in the Cloud Shell pane.

1. Ensure **PowerShell** is selected in the upper-left drop-down menu of the Cloud Shell pane.

1. In the PowerShell session within the Cloud Shell pane, run the following to add a software-protected key to the Key Vault: 

    ```powershell
    $kv = Get-AzKeyVault -ResourceGroupName 'AZ500LAB10'

    $key = Add-AZKeyVaultKey -VaultName $kv.VaultName -Name 'MyLabKey' -Destination 'Software'
    ```

    >**Note**: The name of the key is **MyLabKey**

1. In the PowerShell session within the Cloud Shell pane, run the following to verify the key was created:

    ```powershell
    Get-AZKeyVaultKey -VaultName $kv.VaultName
    ```

1. In the PowerShell session within the Cloud Shell pane, run the following to display the key identifier:

    ```powershell
    $key.key.kid
    ```

1. Minimize the Cloud Shell pane. 

1. Back in the Azure portal, on the Key Vault blade, in the **Settings** section, click **Keys**.

1. In the list of keys, click the **MyLabKey** entry and then, on the **MyLabKey** blade, click the entry representing the current version of the key.

    >**Note**: Examine the information about the key you created.

    >**Note**: You can reference any key by using the key identifier. To get the most current version, reference `https://<key_vault_name>.vault.azure.net/keys/MyLabKey` or get the specific version with: `https://<key_vault_name>.vault.azure.net/keys/MyLabKey/<key_version>`