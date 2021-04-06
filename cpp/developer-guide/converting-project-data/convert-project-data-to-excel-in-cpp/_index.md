---
title: Convert Project Data to Excel in CPP
type: docs
weight: 10
url: /cpp/convert-project-data-to-excel-in-cpp/
---

{{% alert color="primary" %}} 

This article demonstrates how to save project data to XLSX format using Aspose.Tasks for C++.

{{% /alert %}} 

The [Project](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project) class exposes the Save method which is used to save a project in various formats. The Save method allows you to save project tasks, resources and assignments to separate worksheets to XLSX format using the SaveFileFormat enumeration type.

To save a project to XLSX:

1. Load a Microsoft Project file.
2. Save the project to XLSX using SaveFileFormat.XLSX.
## **Saving a Project as XLSX**
The following lines of code demonstrate how to achieve this using C++.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-ConvertingProjectData-SaveProjectAsXLSX-SaveProjectAsXLSX.cpp" >}}
### **Using XlsxOptions**
With XlsxOptions, you can modify how the project is exported.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-ConvertingProjectData-UsingXlsxOptions-UsingXlsxOptions.cpp" >}}
## **Save Project Data to Spreadsheet2003 XML**
There are two ways to save data to Spreadsheet2003 XML format: default, or using save options. Using the SaveFileFormat instance, the default view data is saved.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-ConvertingProjectData-SaveProjectDataToSpreadsheet2003XML-SaveProjectDataToSpreadsheet2003XML.cpp" >}}


### **Using Spreadsheet2003SaveOptions**
Aspose.Tasks provides Spreadsheet2003SaveOptions for modifying the view data.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-ConvertingProjectData-UsingSpreadsheet2003SaveOptions-UsingSpreadsheet2003SaveOptions.cpp" >}}
