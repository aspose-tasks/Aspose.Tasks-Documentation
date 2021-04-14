---
title: Setting Resource Properties in PHP
description: "Learn how to set Microsoft Project (MPP/XML) resource fields using Aspose.Tasks Java for PHP."
type: docs
weight: 50
url: /java/setting-resource-properties-in-php/
---

## **Aspose.Tasks - Setting Resource Properties**
To set resource properties using **Aspose.Tasks Java for PHP**, simply invoke **SetResourceProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
$project = new Project();
$rsc = $project->getResources()->add("Rsc");
$resource = new Rsc();
$bigDecimal = new BigDecimal();
$rsc->set($resource->STANDARD_RATE, $bigDecimal->valueOf(15));
$rsc->set($resource->OVERTIME_RATE, $bigDecimal->valueOf(20));
print "Set resource properties";
{{< /highlight >}}

## **Download Running Code**
Download **Setting Resource Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResources/SetResourceProperties.php)
