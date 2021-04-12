---
title: Retrieving Calendar Exceptions in Ruby
description: "This article explains how to retrieve calendar exception data using Aspose.Tasks Java for Ruby."
type: docs
weight: 50
url: /java/retrieving-calendar-exceptions-in-ruby/
---

## **Aspose.Tasks - Retrieving Calendar Exceptions**
To get Calendar Exceptions using **Aspose.Tasks Java for Ruby**, simply invoke **GetCalendarExceptions** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
calendars = project.getCalendars().toList()
i = 0
while i < calendars.size()
  cal = calendars.get(i)
  calException = cal.getExceptions().getCount()
  if calException > 0
    puts "From: " + calException.getFromDate().toString()
    puts "To: " + calException.getToDate().toString()
  end
  i += 1
end
{{< /highlight >}}

## **Download Running Code**
Download **Retrieving Calendar Exceptions (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Calendars/getcalendarexceptions.rb)
