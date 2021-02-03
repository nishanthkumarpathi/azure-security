---
title: "4.3 Create Azure AD users and groups."
date: 2021-01-30T13:58:35+03:00
weight: 3
---

#### Task 3: Create Azure AD users and groups.

In this task, you will create three users: aaduser1 (Global Admin), aaduser2 (user), and aaduser3 (user). You will need each user's principal name and password for later tasks. 

1. Navigate back to the **AdatumLab500-04** Azure Active Directory blade and, in the **Manage** section, click **Users**.

1. On the **Users \| All users** blade, click **+ New User**. 

1. On the **New user** blade, ensure that the **Create user** option is selected, and specify the following settings (leave all others with their default values) and click **Create**:

   |Setting|Value|
   |---|---|
   |User name|**aaduser1**|
   |Name|**aaduser1**|
   |Password|ensure that the option **Auto-generate password** is selected and click **Show Password**|
   |Groups|**0 groups selected**|
   |Roles|click **User**, then click **Global administrator**, and click **Select**|
   |Usage Location|**United States**|  

    >**Note**: Record the full user name. You can copy its value by clicking the **Copy to clipboard** button on the right hand side of the drop-down list displaying the domain name. 

    >**Note**: Record the user's password. You will need this later in this lab. 

1. Back on the **Users \| All users** blade, click **+ New User**. 

1. On the **New user** blade, ensure that the **Create user** option is selected, and specify the following settings (leave all others with their default values):

   |Setting|Value|
   |---|---|
   |User name|**aaduser2**|
   |Name|**aaduser2**|
   |Password|ensure that the option **Auto-generate password** is selected and click **Show Password**|
   |Groups|**0 groups selected**|
   |Roles|**User**|
   |Usage Location|**United States**|  

    >**Note**: Record the full user name and the password.

1. Back on the **Users \| All users** blade, click **+ New User**. 

1. Click **New User**,complete the new user configuration settings, and then click **Create**.

   |Setting|Value|
   |---|---|
   |User name|**aaduser3**|
   |Name|**aaduser3**|
   |Password|ensure that the option **Auto-generate password** is selected and click **Show Password**|
   |Groups|**0 groups selected**|
   |Roles|**User**|
   |Usage Location|**United States**|  

    >**Note**: Record the full user name and the password.

1. On the **New user** blade, click **Create**.

    >**Note**: At this point, you should have three new users listed on the **Users** page. 