---
title: Aspose.Tasks for C++ 21.1 Release Notes
type: docs
weight: 100
url: /cpp/aspose-tasks-for-cpp-21-1-release-notes/
---

{{% alert color="primary" %}} 

This page contains release notes information for [Aspose.Tasks for C++ 21.1](https://downloads.aspose.com/tasks/cpp/new-releases/aspose.tasks-for-c---21.1/).

{{% /alert %}}
## **All Changes**
|**Key**|**Summary**|**Issue Type**|
| :- | :- | :- |
| TASKSNET-4597 | Add support for 'Task Summary Name' field. | Enhancement |
| TASKSNET-4631 | Fix incorrect position of not fit task labels when rendering Gantt chart view | Bug |
| TASKSNET-4628 | Fix incorrect error message shown when trying to read a list of projects from empty Project Online account | Bug |
| TASKSNET-4599 | Fix application of bar styles with non-default names when rendering Gantt chart view | Bug |
| TASKSNET-4588 | Fix exception when trying to add a new task in XER project | Bug |
| TASKSNET-4601 | Fix duplicated resources when reading XER of P6XML file | Bug |

## **Public API and Backwards Incompatible Changes**

|**The following public enumerations were added:**|**Description**|
| :- | :- |
| Aspose.Tasks.Visualization.Shape.Diamond | Indicates Diamond shape. |
| Aspose.Tasks.Field.TaskSummaryName | The name of the summary task associated with the task. |

|**The following public methods and properties were added:** | **Description** |
| :- | :- |
| Aspose.Tasks.View.#ctor(ViewScreen) | Initializes a new instance of the <see cref="View"/> class which can be displayed in the specified ViewScreen. |


## **Examples**

Related issue: TASKSNET-4597 - Field 'TaskSummaryName' can be used in view's columns

In order to show 'TaskSummaryName' column in exported document the next code sample can be used:
{{< highlight csharp >}}
var field = new TableField
{
    Field = Field.TaskSummaryName,
    Title = "Task Summary Name",
    Width = 30
};

project.Views.ToList()[0].Table.TableFields.Add(field);
{{< /highlight >}}