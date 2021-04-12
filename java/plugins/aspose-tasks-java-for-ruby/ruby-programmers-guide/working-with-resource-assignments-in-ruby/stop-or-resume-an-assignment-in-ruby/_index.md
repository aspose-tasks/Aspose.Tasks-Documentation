---
title: Stop or Resume an Assignment in Ruby
description: "Learn how to stop or resume Microsoft Project (MPP/XML) resource assignments using Aspose.Tasks Java for Ruby."
type: docs
weight: 80
url: /java/stop-or-resume-an-assignment-in-ruby/
---

## **Aspose.Tasks - Stop or Resume an Assignment**
To Stop or Resume an Assignment using **Aspose.Tasks Java for Ruby**, simply invoke **StopAndResumeAssignment** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
resource_assignments = project.getResourceAssignments().toList()
i = 0
while i < resource_assignments.size()
  assignment = resource_assignments.get(i)
  if assignment.get(Rjb::import('com.aspose.tasks.Asn').STOP).toString() == "1/1/2000"
    puts "NA"
  else
     puts assignment.get(Rjb::import('com.aspose.tasks.Asn').STOP).toString()
  end
  if assignment.get(Rjb::import('com.aspose.tasks.Asn').RESUME).toString() == "1/1/2000"
    puts "NA"
  else
    puts assignment.get(Rjb::import('com.aspose.tasks.Asn').RESUME).toString()
  end
  i += 1
end
{{< /highlight >}}

## **Download Running Code**
Download **Stop or Resume an Assignment (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/ResourceAssignments/stopandresumeassignment.rb)
