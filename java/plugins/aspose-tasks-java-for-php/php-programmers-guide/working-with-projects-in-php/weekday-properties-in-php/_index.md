---
title: Weekday Properties in PHP
description: "Learn how to work with Microsoft Project (MPP/XML) weekday properties using Aspose.Tasks Java for PHP."
type: docs
weight: 160
url: /java/weekday-properties-in-php/
---

## **Aspose.Tasks - Reading Weekday Properties**
To read weekday properties using **Aspose.Tasks Java for PHP**, call **get_weekday_properties** method of **WeekdayProperties** module. Here you can see example code.

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$prj = new Prj();
print "Week Start Date : " . (string)$project->get($prj->WEEK_START_DAY);
print "\nDays Per Month : " . (string)$project->get($prj->DAYS_PER_MONTH);
print "\nMinutes Per Day : " . (string)$project->get($prj->MINUTES_PER_DAY);
print "\nMinutes Per Week : " . (string)$project->get($prj->MINUTES_PER_WEEK);
{{< /highlight >}}

## **Aspose.Tasks - Writing Weekday Properties**
To write weekday properties using **Aspose.Tasks Java for PHP**, call **set_weekday_properties** method of **WeekdayProperties** module. Here you can see example code.

{{< highlight php >}}
$project = new Project();
$prj = new Prj();
$dayType = new DayType();
$project->set($prj->WEEK_START_DAY, $dayType->Monday);
$project->set($prj->DAYS_PER_MONTH, 24);
$project->set($prj->MINUTES_PER_DAY, 540);
$project->set($prj->MINUTES_PER_WEEK, 3240);
$saveFileFormat = new SaveFileFormat();
$project->save("weekday_properties.xml", $saveFileFormat->XML);
print "Set weekday properties, please check the output file.";
{{< /highlight >}}

## **Download Running Code**
Download **Weekday Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/WeekdayProperties.php)
