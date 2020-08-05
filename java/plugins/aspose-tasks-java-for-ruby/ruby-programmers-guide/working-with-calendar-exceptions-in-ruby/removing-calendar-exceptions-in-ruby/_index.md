---
title: Removing Calendar Exceptions in Ruby
type: docs
weight: 40
url: /java/removing-calendar-exceptions-in-ruby/
---

## **Aspose.Tasks - Removing Calendar Exceptions**
To Remove Calendar Exceptions using **Aspose.Tasks Java for Ruby**, simply invoke **RemoveCalendarException** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

\# Remove an exception

cal = project.getCalendars().toList().get(0)

if cal.getExceptions().getCount() > 1

    exc = cal.getExceptions().toList().get(0)

    cal.getExceptions().remove(exc)

    puts "Removed calendar exception."

end

{{< /highlight >}}
## **Download Running Code**
Download **Removing Calendar Exceptions (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Calendars/removecalendarexception.rb)
