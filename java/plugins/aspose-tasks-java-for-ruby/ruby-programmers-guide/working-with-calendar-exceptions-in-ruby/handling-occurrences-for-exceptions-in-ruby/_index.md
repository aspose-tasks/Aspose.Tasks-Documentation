---
title: Handling Occurrences for Exceptions in Ruby
type: docs
weight: 30
url: /java/handling-occurrences-for-exceptions-in-ruby/
---

## **Aspose.Tasks - Handling Occurrences for Exceptions**
To Handle Occurrences for Exceptions using **Aspose.Tasks Java for Ruby**, simply invoke **HandleOccurrencesForExceptions** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 except = Rjb::import('com.aspose.tasks.CalendarException').new

except.setEnteredByOccurrences(true)

except.setOccurrences(5)

except.setType(Rjb::import('com.aspose.tasks.CalendarExceptionType').YearlyByDay)

puts "Set Occurrences for exceptions"

{{< /highlight >}}
## **Download Running Code**
Download **Handling Occurrences for Exceptions (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Calendars/handleoccurrencesforexceptions.rb)
