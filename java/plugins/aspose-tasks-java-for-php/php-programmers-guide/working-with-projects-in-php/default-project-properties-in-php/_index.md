---
title: Default Project Properties in PHP
type: docs
weight: 30
url: /java/default-project-properties-in-php/
---

## **Aspose.Tasks - Default Project Properties**
To get Default Project Properties using **Aspose.Tasks Java for PHP**, call **get_default_project_properties** method of **ProjectProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
public static function get_default_project_properties()
{
    $project = new Project('Sample.xml');
    $prj = new Prj();
    print "Project Version : " . (string)$project->get($prj->SAVE_VERSION).PHP_EOL;
    print "New Task Default Start: ". (string)$project->get($prj->DEFAULT_START_TIME).PHP_EOL;
    print "New Task Default Type: ". (string)$project->get($prj->DEFAULT_TASK_TYPE).PHP_EOL;
    print "Resource Default Standard Rate: ". (string)$project->get($prj->DEFAULT_STANDARD_RATE).PHP_EOL;
    print "Resource Default Overtime Rate: ". (string)$project->get($prj->DEFAULT_OVERTIME_RATE).PHP_EOL;
    print "Default Task EV Method: ". (string)$project->get($prj->DEFAULT_TASK_EV_METHOD).PHP_EOL;
    print "Default Cost Accrual: ". (string)$project->get($prj->DEFAULT_FIXED_COST_ACCRUAL).PHP_EOL;
}
{{< /highlight >}}

## **Download Running Code**
Download **Default Project Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/ProjectProperties.php)
