---
title: General Calendar Properties in Ruby
type: docs
weight: 30
url: /java/general-calendar-properties-in-ruby/
---

## **Aspose.Tasks - General Calendar Properties**
To get Calendar Properties using **Aspose.Tasks Java for Ruby**, simply invoke **CalendarProperties** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 def initialize()

    data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



    # Instantiate project object

    project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

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

      i +=1

    end

end

{{< /highlight >}}
## **Download Running Code**
Download **General Calendar Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Calendars/calendarproperties.rb)
