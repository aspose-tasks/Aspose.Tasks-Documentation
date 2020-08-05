---
title: Working with Outline Codes in a Project
type: docs
weight: 120
url: /net/working-with-outline-codes-in-a-project/
---

{{% alert color="primary" %}} 

Custom outline codes are tags you define for tasks or resources that provide a project structure that is different from WBS codes or outline numbers. Aspose.Tasks lets you retrieve these outline codes and their properties, such as Alias, AllLevelsRequired, Enterprise, EnterpriseOutlineCodeAlias, FieldId, FieldName, PhoneticAlias, Guid, Masks and Values.

{{% /alert %}} 
## **Reading Outline Codes**
The [Project]() class exposes [OutlineCodes]() which is a collection of [OutlineCodeDefinition]() items. The OutlineCodeDefinition provides all the detail as shown in the following sample code.

The following lines of code retrieve a project's outline code information.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-WorkingWithOutlineCodes-ReadOutlineCodes.cs" >}}


## **Check Outline Code Id Uniqueness**
While working with OutlineCode, Aspose.Tasks shall check the uniqueness of the Outline Code Id and duplicate Ids will be replaced with unique values.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-WorkingWithOutlineCodes-CheckOutlineCodeIdUniqueness.cs" >}}
