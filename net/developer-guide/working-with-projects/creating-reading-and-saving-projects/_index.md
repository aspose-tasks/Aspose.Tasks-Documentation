---
title: Creating, Reading and Saving Projects
type: docs
weight: 10
url: /net/creating-reading-and-saving-projects/
---

{{% alert color="primary" %}} 

Aspose.Tasks for .NET lets you work with Microsoft Project files without having Microsoft Project installed, or using Microsoft Office Automation. A powerful and flexible API, Aspose.Tasks saves you time and effort by giving you the tools you need to write efficient code for manipulating project files.

Aspose.Tasks can open existing files, but it can also create new files. This article explains how to create a new and empty project file from the stream using the Project class.  as well as open existing files.

{{% /alert %}} 
## **Creating an Empty Project File**
The [Project](https://apireference.aspose.com/tasks/net/aspose.tasks/project) class is the main class in Aspose.Tasks used to set and get properties associated with a project, as well as behavior. The Save method offered by this class makes it possible to render the Project to various output formats such as XML, MPP, PDF, HTML, etc. with a single API call. This method accepts a file stream or file name, and one of the values provided by the [SaveFileFormat](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat) enumeration type.

At present, Aspose.Tasks provides the facility to create **XML** project files only. The following lines of code create a simple project file in XML format.

The XML project file can be opened in Microsoft Project:

1. ON the **File** menu, select **Open**.
1. Select the XML format (*.xml) option from the file types and browse to the output XML file.
1. On the **Project** menu, select **Project Information**
### **Create an Empty Project And Saving as XML File**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-CreateEmptyProjectSaveXML-CreateEmptyProjectSaveXML.cs" >}}
### **Create an Empty Project and Save to Stream**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-CreateEmptyProjectSaveStream-CreateEmptyProjectSaveStream.cs" >}}
### **Create an Empty Project and Save to MPP**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-CreateEmptyProjectSaveMPP-CreateEmptyProjectSaveMPP.cs" >}}
## **Reading a Project File**
We mentioned earlier that Aspose.Tasks can export to Microsoft Project's XML format only. This is true if you are creating a new project. Aspose.Tasks lets you read existing MPP files and save these back in MPP format after updating. This allows reading MPP as well as MPT formats as input templates. This article shows how a Project file (**XML**, **MPP**, **MPT**) can be read using the Project class's constructor.
### **Reading Project Files as a Template**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-ReadProjectFiles-ReadProjectFiles.cs" >}}
### **Reading Project File from Stream**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-ReadProjectFileFromStream-ReadProjectFileFromStream.cs" >}}
### **Importing Project Data From Microsoft Project Database**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-ImportProjectDataFromDatabase-ImportProjectDataFromDatabase.cs" >}}
### **Import Project Data from Microsoft MPD File**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-ImportProjectDataFromMPDFile-ImportProjectDataFromMPDFile.cs" >}}
### **Ignoring invalid characters during loading Project**
Some files may have invalid characters in the custom fields. MS Project does not allow invalid character so the files have been created or manipulated with automation or some other tools.
If these be loaded using the API, they may lead to an exception. In order to ignore such invalid characters, the overloaded constructor of Project class can be used with the delegate method ParseErrorCallBack.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-IgnoreInvalidCharactersDuringloadingProject-IgnoreInvalidCharactersDuringloadingProject.cs" >}}
## **Read Password Protected Projects (2003 Format)**
The [Project](https://apireference.aspose.com/tasks/net/aspose.tasks/project) class exposes the Project() constructor which is capable of reading password-protected files in 2003 format. Saving a password-protected file is not supported yet.

To read a password-protected project file:

1. Load a Microsoft Project file.
1. In the constructor, provide a password as the second argument to the constructor.

The following lines of code demonstrate how to achieve this using C#.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-ReadPasswordProtectedProjectFile-ReadingPasswordProtectedProjectFile.cs" >}}

The following code example demonstrates how to check if the project file is password protected.
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ExProject-CheckIfProjectIsPasswordProtected.cs" >}}

## **Working With Encodings**
Aspose.Tasks provides support for the encoding of MPX files. The following code example shows the encoding settings.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-WorkingWithEncodings-WorkingWithEncodings.cs" >}}
