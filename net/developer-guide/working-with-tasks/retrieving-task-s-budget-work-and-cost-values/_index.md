---
title: Retrieving Task's Budget Work and Cost Values
type: docs
weight: 240
url: /net/retrieving-task-s-budget-work-and-cost-values/
---

{{% alert color="primary" %}} 

Microsoft Project 2007 and 2010 provide budget cost and budget work as task fields. Aspose.Tasks provides these properties as Task.BudgetWork and Task.BudgetCost.

{{% /alert %}} 
## **Reading budget work and cost value**
Before Aspose.Tasks for .NET 5.0.0, budget work and cost could be calculated by accessing an activity's resource assignments and summing up the budget cost and work values. From Aspose.Task for .NET 5.0.0, it can be obtained directly as described in the following code.
### **Programming Samples**
The following lines of code retrieve a task's budget work and cost information.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-ReadBudgetWorkAndCost-ReadBudgetWorkAndCost.cs" >}}
