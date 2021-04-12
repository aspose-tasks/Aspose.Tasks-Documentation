---
title: Working with Project Pages
description: "Learn how to calculate the total number of pages while exporting Microsoft Project (MPP/XML) documents in graphical formats using Aspose.Tasks for Java."
type: docs
weight: 40
url: /java/working-with-project-pages/
---

Aspose.Tasks for Java can retrieve the total number of pages in a project. The getPageCount method offered by Aspose.Tasks' Visualization namespace returns the total page count in a project with options of rendering them based on Timescale.Days, Timescale.Months or Timescale.ThirdsOfMonths.

## **Getting number of pages in a project**
The [Project](https://apireference.aspose.com/tasks/java/com.aspose.tasks/project) class exposes the getPageCount method which is used to get the number of total pages in a project. The total count of pages in a project can be retrieved for Timescale.Days, Timescale.Months or Timescale.ThirdsOfMonths.

To save a project to PDF:

1. Load a Microsoft Project file.
2. Get the project's total page count using the getPageCount method with optional timescale settings.

**Programming Sample: Get Number of Pages in Project**
The following lines of code shows how to achieve this using Java:

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-GetNumberOfPagesInProject-read-number-of-pages-in-project.java" >}}

**Programming Sample: Get Number of Pages for Different Views**
Aspose.Tasks for Java supports rendering a project's resource usage, resource sheet and task usage to PDF format, and enables users to get the number of pages in the rendered output for these views. This programming sample demonstrates rendering a projects' usage view and getting the number of pages in the rendered output.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-GetNumberOfPagesInProject-read-number-of-pages-in-different=views.java" >}}

**Programming Sample: Get number of pages based on Start and End Dates**

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-GetNumberOfPagesInProject-GetPageCountBetweenStartAndEndDates.java" >}}
