---
title: Convert Microsoft Project to Excel
description: "Aspose.Tasks for .NET allows converting Microsoft Project (MPP) to Microsoft XLS and XLSX format."
keywords: "Export your project to Excel, MPP to XLS, Convert your MPP to XLS, Convert Microsoft Project to Excel, convert MPP to XLSX, Aspose.Tasks, C#"
type: docs
weight: 30
url: /net/convert-ms-project-to-excel/
---

{{% alert color="primary" %}} 

This article shows how to save project data to XLSX format using Aspose.Tasks for .NET.

{{% /alert %}} 

The [Project](https://apireference.aspose.com/tasks/net/aspose.tasks/project/) class exposes the Save method which is used to save a project in various formats. The Save method allows you to save project tasks, resources and assignments to separate worksheets to XLSX format using the SaveFileFormat enumeration type.

To save a project to XLSX:

1. Load a Microsoft Project file.
2. Save the project to XLSX using SaveFileFormat.XLSX.
## **Saving a Project as XLSX**
The following lines of code show how to achieve this using C#.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-SaveProjectAsXLSX-SaveProjectAsXLSX.cs" >}}
### **Using XlsxOptions**
With XlsxOptions, you can modify how the project is exported.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-UsingXlsxOptions-UsingXlsxOptions.cs" >}}
## **Save Project Data to Spreadsheet2003 XML**
There are two ways to save data to Spreadsheet2003 XML format: default, or using [save options](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/mppsaveoptions). Using the SaveFileFormat instance, the default view data is saved.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-SaveProjectDataToSpreadsheet2003XML-SaveProjectDataToSpreadsheet2003XML.cs" >}}


### **Using Spreadsheet2003SaveOptions**
Aspose.Tasks for .NET provides Spreadsheet2003SaveOptions for modifying the view data.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-UsingSpreadsheet2003SaveOptions-UsingSpreadsheet2003SaveOptions.cs" >}}
