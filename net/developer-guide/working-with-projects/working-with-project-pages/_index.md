---
title: Working with Project Pages
description: "Learn how to calculate the total number of pages while exporting Microsoft Project (MPP/XML) documents in graphical formats using Aspose.Tasks for .NET."
type: docs
weight: 70
url: /net/working-with-project-pages/
---

Aspose.Tasks for .NET can retrieve the total number of pages in a project. The [GetPageCount](https://apireference.aspose.com/tasks/net/aspose.tasks/project/methods/getpagecount) method offered by [Aspose.Tasks.Visualization](https://apireference.aspose.com/tasks/net/aspose.tasks.visualization) namespace returns the total page count in a project with options of rendering them based on [Timescale.Days](https://apireference.aspose.com/tasks/net/aspose.tasks.visualization/timescale), Timescale.Months or Timescale.ThirdsOfMonths.

## **Get Number of Pages in Project**
The [Project](https://apireference.aspose.com/tasks/net/aspose.tasks/project) class exposes the GetPageCount method which is used to get the number of total pages in a project. The total count of pages in a project can be retrieved for Timescale.Days, Timescale.Months or Timescale.ThirdsOfMonths.

To save a project to PDF:

1. Load a Microsoft Project file.
2. Get the project's total page count using the GetPageCount method with optional timescale settings.

### **Programming Sample: Get Number of Pages in Project**
The following lines of code shows how to achieve this using C#.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-GetNumberOfPages-GetNumberOfPages.cs" >}}

### **Programming Sample: Get the number of pages for different Views**
Aspose.Tasks supports rendering a project's resource usage, resource sheet and task usage to PDF format, and enables users to get the number of pages in the rendered output for these views. This programming sample demonstrates rendering a projects' usage view and getting the number of pages in the rendered output.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-GetNumberOfPagesForViews-GetNumberOfPagesForViews.cs" >}}

### **Programming Sample: Get number of pages based on Start and End Dates**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithProjects-GetPageCountOnStartAndEndDates-GetPageCountOnStartAndEndDates.cs" >}}
