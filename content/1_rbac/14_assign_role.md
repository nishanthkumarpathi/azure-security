---
title: "1.4 Assign Role"
date: 2021-01-29T13:42:29+03:00
draft: false
weight: 4
---


#### Task 4: Assign the Service Desk Virtual Machine Contributor permissions. 

1. On the **Resource groups** blade, click the **AZ500LAB01** resource group entry.

1. On the **AZ500Lab01** blade, click **Access control (IAM)**.

1. On the **AZ500Lab01 \| Access control (IAM)** blade, click **+ Add** and then, in the drop-down menu, click **Add role assignment**.

1. On the **Add role assignment** blade, specify the following settings:

   |Setting|Value|
   |---|---|
   |Role|**Virtual Machine Contributor**|
   |Assign access to|**User, group, or service principal**|
   |Select|**Service Desk**|

1. Choose **Save** to create the role assignment.

1. From the **Access control (IAM)** blade, select **Role assignments**.

1. On the **AZ500Lab01 \| Access control (IAM)** blade, on the **Check access** tab, in the **Search by name or email address** text box, type **Dylan Williams**.

1. In the list of search results, select the user account of Dylan Williams and, on the **Dylan Williams assignments - AZ500Lab01** blade, view the newly created assignment.

1. Close the **Dylan Williams assignments - AZ500Lab01** blade.

1. Repeat the same last two steps to check access for **Joseph Price**. 

> Result: You have assigned and checked RBAC permissions. 