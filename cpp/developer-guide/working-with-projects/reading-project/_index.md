---
title: Reading Project
type: docs
weight: 20
url: /cpp/reading-project/
---

{{% alert color="primary" %}} 

Aspose.Tasks for C++ lets you work with Microsoft Project files without having Microsoft Project installed, or using Microsoft Office Automation. A powerful and flexible API, Aspose.Tasks saves you time and effort by giving you the tools you need to write efficient code for manipulating project files in your C++ applications.

This article explains how to open and read project file.

{{% /alert %}} 
## **Reading a Project File**
At the moment, Aspose.Tasks can export Microsoft Project to Microsoft Project's XML format only. This is true if you are creating a new project. Aspose.Tasks lets you read existing MPP files and save these back in MPP format after updating. This allows reading MPP as well as MPT formats as input templates. This article shows how a Project file (**XML**, **MPP**, **MPT**) can be read using the Project class's constructor.
### **Reading Project Files as a Template**
{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-CreatingReadingAndSaving-ReadProjectFiles-ReadProjectFiles.cpp" >}}
### **Reading Project File from Stream**
{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-CreatingReadingAndSaving-ReadProjectFileFromStream-ReadProjectFileFromStream.cpp" >}}


### **Ignoring invalid characters during loading Project**
Some files may have invalid characters in the custom fields. MS Project does not allow invalid character so the files have been created or manipulated with automation or some other tools. If these files are loaded using the API, they may lead to an exception. In order to ignore such invalid characters, the overloaded constructor of Project class can be used with the delegate method ParseErrorCallBack.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-CreatingReadingAndSaving-IgnoreInvalidCharactersDuringloadingProject-IgnoreInvalidCharactersDuringloadingProject.cpp" >}}
## **Read Password Protected Projects (2003 Format)**
The [Project](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project/) class exposes the Project() constructor which is capable of reading password-protected files in 2003 format. Saving a password-protected file is not supported yet.

To read a password-protected project file:

1. Load a Microsoft Project file.
2. In the constructor, provide a password as the second argument to the constructor.

The following code example demonstrates how to read password-protected project file.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-CreatingReadingAndSaving-ReadPasswordProtectedProjectFile-ReadingPasswordProtectedProjectFile.cpp" >}}
## **Working With Encodings**
Aspose.Tasks provides support for the encoding of MPX files. The following code example demonstrates how to use the encoding settings.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-CreatingReadingAndSaving-WorkingWithEncodings-WorkingWithEncodings.cpp" >}}
