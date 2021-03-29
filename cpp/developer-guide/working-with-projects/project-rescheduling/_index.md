---
title: Project Rescheduling
type: docs
weight: 40
url: /cpp/project-rescheduling/
---

## **Reschedule Project From Start or Finish Date**
This topic shows how to reschedule a project from the project start/finish date using Aspose.Tasks for C++.

We can recalculate dates from finish date by setting the project finish date and then invoking Task.Recalculate(). Rescheduling is made faster by the public method Project.CalcSlacks(). You can calculate tasks slacks based on their early/late dates.
### **Programming Sample: Rescheduling a Project from the Finish Date**
The following lines of code demonstrate how to achieve rescheduling of a project from the finish date.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-Rescheduling-RescheduleProjectFromFinishDate-RescheduleProjectFromFinishDate.cpp" >}}
### **Programming Sample: Rescheduling a Project from the Start Date**
The following lines of code demonstrate how to achieve rescheduling of a project from the start date.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-Rescheduling-RescheduleProjectFromStartDate-ReschedueProjectFromStartDate.cpp" >}}
## **Update Project and Reschedule Uncomplete Work**
Microsoft Project provides the facility to update and reschedule work through a defined date. This helps identify work completed up to the specified date as well as reschedule any uncompleted work from a specified date. Aspose.Tasks' [Project]() API provides the same functionality by exposing the UpdateProjectWorkAsComplete and RescheduleUncompletedWorkToStartAfter methods. This topic provides a working example of both these methods as a single-use case.
### **Update Project**
The example below demonstrates how to update a project through a specified date. The UpdateProjectWorkAsComplete method updates all the work as complete through a specified date for an entire project.

1. If the Boolean input parameter is set to true, the method updates only those tasks to 100% complete that have finish dates before the specified completed-through date.
2. If the Boolean input parameter is set to false, the method calculates a percentage complete value based on the scheduled state and complete-through dates.
3. If a list of task is specified, the method updates all work as complete through the specified date for the list of tasks.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-Rescheduling-UpdateProjectAndRescheduleUncompletedWork-UpdateProjectAndRescheduleUncompletedWork.cpp" >}}
