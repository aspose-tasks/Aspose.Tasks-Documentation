---
title: Defining Weekdays for Exceptions in Ruby
type: docs
weight: 20
url: /java/defining-weekdays-for-exceptions-in-ruby/
---

## **Aspose.Tasks - Defining Weekdays for Exceptions**
To Define Weekdays for Exceptions using **Aspose.Tasks Java for Ruby**, simply invoke **DefineWeekdaysForExceptions** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
cal = project.getCalendars().add("Calendar1")
except = Rjb::import('com.aspose.tasks.CalendarException').new
except.setEnteredByOccurrences(false)
cal_object = Rjb::import('java.util.Calendar').getInstance()
cal_object.set(2009, 12, 24, 0, 0, 0)
except.setFromDate(cal_object.getTime())
cal_object.set(2009, 12, 31, 23, 59, 0)
except.setToDate(cal_object.getTime())
except.setType(Rjb::import('com.aspose.tasks.CalendarExceptionType').Daily)
except.setDayWorking(false)
cal.getExceptions().add(except)
puts "Defined weekdays for exceptions."
{{< /highlight >}}

## **Download Running Code**
Download **Defining Weekdays for Exceptions (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Calendars/defineweekdaysforexceptions.rb)
