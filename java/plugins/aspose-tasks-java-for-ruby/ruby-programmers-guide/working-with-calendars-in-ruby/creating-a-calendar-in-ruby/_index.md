---
title: Creating a Calendar in Ruby
type: docs
weight: 10
url: /java/creating-a-calendar-in-ruby/
---

## **Aspose.Tasks - Creating a Calendar**
To Create a Calendar using **Aspose.Tasks Java for Ruby**, simply invoke **CreateCalendar** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

\# Define Calendar

cal1 = project.getCalendars().add("no info")

cal2 = project.getCalendars().add("no name")

cal3 = project.getCalendars().add("cal3")

\# Save the Project

project.save(data_dir + "CreateCalendar.xml", Rjb::import('com.aspose.tasks.SaveFileFormat').XML)

puts "Created calendar, please check the output file."

{{< /highlight >}}
## **Download Running Code**
Download **Creating a Calendar (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Calendars/createcalendar.rb)
