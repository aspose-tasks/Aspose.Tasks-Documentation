---
title: Managing Assignment Cost in Ruby
description: "Learn how to manage Microsoft Project (MPP/XML) resource assignment costs using Aspose.Tasks Java for Ruby."
type: docs
weight: 70
url: /java/managing-assignment-cost-in-ruby/
---

## **Aspose.Tasks - Managing Assignment Cost**
To manage Assignment Cost using **Aspose.Tasks Java for Ruby**, simply invoke **AssignmentCost** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
resource_assignments = project.getResourceAssignments().toList()
i = 0
while i < resource_assignments.size()
  assignment = resource_assignments.get(i)
  puts "COST: " + assignment.get(Rjb::import('com.aspose.tasks.Asn').COST).to_string
  puts "ACWP: " + assignment.get(Rjb::import('com.aspose.tasks.Asn').ACWP).to_string
  puts "BCWP: " + assignment.get(Rjb::import('com.aspose.tasks.Asn').BCWP).to_string
  puts "BCWS: " + assignment.get(Rjb::import('com.aspose.tasks.Asn').BCWS).to_string
  puts "--------------------------------------------------------"
  i += 1
end
{{< /highlight >}}

## **Download Running Code**
Download **Managing Assignment Cost (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/ResourceAssignments/assignmentcost.rb)
