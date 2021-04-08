---
title: Rendering Project Data on Pre-Defined Page sizes
type: docs
weight: 10
url: /java/rendering-project-data-on-pre-defined-page-sizes/
---

{{% alert color="primary" %}} 

Aspose.Tasks for Java supports rendering project views such as Gantt charts, task usage, resource usage and resource sheets to pre-defined page sizes, for example A0, A1, Letter, etc. The PageSize enumerator provides the following pre-defined page sizes:

- A0
- A1
- A2
- A3
- A4
- Ledger
- Letter

{{% /alert %}} 
## **Rendering Project Data to Pre-Defined Page Sizes**
The following code sample shows how to render a project's different views to pre-defined page sizes.

**Java**

{{< highlight java >}}

 //Source File to Render

//Source File to Render

String file = "RenderMe.mpp";

Project project = new Project(file);

//Render the project to A3 size

PdfSaveOptions options = new PdfSaveOptions();

options.setPresentationFormat(PresentationFormat.GanttChart);

options.setFitContent(true);

options.setPageSize(PageSize.A3);

String resFile = "result_" + "Gantt chart" + "_" + PageSize.A3 + ".pdf";

project.save(resFile, options);

{{< /highlight >}}
