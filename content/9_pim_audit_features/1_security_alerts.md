---
title: "9.1 Security alerts for Azure AD"
date: 2021-02-03T11:08:35+03:00
weight: 10
---


#### Task 1: Configure security alerts for Azure AD directory roles in PIM

In this task, you will reduce the risk associated with "stale" role assignments. You will do this by creating a PIM access review to ensure that assigned roles are still valid. Specifically, you will review the Global Reader role. 

1. Sign-in to the Azure portal **`https://portal.azure.com/`** using your account.

    >**Note**: Ensure that you are signed-in to the **AdatumLab500-04** Azure AD tenant. You can use the **Directory + subscription** filter to switch between Azure AD tenants. Ensure you are signed in as a user with the Global Administrator role.

1. In the Azure portal, in the **Search resources, services, and docs** text box at the top of the Azure portal page, type **Azure AD Privileged Identity Management** and press the **Enter** key.

1. Navigate to the **Azure AD Privileged Identity Management** blade. 

1. On the **Privileged Identity Management \| Quick start** blade, in the **Manage** section, click **Azure AD Roles**.

1. On the **AdatumLab500-04 \| Quick start** blade, in the **Manage** section, click **Access reviews**.

1. On the **AdatumLab500-04 \| Access reviews** blade, click **New**:

1. On the **Create an access review** blade, specify the following settings (leave others with their default values): 

   |Setting|Value|
   |---|---|
   |Review name|**Global Reader Review**|
   |Start Date|today's date| 
   |Frequency|**One time**|
   |End Date|end of the current month|
   |Review role membership|**Global Reader**|
   |Reviewers|**Selected users**|
   |Select reviewers|your account|

1. On the **Create an access review** blade, click **Start**:
 
    >**Note**: It will take about a minute for the review to deploy and appear on the **AdatumLab500-04 \| Access reviews** blade. You might have to refresh the web page. The review status will be **Active**. 

1. On the **AdatumLab500-04 \| Access reviews** blade, under the **Global Admin Review** header, click the **Global Reader** entry. 

1. On the **Global Reader Review** blade, examine the **Overview** page and note that the **Progress** charts shows a single users in the **Not reviewed** category. 

1. On the **Global Reader Review** blade, in the **Manage** section, click **Results**. Note that aaduser2 is listed as having access to this role.

1. Click **aaduser2** to view a detailed audit log with entries representing PIM activities that involve that user.

1. Navigate back to the **AdatumLab500-04 \| Access reviews** blade.

1. On the the **AdatumLab500-04 \| Access reviews** blade, in the **Tasks** section, click **Review access** and then, click the **Global Reader Review** entry. 

1. On the **Global Reader Review** blade, click the **aaduser2** entry. 

1. In the **Reason** text box, type a rationale for approval and then click either **Approve** to maintain the current role membership or **Deny** to revoke it. 

1. Navigate back to the **Azure AD Privileged Identity Management** blade and, in the **Manage** section, click **Azure AD roles**.

1. On the **AdatumLab500-04 \| Quick start** blade, in the **Manage** section, click **Access reviews**.

1. Select the entry representing the **Global Reader** review. Note that the **Progress** chart has been updated to show your review. 