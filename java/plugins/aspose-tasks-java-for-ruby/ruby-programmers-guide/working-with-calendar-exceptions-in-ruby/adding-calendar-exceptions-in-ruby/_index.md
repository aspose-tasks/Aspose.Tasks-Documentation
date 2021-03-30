---
title: Adding Calendar Exceptions in Ruby
type: docs
weight: 10
url: /java/adding-calendar-exceptions-in-ruby/
---

## **Aspose.Tasks - Adding Calendar Exceptions**
To Add Calendar Exceptions using **Aspose.Tasks Java for Ruby**, simply invoke **AddCalendarException** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

cal = project.getCalendars().toList().get(0)

\# Add an exception

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
