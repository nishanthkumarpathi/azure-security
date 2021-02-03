---
title: "3.3 Test the ReadOnly lock "
date: 2021-01-29T15:29:23+03:00
weight: 3
---


#### Task 3: Test the ReadOnly lock 

1. In the **Settings** section of the storage account blade, click **Configuration**.

1. Set the **Secure transfer required** option to **Disabled** and then click **Save**.

1. You should be able to spot a notification stating **Failed to update storage account**.

1. Click the **Notifications** icon in the toolbar at the top of the Azure portal and review the notification, which will resemble the following text: 

	> **"Failed to update storage account 'xxxxxxxx'. Error: The scope 'xxxxxxxx' cannot perform write operation because following scope(s) are locked: '/subscriptions/xxxxx-xxx-xxxx-xxxx-xxxxxxxx/resourceGroups/AZ500LAB03/providers/Microsoft.Storage/storageAccounts/xxxxxxx'. Please remove the lock and try again"**

1. Return the the **Configuration** blade of the storage account and click **Discard**. 

1. On the storage account blade, select **Overview** and, on the **Overview** blade, click **Delete**.

1. On the **Delete storage account** blade, type in the name of the storage account to confirm that you intend to proceed and then click **Delete**.

1. Review the newly generated notification, which will resemble the following text: 

	> **"Failed to delete storage account 'xxxxxxx'. Error: The scope 'xxxxxxx' cannot perform delete operation because following scope(s) are locked: '/subscriptions/xxxx-xxxx-xxxx-xxxx-xxxxxx/resourceGroups/AZ500LAB03/providers/Microsoft.Storage/storageAccounts/xxxxxxx'. Please remove the lock and try again."**

   >**Note**:  You have now verified that a ReadOnly lock will stop accidental deletion and modification of a resource.
