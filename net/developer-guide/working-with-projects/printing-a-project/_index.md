---
title: Printing a Microsoft Project files
description: "Learn how to print Microsoft Project files using Aspose.Tasks for .NET."
type: docs
weight: 60
url: /net/printing-a-project/
---

Aspose.Tasks for .NET provides the facility to print projects to the default printer or any custom printer using the Project.Print function. It also provides advanced printing features like changing the printing options and settings.

## **Printing Project Data**
The [Project](https://apireference.aspose.com/tasks/net/aspose.tasks/project) class exposes the [Print](https://apireference.aspose.com/tasks/net/aspose.tasks/project/methods/print/index) function to print the project. The Print function uses [PrintOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/printoptions) to set different settings for printing like **TimeScale**, **StartDate**, **EndDate**, **FitContent**, **LegendOnEachPage** and more. Another class (from [System.Drawing.Printing](https://apireference.aspose.com/drawing/net/system.drawing.printing) namespace), PrinterSettings is used to configure the printer to print all pages, page start (FromPage), page end (ToPage), PaperSize and so on. Both the objects of PrintOptions and PrinterSettings are passed to Project.Print() for final printing.

To print a project:

1. Load a Microsoft Project file.
2. Call the print function along with the specified arguments.

### **Print to the Default Printer**
The following lines of code shows how to achieve this using C#.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-Printing-PrintTheProject-PrintTheProject.cs" >}}

### **Print the project to a custom printer**

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-Printing-PrintProjectUsingCustomPrinter-PrintProjectUsingCustomPrinter.cs" >}}

### **Print Large Files**

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-Printing-PrintLargeFiles-PrintLargeFiles.cs" >}}

### **Print with PrintOptions and PrinterSettings**

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-Printing-PrintPrintOptionsAndPrinterSettings-PrintPrintOptionsAndPrinterSettings.cs" >}}
