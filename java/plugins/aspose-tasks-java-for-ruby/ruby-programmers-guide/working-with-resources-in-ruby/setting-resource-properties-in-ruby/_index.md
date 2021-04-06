---
title: Setting Resource Properties in Ruby
type: docs
weight: 50
url: /java/setting-resource-properties-in-ruby/
---

## **Aspose.Tasks - Setting Resource Properties**
To set resource properties using **Aspose.Tasks Java for Ruby**, simply invoke **SetResourceProperties** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new
rsc = project.getResources().add("Rsc")
rsc.set(Rjb::import('com.aspose.tasks.Rsc').STANDARD_RATE, Rjb::import('java.math.BigDecimal').valueOf(15))
rsc.set(Rjb::import('com.aspose.tasks.Rsc').OVERTIME_RATE, Rjb::import('java.math.BigDecimal').valueOf(20))
puts "Set resource properties"
{{< /highlight >}}

## **Download Running Code**
Download **Setting Resource Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Resources/setresourceproperties.rb)
