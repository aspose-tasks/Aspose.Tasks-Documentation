---
title: Convert MS Project to HTML, CSV, Text and Template MPT
type: docs
description: "Aspose.Tasks for .NET allows converting MS Project (MPP) to HTML, CSV, Text and Template MPT format."
keywords: "Export your project to HTML, MPP to HTML, MPP to CSV, MPP to Text, MPP to MPT, Convert MPP to Text, Convert MS Project to HTML, Convert MPP to MPT, convert MPP to CSV, Save Project Data as MPT Template, Aspose.Tasks, C#"
weight: 50
url: /net/convert-ms-project-to-html-csv-text-and-template-mpt/
---

{{% alert color="primary" %}} 

Microsoft Project (MSP) allows developers to save project data (MPP/XML) to HTML, comma-delimited (CSV), text and MPT templates. Aspose.Tasks also allows you to save project data to the same formats similar to MSP. This is achieved using the standard Save method exposed by the [Project]() class.

{{% /alert %}} 
# **Saving Project Data as HTML**
Aspose.Tasks can export project data to HTML format. It allows to save all the data to HTML or export only required pages to HTML by using the SaveOptions as shown in the following code samples.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-SaveProjectDataAsHTML-SaveProjectDataAsHTML.cs" >}}


#### **Controlling Document Header Name during Export to HTML**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-ControlHeaderNameDuringHTMLExport-ControlHeaderNameDuringHTMLExport.cs" >}}
#### **Saving Fonts, Images and CSS Styles Separately**
Aspose.Tasks API gives you enough power to save fonts, images, and CSS styles information separately to files while saving Project Data to HTML. This is achieved using the HtmlSaveOptions class by providing information about CSS, Font and Image destinations. 

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithResources-ResourcePrefixForNestedResources-ResourcePrefixForNestedResources.cs" >}}
#### **Adding Page Prefix in CSS Classes While Exporting to HTML**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-AddingCssStylePrefix-AddingCssStylePrefix.cs" >}}
## **Saving a Project as CSV**
The following code snippet shows how to save a project as a CSV format.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-SaveProjectAsCSV-SaveProjectAsCSV.cs" >}}


The following lines of code show how to write string data to a project using CsvOptions, DataCategory and CsvTextDelimiter.

{{< highlight java >}}

 string CSV = @"ID;Resource_Name;Group_Name;Max_Units;Peak;Std_Rate;Ovt_Rate;Cost;Work

1;Clerical Support;Office;200%;100%;$50.00/hr;$0.00/hr;$1600.00;32 hrs

2;Sales Engineer;Office;100%;200%;$80.00/hr;$0.00/hr;$15360.00;192 hrs

3;Scheduler;Office;200%;100%;$60.00/hr;$0.00/hr;$1920.00;32 hrs

4;Systems Engineer;Office;200%;200%;$80.00/hr;$0.00/hr;$21120.00;264 hrs

5;Bid Manager;Office;100%;200%;$100.00/hr;$0.00/hr;$9600.00;96 hrs" + Environment.NewLine;

string writtenCSV;

CsvOptions options = new CsvOptions();

options.DataCategory = DataCategory.Resources;

options.TextDelimiter = CsvTextDelimiter.Semicolon;

options.Filter = new FilterWorkResources();

using (MemoryStream ms = new MemoryStream())

{

    project.Save(ms, options);

    ms.Seek(0, SeekOrigin.Begin);

    using (StreamReader sr = new StreamReader(ms, options.Encoding))

    {

        writtenCSV = sr.ReadToEnd();

    }

}

//Verify

if(CSV == writtenCSV)

    Console.WriteLine("Both the strings are equal");

{{< /highlight >}}
## **Save Project to Text**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-SaveProjectAsText-SaveProjectAsText.cs" >}}
## **Save Project Data as Template (MPT)**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-SaveProjectDataAsTemplate-SaveProjectDataAsTemplate.cs" >}}
