---
title: Retrieving Calendar Exceptions in Ruby
type: docs
weight: 50
url: /java/retrieving-calendar-exceptions-in-ruby/
---

## **Aspose.Tasks - Retrieving Calendar Exceptions**
To get Calendar Exceptions using **Aspose.Tasks Java for Ruby**, simply invoke **GetCalendarExceptions** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

calendars = project.getCalendars().toList()

i = 0

while i < calendars.size()

  cal = calendars.get(i)

  calexc = cal.getExceptions().getCount()

  if calexc > 0

    puts "From: " + calexc.getFromDate().toString()

    puts "To: " + calexc.getToDate().toString()

  end

  i +=1

end

{{< /highlight >}}
## **Download Running Code**
Download **Retrieving Calendar Exceptions (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Calendars/getcalendarexceptions.rb)
