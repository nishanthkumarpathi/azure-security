---
title: "7.1 Make a user eligible for a role"
date: 2021-02-03T11:01:41+03:00
draft: true
---

#### Task 1: Make a user eligible for a role

In this task, you will make a user eligible for an Azure AD directory role.

1. Sign-in to the Azure portal **`https://portal.azure.com/`**.

    >**Note**: Ensure that you are signed-in to the **AdatumLab500-04** Azure AD tenant. You can use the **Directory + subscription** filter to switch between Azure AD tenants. Ensure you are signed in as a user with the Global Administrator role.

1. In the Azure portal, in the **Search resources, services, and docs** text box at the top of the Azure portal page, type **Azure AD Privileged Identity Management** and press the **Enter** key.

1. On the **Azure AD Privileged Identity Management** blade, in the **Manage** section, click **Azure AD roles**.

1. On the **AdatumLab500-04 \| Quick start** blade, in the **Manage** section, click **Roles**.

1. On the **AdatumLab500-04 \| Roles** blade, click **+ Add assignments**.

1. On the **Add assignments** blade, in the **Select a role** drop-down, select **Billing Administrator**.

1. Click the **No member selected** link, on the **Select a member** blade, click **aaduser2**, and then click **Select**.

1. Back on the **Add assignments** blade, click **Next**. 

1. Ensure the **Assignment type** is set to **Eligible** and click **Assign**.
 
1. Back on the **AdatumLab500-04 \| Roles** blade, in the **Manage** section, click **Assignments**.

1. Back on the **AdatumLab500-04 \| Assignments** blade, note the tabs for **Eligible assignments**, **Active assignments**, and **Expired assignments**.

1. Verify on the **Eligible assignments** tab that **aaduser2** is shown as a **Billing administrator**. 

    >**Note**: During sign-in, aaduser2 will be eligible to use the Billing administrator role. 
