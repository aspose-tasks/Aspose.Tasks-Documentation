---
title: Defining Link Type in PHP
description: "Learn how to change Microsoft Project (MPP/XML) task link types using Aspose.Tasks Java for PHP."
type: docs
weight: 20
url: /java/defining-link-type-in-php/
---

## **Aspose.Tasks - Defining Link Type**
To Define Link Type using **Aspose.Tasks Java for PHP**, simply invoke **DefineLinkType** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project();
$pred = $project->getRootTask()->getChildren()->add("Task 1");
$succ = $project->getRootTask()->getChildren()->add("Task 2");
$link = $project->getTaskLinks()->add($pred, $succ);
$taskLinkType = new TaskLinkType();
$link->setLinkType($taskLinkType->StartToStart);
print "Defined task link type.";
{{< /highlight >}}

## **Download Running Code**
Download **Defining Link Type (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithTaskLinks/DefineLinkType.php)
