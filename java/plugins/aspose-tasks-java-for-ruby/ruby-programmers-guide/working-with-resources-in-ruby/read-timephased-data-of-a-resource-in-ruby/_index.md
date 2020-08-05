---
title: Read Timephased Data of a Resource in Ruby
type: docs
weight: 20
url: /java/read-timephased-data-of-a-resource-in-ruby/
---

## **Aspose.Tasks - Read Timephased Data of a Resource**
To Read Timephased Data of a Resource using **Aspose.Tasks Java for Ruby**, simply invoke **ReadTimephasedResourceData** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

\# Get the Resource by its ID

resource = project.getResources().getByUid(1)

prj = Rjb::import('com.aspose.tasks.Prj')

\# Print Timephased data of ResourceWork

puts "Timephased data of Resource Work"

result = resource.getTimephasedData(project.get(prj.START_DATE), project.get(prj.FINISH_DATE)).toList()

i = 0

while i < result.size()	

    td = result.get(i)

    puts "Start: " + td.getStart().toString()

    puts "Work: " + td.getValue()

    i +=1

end

{{< /highlight >}}
## **Download Running Code**
Download **Read Timephased Data of a Resource (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Resources/readtimephasedresourcedata.rb)
