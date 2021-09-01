---
title: Creating, Reading and Saving Projects
description: "Learn how to create, edit, and save projects in different formats (MPP, Primavera XML, PDF, JPEG) using Aspose.Tasks for .NET."
type: docs
weight: 10
url: /net/creating-reading-and-saving-projects/
---

Aspose.Tasks for .NET lets you work with Microsoft Project (MPP/XML) files without having Microsoft Project installed, or using Microsoft Office Automation. A powerful and flexible API, Aspose.Tasks saves you time and effort by giving you the tools you need to write efficient code for manipulating project files.

Aspose.Tasks can open existing files, but it can also create new files. This article explains how to create a new and empty project file from the stream using the Project class.  as well as open existing files.

## **Creating an Empty Project File**
The [Project](https://apireference.aspose.com/tasks/net/aspose.tasks/project) class is the main class in Aspose.Tasks used to set and get properties associated with a project, as well as behavior. The Save method offered by this class makes it possible to render the Project to various output formats such as XML, MPP, PDF, HTML, etc. with a single API call. This method accepts a file stream or file name, and one of the values provided by the [SaveFileFormat](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat) enumeration type.

The following lines of code create a simple project file in XML format.

### **Create an Empty Project And Saving as XML File**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-CreateEmptyProjectSaveXML.cs" >}}

The resulting XML project file can be opened in Microsoft Project using the following steps:

1. On the **File** menu, select **Open**.
2. Select the XML format (*.xml) option from the file types and browse to the output XML file.
3. On the **Project** menu, select **Project Information**

### **Create an Empty Project and Save to Stream**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-CreateEmptyProjectSaveStream.cs" >}}

### **Create an Empty Project and Save to MPP**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-CreateEmptyProjectSaveMPP.cs" >}}

## **Reading a Project File**
Aspose.Tasks for .NET lets you read existing project in different formats: **XML**, **MPP**, **MPT**, **MPX**, **XER**, Primavera P6 XML, etc and save these back in MPP or another format after updating. The following snippets show how a project file can be read using the Project class's constructor.

### **Reading Project Files as a Template**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-ReadProjectFiles.cs" >}}

### **Reading Project File from Stream**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-ReadProjectFileFromStream.cs" >}}

### **Importing Project Data From Microsoft Project Server Database**

We plan to retire the importing of project data from Microsoft Project Server Database in a future release.
Instead you can use import \ export of project data using Microsoft Project Server's PWA API.

See documentation for [ProjectServerManager](https://apireference.aspose.com/tasks/net/aspose.tasks/projectservermanager) class for more details.

{{< highlight csharp >}}
// Create connection string
SqlConnectionStringBuilder sqlConnectionString = new SqlConnectionStringBuilder();
sqlConnectionString.DataSource = "192.168.56.2,1433";
sqlConnectionString.Encrypt = true;
sqlConnectionString.TrustServerCertificate = true;
sqlConnectionString.InitialCatalog = "ProjectServer_Published";
sqlConnectionString.NetworkLibrary = "DBMSSOCN";
sqlConnectionString.UserID = "sa";
sqlConnectionString.Password = "*****";

// Use Aspose.Tasks.Connectivity namespace
MspDbSettings settings = new MspDbSettings(sqlConnectionString.ConnectionString, new Guid("E6426C44-D6CB-4B9C-AF16-48910ACE0F54"));
Project project = new Project(settings);{{< /highlight >}}

### **Import Project Data from MPD (Microsoft Project Database) File**

{{< highlight csharp >}}
DbSettings settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + "MpdFileToRead.mpd", 1);
Project project = new Project(settings);
{{< /highlight >}}

### **Ignoring invalid characters during loading Project**
Some files may have invalid characters in the custom fields. Microsoft Project does not allow invalid character so the files have been created or manipulated with automation or some other tools.
If these be loaded using the API, they may lead to an exception. In order to ignore such invalid characters, the overloaded constructor of Project class can be used with the delegate method ParseErrorCallBack.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-IgnoreInvalidCharactersDuringloadingProject.cs" >}}

## **Working With Encodings**
Aspose.Tasks for .NET provides support for the encoding of MPX files. The following code example shows the encoding settings.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-WorkingWithEncodings.cs" >}}
