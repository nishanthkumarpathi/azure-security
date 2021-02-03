---
title: "11.3 VM with ASG"
date: 2021-02-03T11:19:26+03:00
weight: 30
---


#### Task 3: Associate each virtual machines network interface to its application security group.

In this task, you will associate each virtual machines network interface with the corresponding application security group. The myVMWeb virtual machine interface will be associated to the myAsgWebServers ASG. The myVMMgmt virtual machine interface will be associated to the myAsgMgmtServers ASG. 

1. In the Azure portal, navigate back to the **Virtual machines** blade and verify that both virtual machines are listed with the **Running** status.

1. In the list of virtual machines, click the **myVMWeb** entry.

1. On the **myVMWeb** blade, in the **Settings** section, click **Networking** and then, on the **myVMWeb \| Networking** blade, click the **Application security groups** tab.

1. Click **Configure the application security groups**, in the **Application security group** drop-down list, select **myAsgWebServers**, and then click **Save**.

1. Navigate back to the **Virtual machines** blade and in the list of virtual machines, click the **myVMMgmt** entry.

1. On the **myVMMgmt** blade, in the **Settings** section, click **Networking** and then, on the **myVMMgmt \| Networking** blade, click the **Application security groups** tab.

1. Click **Configure the application security groups**, in the **Application security group** drop-down list, select **myAsgMgmtServers**, and then click **Save**.