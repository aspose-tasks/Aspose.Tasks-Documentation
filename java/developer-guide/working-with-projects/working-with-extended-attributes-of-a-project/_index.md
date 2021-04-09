---
title: Working with Extended Attributes of a Project
description: "Learn how to work with Microsoft Project (MPP/XML) extended attributes and custom field using Aspose.Tasks for Java."
type: docs
weight: 80
url: /java/working-with-extended-attributes-of-a-project/
---

{{% alert color="primary" %}}

Microsoft Project has an extensive XML data interchange schema that exchanging information between applications - and programming with project files - easier. The schema allows you to add extended attributes to tasks, resources and assignments. This article shows how to assign an extended attribute to a [resource assignment](/tasks/java/creating-resource-assignments/) with Aspose.Tasks.

{{% /alert %}}

**Setting Extended Attributes**
The ExtendedAttribute property exposed by the [ResourceAssignment](https://apireference.aspose.com/tasks/java/com.aspose.tasks/resourceassignment) class can be used to manage the extended attributes of an assignment. This property reads or writes a List of the ExtendedAttribute objects to deal with a resource's extended attributes. The [ExtendedAttribute](https://apireference.aspose.com/tasks/java/com.aspose.tasks/extendedattribute) object further exposes the relevant properties.

The following example shows setting the extended attributes of a resource.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-ExtendedAttributes-ExtendedAttributes.java" >}}






