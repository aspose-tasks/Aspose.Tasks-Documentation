---
title: Adding Calendar Exceptions in Ruby
description: "Learn how to add Microsoft Project (MPP/XML) calendar exceptions using Aspose.Tasks Java for Ruby."
type: docs
weight: 10
url: /java/adding-calendar-exceptions-in-ruby/
---

## **Aspose.Tasks - Adding Calendar Exceptions**
To add Calendar Exceptions using **Aspose.Tasks Java for Ruby**, simply invoke **AddCalendarException** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
cal = project.getCalendars().toList().get(0)
calException = Rjb::import('com.aspose.tasks.CalendarException').new
calObject = Rjb::import('java.util.Calendar').getInstance()
calObject.set(2009, 1, 1, 0, 0, 0)
calException.setFromDate(calObject.getTime())
calObject.set(2009, 1, 3, 0, 0, 0)
calException.setToDate(calObject.getTime())
cal.getExceptions().add(calException)
puts "Added calendar exception."
{{< /highlight >}}

## **Download Running Code**
Download **Adding Calendar Exceptions (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Calendars/addcalendarexception.rb)
