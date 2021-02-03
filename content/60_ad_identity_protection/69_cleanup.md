---
title: "Cleanup"
date: 2021-02-03T10:59:24+03:00
---


**Clean up resources**

> We need to remove identity protection resources that you no longer use. 

Use the following steps to disable the identity protection policies in the **AdatumLab500-04** Azure AD tenant.

1. In the Azure portal, navigate back to the **AdatumLab500-04** Azure Active Directory tenant blade.

1. On the **AdatumLab500-04** blade, in the **Manage** section, click **Security**.

1. On the **Security \| Getting started** blade, in the **Protect** section, click **Identity Protection**.

1. On the **Identity Protection \| Overview** blade, click **User risk policy**.

1. On the **Identity Protection \| User risk policy** blade, set **Enforce policy** to **Off** and then click **Save**.

1. On the **Identity Protection \| User risk policy** blade, click **Sign-in risk policy**

1. On the **Identity Protection \| Sign-in risk policy** blade, set **Enforce policy** to **Off** and then click **Save**.

Use the following steps to stop the Azure VM you provisioned earlier in the lab.

1. In the Azure portal, set the **Directory + subscription** filter to the the Azure AD tenant associated with the Azure subscription into which you deployed the **az500-04-vm1** Azure VM.

1. In the Azure portal, in the **Search resources, services, and docs** text box at the top of the Azure portal page, type **Virtual machines** and press the **Enter** key.

1. On the **Virtual machines** blade, click the **az500-04-vm1** entry. 
 
1. On the **az500-04-vm1** blade, click **Stop** and, when prompted to confirm, click **OK** 

>  Do not remove any resources provisioned in this lab, since the PIM lab has a dependency on them.