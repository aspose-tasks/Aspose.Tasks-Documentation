---
title: Adding Calendar Exceptions in PHP
description: "Learn how to add Microsoft Project (MPP/XML) calendar exceptions using Aspose.Tasks Java for PHP."
type: docs
weight: 10
url: /java/adding-calendar-exceptions-in-php/
---

## **Aspose.Tasks - Adding Calendar Exceptions**
To add Calendar Exceptions using **Aspose.Tasks Java for PHP**, simply invoke **AddCalendarException** module. Here you can see example code.

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$cal = $project->getCalendars()->toList()->get(0);
$calException = new CalendarException();
$calendar = new Calendar();
$calObject = $calendar->getInstance();
$calObject->set(2009, 1, 1, 0, 0, 0);
$calException->setFromDate($calObject->getTime());
$calObject->set(2009, 1, 3, 0, 0, 0);
$calException->setToDate($calObject->getTime());
$cal->getExceptions()->add($calException);
print "Added calendar exception.";
{{< /highlight >}}

You can download the working code example from [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithCalendarExceptions/AddCalendarException.php).
