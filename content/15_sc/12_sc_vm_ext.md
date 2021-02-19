---
title: "15.2 Install Guest Config Extension"
weight: 12
---

#### Task 2: Implement a Security Center recommendation

In this task, you will implement the Security Center recommendation to install endpoint protection on the virtual machine. 

1. In the Azure portal, navigate back to the **Security Center \| Overview** blade. 

1. On the **Security Center \| Overview** blade, review the **Secure Score** tile.

    >**Note**: Record the current score if it is available.

1. On the **Security Center \| Overview** blade, review the **Insights** tile.

1. On the **Insights** tile, click the **Install endpoint protection solution on virtual machines** entry.

1. Select the **myVM** entry.

    >**Note**: You might have to wait a few minutes and refresh the browser page for the entry to appear.
    
1. Click **Install on 1 VM**. Select **Microsoft Antimalware** then **Create** > **OK**

    >**Note**: Monitor the progress of installation by clicking on the **Notifications** icon in the toolbar and viewing the **Notifications** blade. 

    >**Note**: Security Center will automatically rescan the virtual machine. That will be reflected by an increase in the secure score.

    >**Note**: Do not wait for the intallation to complete but instead continue to the next task. 
