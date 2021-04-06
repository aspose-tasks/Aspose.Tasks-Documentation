---
title: Creating a Calendar in PHP
type: docs
weight: 10
url: /java/creating-a-calendar-in-php/
---

## **Aspose.Tasks - Creating a Calendar**
To create a Calendar using **Aspose.Tasks Java for PHP**, simply invoke **CreateCalendar** module. Here you can see example code.

{{< highlight php >}}
$project = new Project($dataDir . 'test_tasks.mpp');
$cal1 = $project->getCalendars()->add("no info");
$cal2 = $project->getCalendars()->add("no name");
$cal3 = $project->getCalendars()->add("cal3");
$saveFileFormat=new SaveFileFormat();
$project->save($dataDir . "CreateCalendar.xml", $saveFileFormat->XML);
print "Created calendar, please check the output file.".PHP_EOL;
{{< /highlight >}}

## **Download Running Code**
Download **Creating a Calendar (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithCalendars/CreateCalendar.php)
