---
title: "7.2 Role to Require Approval"
date: 2021-02-03T11:01:55+03:00
---


#### Task 2: Configure a role to require approval to activate and add an eligible member

1. In the Azure Portal, navigate back to the **Azure AD Privileged Identity Management** blade and click **Azure AD roles**.

1. On the **AdatumLab500-04 \| Quick start** blade, in the **Manage** section, click **Roles**.

1. On the **AdatumLab500-04 \| Roles** blade, click the **Global reader** role entry. 

1. On the **Global Reader \| Assignments** blade, click **Settings** icon in the toolbar of the blade and review configuration settings for the role, including Azure Multi-Factor Authentication requirements.

1. Click **Edit**.

1. On the **Activation** tab, enable the **Require approval to activate** check box.

1. Click **Select approvers(s)**, on the **Select a member** blade, click **aaduser3**, and then click **Select**.

1. Click **Next:Assignment**.

1. Clear the **Allow permanent eligible assignment** check box, leaving all other settings with their default values.

1. Click **Next:Notification**.

1. On the **Edit role setting - Global Reader** blade, review the settings and click **Update**.

    >**Note**: Anyone trying to use the Global Reader role will now need approval from aaduser3. 

1. On the **Global Reader \| Assignments** blade, click **+ Add assignments**.

1. On the **Add assignments** blade, click **No member selected**, on the **Select a member** blade, click **aaduser2**, and then click **Select**.

1. Click **Next**. 

1. Ensure the **Assignment type** is **Eligible** and review the eligible duration settings.

1. Click **Assign**.

    >**Note**: User aaduser2 is eligible for the Global Reader role. 