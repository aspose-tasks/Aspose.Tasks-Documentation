---
title: Removing Calendar Exceptions in PHP
type: docs
weight: 40
url: /java/removing-calendar-exceptions-in-php/
---

## **Aspose.Tasks - Removing Calendar Exceptions**
To Remove Calendar Exceptions using **Aspose.Tasks Java for PHP**, simply invoke **RemoveCalendarException** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 # Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

\# Remove an exception

$cal = $project->getCalendars()->toList()->get(0);

if((int)(string)($cal->getExceptions()->getCount()) > 1) {

$exc = $cal -> getExceptions() -> toList() -> get(0);

$cal -> getExceptions() -> remove($exc);

print "Removed calendar exception.".PHP_EOL;

}


{{< /highlight >}}
## **Download Running Code**
Download **Removing Calendar Exceptions (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithCalendarExceptions/RemoveCalendarException.php)
