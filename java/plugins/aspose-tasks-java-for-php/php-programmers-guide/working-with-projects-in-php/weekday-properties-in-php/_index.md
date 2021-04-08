---
title: Weekday Properties in PHP
type: docs
weight: 160
url: /java/weekday-properties-in-php/
---

## **Aspose.Tasks - Reading Weekday Properties**
To read Weekday Properties using **Aspose.Tasks Java for PHP**, call **get_weekday_properties** method of **WeekdayProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$prj = new Prj();
print "Week Start Date : " . (string)$project->get($prj->WEEK_START_DAY).PHP_EOL;
print "Days Per Month : " . (string)$project->get($prj->DAYS_PER_MONTH).PHP_EOL;
print "Minutes Per Day : " . (string)$project->get($prj->MINUTES_PER_DAY).PHP_EOL;
print "Minutes Per Week : " . (string)$project->get($prj->MINUTES_PER_WEEK).PHP_EOL;
{{< /highlight >}}

## **Aspose.Tasks - Writing Weekday Properties**
To write Weekday Properties using **Aspose.Tasks Java for PHP**, call **set_weekday_properties** method of **WeekdayProperties** module. Here you can see example code.

**PHP Code**

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
print "Set weekday properties, please check the output file.".PHP_EOL;
{{< /highlight >}}

## **Download Running Code**
Download **Weekday Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/WeekdayProperties.php)
