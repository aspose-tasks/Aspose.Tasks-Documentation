---
title: General Project Properties in PHP
type: docs
weight: 60
url: /java/general-project-properties-in-php/
---

## **Aspose.Tasks - General Project Properties**
To get General Project Properties using **Aspose.Tasks Java for PHP**, call **get_general_project_properties** method of **ProjectProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 public static function get_general_project_properties($dataDir=null)

{

\# Instantiate project object

$project = new Project($dataDir . 'Sample.xml');

$prj = new Prj();

if ($project -> get($prj->SCHEDULE_FROM_START) -> getValue()) {

print "Project Start Date : " . (string)$project->get($prj->START_DATE).PHP_EOL;

}

else{

print "Project Finish Date : " . (string)$project -> get($prj -> FINISH_DATE).PHP_EOL;

}

$strSchdl = $project->get($prj->SCHEDULE_FROM_START)->getValue() ? "Project Start Date" : "Project Finish Date";

print "Project Schedule From : " . (string)$strSchdl.PHP_EOL;

print "Current Date : " . (string)$project->get($prj->CURRENT_DATE).PHP_EOL;

print "Status Date : " . (string)$project->get($prj->STATUS_DATE).PHP_EOL;

print "Calendar : " . (string)$project->get($prj->CALENDAR).PHP_EOL.PHP_EOL;

}

{{< /highlight >}}
## **Download Running Code**
Download **General Project Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/ProjectProperties.php)
