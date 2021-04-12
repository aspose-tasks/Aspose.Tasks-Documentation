---
title: Resource Cost in PHP
description: "Learn how to work with Microsoft Project (MPP/XML) resource costs using Aspose.Tasks Java for PHP."
type: docs
weight: 40
url: /java/resource-cost-in-php/
---

## **Aspose.Tasks - Resource Cost**
To get Resource Cost using **Aspose.Tasks Java for PHP**, simply invoke **ResourceCost** module. Here you can see example code.

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$resources = $project->getResources()->toList();
$rsc = new Rsc();
$i = 0;
while ($i < sizeof($resources))
{
    $resource = $resources -> get($i);
    if ($resource -> get($rsc -> NAME) != null) {
        print "Cost: " . (string)$resource -> get($rsc -> COST).PHP_EOL;
        print "ACWP: " . (string)$resource -> get($rsc -> ACWP).PHP_EOL;
        print "BCWS: " . (string)$resource -> get($rsc -> BCWS).PHP_EOL;
        print "BCWP: " . (string)$resource -> get($rsc -> BCWP).PHP_EOL;
        print "---------------------------------------------".PHP_EOL;
    }
    $i += 1;
}
{{< /highlight >}}

## **Download Running Code**
Download **Resource Cost (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResources/ResourceCost.php)
