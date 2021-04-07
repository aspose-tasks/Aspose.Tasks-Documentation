---
title: Managing Resource Extended Attributes in PHP
description: "Learn how to add, edit or remove Microsoft Project (MPP/XML) resource extended attributes using Aspose.Tasks Java for PHP."
type: docs
weight: 10
url: /java/extended-resource-attributes-in-php/
---

## **Aspose.Tasks - Extended Resource Attributes**
To set extended resource attributes using **Aspose.Tasks Java for PHP**, simply invoke **ExtendedResourceAttributes** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

$project = new Project('test_tasks.mpp');

$res = $project->getResources()->toList()->get(0);

$attribute = new ExtendedAttribute();

$attribute->setFieldId("11");

$attribute->setValue("MyValueEA");

$attribute->setValueGuid("MyValueGuidEA");

$res->getExtendedAttributes()->add($attribute);

print "Set extended resource attributes.".PHP_EOL;


{{< /highlight >}}
## **Download Running Code**
Download **Extended Resource Attributes (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithResources/ExtendedResourceAttributes.php)
