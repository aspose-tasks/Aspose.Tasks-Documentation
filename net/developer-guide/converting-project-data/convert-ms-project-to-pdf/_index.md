---
title: Convert MS Project to PDF
type: docs
description: "Aspose.Tasks for .NET allows converting Microsoft Project (MPP) to PDF."
keywords: "Export your project to PDF, MPP to PDF, Convert your MPP to PDF, Convert Microsoft Project to PDF, convert MPP to PDF, save project data to PDF, Aspose.Tasks, C#"
weight: 10
url: /net/convert-ms-project-to-pdf/
---

{{% alert color="primary" %}} 

Aspose.Tasks API provides the capability to render project data in PDF format. This article gives a detailed overview of the variety of options available in Aspose.Tasks for exporting projects to PDF.

{{% /alert %}} 


## **Saving a Project as a PDF**
The [Project](https://apireference.aspose.com/net/tasks/aspose.tasks/project) class exposes the Save method which is used to save a project in various formats. The [Save](https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/3) method allows you to render project data to PDF using the [SaveFileFormat](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat) enumeration type.

To save a project to PDF:

1. Load a Microsoft Project file.
2. Save the project to PDF using SaveFileFormat.PDF.
### **PDF Creator Information**
- Please note that you cannot set values against the **Application** and **Producer** fields, because of Aspose Ltd. and Aspose.Tasks for .NET x.x.x will be displayed against these fields.
### **Programming Sample**
The following lines of code demonstrate how to achieve this using C#.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-SaveProjectAsPDF-SaveProjectAsPDF.cs" >}}


## **Fitting Contents to Cell Size**
Commonly, a task (or resource) name is so long that it is truncated when project views are rendered. Aspose.Tasks provides the FitContent property in the SaveOptions class to avoid truncation of task and resource names. The code example below renders a project to PDF format with the FitContent property set to true.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-FitContentsToCellSize-FitContentsToCellSize.cs" >}}


## **Printing or Hiding Legends when Rendering**
To let you print or hide the legends on each page, the SaveOptions class provides the LegendOnEachPage property. If this flag is set to true, legends are printed on each page in the output file.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-HideLegendsDuringSave-HideLegendsDuringSave.cs" >}}
## **Supported Graphical Column Indicators**
Aspose.Tasks draws graphical column indicators when rendering project data to output PDF. The following graphical indicators are supported by Aspose.Tasks:

|**Indicator Type**|**Graphical Indicator**|
| :- | :- |
|Task Indicators|![task graphical indicators](convert-ms-project-to-pdf_1.png)|
|Resource Indicators|![resource graphical indicators](convert-ms-project-to-pdf_2.png)|
|Assignment Indicators|![assignment graphical indicators](convert-ms-project-to-pdf_3.png)|
## **Saving to Multiple PDF Files**
To save project data to multiple PDF files, set the SaveToSeparateFiles flag to true.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-SaveToMultiplePDFFiles-SaveToMultiplePDFFiles.cs" >}}
## **Customizing TextStyle for Project Data**
Aspose.Tasks API allows developers to customize the text style for over-allocated resources. By default, the style used for overallocated resources is similar to Microsoft Project (MSP), that is, red and bold. TextItemType.OverallocatedResources makes it possible to customize the color and style for the overallocated resources.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-CustomizeTextStyle-CustomizeTextStyle.cs" >}}
## **Customizing Date Formats**
Aspose.Tasks API allows developers to customize the date format using the DateFormat enumerator when rendering project data.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-AddDefaultFontDuringSavingAsPDF-AddDefaultFontDuringSavingAsPDF.cs" >}}
## **Setting Default Font**
Setting default font during rending of documents helps when a font is not found. In such a case, the default font replaces the missing font and output is not affected. Aspose.Tasks API lets you specify the default font using the DefaultFontName property of the PdfSaveOptions as shown in the following code sample.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-CustomizeDateFormats-CustomizeDateFormats.cs" >}}
