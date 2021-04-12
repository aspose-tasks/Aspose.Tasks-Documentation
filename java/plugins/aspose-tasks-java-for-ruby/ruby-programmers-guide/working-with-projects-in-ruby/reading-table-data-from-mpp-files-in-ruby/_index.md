---
title: Reading Table Data from MPP files in Ruby
description: "This article explains how to read table data from Microsoft Project (MPP/XML) files using Aspose.Tasks Java for Ruby."
keywords: "read table data, read MPP table data, Export table data MPP, Aspose.Tasks Java for Ruby, Ruby"
type: docs
weight: 100
url: /java/reading-table-data-from-mpp-files-in-ruby/
---

## **Aspose.Tasks - Reading Table Data from MPP files**
To read Table Data from MPP files using **Aspose.Tasks Java for Ruby**, simply invoke **ReadingTableData** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
t1 = project.getTables().toList().get(0)
puts "Table Fields Count" + t1.getTableFields().size().to_s
f = t1.getTableFields().get(0)
puts "Field width: " + f.getWidth().to_s
puts "Field Title: " + f.getTitle().to_s
puts "Field Title Alignment: " + f.getAlignTitle().to_s
puts "Field Align Data: " + f.getAlignData().to_s
f = t1.getTableFields().get(1)
puts "Field width: " + f.getWidth().to_s
puts "Field Title: " + f.getTitle().to_s
puts "Field Title Alignment: " + f.getAlignTitle().to_s
puts "Field Align Data: " + f.getAlignData().to_s
{{< /highlight >}}

## **Download Running Code**
Download **Reading Table Data from MPP files (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/readingtabledata.rb)
