---
title: Creating and Saving Microsoft Project (MPP/XML) Files
description: "Learn how to create, edit or save Microsoft Project (MPP/XML) files using Aspose.Tasks for C++ API without having Microsoft Office dependencies installed."
type: docs
weight: 10
url: /cpp/creating-and-saving/
---

{{% alert color="primary" %}} 

Aspose.Tasks for C++ lets you work with Microsoft Project (MPP/XML) files without having Microsoft Project installed, or using Microsoft Office Automation. A powerful and flexible API, Aspose.Tasks saves you time and effort by giving you the tools you need to write efficient code for manipulating project files in your C++ applications.

Aspose.Tasks can be used to open existing files or creating a new files. This article explains how to create a new and empty project file from the stream using the Project class as well as open existing files.

{{% /alert %}}

## **Creating an Empty Project File**
The [Project](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project) class is the main class in Aspose.Tasks used to set and get properties associated with a project, as well as project behavior. The Save method offered by this class makes it possible to render the Project to various output formats such as XML, MPP, PDF, HTML, etc. with a single API call. This method accepts a file stream or file name, and one of the values provided by the SaveFileFormat enumeration type.

At present, Aspose.Tasks provides the facility to create the **XML** project files only. The following lines of code create a simple project file in the XML format.

The XML project file can be opened in Microsoft Project:

1. On the **File** menu, select **Open**.
2. Select the XML format (*.xml) option from the file types and browse to the output XML file.
3. On the **Project** menu, select **Project Information**

### **Create an Empty Project And Saving as XML File**

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-CreatingReadingAndSaving-CreateEmptyProjectSaveXML-CreateEmptyProjectSaveXML.cpp" >}}

### **Create an Empty Project and Save to Stream**

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-CreatingReadingAndSaving-CreateEmptyProjectSaveStream-CreateEmptyProjectSaveStream.cpp" >}}

### **Create an Empty Project and Save to MPP**

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-CreatingReadingAndSaving-CreateEmptyProjectSaveMPP-CreateEmptyProjectSaveMPP.cpp" >}}
