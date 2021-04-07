---
title: Working with Filter Data from MPP files in Ruby
type: docs
weight: 170
url: /java/working-with-filter-data-from-mpp-files-in-ruby/
---

## **Aspose.Tasks - Reading Filter Definition Data**
To Read Filter Definition Data using **Aspose.Tasks Java for Ruby**, call **get_filter_definition_data** method of **FilterData** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
task_filters = project.getTaskFilters().toList()
puts "Task Filters Count: " + task_filters.size().to_s
puts "All Tasks: " + task_filters.get(0).getName().to_s
puts "Task Item: " + task_filters.get(0).getFilterType().to_s
puts "Task Filters Show In Menu: " + task_filters.get(0).getShowInMenu().to_s
puts "Task filter ShowRelatedSummaryRows: "  + task_filters.get(0).getShowRelatedSummaryRows().to_s
rsc_filters = project.getResourceFilters().toList()
puts "Project.ResourceFilters count: " +  rsc_filters.size().to_s
puts "Resource Filter Item Type: Item.ResourceType: "  + rsc_filters.get(0).getFilterType().to_s
puts "Resource filter ShowInMenu"  + rsc_filters.get(0).getShowInMenu().to_s
puts "Resource filter ShowRelatedSummaryRows: " + rsc_filters.get(0).getShowRelatedSummaryRows().to_s
{{< /highlight >}}

## **Download Running Code**
Download **Working with Filter Data from MPP files (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/filterdata.rb)
