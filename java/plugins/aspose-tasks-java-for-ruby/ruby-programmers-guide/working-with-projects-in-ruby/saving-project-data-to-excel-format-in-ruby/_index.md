---
title: Saving Project Data to Excel Format in Ruby
type: docs
weight: 130
url: /java/saving-project-data-to-excel-format-in-ruby/
---

## **Aspose.Tasks - Saving Project Data to Excel Format**
To Save Project Data to Excel Format using **Aspose.Tasks Java for Ruby**, simply invoke **SaveProjectDataToExcel** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

\# Save the Project as XLSX

project.save(data_dir + "Project.XLSX", Rjb::import('com.aspose.tasks.SaveFileFormat').XLSX)

puts "Saved project data to Excel, please check the output file"

{{< /highlight >}}
## **Download Running Code**
Download **Saving Project Data to Excel Format (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/saveprojectdatatoexcel.rb)
