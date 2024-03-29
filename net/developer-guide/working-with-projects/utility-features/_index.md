---
title: Utility Features Available in Aspose.Tasks for .NET
description: "The page describes a set of useful utility functions that can be applied to project files using Aspose.Tasks for .NET. such as a critical path calculation, working with task filters and so on."
type: docs
weight: 140
url: /net/utility-features/
---

## **Calculate Critical Path**
The critical path is the tasks, or task, that ultimately determine when your project will end. Keeping track of the critical path and the resources assigned to them helps keep the project on time. Microsoft Project calculates the critical path based on tasks that have no slack, have specific date constraints (must start on, must finish on, as soon as possible or as late as possible) or have the same, or later, end date as the project. Aspose.Tasks allows you to calculate the critical path.

The [Project](https://reference.aspose.com/tasks/net/aspose.tasks/project) class provides the [CriticalPath](https://reference.aspose.com/tasks/net/aspose.tasks/project/properties/criticalpath) property which is used to retrieve the collection of tasks that comprise the project's critical path. The following piece of code calculates and displays the tasks in the critical path.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-Miscellaneous-CalculateCriticalPath.cs" >}}

## **Printing the TaskWritingException**
A project consists of a number of tasks and Aspose.Tasks for .NET API allows adding, removing and updating task information. If there's a problem when writing tasks, use [TasksWritingException](https://reference.aspose.com/tasks/net/aspose.tasks/taskswritingexception) to catch them.

Aspose.Tasks for .NET supports printing a message when there's an exception in writing a task. This is done with TaskWritingException, in a similar way to how TaskReadingException is used.

The log message is contained in the public property [TasksWritingException.LogText](https://reference.aspose.com/tasks/net/aspose.tasks/tasksloggedexception/properties/logtext), as shown in the following code example.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-Miscellaneous-PrintTaskWritingException.cs" >}}

## **Working with Filter Data from MPP Files**
Aspose.Tasks allows developers to read information about filters applied to MPP file data. This article shows how to retrieve filter definition and filter criteria data from a Microsoft Project MPP file.

### **Reading Filter Definition Data**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-Miscellaneous-ReadFilterDefinitionData.cs" >}}

### **Reading Filter Criteria Data**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-Miscellaneous-ReadFilterCriteriaData.cs" >}}

## **Reading Group Definition Data**
A Microsoft Project data file may contain data in groups. Aspose.Tasks for .NET provides the facility to read the group definition data as shown in the below example.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-Miscellaneous-ReadGroupDefinitionData.cs" >}}

## **Reading Table Data from MPP File**
The Aspose.Tasks for .NET API supports reading table data from Microsoft Project data files. Project.Tables implements the ICollection interface to provide access to an MPP file's table data. The feature is supported for all versions of Microsoft Project data files, including MPP 2003, 2007, 2010 and 2013.

The below example shows how to retrieve table data from a Microsoft Project MPP file. The values of table properties such as width, title, title alignment and data alignment are displayed here for demonstration.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-Miscellaneous-ReadTableDataFromProjectFile.cs" >}}

## **Extracting Embedded Objects from Task or Review form**
Microsoft Project data files (MPP/XML) may contain embedded objects such as documents, excel sheets, PDF, images etc. in Task or Resource views. Aspose.Tasks for .NET API provides the capability to extract these from a project's Task or Resource view as shown in the below topics.

### **Extracting Embedded Objects**
Embedded objects (those which were created from the file by selecting a file path) are packed into OLE Package inside MPP file. To extract the original file you can use Content and FullPath properties of an instance of the OleObject class.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-Miscellaneous-ExtractEmbeddedObjects.cs" >}}

Embedded objects which were created inside Microsoft Project application can be extracted this way:

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-Miscellaneous-EmbeddedObjectsCreatedInsideApplication.cs" >}}
