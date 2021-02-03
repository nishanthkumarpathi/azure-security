---
title: "5.1 Configure a conditional access policy"
date: 2021-02-03T10:36:11+03:00
weight: 1
---

#### Task 1 - Configure a conditional access policy. 

In this task, you will review conditional access policy settings and create a policy that requires MFA when signing in to the Azure portal. 

1. In the Azure portal, navigate back to the **AdatumLab500-04** Azure Active Directory tenant blade.

1. On the **AdatumLab500-04** blade, in the **Manage** section, click **Security**.

1. On the **Security \| Getting started** blade, in the **Protect** section, click **Conditional Access**.

1. On the **Conditional Access \| Policies** blade, click **+ New policy**. 

1. On the **New** blade, configure the following settings:

   - In the **Name** text box, type **AZ500Policy1**
	
   - Click **Users and groups**, select the **Users and Groups** checkbox, on the **Select** blade, click **aaduser2**, and click **Select**.
	
   - Click **Cloud apps or actions**, click **Select apps**, on the **Select** blade, click **Microsoft Azure Management**, and click **Select**. 

    >**Note**: Review the warning that this policy impacts access to the Azure Portal.
	
   - Click **Conditions**, click **Sign-in risk**, on the **Sign-in risk** blade, review the risk levels but do not make any changes and close the **Sign-in risk** blade.
	
   - Click **Device platforms**, review the device platforms that can included and click **Done**.
	
   - Click **Locations** and review the location options without making any changes.
	
   - Click **Grant** in the **Access controls** section, on the **Grant** blade, select the **Require multi-factor authentication** checkbox and click **Select**
	
   - Set the **Enable policy** to **On**.


1. On the **New** blade, click **Create**. 

    >**Note**: At this point, you have a conditional access policy that requires MFA to sign in to the Azure portal. 