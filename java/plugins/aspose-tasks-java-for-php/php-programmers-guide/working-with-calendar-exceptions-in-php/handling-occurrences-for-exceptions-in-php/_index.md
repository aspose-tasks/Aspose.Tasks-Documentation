---
title: Handling Occurrences for Exceptions in PHP
type: docs
weight: 30
url: /java/handling-occurrences-for-exceptions-in-php/
---

## **Aspose.Tasks - Handling Occurrences for Exceptions**
To Handle Occurrences for Exceptions using **Aspose.Tasks Java for PHP**, simply invoke **HandleOccurrencesForExceptions** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 $except = new CalendarException();

$except->setEnteredByOccurrences(true);

$except->setOccurrences(5);

$calendarExceptionType=new CalendarExceptionType();

$except->setType($calendarExceptionType->YearlyByDay);

print "Set Occurences for exeptions".PHP_EOL;

{{< /highlight >}}
## **Download Running Code**
Download **Handling Occurrences for Exceptions (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithCalendarExceptions/HandleOccurrencesForExceptions.php)
