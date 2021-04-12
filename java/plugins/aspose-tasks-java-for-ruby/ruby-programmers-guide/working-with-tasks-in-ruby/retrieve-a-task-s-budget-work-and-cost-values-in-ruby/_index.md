---
title: Retrieve a Task's Budget Work and Cost Values in Ruby
description: "Learn how to read Microsoft Project (MPP/XML) task budget work and cost values using Aspose.Tasks Java for Ruby."
type: docs
weight: 150
url: /java/retrieve-a-task-s-budget-work-and-cost-values-in-ruby/
---

## **Aspose.Tasks - Retrieve a Task's Budget Work and Cost Values**
To Retrieve a Task's Budget Work and Cost Values using **Aspose.Tasks Java for Ruby**, simply invoke **GetBudgetWorkAndCostValue** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
project_summary = project.getRootTask()
tsk = Rjb::import('com.aspose.tasks.Tsk')
rsc = Rjb::import('com.aspose.tasks.Rsc')
puts "Project Budget Work = " + project_summary.get(tsk.BUDGET_WORK).to_string
puts "Project Budget Cost = " + project_summary.get(tsk.BUDGET_COST).to_string
resource = project.getResources().getByUid(1)
puts "Resource BudgetWork = " + resource.get(rsc.BUDGET_WORK).to_string
resource = project.getResources().getByUid(2)
puts "Resource BudgetCost = " + resource.get(rsc.BUDGET_COST).to_string
{{< /highlight >}}

## **Download Running Code**
Download **Retrieve a Task's Budget Work and Cost Values (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/getbudgetworkandcostvalue.rb)
