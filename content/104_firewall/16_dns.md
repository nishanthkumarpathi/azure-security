---
title: "104.6 DNS Server"
date: 2021-02-03T11:23:01+03:00
---



#### Task 6: Configure the virtual machine DNS servers

In this task, you will configure the primary and secondary DNS addresses for the virtual machine. This is not a firewall requirement. 

1. In the Azure portal, navigate back to the **AZ500LAB08** resource group.

1. On the **AZ500LAB08** blade, in the list of resources, click the **Srv-Work** virtual machine.

1. On the **Srv-Work** blade, in the **Settings** section, click **Networking**.

1. On the **Srv-Work \| Networking** blade, click the link next to the **Network interface** entry.

1. On the network interface blade, in the **Settings** section, click **DNS servers**, select the **Custom** option, add the two DNS servers referenced in the network rule: **209.244.0.3** and **209.244.0.4**, and click **Save** to save the change.

1. Return to the **Srv-Work** virtual machine page.

    >**Note**: Wait for the update to complete.

    >**Note**: Updating the DNS servers for a network interface will automatically restart the virtual machine to which that interface is attached, and if applicable, any other virtual machines in the same availability set.