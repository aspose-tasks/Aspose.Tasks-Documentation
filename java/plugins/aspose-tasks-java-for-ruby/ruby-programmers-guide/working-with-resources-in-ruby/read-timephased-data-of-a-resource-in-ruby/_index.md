---
title: Read Timephased Data of a Resource in Ruby
description: "Learn how to generate or edit timephased data of Microsoft Project (MPP/XML) resources using Aspose.Tasks Java for Ruby."
type: docs
weight: 20
url: /java/read-timephased-data-of-a-resource-in-ruby/
---

## **Aspose.Tasks - Read Timephased Data of a Resource**
To read timephased data of a resource using **Aspose.Tasks Java for Ruby**, one can simply invoke **ReadTimephasedResourceData** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
resource = project.getResources().getByUid(1)
prj = Rjb::import('com.aspose.tasks.Prj')
puts "Timephased data of Resource Work"
result = resource.getTimephasedData(project.get(prj.START_DATE), project.get(prj.FINISH_DATE)).toList()
i = 0
while i < result.size()
    td = result.get(i)
    puts "Start: " + td.getStart().toString()
    puts "Work: " + td.getValue()
    i += 1
end
{{< /highlight >}}

You can download the working code example from [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Resources/readtimephasedresourcedata.rb).