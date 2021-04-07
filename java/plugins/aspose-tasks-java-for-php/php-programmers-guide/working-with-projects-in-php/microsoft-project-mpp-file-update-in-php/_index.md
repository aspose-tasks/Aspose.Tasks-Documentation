---
title: Microsoft Project MPP File Update in PHP
description: "Learn how to update Microsoft Project (MPP/XML) project files using Aspose.Tasks Java for PHP."
type: docs
weight: 80
url: /java/microsoft-project-mpp-file-update-in-php/
---

## **Aspose.Tasks - Update Project File**
To Update Project File using **Aspose.Tasks Java for PHP**, simply invoke **UpdateProjectFile** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
    $project = new Project('test_tasks.mpp');
    $task = $project->getRootTask()->getChildren()->add("Task1");
    $cal = new Calendar();
    $cal = $cal->getInstance();
    $cal->set(2015, 7, 1, 8, 0,0);
    $tsk = new Tsk();
    $task->set($tsk->START, $cal->getTime());
    $cal->set(2015, 7, 1, 17, 0, 0);
    $task->set($tsk->FINISH , $cal->getTime());
    $saveFileFormat = new SaveFileFormat();
    $project->save("AfterLinking.mpp", $saveFileFormat->MPP);
    print "Project file updated, please check the output file.".PHP_EOL;
{{< /highlight >}}

## **Download Running Code**
Download **Update Project File (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/UpdateProjectFile.php)
