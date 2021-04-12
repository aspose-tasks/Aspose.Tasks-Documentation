---
title: Defining Weekdays for Calendar in Ruby
description: "Learn how to define calendar weekdays for Microsoft Project (MPP/XML) projects using Aspose.Tasks Java for Ruby."
keywords: "Defining Weekdays for Exceptions, work with weekdays exceptions, weekday calendar exception, Aspose.Tasks, Java, Ruby"
type: docs
weight: 20
url: /java/defining-weekdays-for-calendar-in-ruby/
---

## **Aspose.Tasks - Defining Weekdays for Calendar**
To Define Weekdays for Calendar using **Aspose.Tasks Java for Ruby**, simply invoke **DefineWeekdaysForCalendar** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new
cal = project.getCalendars().add("Calendar1")
weekday = Rjb::import('com.aspose.tasks.WeekDay')
dayType = Rjb::import('com.aspose.tasks.DayType')
cal.getWeekDays().add(weekday.createDefaultWorkingDay(dayType.Monday))
cal.getWeekDays().add(weekday.createDefaultWorkingDay(dayType.Tuesday))
cal.getWeekDays().add(weekday.createDefaultWorkingDay(dayType.Wednesday))
cal.getWeekDays().add(weekday.createDefaultWorkingDay(dayType.Thursday))
cal.getWeekDays().add(Rjb::import('com.aspose.tasks.WeekDay').new(dayType.Saturday))
cal.getWeekDays().add(Rjb::import('com.aspose.tasks.WeekDay').new(dayType.Sunday))
myWeekDay = Rjb::import('com.aspose.tasks.WeekDay').new(dayType.Friday)
time1 = Rjb::import('com.aspose.tasks.WorkingTime').new
calTime = Rjb::import('java.util.Calendar').getInstance()
calTime.set(1,1,1,9,0,0)
date = calTime.getTime()
time1.setFromTime(date)
calTime.set(1,1,1,12,0,0)
date = calTime.getTime()
time1.setToTime(date)
time2 = Rjb::import('com.aspose.tasks.WorkingTime').new
calTime.set(1,1,1,13,0,0)
date = calTime.getTime()
time2.setFromTime(date)
calTime.set(1,1,1,16,0,0)
date = calTime.getTime()
time2.setToTime(date)
myWeekDay.getWorkingTimes().add(time1)
myWeekDay.getWorkingTimes().add(time2)
myWeekDay.setDayWorking(true)
cal.getWeekDays().add(myWeekDay)
project.save("CalendarWeekdays.xml", Rjb::import('com.aspose.tasks.SaveFileFormat').XML)
puts "Defined weekdays for calendar, please check the output file."
{{< /highlight >}}

## **Download Running Code**
Download **Defining Weekdays for Calendar (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Calendars/defineweekdaysforcalendar.rb)
