---
title: Export MS Project to Excel Formats
description: "Write your own MS Project convertor using Aspose.Tasks for .NET and convert MPP files to Microsoft Excel spreadsheet file formats."
keywords: "ms project convertor, convert mpp to excel, export ms project to excel, microsoft project export to excel, microsoft project converter"
type: docs
weight: 30
url: /net/convert-ms-project-to-excel/
---

In this article we are going to shows how to export MS Project to Microsoft Excel spreadsheet file formats ([Spreadsheet2003 XML](https://en.wikipedia.org/wiki/SpreadsheetML), [XLSX](https://docs.fileformat.com/spreadsheet/xlsx/), [CSV](https://docs.fileformat.com/spreadsheet/csv/)) using Aspose.Tasks for .NET API.

## **Convert MS Project files to Spreadsheet2003 XML (Excel 2003)**
There are two ways to convert projects to [Spreadsheet2003 XML](https://en.wikipedia.org/wiki/SpreadsheetML) format. The first one is to use [SaveFileFormat](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat) enumeration. The second one is to use [Spreadsheet2003SaveOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/spreadsheet2003saveoptions) class.

In order to convert a MS Project MPP file to Spreadsheet2003 XML format with default settings using [SaveFileFormat](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat):

1. Create a new project instance and load the MPP file.
2. Convert the project to Spreadsheet2003 XML using [Project.Save](https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/1) method and specify the SaveFileFormat.Spreadsheet2003 as the argument.

The following lines of code show how to achieve this in .NET:

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-SaveProjectDataToSpreadsheet2003XML.cs" >}}

To convert MPP files with a non-default settings the [Spreadsheet2003SaveOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/spreadsheet2003saveoptions) class is provided. With this class one can specify additional options while rendering project pages to Spreadsheet2003 XML.

1. Create a new project instance and load the MPP file.
2. Convert the project to Excel using [Project.Save](https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/2) method and pass the [Spreadsheet2003SaveOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/spreadsheet2003saveoptions) instance as the argument.

Presented below is .NET example showing how to use the convert options:

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-UsingSpreadsheet2003SaveOptions.cs" >}}

## **Convert MS Project files to Excel XSLX (Excel 2007 and later)**

The [Project](https://apireference.aspose.com/tasks/net/aspose.tasks/project/) class exposes the Save method which is used to save a project in various formats. The [Project.Save](https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/1) method allows you to export project tasks, resources and assignments to separate worksheets to Microsoft Excel [XLSX](https://docs.fileformat.com/spreadsheet/xlsx/) format using the [SaveFileFormat](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat) enumeration type or the [XlsxOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/xlsxoptions) class.

In order to convert MS Project MPP file to XLSX format with default settings using [SaveFileFormat](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat):

1. Create a new project instance and load the MPP file.
2. Convert the project to Excel XLSX using Project.Save method and specify the SaveFileFormat.XLSX as the argument.

The following lines of code show how to achieve this in .NET:

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-SaveProjectAsXLSX.cs" >}}

To convert MPP files with a non-default settings the [XlsxOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/xlsxoptions) class is provided. With this class one can specify additional options while rendering project pages to XLSX.

1. Create a new project instance and load the MPP file.
2. Convert the project to Excel using Project.Save method and pass the [XlsxOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/xlsxoptions) instance as the argument.

Presented below is .NET example showing how to use the options:

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-UsingXlsxOptions.cs" >}}

## **Convert MS Project files to CSV**

Another option to convert MS Project to Excel spreadsheet format is to use [CSV](https://docs.fileformat.com/spreadsheet/csv/). There are two ways to do it: use [SaveFileFormat](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat) enumeration or the [CsvOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/csvoptions) class.

In order to convert MS Project MPP file to CSV format with default settings using [SaveFileFormat](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat):

1. Create a new project instance and load the MPP file.
2. Convert the project to CSV using Project.Save method and specify the SaveFileFormat.CSV as the argument.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-SaveProjectAsCSV.cs" >}}

To convert MPP files with a non-default settings the [CsvOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/csvoptions) class is provided. With this class one can specify additional options while rendering project pages to CSV.

1. Create a new project instance and load the MPP file.
2. Convert the project to Excel using Project.Save method and pass the [CsvOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/csvoptions) instance as the argument.

Presented below is .NET example showing how to change text delimiter using the options:

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-UsingCsvOptions.cs" >}}

### **How to change the view while convert MPP to CSV**

By default the Gantt Chart view is used to decide what column headers will be exported. To change the view the [DataCategory](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/csvoptions/properties/datacategory) property can be used:

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-UsingCsvOptions-ChangeDataCategory.cs" >}}

### **How to sort tasks while convert to CSV**

By using [CsvOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/csvoptions) one can tune the export parameters e.g. control the view to export and/or filter exported tasks. Lets take a look on the some of options available.

Another option is allowing to change the sorting order the tasks by assigning a custom [comparer](https://docs.microsoft.com/en-us/dotnet/api/system.collections.generic.comparer-1?view=net-5.0) to the [TasksComparer](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/saveoptions/properties/taskscomparer) property. Presented below is the example where tasks sorted by name are exported reversed order:

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-UsingCsvOptions-CustomTaskComparer.cs" >}}

### **How to filter tasks while convert to CSV**

In order to filter the exported tasks one can specify the task filter by assigning a custom [condition](https://apireference.aspose.com/tasks/net/aspose.tasks.util.icondition/1) to 
the [TasksFilter](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/saveoptions/properties/tasksfilter) property:

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-UsingCsvOptions-CustomTaskFilter.cs" >}}

### **How to change delimiter while converting to CSV**

CSV is a text format that uses text delimiters to split data fields. To change the text delimiter one can set the [TextDelimiter](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/csvoptions/properties/textdelimiter) property to one of the next values:

- Comma;
- Semicolon (the default delimiter);
- Space;
- Tab.

The available delimiters are defined in [CsvTextDelimiter](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/csvtextdelimiter) enumeration.

Presented below is the example in which data fields are being split by tab symbol:

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-UsingCsvOptions-CustomTextDelimiter.cs" >}}

### **How to change encoding while converting to CSV**

By default CSV is being exported in [Encoding.Default](https://docs.microsoft.com/en-us/dotnet/api/system.text.encoding.default) encoding. To change the encoding the [Encoding](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/csvoptions/properties/encoding) property can be used:

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-UsingCsvOptions-CustomEncoding.cs" >}}

### **How to hide column headers while converting to CSV**

By default column headers are being exported in CSV format. To suppress export of column headers the [IncludeHeaders](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/csvoptions/properties/includeheaders) property can be used:

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-UsingCsvOptions-HideColumnHeaders.cs" >}}
