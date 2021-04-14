---
title: Making a Standard Calendar in PHP
description: "Learn how to create Microsoft Project (MPP/XML) standard calendars using Aspose.Tasks Java for PHP."
type: docs
weight: 40
url: /java/making-a-standard-calendar-in-php/
---

## **Aspose.Tasks - Making a Standard Calendar**
To create a Standard Calendar using **Aspose.Tasks Java for PHP**, simply invoke **CreateStandardCalendar** module. Here you can see example code.

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$cal1 = $project->getCalendars()->add("My Cal");
$calendar = new Calendar();
$calendar->makeStandardCalendar($cal1);
$saveFileFormat = new SaveFileFormat();
$project->save("CreateStandardCalendar.xml", $saveFileFormat->XML);
print "Created standard calendar, please check the output file.";
{{< /highlight >}}

## **Download Running Code**
Download **Making a Standard Calendar (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithCalendars/CreateStandardCalendar.php)
