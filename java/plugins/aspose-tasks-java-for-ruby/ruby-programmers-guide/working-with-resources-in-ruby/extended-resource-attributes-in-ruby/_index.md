---
title: Managing Resource Extended Attributes in Ruby
description: "Learn how to add, edit or remove Microsoft Project (MPP/XML) resource extended attributes using Aspose.Tasks Java for Ruby."
type: docs
weight: 10
url: /java/extended-resource-attributes-in-ruby/
---

## **Aspose.Tasks - Extended Resource Attributes**
To set Extended Resource Attributes using **Aspose.Tasks Java for Ruby**, simply invoke **ExtendedResourceAttributes** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
res = project.getResources().toList().get(0)
attribute = Rjb::import('com.aspose.tasks.ExtendedAttribute').new
attribute.setFieldId("11")
attribute.setValue("MyValueEA")
attribute.setValueGuid("MyValueGuidEA")
res.getExtendedAttributes().add(attribute)
puts "Set extended resource attributes."
{{< /highlight >}}

## **Download Running Code**
Download **Extended Resource Attributes (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Resources/extendedresourceattributes.rb)
