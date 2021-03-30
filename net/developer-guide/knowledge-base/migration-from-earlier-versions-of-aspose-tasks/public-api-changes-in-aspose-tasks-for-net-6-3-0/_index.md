---
title: Public API Changes in Aspose.Tasks for .NET 6.3.0
type: docs
weight: 10
url: /net/public-api-changes-in-aspose-tasks-for-net-6-3-0/
---

{{% alert color="primary" %}} 

This page list public API changes that were introduced in Aspose.Tasks for .NET 6.3.0. It includes new and obsolete public methods, as well as a description of any changes in the behavior of the API that may affect existing code.

{{% /alert %}} 

## **UpdateProjectWorkAsComplete(DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly) method added to Project.**

It updates all work as complete through a specified date for the entire project. Set bool parameter setZeroOrHundredPercentCompleteOnly to false if you want to calculate whether the task is not started, 100% complete or percentage complete value. Set the setZeroOrHundredPercentCompleteOnly to true if you want in-progress tasks to remain at 0 percent. Any tasks whose scheduled finish date is after the complete-through date will not have any progress updated for them.

## **UpdateProjectWorkAsComplete(DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly, List<Task> tasks) method added to Project.**

It updates all work as complete through a specified date for the specified list of tasks in a project. RescheduleUncompletedWorkToStartAfter(DateTime after) method added to Project. It reschedules uncompleted project work for all tasks in a project to start after a specified date.

## **RescheduleUncompletedWorkToStartAfter(DateTime after, List<Task> tasks) method added to Project.**

It reschedules uncompleted project work for the specified list of tasks in a project to start after a specified date.

## **TaskToBarTextConverter BarTextConverter delegate property added to Visualization.BarStyle.**

A declaration of TaskToBarTextConverter is "delegate string BarStyle.TaskToBarTextConverter(Task task);"
It allows to specify a code to be used to render text on the right of task bar when rendering Gantt chart view.
Resource names are rendered by default if BarTextConverter is not provided.

## **IComparer<Task> TasksComparer property added to Saving.SaveOptions.**

It allows to specify sorting order of tasks in the Gantt chart view.
By default tasks are sorted by Task.Id property.

## **StringAlignment property added to GanttChartColumn and ResourceViewColumn.**

It allows left, right or centered alignment of text in columns of PresentationFormat.GanttChart, PresentationFormat.TaskUsage, PresentationFormat.ResourceUsage and PresentationFormat.ResourceSheet presentation formats.

## **CalcSlacks() method has been removed**

The CalcSlacks() method has been removed and is obsolete now as these are already recalculated in Task.Recalculate(Project.RootTask) method with Early/Late dates. Improper use of this method could lead to wrong results and, hence, it has been marked as obsolete now.
