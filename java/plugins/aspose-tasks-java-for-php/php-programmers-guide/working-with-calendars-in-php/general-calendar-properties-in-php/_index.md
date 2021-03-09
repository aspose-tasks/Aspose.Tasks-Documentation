---
title: General Calendar Properties in PHP
type: docs
weight: 30
url: /java/general-calendar-properties-in-php/
---

## **Aspose.Tasks - General Calendar Properties**
To get Calendar Properties using **Aspose.Tasks Java for PHP**, simply invoke **CalendarProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 # Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

$calendars = $project->getCalendars()->toList();

$i = 0;

while ($i < sizeof($calendars)) {

$cal = $calendars->get($i);

if ($cal->getName() != null) {

print "Base Calendar : ";

if ($cal -> isBaseCalendar()) {

print "Self";

} else {

$cal->getBaseCalendar()->getName();

}

print "UID : " . (string)$cal->getUid();

print "Name : " . (string)$cal->getName();

}

$i += 1;

}

{{< /highlight >}}
## **Download Running Code**
Download **General Calendar Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithCalendars/CalendarProperties.php)
