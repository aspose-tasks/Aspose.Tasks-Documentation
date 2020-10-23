---
title: Read a Task's Timephased Data
type: docs
weight: 210
url: /java/read-a-task-s-timephased-data/
---

{{% alert color="primary" %}} 

In Microsoft Project, time-phased data is displayed on the right side of the Task Usage and Resource Usage views. Users can write this data manually and with Aspose.Tasks, you can write it programmatically, or get it from a project into your application.

{{% /alert %}} 
## **Working with Timephased Data**
Aspose.Tasks supports reading a task's time-phased data from Microsoft Project (MPP) files. The time-phased data is retrieved using the [Task](https://apireference.aspose.com/tasks/java/com.aspose.tasks/Task/) object's Timescaledata method.

- To retrieve the task work's time-phased data, the Timescaledata method takes the project's start and finish dates as input parameters.
- To retrieve the task cost's time-phased data, it takes an additional input parameter that specifies the type of time phase data as TaskCost.

The following piece of code shows how to read a task's time-phased data.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-TaskTimephasedData-task-time-phased-data.java" >}}
