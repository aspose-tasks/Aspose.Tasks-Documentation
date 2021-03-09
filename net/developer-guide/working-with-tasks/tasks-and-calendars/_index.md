---
title: Tasks and Calendars
type: docs
weight: 30
url: /net/tasks-and-calendars/
---

{{% alert color="primary" %}} 

It is possible to associate calendars with particular tasks in Microsoft Project. Aspose.Task supports this functionality.

{{% /alert %}} 
## **Tasks with Calendars**
The [Tsk](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk) class exposes the [Calendar](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/calendar) field used to set or get the calendar associated with a task. This property accepts or returns an Aspose.Tasks.Calendar object.

To create a calendar for a task in Microsoft Project:

1. Open a project in Microsoft Project.
2. On the **Project** menu, select **Change Working Times**, then **Create New Calendar**.
3. To assign the calendar to a task, double-click the task in the Task Entry form.
4. Select the **Advanced** tab.
### **Setting Task Calendar**
Create a standard calendar and create a task. Assign the Calendar to the task.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-WriteTaskCalendar-WriteTaskCalendar.cs" >}}
### **Getting Task Calendar**
Get task calendar by traversing the tasks in a project.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-ReadTaskCalendar-ReadTaskCalendar.cs" >}}
