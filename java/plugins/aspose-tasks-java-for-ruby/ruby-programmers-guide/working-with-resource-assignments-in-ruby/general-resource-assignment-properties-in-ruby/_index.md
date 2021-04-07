---
title: General Resource Assignment Properties in Ruby
description: "Learn how to read or edit properties of Microsoft Project (MPP/XML) resource assignments using Aspose.Tasks Java for Ruby."
type: docs
weight: 50
url: /java/general-resource-assignment-properties-in-ruby/
---

## **Aspose.Tasks - Getting General Resource Assignment Properties**
To get general resource assignment properties using **Aspose.Tasks Java for Ruby**, call **get_resource_assignments** method of **ResourceAssignmentProperties** module. Here you can see example code.

{{< highlight ruby >}}
 def get_resource_assignments()  
    project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
    resource_assignments = project.getResourceAssignments().toList()
    i = 0
    while i < resource_assignments.size()
      assignment = resource_assignments.get(i)
      puts assignment.get(Rjb::import('com.aspose.tasks.Asn').UID).to_string
      puts assignment.get(Rjb::import('com.aspose.tasks.Asn').START).to_string
      puts assignment.get(Rjb::import('com.aspose.tasks.Asn').FINISH).to_string
      puts "--------------------------------------------------------"
      i += 1
    end
end
{{< /highlight >}}

## **Aspose.Tasks - Setting General Resource Assignment Properties**
To set General Resource Assignment Properties using **Aspose.Tasks Java for Ruby**, call **set_resource_assignments** method of **ResourceAssignmentProperties** module. Here you can see example code.

{{< highlight ruby >}}
def set_resource_assignments()  
    project = Rjb::import('com.aspose.tasks.Project').new
    task = project.getRootTask().getChildren().add("Task")
    rsc = project.getResources().add("Rsc")
    rsc.set(Rjb::import('com.aspose.tasks.Rsc').STANDARD_RATE, Rjb::import('java.math.BigDecimal').valueOf(10))
    rsc.set(Rjb::import('com.aspose.tasks.Rsc').OVERTIME_RATE, Rjb::import('java.math.BigDecimal').valueOf(15))
    assignment = project.getResourceAssignments().add(task, rsc)
    puts "Set resource assignment properties."
end
{{< /highlight >}}

## **Download Running Code**
Download **General Resource Assignment Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/ResourceAssignments/resourceassignmentproperties.rb)
