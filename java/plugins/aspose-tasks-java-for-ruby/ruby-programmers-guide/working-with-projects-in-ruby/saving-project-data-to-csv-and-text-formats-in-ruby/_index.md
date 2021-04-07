---
title: Saving Project Data to CSV and Text Formats in Ruby
type: docs
weight: 120
url: /java/saving-project-data-to-csv-and-text-formats-in-ruby/
---

## **Aspose.Tasks - Saving a Project as CSV**
To Save a Project as CSV using **Aspose.Tasks Java for Ruby**, call **save_to_csv** method of **SaveProjectDataToOtherFormats** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
project.save("Project.csv", Rjb::import('com.aspose.tasks.SaveFileFormat').CSV)
puts "Saved project data to CSV, please check the output file"
{{< /highlight >}}

## **Aspose.Tasks - Saving a Project as Text**
To Save a Project as Text using **Aspose.Tasks Java for Ruby**, call **save_to_text** method of **SaveProjectDataToOtherFormats** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
project.save("Project.txt", Rjb::import('com.aspose.tasks.SaveFileFormat').TXT)
puts "Saved project data to Text, please check the output file"
{{< /highlight >}}

## **Download Running Code**
Download **Saving Project Data to CSV and Text Formats (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/saveprojectdatatootherformats.rb)
