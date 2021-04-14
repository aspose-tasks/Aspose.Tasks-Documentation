---
title: Stop or Resume an Assignment in PHP
description: "Learn how to stop or resume Microsoft Project (MPP/XML) resource assignments using Aspose.Tasks Java for PHP."
type: docs
weight: 80
url: /java/stop-or-resume-an-assignment-in-php/
---

## **Aspose.Tasks - Stop or Resume an Assignment**
To Stop or Resume an Assignment using **Aspose.Tasks Java for PHP**, simply invoke **StopAndResumeAssignment** module. Here you can see example code.

{{< highlight php >}}
$project = new Project('test_tasks.mpp');
$resource_assignments = $project->getResourceAssignments()->toList();
$i = 0;
$asn = new Asn();
while ($i < sizeof($resource_assignments))
{
    $assignment = $resource_assignments -> get($i);
    if ((string)$assignment -> get($asn -> STOP) == "1/1/2000")
    {
        print "NA";
    }
    else
    {
        print (string)$assignment -> get($asn -> STOP);
    }

    if ((string)$assignment -> get($asn -> RESUME) == "1/1/2000")
    {
        print "NA";
    }
    else
    {
        print (string)$assignment -> get($asn -> RESUME);
    }
    $i += 1;
}
{{< /highlight >}}

## **Download Running Code**
Download **Stop or Resume an Assignment (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResourceAssignments/StopAndResumeAssignment.php)
