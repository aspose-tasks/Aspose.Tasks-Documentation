---
title: Making a Standard Calendar in Ruby
description: "Learn how to create Microsoft Project (MPP/XML) standard calendars using Aspose.Tasks Java for Ruby."
type: docs
weight: 40
url: /java/making-a-standard-calendar-in-ruby/
---

## **Aspose.Tasks - Making a Standard Calendar**
To create a Standard Calendar using **Aspose.Tasks Java for Ruby**, simply invoke **CreateStandardCalendar** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
cal1 = project.getCalendars().add("My Cal")
Rjb::import('com.aspose.tasks.Calendar').makeStandardCalendar(cal1)
project.save("CreateStandardCalendar.xml", Rjb::import('com.aspose.tasks.SaveFileFormat').XML)
puts "Created standard calendar, please check the output file."
{{< /highlight >}}

## **Download Running Code**
Download **Making a Standard Calendar (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Calendars/createstandardcalendar.rb)
