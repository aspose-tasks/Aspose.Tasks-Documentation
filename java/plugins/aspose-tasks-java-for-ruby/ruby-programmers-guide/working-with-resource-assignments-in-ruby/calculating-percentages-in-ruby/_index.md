---
title: Calculating Percentages in Ruby
description: "Learn how to calculate percentages in Microsoft Project (MPP/XML) files using Aspose.Tasks Java for Ruby."
type: docs
weight: 20
url: /java/calculating-percentages-in-ruby/
---

## **Aspose.Tasks - Calculating Percentages**
To Calculate Percentage of the completed work using **Aspose.Tasks Java for Ruby**, simply invoke **AssignmentPercentWorkComplete** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
resource_assignments = project.getResourceAssignments().toList()
i = 0
while i < resource_assignments.size()
  assignment = resource_assignments.get(i)
  puts "Percentage of the Completed Work: " + assignment.get(Rjb::import('com.aspose.tasks.Asn').PERCENT_WORK_COMPLETE).toString()
  puts "--------------------------------------------------------"
  i += 1
end
{{< /highlight >}}

## **Download Running Code**
Download **Calculating Percentages (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/ResourceAssignments/assignmentpercentworkcomplete.rb)
