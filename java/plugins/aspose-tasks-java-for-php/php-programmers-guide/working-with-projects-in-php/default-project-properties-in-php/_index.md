---
title: Default Project Properties in PHP
description: "Learn how to work with default project properties of Microsoft Project (MPP/XML) projects using Aspose.Tasks Java for PHP."
type: docs
weight: 30
url: /java/default-project-properties-in-php/
---

## **Aspose.Tasks - Default Project Properties**
To get Default Project Properties using **Aspose.Tasks Java for PHP**, call **get_default_project_properties** method of **ProjectProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('Sample.xml');
$prj = new Prj();
print "Project Version : " . (string)$project->get($prj->SAVE_VERSION);
print "\nNew Task Default Start: ". (string)$project->get($prj->DEFAULT_START_TIME);
print "\nNew Task Default Type: ". (string)$project->get($prj->DEFAULT_TASK_TYPE);
print "\nResource Default Standard Rate: ". (string)$project->get($prj->DEFAULT_STANDARD_RATE);
print "\nResource Default Overtime Rate: ". (string)$project->get($prj->DEFAULT_OVERTIME_RATE);
print "\nDefault Task EV Method: ". (string)$project->get($prj->DEFAULT_TASK_EV_METHOD);
print "\nDefault Cost Accrual: ". (string)$project->get($prj->DEFAULT_FIXED_COST_ACCRUAL);
{{< /highlight >}}

## **Download Running Code**
Download **Default Project Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/ProjectProperties.php)
