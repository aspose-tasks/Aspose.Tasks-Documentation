---
title: Reschedule Project tasks and resource assignments
description: "Learn how to reschedule the project using Aspose.Tasks for .NET."
type: docs
weight: 50
url: /net/project-rescheduling/
---

## **Reschedule Project From Start or Finish Date**
This topic shows how to reschedule a project from the project start/finish date using Aspose.Tasks for .NET.

We can recalculate dates from finish date by setting the project finish date and then invoking [Project.Recalculate()](https://apireference.aspose.com/tasks/net/aspose.tasks/project/methods/recalculate).

**Programming Sample: Rescheduling a Project from the Finish Date**
The following lines of code show how to achieve this using C#.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-Rescheduling-RescheduleProjectFromFinishDate-RescheduleProjectFromFinishDate.cs" >}}

**Programming Sample: Rescheduling a Project from the Start Date**
The following lines of code shows how to achieve this using C#.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-Rescheduling-RescheduleProjectFromStartDate-ReschedueProjectFromStartDate.cs" >}}

## **Update Project and Reschedule Incomplete Work**
Microsoft Project provides the facility to update and reschedule work through a defined date. This helps identify work completed up to the specified date as well as reschedule any uncompleted work from a specified date. Aspose.Tasks's [Project](https://apireference.aspose.com/tasks/net/aspose.tasks/project) API provides the same functionality by exposing the [UpdateProjectWorkAsComplete](https://apireference.aspose.com/tasks/net/aspose.tasks/project/methods/updateprojectworkascomplete/index) and [RescheduleUncompletedWorkToStartAfter methods](https://apireference.aspose.com/tasks/net/aspose.tasks/project/methods/rescheduleuncompletedworktostartafter/index). This topic provides a working example of both these methods as a single use case.

### **Update Project Files**
The example below demonstrates how to update a project through a specified date. The **UpdateProjectWorkAsComplete** method updates all the work as complete through a specified date for an entire project.

1. If the Boolean input parameter is set to true, the method updates only those tasks to 100% complete that have finish dates before the specified completed-through date.
2. If the Boolean input parameter is set to false, the method calculates a percentage complete value based on the scheduled state and complete-through dates.
3. If a list of task is specified, the method updates all work as complete through the specified date for the list of tasks.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-Rescheduling-UpdateProjectAndRescheduleUncompletedWork-UpdateProjectAndRescheduleUncompletedWork.cs" >}}
