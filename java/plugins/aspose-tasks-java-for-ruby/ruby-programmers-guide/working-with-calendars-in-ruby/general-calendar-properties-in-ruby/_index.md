---
title: General Calendar Properties in Ruby
description: "Learn how to read general properties of Microsoft Project (MPP/XML) projects using Aspose.Tasks Java for Ruby."
type: docs
weight: 30
url: /java/general-calendar-properties-in-ruby/
---

## **Aspose.Tasks - General Calendar Properties**
To get Calendar Properties using **Aspose.Tasks Java for Ruby**, simply invoke **CalendarProperties** module. Here you can see example code.

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
calendars = project.getCalendars().toList()
i = 0
while i < calendars.size()
  cal = calendars.get(i)
  if cal.getName() != nil
    puts "Base Calendar : "
    if cal.isBaseCalendar()
      puts "Self"
    else
      cal.getBaseCalendar().getName()
    end
    puts "UID : " + cal.getUid().to_s
    puts "Name : " + cal.getName().to_s
  end
  i += 1
end
{{< /highlight >}}

## **Download Running Code**
Download **General Calendar Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Calendars/calendarproperties.rb)
