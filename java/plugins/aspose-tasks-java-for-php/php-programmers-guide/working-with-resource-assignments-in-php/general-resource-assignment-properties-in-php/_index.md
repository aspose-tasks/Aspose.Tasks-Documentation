---
title: General Resource Assignment Properties in Php
type: docs
weight: 50
url: /java/general-resource-assignment-properties-in-php/
---

## **Aspose.Tasks - Getting General Resource Assignment Properties**
To Get General Resource Assignment Properties using **Aspose.Tasks Java for PHP**, call **get_resource_assignments** method of **ResourceAssignmentProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 public static function get_resource_assignments($dataDir=null){

\# Instantiate project object

$project = new Project($dataDir . 'test_tasks.mpp');

$resource_assignments = $project->getResourceAssignments()->toList();

\# Parse through all the collected resource assignments

$i = 0;

while ($i < sizeof($resource_assignments)){

$ra = $resource_assignments->get($i);

$asn=new Asn();

print $ra->get($asn->UID).PHP_EOL;//.to_string

print $ra->get($asn->START).PHP_EOL;//.to_string

print $ra->get($asn->FINISH).PHP_EOL;//.to_string

print "--------------------------------------------------------".PHP_EOL;

$i +=1;

}

}


{{< /highlight >}}
## **Aspose.Tasks - Setting General Resource Assignment Properties**
To Set General Resource Assignment Properties using **Aspose.Tasks Java for PHP**, call **set_resource_assignments** method of **ResourceAssignmentProperties** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 public static function set_resource_assignments($dataDir=null){

\# Instantiate project object

$project = new Project();

$task = $project->getRootTask()->getChildren()->add("Task");

$rsc = $project->getResources()->add("Rsc");

$rscc=new Rsc();

$bigDecimal=new BigDecimal();

$rsc->set($rscc->STANDARD_RATE, $bigDecimal->valueOf(10));

$rsc->set($rscc->OVERTIME_RATE, $bigDecimal->valueOf(15));

$assn = $project->getResourceAssignments()->add($task, $rsc);

print "Set resource assignment properties.".PHP_EOL;

}

{{< /highlight >}}
## **Download Running Code**
Download **General Resource Assignment Properties (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResourceAssignments/ResourceAssignmentProperties.php)
- [CodePlex](https://asposetasksjavaphp.codeplex.com/SourceControl/latest#src/aspose/tasks/WorkingWithResourceAssignments/ResourceAssignmentProperties.php)
