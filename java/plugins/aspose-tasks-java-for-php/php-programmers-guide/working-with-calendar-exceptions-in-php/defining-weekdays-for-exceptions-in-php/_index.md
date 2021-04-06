---
title: Defining Weekdays for Exceptions in PHP
type: docs
weight: 20
url: /java/defining-weekdays-for-exceptions-in-php/
---

## **Aspose.Tasks - Defining Weekdays for Exceptions**
To Define Weekdays for Exceptions using **Aspose.Tasks Java for PHP**, simply invoke **DefineWeekdaysForExceptions** module. Here you can see example code.

{{< highlight php >}}
$project = new Project($dataDir . 'test_tasks.mpp');
$cal = $project->getCalendars()->add("Calendar1");
$except = new CalendarException();
$except->setEnteredByOccurrences(false);
$calendar=new Calendar();
$calendarExceptionType=new CalendarExceptionType();
$cal_object = $calendar->getInstance();
$cal_object->set(2009, 12, 24, 0, 0, 0);
$except->setFromDate($cal_object->getTime());
$cal_object->set(2009, 12, 31, 23, 59, 0);
$except->setToDate($cal_object->getTime());
$except->setType($calendarExceptionType->Daily);
$except->setDayWorking(false);
$cal->getExceptions()->add($except);
print "Defined weekdays for exceptions.".PHP_EOL;
{{< /highlight >}}

## **Download Running Code**
Download **Defining Weekdays for Exceptions (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithCalendarExceptions/DefineWeekdaysForExceptions.php)
