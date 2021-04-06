---
title: Working with Outline Codes in a Project
description: "Learn how to work with Microsoft Project outline codes using Aspose.Tasks for .NET."
type: docs
weight: 120
url: /net/working-with-outline-codes-in-a-project/
---

Custom outline codes are tags you define for tasks or resources that provide a project structure that is different from WBS codes or outline numbers. Aspose.Tasks lets you retrieve these outline codes and their properties, such as Alias, AllLevelsRequired, Enterprise, EnterpriseOutlineCodeAlias, FieldId, FieldName, PhoneticAlias, Guid, Masks and Values.
 
## **Reading Outline Codes**
The [Project](https://apireference.aspose.com/tasks/net/aspose.tasks/project) class exposes [OutlineCodes](https://apireference.aspose.com/tasks/net/aspose.tasks/task/properties/outlinecodes) which is a collection of [OutlineCodeDefinition](https://apireference.aspose.com/tasks/net/aspose.tasks/outlinecodedefinition) items. The OutlineCodeDefinition provides all the detail as shown in the following sample code.

The following lines of code retrieve a project's outline code information.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-WorkingWithOutlineCodes-ReadOutlineCodes.cs" >}}

## **Check Outline Code Id Uniqueness**
While working with OutlineCode, Aspose.Tasks shall check the uniqueness of the Outline Code Id and duplicate Ids will be replaced with unique values.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-WorkingWithOutlineCodes-CheckOutlineCodeIdUniqueness.cs" >}}
