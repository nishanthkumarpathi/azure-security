---
title: "3.4 ReadOnly lock and Delete Lock"
date: 2021-01-29T15:29:41+03:00
---


#### Task 4: Remove the ReadOnly lock and create a Delete lock.

In this task, you remove the ReadOnly lock from the storage account and create a Delete lock. 

1. In the Azure portal, navigate back to the blade displaying properties of the newly created storage account.

1. In the **Settings** section , select **Locks**.  

1. On the **Locks** blade, click on the **Delete** icon on the far right of the **ReadOnly Lock** entry.

1. Click **+ Add** and specify the following settings:

   |Setting|Value|
   |---|---|
   |Lock name|**Delete Lock**|
   |Lock type|**Delete**|

1. Click **OK**. 
