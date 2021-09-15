---
title: Convert Microsoft Project MPP file to CSV Format
description: "Write your own Microsoft Project convertor using Aspose.Tasks for .NET and convert MPP files to CSV file."
keywords: "ms project convertor, mpp2csv, microsoft project mpp to csv converter, microsoft project mpp to csv convertor, export ms project mpp to csv"
type: docs
weight: 31
url: /net/convert-ms-project-mpp-to-csv/
aliases: 
    - /net/convert-mpp-to-csv/
---

In this article we are going to show how to export Microsoft Project MPP file to [CSV](https://docs.fileformat.com/spreadsheet/csv/)) file format using Aspose.Tasks for .NET API.

## **Convert MS Project files to CSV**

There are two ways to convert Microsoft Project Project to CSV (Comma-Separated Values) format: use [SaveFileFormat](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat) enumeration or the [CsvOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/csvoptions) class.

In order to convert MS Project MPP file to CSV format with default settings using [SaveFileFormat](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat):

1. Create a new project instance and load the MPP file.
2. Convert the project to CSV using Project.Save method and specify the SaveFileFormat.CSV as the argument.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-SaveProjectAsCSV.cs" >}}

To convert MPP files with a non-default settings the [CsvOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/csvoptions) class can be used. With this class one can specify additional options while rendering project pages to CSV.

1. Create a new project instance and load the MPP file.
2. Convert the project to Excel using Project.Save method and pass the [CsvOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/csvoptions) instance as the argument.

Presented below is .NET example showing how to change text delimiter using the options:

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-UsingCsvOptions.cs" >}}

### **How to change the view while convert MPP to CSV**

By default the Gantt Chart view is used to decide what column headers will be exported. To change the view the [DataCategory](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/csvoptions/properties/datacategory) property can be used:

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-UsingCsvOptions-ChangeDataCategory.cs" >}}

### **How to sort tasks while converting to CSV**

By using [CsvOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/csvoptions) one can tune the export parameters e.g. control the view to export and/or filter exported tasks. Lets take a look at some of the options available.

For example, one can customize the sorting order of the tasks by assigning a custom [comparer](https://docs.microsoft.com/en-us/dotnet/api/system.collections.generic.comparer-1?view=net-5.0) to the [TasksComparer](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/saveoptions/properties/taskscomparer) property. Presented below is the example where tasks sorted by name are exported reversed order:

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
