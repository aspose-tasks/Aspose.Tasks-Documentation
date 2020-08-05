---
title: Making a Standard Calendar in PHP
type: docs
weight: 40
url: /java/making-a-standard-calendar-in-php/
---

## **Aspose.Tasks - Making a Standard Calendar**
To Create a Standard Calendar using **Aspose.Tasks Java for PHP**, simply invoke **CreateStandardCalendar** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 # Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

\# Define Calendar

$cal1 = $project->getCalendars()->add("My Cal");

$calendar=new Calendar();

$calendar->makeStandardCalendar($cal1);

\# Save the Project

$saveFileFormat=new SaveFileFormat();

$project->save($dataDir . "CreateStandardCalendar.xml", $saveFileFormat->XML);

print "Created standard calendar, please check the output file.".PHP_EOL;

{{< /highlight >}}
## **Download Running Code**
Download **Making a Standard Calendar (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithCalendars/CreateStandardCalendar.php)
- [CodePlex](https://asposetasksjavaphp.codeplex.com/SourceControl/latest#src/aspose/tasks/WorkingWithCalendars/CreateStandardCalendar.php)
