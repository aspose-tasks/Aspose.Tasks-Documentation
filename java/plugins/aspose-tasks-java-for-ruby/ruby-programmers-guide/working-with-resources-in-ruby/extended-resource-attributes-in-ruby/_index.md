---
title: Extended Resource Attributes in Ruby
type: docs
weight: 10
url: /java/extended-resource-attributes-in-ruby/
---

## **Aspose.Tasks - Extended Resource Attributes**
To set Extended Resource Attributes using **Aspose.Tasks Java for Ruby**, simply invoke **ExtendedResourceAttributes** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

res = project.getResources().toList().get(0)

ea = Rjb::import('com.aspose.tasks.ExtendedAttribute').new

ea.setFieldId("11")

ea.setValue("MyValueEA")

ea.setValueGuid("MyValueGuidEA")

res.getExtendedAttributes().add(ea)

puts "Set extended resource attributes."

{{< /highlight >}}
## **Download Running Code**
Download **Extended Resource Attributes (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Resources/extendedresourceattributes.rb)
