---
title: Retrieve a Task's Budget Work and Cost Values in Ruby
type: docs
weight: 150
url: /java/retrieve-a-task-s-budget-work-and-cost-values-in-ruby/
---

## **Aspose.Tasks - Retrieve a Task's Budget Work and Cost Values**
To Retrieve a Task's Budget Work and Cost Values using **Aspose.Tasks Java for Ruby**, simply invoke **GetBudgetWorkAndCostValue** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

project_summary = project.getRootTask()

tsk = Rjb::import('com.aspose.tasks.Tsk')

rsc = Rjb::import('com.aspose.tasks.Rsc')

puts "Project Budget Work = " + project_summary.get(tsk.BUDGET_WORK).to_string

puts "Project Budget Cost = " + project_summary.get(tsk.BUDGET_COST).to_string

\# Get resource by Uid

resource = project.getResources().getByUid(1)

\# Display resource budget work

puts "Resource BudgetWork = " + resource.get(rsc.BUDGET_WORK).to_string

\# Get next resource by Uid

resource = project.getResources().getByUid(2)

\# Display resource budget cost

puts "Resource BudgetCost = " + resource.get(rsc.BUDGET_COST).to_string

{{< /highlight >}}
## **Download Running Code**
Download **Retrieve a Task's Budget Work and Cost Values (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Tasks/getbudgetworkandcostvalue.rb)
