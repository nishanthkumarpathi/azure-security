---
title: "3.5 Delete Lock Testing"
date: 2021-01-29T15:29:52+03:00
---

#### Task 5: Test the Delete lock.

In this task, you will test the Delete lock. You should be able to modify the storage account, but not delete it. 

1. In the **Settings** section of the storage account blade, click **Configuration**.

1. Set the **Secure transfer required** option to **Disabled** and then click **Save**.

   >**Note**:  This time, the change should be successful.

1. On the storage account blade, select **Overview** and, on the **Overview** blade, click **Delete**.

1. On the **Delete storage account** blade, type in the name of the storage account to confirm that you intend to proceed and then click **Delete**.

1. Review the notification that resembles the following text: 

	> **'xxxxxx' can't be deleted because this resource or its parent has a delete lock. Locks must be removed before this resource can be deleted"**

   >**Note**:  You have now verified that a **Delete** lock will allow configuration changes but stop accidental deletion.

   >**Note**:  By using Resource Locks you can implement an extra line of defense against accidental or malicious changes and/or deletion of the most important resources. Resource locks can be removed by any user with the **Owner** role, but doing so requires a conscious effort. Locks supplement Role Based Access Control. 

> Results: In this exercise, you learned to use Resource Manager locks to protect resources from modification and accidental deletion.
