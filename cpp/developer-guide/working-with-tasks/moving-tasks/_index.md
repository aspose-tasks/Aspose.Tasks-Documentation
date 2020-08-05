---
title: Moving Tasks
type: docs
weight: 230
url: /cpp/moving-tasks/
---

{{% alert color="primary" %}} 

Microsoft Project allows moving one task under another task. In this case, the child tasks of the selected tasks are also moved with it. Aspose.Tasks API provides the same feature by moving a task under another task. This can be achieved by adding the selected task to the children of the new parent as shown in this article. The task can be moved under a different parent or the same parent.

{{% /alert %}} 
## **Move Task Under Another Parent**
Please note that using *CalculationMode.None* can improve performance when you add several tasks and call *Recalculate* method one time.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-MoveTaskUnderAnotherParent-MoveTaskUnderAnotherParent.cpp" >}}
## **Moving Task Under the Same Parent**
The MoveToSibling method allows moving a task under the same parent to a specific position.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-MoveTaskUnderSameParent-MoveTaskUnderSameParent.cpp" >}}
## **Add Task To The End**
To add a task to the end of the collection use -1.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-MoveTaskAtTheEnd-MoveTaskAtTheEnd.cpp" >}}
## **Setting a Task to a SubProject**
{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-CreateSubProjectTask-CreateSubProjectTask.cpp" >}}
