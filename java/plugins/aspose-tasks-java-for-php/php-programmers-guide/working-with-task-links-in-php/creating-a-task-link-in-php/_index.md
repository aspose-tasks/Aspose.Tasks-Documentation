---
title: Creating a Task Link in PHP
description: "Learn how to create task links in Microsoft Project (MPP/XML) files using Aspose.Tasks Java for PHP."
type: docs
weight: 10
url: /java/creating-a-task-link-in-php/
---

## **Aspose.Tasks - Creating a Task Link**
To create a Task Link using **Aspose.Tasks Java for PHP**, simply invoke **CreateTaskLink** module. Here you can see example code.

{{< highlight php >}}
$project = new Project();
$pred = $project->getRootTask()->getChildren()->add("Task 1");
$succ = $project->getRootTask()->getChildren()->add("Task 2");
$link = $project->getTaskLinks()->add($pred, $succ);
print "Created task link.".PHP_EOL;
{{< /highlight >}}

## **Download Running Code**
Download **Creating a Task Link (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTaskLinks/CreateTaskLink.php)
