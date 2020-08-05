---
title: Get Number of Pages in Project in Ruby
type: docs
weight: 70
url: /java/get-number-of-pages-in-project-in-ruby/
---

## **Aspose.Tasks - Get Number of Pages in Project**
To Get Number of Pages in Project using **Aspose.Tasks Java for Ruby**, simply invoke **GetNumberOfPages** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

presentation_format = Rjb::import('com.aspose.tasks.PresentationFormat')

timescale = Rjb::import('com.aspose.tasks.Timescale')

\# Get number of pages

puts "Number of Pages = " + project.getPageCount(presentation_format.ResourceUsage, timescale.Days).to_s

\# Get number of pages (Months)

puts "Number of Pages = " + project.getPageCount(presentation_format.ResourceUsage, timescale.Months).to_s

\# Get number of pages (ThirdsOfMonths)

puts "Number of Pages = " + project.getPageCount(presentation_format.ResourceUsage, timescale.ThirdsOfMonths).to_s

{{< /highlight >}}
## **Download Running Code**
Download **Get Number of Pages in Project (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/getnumberofpages.rb)
