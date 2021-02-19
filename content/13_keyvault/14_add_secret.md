---
title: "13.4 Add Secret to KV"
weight: 14
---


#### Task 4: Add a Secret to Key Vault

1. Switch back to the Cloud Shell pane.

1. In the PowerShell session within the Cloud Shell pane, run the following to create a variable with a secure string value:

    ```powershell
    $secretvalue = ConvertTo-SecureString 'Pa55w.rd1234' -AsPlainText -Force
    ```

1.  In the PowerShell session within the Cloud Shell pane, run the following to add the secret to the vault:

    ```powershell
    $secret = Set-AZKeyVaultSecret -VaultName $kv.VaultName -Name 'SQLPassword' -SecretValue $secretvalue
    ```

    >**Note**: The name of the secret is SQLPassword. 

1.  In the PowerShell session within the Cloud Shell pane, run the following to verify the secret was created.

    ```powershell
    Get-AZKeyVaultSecret -VaultName $kv.VaultName
    ```

1. Minimize the Cloud Shell pane. 

1. In the Azure portal, navigate back to the Key Vault blade, in the **Settings** section, click **Secrets**.

1. In the list of secrets, click the **SQLPassword** entry and then, on the **SQLPassword** blade, click the entry representing the current version of the secret.

    >**Note**: Examine the information about the secret you created.

    >**Note**: To get the most current version of a secret, reference `https://<key_vault_name>.vault.azure.net/secrets/<secret_name>` or get a specific version, reference `https://<key_vault_name>.vault.azure.net/secrets/<secret_name>/<secret_version>`
