---
title: Stop or Resume an Assignment in Php
type: docs
weight: 80
url: /java/stop-or-resume-an-assignment-in-php/
---

## **Aspose.Tasks - Stop or Resume an Assignment**
To Stop or Resume an Assignment using **Aspose.Tasks Java for PHP**, simply invoke **StopAndResumeAssignment** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 # Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

$resource_assignments = $project->getResourceAssignments()->toList();

\# Parse through all the collected resource assignments

$i = 0;

$asn=new Asn();

while ($i < sizeof($resource_assignments)) {

$ra = $resource_assignments -> get($i);

if ((string)$ra -> get($asn -> STOP) == "1/1/2000") {

print "NA".PHP_EOL;

}

else {

print (string)$ra -> get($asn -> STOP);

}

if ((string)$ra -> get($asn -> RESUME) == "1/1/2000"){

print "NA".PHP_EOL;

}

else {

print (string)$ra -> get($asn -> RESUME);

}

$i += 1;

}

{{< /highlight >}}
## **Download Running Code**
Download **Stop or Resume an Assignment (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResourceAssignments/StopAndResumeAssignment.php)
