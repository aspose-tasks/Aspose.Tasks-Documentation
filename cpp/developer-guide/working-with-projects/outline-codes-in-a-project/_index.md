---
title: Outline Codes in a Project
description: "Learn how to work with Microsoft Project (MPP/XML) outline codes using Aspose.Tasks for C++."
type: docs
weight: 90
url: /cpp/outline-codes-in-a-project/
---

{{% alert color="primary" %}}

Custom outline codes are tags you define for tasks or resources that provide a project structure that is different from WBS codes or outline numbers. Aspose.Tasks for C++ lets you retrieve these outline codes and their properties, such as Alias, AllLevelsRequired, Enterprise, EnterpriseOutlineCodeAlias, FieldId, FieldName, PhoneticAlias, GUID, Masks and Values.

{{% /alert %}}

## **Reading Outline Codes**
The Project class exposes OutlineCodes which is a collection of OutlineCodeDefinition items. The OutlineCodeDefinition provides all the detail as shown in the following sample code.

The following lines of code retrieve a project's outline code information.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-WorkingWithOutlineCodes-ReadOutlineCodes.cpp" >}}

## **Check Outline Code Id Uniqueness**
While working with OutlineCode, Aspose.Tasks shall check the uniqueness of the Outline Code Id and duplicate Ids will be replaced with unique values.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-WorkingWithOutlineCodes-CheckOutlineCodeIdUniqueness.cpp" >}}
