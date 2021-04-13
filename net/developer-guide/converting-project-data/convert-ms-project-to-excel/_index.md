---
title: Export MS Project to Excel
description: "Write your own MS Project convertor using Aspose.Tasks for .NET and convert MPP files to Excel OpenXML (XLSX) format."
keywords: "ms project convertor, convert mpp to excel, export ms project to excel, microsoft project export to excel, microsoft project converter"
type: docs
weight: 30
url: /net/convert-ms-project-to-excel/
---

In this article we are going to shows how to export MS Project to Microsoft Excel OpenXML (XLSX) format using Aspose.Tasks for .NET API.

The [Project](https://apireference.aspose.com/tasks/net/aspose.tasks/project/) class exposes the Save method which is used to save a project in various formats. The [Project.Save](https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/1) method allows you to export project tasks, resources and assignments to separate worksheets to Microsoft Excel [XLSX](https://docs.fileformat.com/spreadsheet/xlsx/) format using the [SaveFileFormat](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat) enumeration type or the [XlsxOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/xlsxoptions/properties/index) class.

In order to convert a MS Project MPP file to XLSX format with default settings using [SaveFileFormat](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat):

1. Create a new [Project](https://apireference.aspose.com/tasks/net/aspose.tasks/project/) instance and load the MPP file.
2. Convert the project to Excel XLSX using [Project.Save](https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/1) method with the SaveFileFormat.XLSX argument.

The following lines of code show how to achieve this using in .NET:

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-SaveProjectAsXLSX.cs" >}}

In order to convert MPP file with a non-default settings the [XlsxOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/xlsxoptions/properties/index) class is provided.
With this class one can specify additional options while rendering project pages to XLSX. 

In order to convert a MS Project MPP file to XLSX format using [XlsxOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/xlsxoptions/properties/index) class:

1. Create a new [Project](https://apireference.aspose.com/tasks/net/aspose.tasks/project/) instance and load the MPP file.
2. Convert MS Project to Excel XLSX using [Project.Save](https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/1) method and pass the [XlsxOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/xlsxoptions/properties/index) instance as the argument.

The following lines of code show how to tune convert options using [XlsxOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/xlsxoptions/properties/index) in .NET:

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-UsingXlsxOptions.cs" >}}

## **Save Project Data to Spreadsheet2003 XML**
There are two ways to save data to Spreadsheet2003 XML format: default, or using [save options](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/mppsaveoptions). Using the SaveFileFormat instance, the default view data is saved.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-SaveProjectDataToSpreadsheet2003XML-SaveProjectDataToSpreadsheet2003XML.cs" >}}

### **Using Spreadsheet2003SaveOptions**
Aspose.Tasks for .NET provides Spreadsheet2003SaveOptions for modifying the view data.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-UsingSpreadsheet2003SaveOptions-UsingSpreadsheet2003SaveOptions.cs" >}}
