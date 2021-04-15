---
title: Handling Task Constraints
description: "Learn how to handle Microsoft Project (MPP/XML) task constraints using Aspose.Tasks for .NET."
type: docs
weight: 40
url: /net/handling-task-constraints/
---

Task constraints are used to define a Microsoft Project project's schedule and define when tasks should be started or finished. Constraints can be flexible - start or end as soon as possible or as late as possible - or inflexible. Inflexible constraints are tied to specific dates.

## **Working with Constraints**
The [ConstraintDate](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/constraintdate) and [ConstraintType](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk/fields/constrainttype) properties are exposed by the static class [Tsk](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk) class to handle constraints:

- ConstraintDate accepts and returns the DateTime data type.
- ConstraintType accepts and returns one of the values of the ConstraintType enumeration.

### **Setting Constraints in Microsoft Project**
To set constraints in Microsoft Project:

1. On the **View** menu, select **More Views** and then **Task Entry Form**.
2. Double click a task on the Task Entry Form.
3. Select the Advanced tab.
4. Set a constraint by selecting an option from the **Constraint type** list and a date for the **Constraint date** list.

### **Setting Constraints with Aspose.Tasks**
The constraint date is NA when the constraint type is **As Soon As Possible** or **As Late As Possible**. For date values equal to NA, Aspose.Tasks uses the value "1/1/2000” in the evaluation version, and DateTime.MinValue for the licensed product. In the below case, we take a source project file as an input and apply different types of constraints on various tasks in each case. The following code samples show the application of different Constraint types.

The code samples below set the constraint type set to Start No Earlier Than.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-WorkingWithTaskConstraints-SetConstraintStartNoEarlierThan.cs" >}}

The code samples below set the constraint type set to Finish No Earlier Than.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-WorkingWithTaskConstraints-SetConstraintFinishNoEarlierThan.cs" >}}

The code samples below set the constraint type set to Must Start On.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-WorkingWithTaskConstraints-SetConstraintMustStartOn.cs" >}}

The code samples below set the constraint type set to As Late As Possible.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-WorkingWithTaskConstraints-SetConstraintAsLateAsPossible.cs" >}}

The code sample below shows the constraint type set to Must Finish On.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-WorkingWithTaskConstraints-SetConstraintMustFinishOn.cs" >}}

### **Getting Constraints**
This code sample displays any constraints found when traversing the tasks in the project to a command window.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-WorkingWithTaskConstraints-GetConstraints.cs" >}}
