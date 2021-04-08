---
title: Importing and Exporting Project Data to Primavera Format
description: "Learn how to import projects from Primavera XER/XML formats, edit and export them in any of a wide range of available formats (MPP, Primavera XML, PDF, JPEG, XLSX, etc.) using Aspose.Tasks for .NET."
type: docs
weight: 80
url: /net/importing-and-exporting-project-data-to-primavera-format/
---

Primavera Proprietary Exchange Format (XER), by Oracle Inc., is primarily associated with Primavera Project Management. Aspose.Tasks for .NET provides the capability to export Microsoft Project Data to Primavera XER as well as XML formats. This article shows how to import or export to a variety of Primavera supported formats.
 
## **Importing Data from Primavera File**

### **Importing Data from Primavera XML File Formats**
Aspose.Tasks can import Primavera XML similar to Microsoft Project XML and MPP formats. The Project class provides the capability of loading such type of file using the same constructor as used for other Project files.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-ImportingAndExporting-ImportDataFromXMLFileFormats-ImportDataFromXMLFileFormats.cs" >}}

### **Importing Data from Primavera MPX File Formats**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-ImportingAndExporting-ImportDataFromMPXFileFormats-ImportDataFromMPXFileFormats.cs" >}}

### **Reading Project UIDs from Primavera XML file**
A Primavera XML file may contain multiple projects, each having its own UID. Aspose.Tasks for .NET API provides the capability to read all such UIDs from the project and then load a project using a specific id from the list of UIDs.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-ImportingAndExporting-ReadProjectUIDsFromXMLFile-ReadProjectUIDsFromXMLFile.cs" >}}

### **Reading Primavera XML file with Multiple Projects**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-ImportingAndExporting-ReadXMLFileWithMultipleProjects-ReadXMLFileWithMultipleProjects.cs" >}}

## **Importing Project Data From Primavera Database**
Aspose.Tasks for .NET API provides the capability to read Project data from Primavera Database. The following example code shows how to use the Project class for reading from the database.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-ImportingAndExporting-ImportProjectFromPrimaveraDB-ImportProjectFromPrimaveraDB.cs" >}}

## **Support for Primavera SQLite Database**
Aspose.Tasks for .NET provides support for reading project data from Primavera SQLite database.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-ImportingAndExporting-SupportForSQLiteDatabase-SupportForSQLiteDatabase.cs" >}}

## **Exporting Project Data in Primavera Formats**
The SaveFileFormat enumerator is used to specify the project export type as Primavera XML or XER.

### **Exporting Project Data to Primavera XML Format**

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-ImportingAndExporting-ExportProjectDataToXMLFormat-ExportProjectDataToXMLFormat.cs" >}}

### **Exporting Project Data to Primavera XER Format**

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-ImportingAndExporting-ExportProjectDataToXERFormat-ExportProjectDataToXERFormat.cs" >}}

### **Exporting Project Data to Primavera MPX Format**

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-ImportingAndExporting-ExportProjectDataToPrimaveraMPXFormat-ExportProjectDataToPrimaveraMPXFormat.cs" >}}

### **Primavera XML Save Options**
If Primavera XML file doesn't have any WBS inside (only Activities), Aspose.Tasks can't read properly this type of file, because the API needs a root task to create a tree of tasks.
In this case, the API creates a RootTask, even if it doesn't exist in the file, to be able to read these particular files. If the user wants to save after reading, It'll be saving with created RootTask, which did not exist before reading. This option helps to decide how to save into the file with created RootTask or not. By default it is set to true.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-ImportingAndExporting-UsingPrimaveraXMLSaveOptions-UsingPrimaveraXMLSaveOptions.cs" >}}
