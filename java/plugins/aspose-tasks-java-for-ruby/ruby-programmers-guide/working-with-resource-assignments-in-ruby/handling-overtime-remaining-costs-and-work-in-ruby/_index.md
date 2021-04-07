---
title: Handling Overtime, Remaining Costs and Work in Ruby
type: docs
weight: 60
url: /java/handling-overtime-remaining-costs-and-work-in-ruby/
---

## **Aspose.Tasks - Handling Overtime, Remaining Costs and Work**
To Handle Overtime, Remaining Costs and Work using **Aspose.Tasks Java for Ruby**, simply invoke **AssignmentOvertimeAndRemainingCosts** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
resource_assignments = project.getResourceAssignments().toList()
i = 0
while i < resource_assignments.size()
  assignment = resource_assignments.get(i)
  puts "Overtime Cost: " + assignment.get(Rjb::import('com.aspose.tasks.Asn').OVERTIME_COST).toString()
  puts "Overtime Work: " + assignment.get(Rjb::import('com.aspose.tasks.Asn').OVERTIME_WORK).toString()
  puts "Remaining Cost: " + assignment.get(Rjb::import('com.aspose.tasks.Asn').REMAINING_COST).toString()
  puts "Remaining Overtime Cost: " + assignment.get(Rjb::import('com.aspose.tasks.Asn').REMAINING_OVERTIME_COST).toString()
  puts "Remaining Overtime Work: " + assignment.get(Rjb::import('com.aspose.tasks.Asn').REMAINING_OVERTIME_WORK).toString()
  puts "--------------------------------------------------------"
  i += 1
end
{{< /highlight >}}

## **Download Running Code**
Download **Handling Overtime, Remaining Costs and Work (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/ResourceAssignments/assignmentovertimeandremainingcosts.rb)
