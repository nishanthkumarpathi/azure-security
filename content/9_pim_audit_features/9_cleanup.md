---
title: "Cleanup"
date: 2021-02-03T11:09:31+03:00
weight: 90
---



**Clean up resources**

> Remember to remove any newly created Azure resources that you no longer use. Removing unused resources ensures you will not incur unexpected costs. 

1. In the Azure portal, set the **Directory + subscription** filter to the the Azure AD tenant associated with the Azure subscription into which you deployed the **az500-04-vm1** Azure VM.

1. In the Azure portal, open the Cloud Shell by clicking the first icon in the top right of the Azure Portal. If prompted, click **PowerShell** and **Create storage**.

1. Ensure **PowerShell** is selected in the drop-down menu in the upper-left corner of the Cloud Shell pane.

1. In the PowerShell session within the Cloud Shell pane, run the following to remove the resource group you created in this lab:
  
    ```powershell
    Remove-AzResourceGroup -Name "AZ500LAB04" -Force -AsJob
    ```

1.  Close the **Cloud Shell** pane. 

1. Back in the Azure portal, use the **Directory + subscription** filter to switch to the **AdatumLab500-04** Azure Active Directory tenant.

1. Navigate to the **Azure Active Directory Premium P2 - Licensed users** blade, select the user accounts to which you assigned licenses, click **Remove license**, and, when prompted to confirm, click **OK**.

1. In the Azure portal, navigate to the **Users - All users** blade, click the entry representing the **aaduser1** user account, on the **aaduser1 - Profile** blade click **Delete**, and, when prompted to confirm, select **Yes**.

1. Repeat the same sequence of steps to delete the remaining user accounts you created.

1. Navigate to the **AdatumLab500-04 - Overview** blade of the Azure AD tenant, click **Delete tenant**, on the **Delete directory 'AdatumLab500-04'** blade, click the **Get permission to delete Azure resources** link, on the **Properties** blade of Azure Active Directory, set **Access management for Azure resources** to **Yes** and click **Save**.

1. Sign out from the Azure portal and sign in back. 

1. Navigate back to the **Delete directory 'AdatumLab500-04'** blade and click **Delete**.

> For any additional  information regarding this task, refer to [https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/directory-delete-howto](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/directory-delete-howto)
