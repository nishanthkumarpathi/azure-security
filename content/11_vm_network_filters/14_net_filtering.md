---
title: "11.4 Testing"
date: 2021-02-03T11:19:38+03:00
weight: 40
---



#### Task 4: Test the network traffic filtering

In this task, you will test the network traffic filters. You should be able to RDP into the myVMMgmnt virtual machine. You should be able to connect from the internet to the myVMWeb virtual machine and view the default IIS web page.  

1. Navigate back to the **myVMMgmt** virtual machine blade.

1. On the **myVMMgmt** blade, click **Connect** and, in the drop down menu, click **RDP**. 

1. Click **Download RDP File** and use it to connect to the **myVMMgmt** Azure VM via Remote Desktop. When prompted to authenticate, provide the following credntials:

   |Setting|Value|
   |---|---|
   |User name|**Student**|
   |Password|**Pa55w.rd1234**|

    >**Note**: Verify that the Remote Desktop connection was successful. At this point you have confirmed you can connect via Remote Desktop to myVMMgmt.

1. In the Azure portal, navigate to the **myVMWeb** virtual machine blade.

1. On the **myVMWeb** blade, in the **Operations** section, click **Run command** and then click **RunPowerShellScript**.

1. On the **Run Command Script** pane, run the following to install the Web server role on **myVmWeb**:

    ```powershell
    Install-WindowsFeature -name Web-Server -IncludeManagementTools
    ```

    >**Note**: Wait for the installation to complete. This might take a couple of minutes. At that point, you can verify that myVMWeb can be accessed via HTTP/HTTPS.

1. In the Azure portal, navigate back to the **myVMWeb** blade.

1. On the **myVMWeb** blade, identify the **Public IP address** of the myVmWeb Azure VM.

1. Open another browser tab and navigate to IP address you identified in the previous step.

    >**Note**: The browser page should display the default IIS welcome page because port 80 is allowed inbound from the internet based on the setting of the **myAsgWebServers** application security group. The network interface of the myVMWeb Azure VM is associated with that application security group. 

> Result: You have validated that the NSG and ASG configuration is working and traffic is being correctly managed. 