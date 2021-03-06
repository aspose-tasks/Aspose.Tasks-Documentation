---
title: Determining Project Version in PHP
description: "Learn how to check Microsoft Project (MPP/XML) version using Aspose.Tasks Java for PHP."
type: docs
weight: 40
url: /java/determining-project-version-in-php/
---

## **Aspose.Tasks - Determining Project Version**
To Determine Project Version using **Aspose.Tasks Java for PHP**, simply invoke **ProjectVersion** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project('Sample.xml');
$prj = new Prj();
print "Project Version : " . (string)$project->get($prj->SAVE_VERSION);
print "\nLast Saved : " . (string)$project->get($prj->LAST_SAVED);
{{< /highlight >}}

## **Download Running Code**
Download **Determining Project Version (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithProjects/ProjectVersion.php)
