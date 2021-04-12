---
title: Removing Calendar Exceptions in Ruby
description: "Learn how to remove Microsoft Project (MPP/XML) calendar exceptions using Aspose.Tasks Java for Ruby."
type: docs
weight: 40
url: /java/removing-calendar-exceptions-in-ruby/
---

## **Aspose.Tasks - Removing Calendar Exceptions**
To remove Calendar Exceptions using **Aspose.Tasks Java for Ruby**, simply invoke **RemoveCalendarException** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
cal = project.getCalendars().toList().get(0)
if cal.getExceptions().getCount() > 1
    exception = cal.getExceptions().toList().get(0)
    cal.getExceptions().remove(exception)
    puts "Removed calendar exception."
end
{{< /highlight >}}

## **Download Running Code**
Download **Removing Calendar Exceptions (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Calendars/removecalendarexception.rb)
