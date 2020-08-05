---
title: Actual Properties
type: docs
weight: 50
url: /net/actual-properties/
---

{{% alert color="primary" %}} 

The actual properties are used to find out how much time or money has been sent on a task to date.

{{% /alert %}} 
## **Working with Actual Properties**
The static class [Tsk](http://www.aspose.com/api/net/tasks/aspose.tasks/tsk) exposes a number of properties for determining a task's actual properties:

- ActualCost: a task's actual cost (double).
- ActualOvertimeCost: a task's actual overtime cost (double).
- ActualOvertimeWork: the actual overtime worked on a task (TimeSpan).
- ActualDuration: a task's actual duration (TimeSpan).
- ActualStart: the date and time that a task actually started (DateTime).
- ActualFinish: the date and time that a task actually finished (DateTime).
- Acwp: the actual cost of the work performed on a task (double).

The [ChildTasksCollector](http://www.aspose.com/api/net/tasks/aspose.tasks/tsk) class collects all the child tasks from a given RootTask when used by [TaskUtils](http://www.aspose.com/api/net/tasks/aspose.tasks.util/taskutils).
### **Actual Properties in Microsoft Project**
To access these properties in Microsoft Project:

1. On the **View** menu, select **More Views** and then **Task Entry**.
1. On the **Insert** menu, select **Column** and add the desired columns to the Task Entry form.
### **Getting Actual Properties with Aspose.Tasks**
A tasks' actual properties can be obtained by traversing the tasks in a project. The code samples below write the actual properties for all tasks found in a project to a console window.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-ReadActualTaskProperties-ReadActualTaskProperties.cs" >}}
