---
title: General Resource Assignment Properties in Ruby
type: docs
weight: 50
url: /java/general-resource-assignment-properties-in-ruby/
---

## **Aspose.Tasks - Getting General Resource Assignment Properties**
To Get General Resource Assignment Properties using **Aspose.Tasks Java for Ruby**, call **get_resource_assignments** method of **ResourceAssignmentProperties** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 def get_resource_assignments()  

    data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



   

    project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

    resource_assignments = project.getResourceAssignments().toList()

    # Parse through all the collected resource assignments

    i = 0

    while i < resource_assignments.size()

      ra = resource_assignments.get(i)

      puts ra.get(Rjb::import('com.aspose.tasks.Asn').UID).to_string

      puts ra.get(Rjb::import('com.aspose.tasks.Asn').START).to_string

      puts ra.get(Rjb::import('com.aspose.tasks.Asn').FINISH).to_string

      puts "--------------------------------------------------------"

      i +=1

    end    

end

{{< /highlight >}}
## **Aspose.Tasks - Setting General Resource Assignment Properties**
To Set General Resource Assignment Properties using **Aspose.Tasks Java for Ruby**, call **set_resource_assignments** method of **ResourceAssignmentProperties** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 def set_resource_assignments()  

    data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



   

    project = Rjb::import('com.aspose.tasks.Project').new

    task = project.getRootTask().getChildren().add("Task")

    rsc = project.getResources().add("Rsc")

    rsc.set(Rjb::import('com.aspose.tasks.Rsc').STANDARD_RATE, Rjb::import('java.math.BigDecimal').valueOf(10))

    rsc.set(Rjb::import('com.aspose.tasks.Rsc').OVERTIME_RATE, Rjb::import('java.math.BigDecimal').valueOf(15))

    assn = project.getResourceAssignments().add(task, rsc)

    puts "Set resource assignment properties."

end

{{< /highlight >}}
## **Download Running Code**
Download **General Resource Assignment Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/ResourceAssignments/resourceassignmentproperties.rb)
