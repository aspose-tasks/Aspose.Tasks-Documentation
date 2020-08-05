---
title: Setting Resource Properties in PHP
type: docs
weight: 50
url: /java/setting-resource-properties-in-php/
---

## **Aspose.Tasks - Setting Resource Properties**
To Set Resource Properties using **Aspose.Tasks Java for PHP**, simply invoke **SetResourceProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 $project = new Project();

\# Resource properties are represented by static class Rsc

$rsc = $project->getResources()->add("Rsc");

\# set resource properties

$rscc=new Rsc();

$bigDecimal=new BigDecimal();

$rsc->set($rscc->STANDARD_RATE, $bigDecimal->valueOf(15));

$rsc->set($rscc->OVERTIME_RATE, $bigDecimal->valueOf(20));

print "Set resource properties".PHP_EOL;

{{< /highlight >}}
## **Download Running Code**
Download **Setting Resource Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResources/SetResourceProperties.php)
- [CodePlex](https://asposetasksjavaphp.codeplex.com/SourceControl/latest#src/aspose/tasks/WorkingWithResources/SetResourceProperties.php)
