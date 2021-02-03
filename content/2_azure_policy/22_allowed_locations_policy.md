---
title: "2.2 Allowed Locations Policy"
date: 2021-01-29T15:18:22+03:00
draft: false
weight: 20
tags: ["Azure Policy","Resource Group","Policy Assignments","Allowed Locations"]
---

#### Task 2: Create an Allowed Locations policy assignment.

In this task, you will create an Allowed Locations policy assignment and specify which Azure regions the policy can use. 

1. In the Azure portal, in the **Search resources, services, and docs** text box at the top of the Azure portal page, type **Policy** and press the **Enter** key.

1. On the **Policy** blade, in the **Authoring** section, select **Definitions**.

1. Take a minute to browse the built-in definitions. Use the **Category** drop-down to filter the list of policies.

1. In the **Search** text box, type **Allowed locations**. 

   >**Note**: The **Allowed locations** policy allows you to restrict location of resources, not resource groups. To restrict locations of resource groups, you can use the **Allowed locations for resource groups** policy.

1. Click the **Allowed locations** policy definition to display its details.. 

   >**Note**: This policy definition takes an array of locations as parameters. A policy rule is an ‘if-then’ statement. The ‘if’ clause checks if the resource location is included in the parameter list, and if not, the ‘then’ clause denies the resource creation or, for existing resources, marks them as non-compliant.

1. On the **Allowed locations** blade, click **Assign**.

1. On the **Basics** tab of the **Allowed locations** blade, click the Ellipsis (...) button next to the **Scope** text box and, on the **Scope** blade, specify the following settings:

   |Setting|Value|
   |---|---|
   |Subscription|the name of you Azure subscription|
   |Resource group|**AZ500LAB02**|

1. Click **Select**.

1. On the **Allowed locations** blade, on the **Basics** tab, specify the following settings (leave others with their defualt values):

   |Setting|Value|
   |---|---|
   |Assignment name|**Allow UK South for AZ500LAB02**|
   |Description|**Allow resources to be created in UK South Only for AZ500LAB02**|
   |Policy enforcement|**Enabled**|

1. Click **Next**.

1. On the **Parameters** tab of the **Allowed locations** blade, in the **Allowed locations** drop-down list, select **UK South** as the only allowed location. 

   >**Note**: You can select more than one location. If the policy required a different set of parameters, this tab would provide those selections. 

1. Click **Review + create**, followed by **Create** to create the policy assignment. 

   >**Note**: You will see a notification that the assignment was successful, and that the assignment might take around 30 minutes to complete.

   >**Note**: The reason the Azure policy assignment might take up to 30 minutes to take effect is that is has to replicate globally. Typically this takes only a few minutes.  If the next task fails, simply wait a few minutes and attempt its steps again.


