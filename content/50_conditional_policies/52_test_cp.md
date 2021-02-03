---
title: "5.2 Test the conditional access policy"
date: 2021-02-03T10:36:18+03:00
---



#### Task 2 - Test the conditional access policy.

In this task, you will sign in to the Azure portal as **aaduser2** and verify MFA is required. You will also delete the policy before continuing on to the next exercise. 

1. Open an InPrivate Microsoft Edge window.

1. In the new browser window, navigate to the Azure portal and sign in with the **aaduser2** user account.

1. When prompted, in the **More information required** dialog box, click **Next**.

    >**Note**: The browser seesion will be redirected to the **Keep your account secure** page.
    
1. On the **Keep your account secure** page, select the **I want to set up a different method** link, in the **Which method would you like to use?** drop-down list, select **Phone**, and select **Confirm**.

1. On the **Keep your account secure** page, select your country or region, type your mobile phone number in the **Enter phone number** area, ensure that the **Text me a code** option is selected, and click **Next**.

1. On the **Keep your account secure** page, type the code you received in the text message on your mobile phone, and click **Next**.

1. On the **Keep your account secure** page, ensure that the verification was successful and click **Next**.

1. On the **Keep your account secure** page, click **Done**.

1. When prompted, change your password. Make sure to record the new password.

1. Verify that you successfully signed in to the Azure portal.

1. Sign out as **aaduser2** and close the InPrivate browser window.

    >**Note**: You have now verified that the newly created conditional access policy enforces MFA when aaduser2 signs into the Azure portal.

1. Back in the browser window displaying the Azure portal, navigate back to the **AdatumLab500-04** Azure Active Directory tenant blade.

1. On the **AdatumLab500-04** blade, in the **Manage** section, click **Security**.

1. On the **Security \| Getting started** blade, in the **Protect** section, click **Conditional Access**.

1. On the **Conditional Access \| Policies** blade, click the ellipsis next to **AZ500Policy1**, click **Delete**, and, when prompted to confirm, click **Yes**.

    >**Note**: Result: In this exercise you implement a conditional access policy to require MFA when a user signs into the Azure portal. 

>Result: You have configured and tested Azure AD conditional access.

