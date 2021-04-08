---
title: Import and Export Project Data to Primavera Format
description: "Learn how to import or export Microsoft Project (MPP/XML) files from or to Primavera (XER, P6 XML) formats using Aspose.Tasks for C++."
keywords: "Export project data to primavera, convert project data to primavera, Primavera XML, P6 XML, XER, Aspose.Tasks, C++"
type: docs
weight: 100
url: /cpp/import-and-export-project-data-to-primavera-format/
---

{{% alert color="primary" %}} 

Primavera Proprietary Exchange Format (XER), by Primavera Systems, Inc., is primarily associated with Primavera Project Management. Aspose.Tasks for C++ provides the capability to export Microsoft Project Data to Primavera XER as well as XML formats. This article demonstrates how to import or export to a variety of Primavera supported formats.

{{% /alert %}}

## **Importing Data from Primavera File**
Aspose.Tasks for C++ facilitates to import project data from Primavera XML or MPX formats.

### **Importing Data from Primavera XML File Formats**
Aspose.Tasks for C++ can import Primavera XML similar to Microsoft Project XML and MPP formats. The Project class provides the capability of loading such type of file using the same constructor as used for other Project files.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-ImportingAndExporting-ImportDataFromXMLFileFormats-ImportDataFromXMLFileFormats.cpp" >}}

### **Importing Data from Primavera MPX File Formats**

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-ImportingAndExporting-ImportDataFromMPXFileFormats-ImportDataFromMPXFileFormats.cpp" >}}

### **Reading Project UIDs from Primavera XML file**
A Primavera XML file may contain multiple projects, each having its own UID. Aspose.Tasks for C++ API provides the capability to read all such UIDs from the project and then load a project using a specific id from the list of UIDs.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-ImportingAndExporting-ReadProjectUIDsFromXMLFile-ReadProjectUIDsFromXMLFile.cpp" >}}

### **Reading Primavera XML file with Multiple Projects**

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-ImportingAndExporting-ReadXMLFileWithMultipleProjects-ReadXMLFileWithMultipleProjects.cpp" >}}

## **Exporting Project Data in Primavera Formats**
The SaveFileFormat enumerator is used to specifying the project export type as Primavera XML or XER.

### **Exporting Project Data to Primavera XML Format**

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-ImportingAndExporting-ExportProjectDataToXMLFormat-ExportProjectDataToXMLFormat.cpp" >}}

### **Exporting Project Data to Primavera XER Format**

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-ImportingAndExporting-ExportProjectDataToXERFormat-ExportProjectDataToXERFormat.cpp" >}}

### **Exporting Project Data to Primavera MPX Format**

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-ImportingAndExporting-ExportProjectDataToPrimaveraMPXFormat-ExportProjectDataToPrimaveraMPXFormat.cpp" >}}

### **Primavera XML Save Options**
If Primavera XML file doesn't have any WBS inside (only Activities), Aspose.Tasks for C++ can't read properly this type of file, because the API needs a root task to create a tree of tasks. In this case, the API creates a RootTask, even if it doesn't exist in the file, to be able to read these particular files. If the user wants to save after reading, It'll be saving with created RootTask, which did not exist before reading. This option helps to decide how to save into the file with created RootTask or not. By default, it is set to true.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-ImportingAndExporting-UsingPrimaveraXMLSaveOptions-UsingPrimaveraXMLSaveOptions.cpp" >}}
