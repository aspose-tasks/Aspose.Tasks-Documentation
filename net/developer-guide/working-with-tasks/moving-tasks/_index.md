---
title: Moving Tasks
description: "Learn how to move with Microsoft Project (MPP/XML) the tasks under another ones using Aspose.Tasks for .NET."
type: docs
weight: 270
url: /net/moving-tasks/
---

Microsoft Project allows moving one task under another task. In this case, the child tasks of the selected tasks are also moved with it. Aspose.Tasks for .NET provides the same feature by moving a task under another task. This can be achieved by adding the selected task to the children of the new parent as shown in this article. The task can be moved under a different parent or the same parent.

## **Move Task Under Another Parent**
Please note that using *CalculationMode.None* can improve performance when you add several tasks and call [Recalculate](https://apireference.aspose.com/tasks/net/aspose.tasks/project/methods/recalculate) method one time.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-MoveTaskUnderAnotherParent.cs" >}}

## **Moving Task Under the Same Parent**
The [MoveToSibling](https://apireference.aspose.com/tasks/net/aspose.tasks/task/methods/movetosibling) method allows moving a task under the same parent to a specific position.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-MoveTaskUnderSameParent.cs" >}}

## **Add Task To The End**
To add a task to the end of the collection use -1.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-MoveTaskAtTheEnd.cs" >}}
