---
title: Dealing Variances in Php
type: docs
weight: 40
url: /java/dealing-variances-in-php/
---

## **Aspose.Tasks - Dealing Variances**
To see resource assignment variance using **Aspose.Tasks Java for PHP**, simply invoke **AssignmentVariance** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 # Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

$resource_assignments = $project->getResourceAssignments()->toList();

\# Parse through all the collected resource assignments

$i = 0;

$asn=new Asn();

while ($i < sizeof($resource_assignments)){

$ra = $resource_assignments->get($i);

print "Work Variance: " . (string)$ra -> get($asn -> WORK_VARIANCE).PHP_EOL;

print "Cost Variance: " . (string)$ra -> get($asn -> COST_VARIANCE).PHP_EOL;

print "Start Variance: " . (string)$ra -> get($asn -> START_VARIANCE).PHP_EOL;

print "Finish Variance: " . (string)$ra -> get($asn -> FINISH_VARIANCE).PHP_EOL;

print "--------------------------------------------------------".PHP_EOL;

$i += 1;

}

{{< /highlight >}}
## **Download Running Code**
Download **Dealing Variances (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResourceAssignments/AssignmentVariance.php)
- [CodePlex](https://asposetasksjavaphp.codeplex.com/SourceControl/latest#src/aspose/tasks/WorkingWithResourceAssignments/AssignmentVariance.php)
