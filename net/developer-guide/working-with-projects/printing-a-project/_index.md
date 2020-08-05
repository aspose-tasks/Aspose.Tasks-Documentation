---
title: Printing a Project
type: docs
weight: 60
url: /net/printing-a-project/
---

{{% alert color="primary" %}} 

Aspose.Tasks provides the facility to print projects to the default printer or any custom printer using the Project.Print function. It also provides advanced printing features like changing the printing options and settings.

{{% /alert %}} 
## **Printing Project Data**
The [Project]() class exposes the [Print](http://www.aspose.com/api//net/tasks/aspose.tasks/project/methods/print/index) function to print the project. The Print function uses [PrintOptions](http://www.aspose.com/api/net/tasks/aspose.tasks.saving/printoptions) to set different settings for printing like TimeScale, StartDate, EndDate, FitContent, LegendOnEachPage and more. Another class (from System.Drawing.Printing namespace), PrinterSettings is used to configure the printer to print all pages, page start (FromPage), page end (ToPage), PaperSize and so on. Both the objects of PrintOptions and PrinterSettings are passed to Project.Print() for final printing.

To print a project:

1. Load a Microsoft Project file.
1. Call the print function along with the specified arguments.
### **Print to the Default Printer**
The following lines of code shows how to achieve this using C#.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-Printing-PrintTheProject-PrintTheProject.cs" >}}
### **Print the project to a custom printer**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-Printing-PrintProjectUsingCustomPrinter-PrintProjectUsingCustomPrinter.cs" >}}
### **Print Large Files**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-Printing-PrintLargeFiles-PrintLargeFiles.cs" >}}
### **Print with PrintOptions and PrinterSettings**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-Printing-PrintPrintOptionsAndPrinterSettings-PrintPrintOptionsAndPrinterSettings.cs" >}}
