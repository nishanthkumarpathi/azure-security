---
title: "6.5 Simulate risk events"
date: 2021-02-03T10:51:38+03:00
weight: 5
---


#### Task 5: Simulate risk events against the Azure AD Identity Protection policies 

> Before you start this task, ensure that the template deployment you started in Exercise 1 has completed. The deployment includes an Azure VM named **az500-04-vm1**. 

1. In the Azure portal, set the **Directory + subscription** filter to the the Azure AD tenant associated with the Azure subscription into which you deployed the **az500-04-vm1** Azure VM.

1. In the Azure portal, in the **Search resources, services, and docs** text box at the top of the Azure portal page, type **Virtual machines** and press the **Enter** key.

1. On the **Virtual machines** blade, click the **az500-04-vm1** entry. 

1. On the **az500-04-vm1** blade, click **Connect** and, in the drop down menu, click **RDP**. 

1. Click **Download RDP File** and use it to connect to the **az500-04-vm1** Azure VM via Remote Desktop. When prompted to authenticate, provide the following credntials:

   |Setting|Value|
   |---|---|
   |User name|**Student**|
   |Password|**Pa55w.rd1234**|

    >**Note**: Wait for the Remote Desktop session and **Server Manager** to load.  

    >**Note**: The following steps are performed in the Remote Desktop session to the **az500-04-vm1** Azure VM. 

1. In **Server Manager**, click **Local Server** and then click **IE Enhanced Security Configuration**.

1. In the **Internet Explorer Enhanced Security Configuration** dialog box, set both options to **Off** and click **OK**.

1. Start **Internet Explorer**, click the cog wheel icon in the toolbar, in the drop-down menu, click **Safety** and then click **InPrivate Browsing**.

1. In the InPrivate Internet Explorer window, navigate to the ToR Browser Project at [**https://www.torproject.org/projects/torbrowser.html.en**](https://www.torproject.org/projects/torbrowser.html.en).

1. Download and install the Windows version of the ToR Browser with the default settings. 

1. Once the installation completes, start the ToR Browser, use the **Connect** option on the initial page, and browse to the Application Access Panel at [**https://myapps.microsoft.com**](https://myapps.microsoft.com).

1. When prompted, attempt to sign in with the **aaduser3** account. 

    >**Note**: You will be presented with the message **Your sign-in was blocked**. This is expected, since this account is not configured with multi-factor authentication, which is required due to increased sign-in risk associated with the use of ToR Browser.

1. Use the **Sign out and sign in with a different account option** to sign in as **aaduser1** account you created and configured for multi-factor authentication earlier in this lab.

    >**Note**: This time, you will be presented with the **Suspicious activity detected** message. Again, this is expected, since this account is configured with multi-factor authentiation. Considering the increased sign-in risk associated with the use of ToR Browser, you will have to use multi-factor authentication.

1. Use the **Verify** option and specify whether you want to verify your identity via text or a call.

1. Complete the verification and ensure that you successfully signed in to the Application Access Panel.

1. Close your RDP session. 

    >**Note**: At this point, you attempted two different sign ins. Next, you will review the Azure Identity Protection reports.