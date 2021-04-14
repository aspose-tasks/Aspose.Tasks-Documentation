---
title: Setting Attributes for New Tasks in PHP
description: "Learn how to set Microsoft Project (MPP/XML) project attributes for newly created tasks using Aspose.Tasks Java for PHP."
type: docs
weight: 140
url: /java/setting-attributes-for-new-tasks-in-php/
---

## **Aspose.Tasks - Setting Attributes for New Tasks**
To set attributes for new tasks using **Aspose.Tasks Java for PHP**, simply invoke **SetAttributesForNewTasks** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$prj = new Prj();
$taskStartDateType = new TaskStartDateType();
$project->set($prj->NEW_TASK_START_DATE, $taskStartDateType->CurrentDate);
$saveFileFormat = new SaveFileFormat();
$project->save("set_attributes_for_new_tasks.xml", $saveFileFormat->XML);
print "Set attributes for new tasks, please check the output file.";
{{< /highlight >}}

## **Download Running Code**
Download **Setting Attributes for New Tasks (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/SetAttributesForNewTasks.php)
