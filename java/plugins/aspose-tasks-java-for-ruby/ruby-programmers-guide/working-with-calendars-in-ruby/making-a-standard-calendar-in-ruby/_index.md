---
title: Making a Standard Calendar in Ruby
type: docs
weight: 40
url: /java/making-a-standard-calendar-in-ruby/
---

## **Aspose.Tasks - Making a Standard Calendar**
To Create a Standard Calendar using **Aspose.Tasks Java for Ruby**, simply invoke **CreateStandardCalendar** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

\# Define Calendar

cal1 = project.getCalendars().add("My Cal")

Rjb::import('com.aspose.tasks.Calendar').makeStandardCalendar(cal1)

\# Save the Project

project.save(data_dir + "CreateStandardCalendar.xml", Rjb::import('com.aspose.tasks.SaveFileFormat').XML)

puts "Created standard calendar, please check the output file."

{{< /highlight >}}
## **Download Running Code**
Download **Making a Standard Calendar (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Calendars/createstandardcalendar.rb)
