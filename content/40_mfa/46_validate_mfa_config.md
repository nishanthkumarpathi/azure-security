---
title: "4.6 Validate MFA configuration"
date: 2021-01-30T13:59:32+03:00
---

#### Task 6: Validate MFA configuration

In this task, you will validate the MFA configuration by testing sign in of the aaduser1 user account. 

1. Open an InPrivate browser window.

1. Navigate to the Azure portal and sign in using the **aaduser1** user account. 

    >**Note**: To sign in you will need to provide a fully qualified name of the **aaduser1** user account, including the Azure AD tenant DNS domain name, which you recorded earlier in this lab. This user name is in the format aaduser1@`<your_tenant_name>`.onmicrosoft.com, where `<your_tenant_name>` is the placeholder representing your unique Azure AD tenant name. 

1. When prompted, in the **More information required** dialog box, click **Next**.

    >**Note**: The browser session will be redirected to the **Additional security verification** page.

1. In the **Step 1: How should we contact you?** section, note that you need to set up one of the following options:

   - **Authentication phone**

   - **Mobile app**

1. Ensure that the **Authentication phone** entry appears in the drop-down list and the **Send me a code by text message** option is selected. 

1. In the **Step 1: How should we contact you?** section, in the drop-down list, select your country or region, provide your mobile phone number in the empty text box, and click **Next**.

1. Provide your phone number, click **Next**, in the text box, type the code you received in the text message on your mobile phone, and click **Verify**.

1. On the **Additional security verification** page, review instructions provided in **Step 3: Keep using your existing applications**, and then click **Done**.

1. When prompted, change your password. Make sure to record the new password.

1. Verify that you successfully signed in to the Azure portal.

1. Sign out as **aaduser1** and close the InPrivate browser window.

> Result: You have created a new AD tenant, configured AD users, configured MFA, and tested the MFA experience for a user. 

