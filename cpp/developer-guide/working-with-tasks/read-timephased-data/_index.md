---
title: Read Task Timephased Data
description: "Learn how to read Microsoft Project (MPP/XML) task timephased data using Aspose.Tasks for C++."
type: docs
weight: 190
url: /cpp/read-timephased-data/
---

{{% alert color="primary" %}}

In Microsoft Project, timephased data is displayed on the right side of the Task Usage and Resource Usage views. You can write this data manually and programmatically it can be written with Aspose.Tasks for C++ API or get it from a project into your application.

{{% /alert %}}

## **Working with Timephased Data**
Aspose.Tasks for C++ API supports reading a task's time-phased data from Microsoft Project (MPP) files. The time-phased data is retrieved using the Task object's GetTimephasedData method.

- To retrieve the task work's time-phased data, the GetTimephasedData method takes the project's start and finish dates as input parameters.
- To retrieve the task cost's time-phased data, it takes an additional input parameter that specifies the type of time phase data as TaskCost.

The following piece of code shows how to read a task's timephased data.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-ReadWriteTimephasedData-ReadWriteTimephasedData.cpp" >}}
