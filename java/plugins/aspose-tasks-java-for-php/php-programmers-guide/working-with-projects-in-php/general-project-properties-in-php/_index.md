---
title: General Project Properties in PHP
description: "Learn how to manage Microsoft Project (MPP/XML) general properties using Aspose.Tasks Java for PHP."
type: docs
weight: 60
url: /java/general-project-properties-in-php/
---

## **Aspose.Tasks - General Project Properties**
To get General Project Properties using **Aspose.Tasks Java for PHP**, call **get_general_project_properties** method of **ProjectProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('Sample.xml');
$prj = new Prj();
if ($project -> get($prj->SCHEDULE_FROM_START) -> getValue())
{
    print "Project Start Date : " . (string)$project->get($prj->START_DATE);
}
else
{
    print "Project Finish Date : " . (string)$project -> get($prj -> FINISH_DATE);
}
$strSchedule = $project->get($prj->SCHEDULE_FROM_START)->getValue() ? "Project Start Date" : "Project Finish Date";
print "\nProject Schedule From : " . (string)$strSchedule;
print "\nCurrent Date : " . (string)$project->get($prj->CURRENT_DATE);
print "\nStatus Date : " . (string)$project->get($prj->STATUS_DATE);
print "\nCalendar : " . (string)$project->get($prj->CALENDAR);
{{< /highlight >}}

## **Download Running Code**
Download **General Project Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/ProjectProperties.php)
