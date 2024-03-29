---
title: Create an Empty Project File
description: "Learn how to create an empty Microsoft Project (MPP/XML) file using Aspose.Tasks for .NET."
type: docs
weight: 30
url: /net/create-an-empty-project-file/
---

## **Code Examples**

### **VSTO**
Below is the code to add project file in Microsoft Project

{{< highlight csharp >}}
Project project = this.Application.Projects.Add();
{{< /highlight >}}

### **Aspose.Tasks**
The [Project](https://reference.aspose.com/tasks/net/aspose.tasks/project/) class is the main class in Aspose.Tasks used to set and get properties associated with a project, as well as behavior. The Save method offered by this class makes it possible to render the Project to various output formats such as XML, MPP, PDF, HTML, etc. with a single API call. This method accepts a file stream or file name, and one of the values provided by the [SaveFileFormat](https://reference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat) enumeration type.

At present, Aspose.Tasks for .NET provides the facility to create **XML** project files only. The following lines of code create a simple project file in XML format.

Below is code sample:

{{< highlight csharp >}}
Project project = new Project();
project.Save("NewProject.xml", Saving.SaveFileFormat.XML);
{{< /highlight >}}

## **Download Running Code**
- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-.NET/tree/master/Plugins/Aspose.Tasks%20Vs%20VSTO/Code%20Comparison/Creating%20an%20Empty%20Project%20File)

## **Download Sample Code**
- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-.NET/releases/tag/AsposeTaskNETVsVSTOProjectv1.1)
