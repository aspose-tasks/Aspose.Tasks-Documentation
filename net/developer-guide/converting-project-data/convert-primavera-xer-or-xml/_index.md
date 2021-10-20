---
title: Convert Oracle Primavera P6 Project XML or XER file
description: "Aspose.Tasks for .NET provides the ability to convert Projects in Primavera formats to Excel, PDF, MPP, PNG, JPEG."
keywords: "Export your Primavera P6 Project to PDF, Convert XER to PDF, Convert P6XML to PDF, Convert XER to MPP, Convert P6XML to MPP"
type: docs
weight: 10
url: /net/convert-primavera-xer-or-xml-project
---

Primavera is an enterprise project portfolio management software by Oracle Corporation.

Primavera P6 Professional allows the user to export project data to the following formats:
1) Primavera PM (XER)
2) Primavera Contractor (XER) 
3) Primavera P6 (XML)
4) Excel Spreadsheet (XLSX)
5) Microsoft Project (XML)
6) UN/CEFACT Format 6 (XML).

These are steps to export project data to supported formats in Primavera P6 Professional:

Suppose you have your project opened in Primavera P6 Professional.

1) Select "File\Export" menu item
2) Select output format and click "Next" button.
2) Depending on the selected format choose export options (for example, which entities or which projects should be exported).
4) Click "Finish" button.

Aspose.Tasks for .NET supports import of project data from formats supported by Primavera P6: Primavera XML (P6XML), XER and Primavera P6 Database.
The loaded project data can be exported to any of the supported output formats, such as MS Project MPP file, Primavera P6 XML, Primavera XER, PDF, Excel, JPG, PNG, etc.

## **Saving a Primavera P6 XML or XER file as a Microsoft Project MPP file**
The [Project](https://apireference.aspose.com/tasks/net/aspose.tasks/project) class exposes the Save method which is used to save a project in various formats. The [Save](https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/3) method allows you to render project data to PDF using the [SaveFileFormat](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat) enumeration type.

To save a project to Microsoft Project MPP file:

1. Load a Primavera P6 XML or XER file 
2. Optionally make changes to the loaded project.
3. Save the project to MPP using one of Project.Save method overloads.
Your can use either SaveFileFormat.MPP to save project with default settings or pass MPPSaveOptions to customize export options.

The following lines of code demonstrate how to achieve this using C#.

{{< highlight csharp >}}
Project project = new Project("PrimaveraProject.xer");
project.Save("Output.mpp", SaveFileFormat.MPP);
{{< /highlight >}}

## **Saving a Primavera P6 XML or XER file as a PDF file**

Primavera P6 also allows the user to send project's data visual representation to a printer. Aspose.Tasks for .NET provides more flexibility and allows the user to render project's view in PDF or graphical formats programmatically. In this case you don't need to have Primavera P6 installed on your machine.

The [Project](https://apireference.aspose.com/tasks/net/aspose.tasks/project) class exposes the Save method which is used to save a project in various formats. The [Save](https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/3) method allows you to render project data to PDF using the [SaveFileFormat](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat) enumeration type.

To save a project to PDF:

1. Load a Primavera P6 XML or XER file 
2. Optionally make changes to the loaded project.
3. Save the project to PDF using one of Project.Save method overloads.
Your can use either SaveFileFormat.PDF to save project with default settings or PdfSaveOptions to customize export options.

The following lines of code demonstrate how to achieve this using C#.

{{< highlight csharp >}}
Project project = new Project("PrimaveraProject.xer");
project.Save("Output.pdf", SaveFileFormat.PDF);

Project project2 = new Project("PrimaveraProject.xml");
PdfSaveOptions options = new PdfSaveOptions();
options.PageSize = PageSize.A3;
project2.Save("Output2.pdf", options);
{{< /highlight >}}
