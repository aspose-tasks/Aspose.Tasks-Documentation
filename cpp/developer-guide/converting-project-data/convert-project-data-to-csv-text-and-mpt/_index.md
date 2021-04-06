---
title: Convert Project Data to CSV, Text and MPT
type: docs
weight: 30
url: /cpp/convert-project-data-to-csv-text-and-mpt/
---

{{% alert color="primary" %}} 

Microsoft Project (MSP) allows developers to save project data (MPP/XML) comma-delimited (CSV), text and MPT templates. Aspose.Tasks for C++ API also allows you to save project data to the same formats similar to MSP. This is achieved using the standard Save method exposed by the [Project](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project) class.

{{% /alert %}} 


## **Saving a Project as CSV**
The following code snippet shows how to save a project as a CSV format.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-ConvertingProjectData-SaveProjectAsCSV-SaveProjectAsCSV.cpp" >}}

The following lines of code demonstrate how to write string data to a project using CsvOptions, DataCategory and CsvTextDelimiter.

{{< highlight csharp >}}

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
{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-ConvertingProjectData-SaveProjectAsText-SaveProjectAsText.cpp" >}}
## **Save Project Data as Template (MPT)**
{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-ConvertingProjectData-SaveProjectDataAsTemplate-SaveProjectDataAsTemplate.cpp" >}}
