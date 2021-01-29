---
title: "3.2 ReadOnly lock on the storage account"
date: 2021-01-29T15:29:06+03:00
---


#### Task 2: Add a ReadOnly lock on the storage account. 

In this task, you will add a read only lock to the storage account. This will protect the resource from accidental deletion or modification. 

1. In the Azure portal, in the **Search resources, services, and docs** text box at the top of the Azure portal page, type **Resource groups** and press the **Enter** key.

1. On the **Resource groups** blade, select the **AZ500LAB03** resource group entry.

1. On the **AZ500LAB03** resource group blade, in the list of resources, select the new storage account. 

1. In the **Settings** section, click the "Locks" icon.

1. Click **+ Add** and specify the following settings:

   |Setting|Value|
   |---|---|
   |Lock name|**ReadOnly Lock**|
   |Lock type|**Read-only**|

1. Click **OK**. 

   >**Note**:  The storage account is now protected from accidental deletion and modification.
