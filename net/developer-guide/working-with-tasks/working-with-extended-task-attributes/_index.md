---
title: Working with Extended Task Attributes
description: "Learn how to work with Microsoft Project (MPP/XML) task extended attributes using Aspose.Tasks for .NET."
type: docs
weight: 190
url: /net/working-with-extended-task-attributes/
---

In Microsoft Project, an extended task attribute is an element used to capture data for a custom task field. Aspose.Tasks can create as well as retrieve extended attribute information for all versions of Microsoft Project: 2003, 2007, 2010, and 2013.

## **Adding Extended Attribute Information for a Task**
Creating an Extended attribute requires the following steps:

1. Create [ExtendedAttributeDefinition[(https://apireference.aspose.com/tasks/net/aspose.tasks/extendedattributedefinition) for the Attribute with necessary parameters
2. Create [ExtendedAttribute](https://apireference.aspose.com/tasks/net/aspose.tasks/extendedattribute) from the definition in the previous step
3. Add the created ExtendedAttribute to the task

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-AddTaskExtendedAttributes.cs" >}}

## **Reading Extended Task Attributes Information**
The ExtendedAttribute property exposed by the [Task](https://apireference.aspose.com/tasks/net/aspose.tasks/task) class is used to manage a task's extended attributes. This property reads and writes an ArrayList of ExtendedAttribute objects to deal with a task's extended attributes. The ExtendedAttribute object further exposes the relevant properties.

The following example shows how to view a task's extended attributes with Aspose.Tasks.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-ReadTaskExtendedAttributes.cs" >}}
