---
title: Project Rescheduling
description: "Learn how to reschedule Microsoft Project project files from the project start/finish date using Aspose.Tasks for Java."
type: docs
weight: 30
url: /java/project-rescheduling/
---

## **Reschedule Project From Start or Finish Date**
This topic shows how to reschedule a project from the project start/finish date using Aspose.Tasks for Java.

### **Rescheduling a Project from the Finish Date**
We can recalculate dates from the finish date by setting the project finish date and then invoking the Project.recalculate() method. You can calculate tasks slacks based on their early/late dates.

Programming Sample

The following lines of code show how to achieve this using Java

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-RescheduleProjectFromStartOrFinishDate-schedule-from-finish.java" >}}

### **Rescheduling a Project from the Start Date**
We can calculate dates from start date by setting the project start date and then invoke the Project.recalculate() method.

The following lines of code show how to achieve this using Java.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-RescheduleProjectFromStartOrFinishDate-schedule-from-start.java" >}}

## **Update Project and Reschedule Uncompleted Work**
Microsoft Project lets users update and reschedule work through a defined date. This helps identify work completed up to the specified date as well as reschedule any uncompleted work from a specified date. Aspose.Tasks' [Project](https://apireference.aspose.com/tasks/java/com.aspose.tasks/project) API provides the same functionality by exposing the updateProjectWorkAsComplete and rescheduleUncompletedWorkToStartAfter methods. This article provides a working example of both these methods as a single use case.

### **Update Project**
This topic demonstrates how to update a project through a specified date. The updateProjectWorkAsComplete method updates all the work as complete through a specified date for an entire project.

- If the Boolean input parameter is set to true, the method updates only those tasks to 100% complete that have finish dates before the specified completed-through date.
- If the Boolean input parameter is set to false, the method calculates a percentage complete value based on the scheduled state and complete through dates.
- If a list of task is specified, the method updates all work as complete through the specified date for the list of tasks.

The following sample demonstrates how to achieve this

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-UpdateProjectAndRescheduleuncompletedwork-update-project-and-reschedule-uncompleted-work.java" >}}
