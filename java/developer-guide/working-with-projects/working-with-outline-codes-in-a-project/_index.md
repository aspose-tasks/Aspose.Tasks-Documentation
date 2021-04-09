---
title: Working with Outline Codes in a Project
description: "Learn how to work with Microsoft Project outline codes using Aspose.Tasks for Java."
type: docs
weight: 90
url: /java/working-with-outline-codes-in-a-project/
---

{{% alert color="primary" %}}

Custom outline codes are tags you define for tasks or resources that provide a project structure that is different from WBS codes or outline numbers. Aspose.Tasks for Java lets you retrieve these outline codes and their properties, such as Alias, AllLevelsRequired, Enterprise, EnterpriseOutlineCodeAlias, FieldId, FieldName, PhoneticAlias, Guid, Masks and Values.

{{% /alert %}}

**Retrieving Outline Code Definitions**
The [Project](https://apireference.aspose.com/tasks/java/com.aspose.tasks/project) class exposes [getOutlineCodes()](https://apireference.aspose.com/tasks/java/com.aspose.tasks/Project#getOutlineCodes--) which is a collection of [OutlineCodeDefinition](https://apireference.aspose.com/tasks/java/com.aspose.tasks/outlinecodedefinition) items. The OutlineCodeDefinition provides all the detail as shown in the following sample code.

The following lines of code retrieve a project's outline code information.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-RetrieveOutlineCodes-retrieve-outline-codes.java" >}}
