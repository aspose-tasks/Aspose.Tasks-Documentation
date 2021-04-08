---
title: Creating a Calendar in Ruby
description: "This article explains how to create calendar in Microsoft Project (MPP/XML) files using Aspose.Tasks Java for Ruby."
type: docs
weight: 10
url: /java/creating-a-calendar-in-ruby/
---

## **Aspose.Tasks - Creating a Calendar**
To create a Calendar using **Aspose.Tasks Java for Ruby**, simply invoke **CreateCalendar** module. Here you can see example code.
{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
cal1 = project.getCalendars().add("no info")
cal2 = project.getCalendars().add("no name")
cal3 = project.getCalendars().add("cal3")
project.save("CreateCalendar.xml", Rjb::import('com.aspose.tasks.SaveFileFormat').XML)
puts "Created calendar, please check the output file."
{{< /highlight >}}

## **Download Running Code**
Download **Creating a Calendar (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Calendars/createcalendar.rb)
