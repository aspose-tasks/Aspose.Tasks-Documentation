---
title: Working with Outline Codes in a Project
type: docs
weight: 90
url: /java/working-with-outline-codes-in-a-project/
---

{{% alert color="primary" %}} 

Custom outline codes are tags you define for tasks or resources that provide a project structure that is different from WBS codes or outline numbers. Aspose.Tasks lets you retrieve these outline codes and their properties, such as Alias, AllLevelsRequired, Enterprise, EnterpriseOutlineCodeAlias, FieldId, FieldName, PhoneticAlias, Guid, Masks and Values.

{{% /alert %}} 
## **Retrieving Outline Code Definitions**
The [Project](http://www.aspose.com/api/java/tasks/com.aspose.tasks/classes/Project) class exposes [getOutlineCodes()](http://www.aspose.com/api/java/tasks/com.aspose.tasks/classes/project/methods/getOutlineCodes%28%29/) which is a collection of [OutlineCodeDefinition](http://www.aspose.com/api/java/tasks/com.aspose.tasks/classes/OutlineCodeDefinition) items. The OutlineCodeDefinition provides all the detail as shown in the following sample code.

**Programming Sample**

The following lines of code retrieve a project's outline code information.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-RetrieveOutlineCodes-retrieve-outline-codes.java" >}}
