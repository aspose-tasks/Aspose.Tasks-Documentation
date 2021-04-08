---
title: Removing Calendar Exceptions in PHP
description: "Learn how to remove Microsoft Project (MPP/XML) calendar exceptions using Aspose.Tasks Java for PHP."
type: docs
weight: 40
url: /java/removing-calendar-exceptions-in-php/
---

## **Aspose.Tasks - Removing Calendar Exceptions**
To remove Calendar Exceptions using **Aspose.Tasks Java for PHP**, simply invoke **RemoveCalendarException** module. Here you can see example code.

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$cal = $project->getCalendars()->toList()->get(0);
if((int)(string)($cal->getExceptions()->getCount()) > 1) {
    $exception = $cal -> getExceptions() -> toList() -> get(0);
    $cal -> getExceptions() -> remove($exception);
    print "Removed calendar exception.".PHP_EOL;
}
{{< /highlight >}}

## **Download Running Code**
Download **Removing Calendar Exceptions (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithCalendarExceptions/RemoveCalendarException.php)
