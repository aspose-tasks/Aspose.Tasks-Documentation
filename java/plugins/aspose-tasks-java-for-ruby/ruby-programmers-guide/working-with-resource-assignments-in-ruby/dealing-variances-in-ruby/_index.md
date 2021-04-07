---
title: Dealing Variances in Ruby
description: "Learn how to deal with work variances in Microsoft Project (MPP/XML) files using Aspose.Tasks Java for Ruby."
type: docs
weight: 40
url: /java/dealing-variances-in-ruby/
---

## **Aspose.Tasks - Dealing Variances**
To see resource assignment variance using **Aspose.Tasks Java for Ruby**, simply invoke **AssignmentVariance** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
resource_assignments = project.getResourceAssignments().toList()
i = 0
while i < resource_assignments.size()
  assignment = resource_assignments.get(i)
  puts "Work Variance: " + assignment.get(Rjb::import('com.aspose.tasks.Asn').WORK_VARIANCE).toString()
  puts "Cost Variance: " + assignment.get(Rjb::import('com.aspose.tasks.Asn').COST_VARIANCE).toString()
  puts "Start Variance: " + assignment.get(Rjb::import('com.aspose.tasks.Asn').START_VARIANCE).toString()
  puts "Finish Variance: " + assignment.get(Rjb::import('com.aspose.tasks.Asn').FINISH_VARIANCE).toString()
  puts "--------------------------------------------------------"
  i += 1
end
{{< /highlight >}}

## **Download Running Code**
Download **Dealing Variances (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/ResourceAssignments/assignmentvariance.rb)
