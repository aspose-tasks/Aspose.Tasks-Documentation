---
title: Working with Extended Task Attributes
description: "Learn how to work with Microsoft Project (MPP/XML) task extended attributes using Aspose.Tasks for Java."
type: docs
weight: 190
url: /java/extended-task-attributes/
---

{{% alert color="primary" %}}

In Microsoft Project, an extended task attribute is an element used to capture data for a custom task field. Aspose.Tasks can retrieve extended attribute information for all versions of Microsoft Project: 2003, 2007, 2010, and 2013.

{{% /alert %}}

## **Adding Extended Attribute Information for a Task**
Creating an Extended attribute requires the following steps:

1. Create ExtendedAttributeDefinition for the Attribute with necessary parameters
2. Create ExtendedAttribute from the definition in the previous step
3. Add the created ExtendedAttribute to the task

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-AddTaskExtendedAttributes-AddTaskExtendedAttributes.java" >}}

## **Reading Extended Task Attributes**
The ExtendedAttribute property exposed by the [Task](https://reference.aspose.com/tasks/java/com.aspose.tasks/Task) class is used to manage a task's extended attributes. This property reads and writes an ArrayList of ExtendedAttribute objects to deal with a task's extended attributes. The ExtendedAttribute object further exposes the relevant properties.

The following example shows how to view a task's extended attributes with Aspose.Tasks.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-ExtendedTaskAttributes-ReadTaskExtendedAttributes.java" >}}
