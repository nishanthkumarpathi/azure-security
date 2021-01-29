---
title: "Group Creation"
date: 2021-01-29T13:37:07+03:00
draft: false
weight: 20
---

#### Task 2: Use Azure CLI to create the Service Desk group and add the user account of Dylan to the group. 


In this task, you will create the Service Desk group and assign Dylan to the group. 

1. In the same Bash session within the Cloud Shell pane, run the following to create a new security group named Service Desk.

    ```bash
    az ad group create --display-name "Service Desk" --mail-nickname "ServiceDesk"
    ```
 
1. In the Bash session within the Cloud Shell pane, run the following to list the Azure AD groups (the list should include Service Desk, Senior Admins, and Junior Admins groups):

    ```bash
    az ad group list -o table
    ```

1. In the Bash session within the Cloud Shell pane, run the following to obtain a reference to the user account of Dylan Williams: 

    ```bash
    USER=$(az ad user list --filter "displayname eq 'Dylan Williams'")
    ```

1. In the Bash session within the Cloud Shell pane, run the following to obtain the objectId property of the user account of Dylan Williams: 

    ```bash
    OBJECTID=$(echo $USER | jq '.[].objectId' | tr -d '"')
    ```

1. In the Bash session within the Cloud Shell pane, run the following to add the user account of Dylan to the Service Desk group: 

    ```bash
    az ad group member add --group "Service Desk" --member-id $OBJECTID
    ```

1. In the Bash session within the Cloud Shell pane, run the following to list members of the Service Desk group and verify that it includes the user account of Dylan:

    ```bash
    az ad group member list --group "Service Desk"
    ```

1. Close the Cloud Shell pane.

> Result: Using Azure CLI you created a user and a group accounts, and added the user account to the group. 
