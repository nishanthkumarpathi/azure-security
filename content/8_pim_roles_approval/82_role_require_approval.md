---
title: "8.2 Role that requires approval"
date: 2021-02-03T11:06:00+03:00
weight: 20
---



#### Task 2: Activate a role that requires approval. 

In this task, you will activate a role that requires approval.

1. In the InPrivate browser window, in the Azure portal, while signed in as the **aaduser2** user, navigate back to the **Privileged Identity Management \| Quick start** blade. 

1. On the **Privileged Identity Management \| Quick start** blade, in the **Tasks** section, click **My roles**.

1. On the **My roles \| Azure AD roles** blade, in the list of **Eligible assignments**, in the row displaying the **Global Reader** role, click **Activate**. 

1. On the **Activate - Global Reader** blade, in the **Reason** text box, type a text providing justification for the activation, and then click **Activate**.

1. Click the **Notifications** icon in the toolbar of the Azure portal and view the notification informing that your request is pending approval.

    >**Note**: As the Privileged role administrator you can review and cancel requests at any time. 

1. On the **My roles \| Azure AD roles** blade, locate the **Security Administrator** role, and click **Activate**. 

1. Click the warning **Additional verification required. Click to continue**. 

1. Follow the instructions to verify your identity.

    >**Note**: You only have to authenticate once per session. 

1. Once you are back in the Azure Portal interface, on the **Activate - Security Administrator** blade, in the **Reason** text box, type a text providing justification for the activation, and then click **Activate**.

    >**Note**: The auto approval process should complete.

1. Back on the **My roles \| Azure AD roles** blade, click the **Active assignments** tab and notice that the listing of **active assignments** includes **Security Administrator** but not the **Global Reader** role.

    >**Note**: You will now approve the Global Reader role.

1. Sign out of the Azure portal as **aaduser2**.

1. Sign into the Azure portal as **aaduser3**.

    >**Note**: If you run into problems with authenticating by using any of the user accounts, you can sign in to the Azure AD tenant by using your user account to reset their passwords or reconfigure their sign-in options.

1. In the Azure portal, navigate to **Azure AD Privileged Identity Management**.

1. On the **Privileged Identity Management \| Quick start** blade, in the **Tasks** section, click **Approve requests**.

1. On the **Approve requests \| Azure AD roles** blade, in the **Requests for role activations** section, select the checkbox for the entry representing the role activation request to the **Global Reader** role by **aaduser2**.

1. Click **Approve**. On the **Approve Request** blade, in the **Justification** text box, type a reason for activation, note the start and end times, and then click **Confirm**. 

    >**Note**: You also have the option of denying requests.

1. Sign out of the Azure portal as **aaduser3**.

1. Sign into the Azure portal as **aaduser2**

1. In the Azure portal, navigate to **Azure AD Privileged Identity Management**.

1. On the **Privileged Identity Management \| Quick start** blade, in the **Tasks** section, click **My roles**.

1. On the **My roles \| Azure AD roles** blade, click the **Active Assignments** tab and verify that the Global Reader role is now active.

    >**Note**: You might have to refresh the page to view the updated list of active assignments.

1. Sign out and close the InPrivate browser window.

> Result: You have practiced activating PIM roles with and without approval. 