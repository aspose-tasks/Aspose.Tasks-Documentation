---
title: Extended Task Attributes
type: docs
weight: 180
url: /cpp/extended-task-attributes/
---

{{% alert color="primary" %}} 

In Microsoft Project, an extended task attribute is an element used to capture data for a custom task field. Aspose.Tasks can create as well as retrieve extended attribute information for all versions of Microsoft Project: 2003, 2007, 2010, and 2013.

{{% /alert %}} 
### **Adding Extended Attribute Information for a Task**
Creating an Extended attribute requires the following steps:

1. Create ExtendedAttributeDefinition for the Attribute with necessary parameters
2. Create ExtendedAttribute from the definition in the previous step
3. Add the created ExtendedAttribute to the task

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-AddTaskExtendedAttributes-AddTaskExtendedAttributes.cpp" >}}


### **Reading Extended Task Attributes Information**
The ExtendedAttribute property exposed by the [Task](https://www.aspose.com/api/net/tasks/aspose.tasks/task) class is used to manage a task's extended attributes. This property reads and writes an ArrayList of ExtendedAttribute objects to deal with a task's extended attributes. The ExtendedAttribute object further exposes the relevant properties.

The following code example demonstrates how to view a task's extended attributes.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-ReadTaskExtendedAttributes-ReadTaskExtendedAttributes.cpp" >}}
