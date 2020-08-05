---
title: Managing Assignment Cost in Ruby
type: docs
weight: 70
url: /java/managing-assignment-cost-in-ruby/
---

## **Aspose.Tasks - Managing Assignment Cost**
To Manage Assignment Cost using **Aspose.Tasks Java for Ruby**, simply invoke **AssignmentCost** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

resource_assignments = project.getResourceAssignments().toList()

\# Parse through all the collected resource assignments

i = 0

while i < resource_assignments.size()

  ra = resource_assignments.get(i)

  puts "COST: " + ra.get(Rjb::import('com.aspose.tasks.Asn').COST).to_string

  puts "ACWP: " + ra.get(Rjb::import('com.aspose.tasks.Asn').ACWP).to_string

  puts "BCWP: " + ra.get(Rjb::import('com.aspose.tasks.Asn').BCWP).to_string

  puts "BCWS: " + ra.get(Rjb::import('com.aspose.tasks.Asn').BCWS).to_string

  puts "--------------------------------------------------------"

  i +=1

end    

{{< /highlight >}}
## **Download Running Code**
Download **Managing Assignment Cost (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/ResourceAssignments/assignmentcost.rb)
