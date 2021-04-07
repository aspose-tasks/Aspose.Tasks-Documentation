---
title: Working with Resource Assignment Budgets in Ruby
description: "Learn how to work with Microsoft Project (MPP/XML) resource assignment budgets using Aspose.Tasks Java for Ruby."
type: docs
weight: 10
url: /java/assignment-budget-in-ruby/
---

## **Aspose.Tasks - Assignment Budget**
To get Assignment Budget using **Aspose.Tasks Java for Ruby**, simply invoke **AssignmentBudget** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
resource_assignments = project.getResourceAssignments().toList()
i = 0
while i < resource_assignments.size()
  assignment = resource_assignments.get(i)
  puts "Budget Cost: " + assignment.get(Rjb::import('com.aspose.tasks.Asn').BUDGET_COST).toString()
  puts "Budget Work: " + assignment.get(Rjb::import('com.aspose.tasks.Asn').BUDGET_WORK).toString()
  puts "--------------------------------------------------------"
  i += 1
end
{{< /highlight >}}

## **Download Running Code**
Download **Assignment Budget (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/ResourceAssignments/assignmentbudget.rb)
