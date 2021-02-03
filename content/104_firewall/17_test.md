---
title: "104.7 Test the Firewall"
date: 2021-02-03T11:23:07+03:00
---

#### Task 7: Test the firewall

In this task, you will test the firewall to confirm that it works as expected.

1. In the Azure portal, navigate back to the **AZ500LAB08** resource group.

1. On the **AZ500LAB08** blade, in the list of resources, click the **Srv-Jump** virtual machine.

1. On the **Srv-Jump** blade, click **Connect** and, in the drop down menu, click **RDP**. 

1. Click **Download RDP File** and use it to connect to the **Srv-Jump** Azure VM via Remote Desktop. When prompted to authenticate, provide the following credntials:

   |Setting|Value|
   |---|---|
   |User name|**localadmin**|
   |Password|**Pa55w.rd1234**|

    >**Note**: The following steps are performed in the Remote Desktop session to the **Srv-Jump** Azure VM. 

    >**Note**: You will connect to the **Srv-Work** virtual machine. This is being done so we can test the ability to access the bing.com website.  

1. Within the Remote Desktop session to **Srv-Jump**, right-click **Start**, in the right-click menu, click **Run**, and, from the **Run** dialog box, run the following to connect to **Srv-Work**. 

    ```
    mstsc /v:Srv-Work
    ```

1. When prompted to authenticate, provide the following credentials:

   |Setting|Value|
   |---|---|
   |User name|**localadmin**|
   |Password|**Pa55w.rd1234**|

    >**Note**: Wait for the Remote Desktop session to be established and the Server Manager interface to load.

1. Within the Remote Desktop session to **Srv-Work**, in **Server Manager**, click **Local Server** and then click **IE Enhanced Security Configuration**.

1. In the **Internet Explorer Enhanced Security Configuration** dialog box, set both options to **Off** and click **OK**.

1. Within the Remote Desktop session to **Srv-Work**, start Internet Explorer and browse to **`https://www.bing.com`**. 

    >**Note**: The website should successfully display. The firewall allows you access.

1. Browse to **`http://www.microsoft.com/`**

    >**Note**: Within the browser page, you should receive a message with text resembling the following: `HTTP request from 10.0.2.4:xxxxx to microsoft.com:80. Action: Deny. No rule matched. Proceeding with default action.` This is expected, since the firewall blocks access to this website. 

1. Terminate both Remote Desktop sessions.

> Result: You have successfully configured and tested the Azure Firewall.
