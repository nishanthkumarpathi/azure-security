---
title: "14.5 View and Query Data"
weight: 15
---

#### Task 5: View and query collected data

In this task, you will run a log search on your data collection. 

1. In the Azure portal, navigate back to the Log Analytics workspace you created earlier in this exercise.

1. On the Log Analytics workspace blade, in the **General** section, click **Logs**.

1. On the Logs blade, click **Get started**.  

1. On the **Example queries** pane, clear the **Log Analytics** filter, scroll down to the bottom of the list of resource types, and click **Virtual machine**
    
    >**Note**: If you dont see **Virtual machine**, click Resource Type filter and select **Virtual machines**

1. Review the list of predefined queries, identify the one you want to test, and click the corresponding **Run** button.

    >**Note**: You can start with the query **Virtual machine available memory**. If you don't get any results check the scope is set to virtual machine

1. The query will automatically open in a new query tab. 

    >**Note**: Log Analytics uses the Kusto query language. You can customize the existing queries or create your own. 

    >**Note**: The results of the query you selected are automatically displayed below the query pane. To re-run the query, click **Run**.

    >**Note**: Since this virtual machine was just created, there may not be any data yet. 

    >**Note**: You have the option of displaying data in different formats. You also have the option of creating an alert rule based on the results of the query.

> Results: You used a Log Analytics workspace to configure data sources and query logs. 