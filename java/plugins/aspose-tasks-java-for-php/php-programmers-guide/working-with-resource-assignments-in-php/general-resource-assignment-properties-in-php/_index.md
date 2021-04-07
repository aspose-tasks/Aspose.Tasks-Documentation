---
title: General Resource Assignment Properties in PHP
description: "Learn how to read or edit properties of Microsoft Project (MPP/XML) resource assignments using Aspose.Tasks Java for PHP."
type: docs
weight: 50
url: /java/general-resource-assignment-properties-in-php/
---

## **Aspose.Tasks - Getting General Resource Assignment Properties**
To get General Resource Assignment Properties using **Aspose.Tasks Java for PHP**, call **get_resource_assignments** method of **ResourceAssignmentProperties** module. Here you can see example code.

{{< highlight php >}}
public static function get_resource_assignments()
{
    $project = new Project('test_tasks.mpp');
    $resource_assignments = $project->getResourceAssignments()->toList();
    $i = 0;
    while ($i < sizeof($resource_assignments))
    {
        $assignment = $resource_assignments->get($i);
        $asn=new Asn();
        print $assignment->get($asn->UID).PHP_EOL;//.to_string
        print $assignment->get($asn->START).PHP_EOL;//.to_string
        print $assignment->get($asn->FINISH).PHP_EOL;//.to_string
        print "--------------------------------------------------------".PHP_EOL;
        $i += 1;
    }
}
{{< /highlight >}}

## **Aspose.Tasks - Setting General Resource Assignment Properties**
To set general Resource Assignment Properties using **Aspose.Tasks Java for PHP**, call **set_resource_assignments** method of **ResourceAssignmentProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}
public static function set_resource_assignments()
{
    $project = new Project();
    $task = $project->getRootTask()->getChildren()->add("Task");
    $rsc = $project->getResources()->add("Rsc");
    $resource=new Rsc();
    $bigDecimal=new BigDecimal();
    $rsc->set($resource->STANDARD_RATE, $bigDecimal->valueOf(10));
    $rsc->set($resource->OVERTIME_RATE, $bigDecimal->valueOf(15));
    $assignment = $project->getResourceAssignments()->add($task, $rsc);
    print "Set resource assignment properties.".PHP_EOL;
}
{{< /highlight >}}

## **Download Running Code**
Download **General Resource Assignment Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResourceAssignments/ResourceAssignmentProperties.php)
