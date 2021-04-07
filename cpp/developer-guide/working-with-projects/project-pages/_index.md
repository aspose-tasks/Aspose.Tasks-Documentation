---
title: Project Pages
type: docs
weight: 50
url: /cpp/project-pages/
---

{{% alert color="primary" %}} 

Aspose.Tasks for C++ can retrieve the total number of pages in a project. The GetPageCount method offered by Aspose.Tasks' Visualization namespace returns the total page count in a project with options of rendering them based on Timescale.Days, Timescale.Months or Timescale.ThirdsOfMonths.

{{% /alert %}}

## **Get Number of Pages in Project**
The Project class exposes the GetPageCount method which is used to get the number of total pages in a project. The total count of pages in a project can be retrieved for Timescale.Days, Timescale.Months or Timescale.ThirdsOfMonths.

To save a project to PDF:

1. Load a Microsoft Project file.
2. Get the project's total page count using the GetPageCount method with optional timescale settings.

### **Programming Sample: Get Number of Pages in Project**
The following lines of code demonstrate how to get a number of pages in the project.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-GetNumberOfPages-GetNumberOfPages.cpp" >}}

### **Programming Sample: Get the number of pages for different Views**
Aspose.Tasks for C++ supports rendering a project's resource usage, resource sheet and task usage to PDF format, and enables users to get the number of pages in the rendered output for these views. This programming sample demonstrates rendering a projects' usage view and getting the number of pages in the rendered output.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-GetNumberOfPagesForViews-GetNumberOfPagesForViews.cpp" >}}

### **Programming Sample: Get number of pages based on Start and End Dates**

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-GetPageCountOnStartAndEndDates-GetPageCountOnStartAndEndDates.cpp" >}}
