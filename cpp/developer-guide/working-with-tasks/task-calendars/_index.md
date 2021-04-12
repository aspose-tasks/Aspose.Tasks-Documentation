---
title: Task Calendars
description: "Learn how to work with Microsoft Project (MPP/XML) task calendars using Aspose.Tasks for C++."
type: docs
weight: 40
url: /cpp/task-calendars/
---

It is possible to associate calendars with particular tasks in Microsoft Project. Aspose.Task supports this functionality.

## **Tasks with Calendars**
The [Tsk](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.tsk) class exposes the Calendar field used to set or get the calendar associated with a task. This property accepts or returns an Aspose.Tasks.Calendar object.

To create a calendar for a task in Microsoft Project:

1. Open a project in Microsoft Project.
2. On the **Project** menu, select **Change Working Times**, then **Create New Calendar**.
3. To assign the calendar to a task, double-click the task in the Task Entry form.
4. Select the **Advanced** tab.

### **Setting Task Calendar**
Create a standard calendar and create a task. Assign the Calendar to the task.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-WriteTaskCalendar-WriteTaskCalendar.cpp" >}}

### **Getting Task Calendar**
Get task calendar by traversing the tasks in a project.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-ReadTaskCalendar-ReadTaskCalendar.cpp" >}}
