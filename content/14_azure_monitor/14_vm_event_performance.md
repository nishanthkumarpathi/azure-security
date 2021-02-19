---
title: "14.4 Collect Data"
weight: 14
---


#### Task 4: Collect virtual machine event and performance data

In this task, you will configure collection of the Windows System log and several common performance counters. You will also review other sources that are available.

1. In the Azure portal, navigate back to the Log Analytics workspace you created earlier in this exercise.

1. On the Log Analytics workspace blade, in the **Settings** section, click **Advanced settings**.

1. On the **Advanced Settings** blade, click **Data** and review the available options including Windows Event Logs, Windows Performance Counters, Linux Performance Counters, IIS Logs, and Syslog. 

1. Ensure that **Windows Event Logs** is selected, in the **Collect events from the following event logs** text box, type **System** and then click **+**.

    >**Note**: This is how you add event logs to the workspace. Other choices include, for example, **Hardware events** or **Key Management Service**.  

1. Deselect the **INFORMATION** checkbox, leaving the **ERROR** and **WARNING** check boxes selected.

1. Click **Windows Performance Counters**.

    >**Note**: There is a suggested list of performance counters. You can customize this list. 

1. Click **Add the selected performance counters**. 

    >**Note**: The counters are added and configured with 10 second collection sample interval.
  
1. On the **Advanced Settings** blade, click **Save** at the top of page and then, to acknowledge the confirmation, click **OK**.
