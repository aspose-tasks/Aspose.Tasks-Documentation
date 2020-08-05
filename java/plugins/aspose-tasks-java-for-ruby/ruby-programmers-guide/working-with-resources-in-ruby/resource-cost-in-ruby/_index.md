---
title: Resource Cost in Ruby
type: docs
weight: 40
url: /java/resource-cost-in-ruby/
---

## **Aspose.Tasks - Resource Cost**
To get Resource Cost using **Aspose.Tasks Java for Ruby**, simply invoke **ResourceCost** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'project.mpp')

resources = project.getResources().toList()

rsc = Rjb::import('com.aspose.tasks.Rsc')

\# Parse through all the collected tasks

i = 0

while i < resources.size()

    resource = resources.get(i)

    if resource.get(rsc.NAME) != nil

      puts "Cost: " + resource.get(rsc.COST).to_string

      puts "ACWP: " + resource.get(rsc.ACWP).to_string

      puts "BCWS: " + resource.get(rsc.BCWS).to_string

      puts "BCWP: " + resource.get(rsc.BCWP).to_string

      puts "---------------------------------------------"

    end

    i +=1

end

{{< /highlight >}}
## **Download Running Code**
Download **Resource Cost (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Resources/resourcecost.rb)
