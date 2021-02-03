---
title: "8.1 Role that does not require approval"
date: 2021-02-03T11:05:48+03:00
weight: 10
---


#### Task 1: Activate a role that does not require approval.

In this task, you will activate a role that does not require approval.

1. Open an InPrivate browser window.

1. In the InPrivate browser window, navigate to the Azure portal and sign in using the **aaduser2** user account.

    >**Note**: To sign in you will need to provide a fully qualified name of the **aaduser2** user account, including the Azure AD tenant DNS domain name, which you recorded earlier in this lab. This user name is in the format aaduser2@`<your_tenant_name>`.onmicrosoft.com, where `<your_tenant_name>` is the placeholder representing your unique Azure AD tenant name. 

1. In the Azure portal, in the **Search resources, services, and docs** text box at the top of the Azure portal page, type **Azure AD Privileged Identity Management** and press the **Enter** key.

1. On the **Azure AD Privileged Identity Management** blade, in the **Tasks** section, click **My roles**.

1. You should see three **Eligible roles** for **aaduser2**: **Global Reader**, **Security Administrator**, and **Billing Administrator**. 

1. In the row displaying the **Billing Administrator** role entry, click **Activate**.

1. If needed, click the warning **Additional verification required. Click to continue** and follow the instructions to verify your identity.

1. On the **Activate - Billing Administrator** blade, in the **Reason** text box, type a text providing justification for the activation, and then click **Activate**.

    >**Note**: When you activate a role in PIM, it can take up to 10 minutes for the activation to take effect. 
	
    >**Note**: This role does not require approval, so you will be able to sign out and log back in to begin using the activated role. 

1. Sign out and sign back into the Azure portal by using the **aaduser2** user account.

1. Navigate back to the **Azure AD Privileged Identity Management** blade and, in the **Tasks** section, click **My roles**.

1. On the **My roles \| Azure AD roles** blade, switch to the **Active assignments** tab. Notice the **Billing Administrator** role is **Activated**.

    >**Note**: Once a role has been activated, it automatically deactivates when its time limit under **End time**(eligible duration) is reached.

    >**Note**: If you complete your administrator tasks early, you can deactivate a role manually.

1.  In the list of **Active Assignments**, in the row representing the Billing Administrator role, click the **Deactivate** link.

1.  On the **Deactivate - Billing Administrator** blade, click **Deactivate** again to confirm the your intent.
