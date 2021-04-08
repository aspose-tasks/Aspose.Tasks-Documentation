---
title: Rendering Resource Usage and Resource Sheet Views
description: "Learn how to read Microsoft Project (MPP/XML) resource usage and resource sheet views using Aspose.Tasks for Java."
type: docs
weight: 100
url: /java/rendering-resource-usage-and-resource-sheet-view/
---

Being able to render individual project views, for example resource usage against tasks, is a common requirement for developer who work with Microsoft Project files. Aspose.Tasks for Java supports this requirements and lets you render project resources to various formats, for example PDF. Resource usage can be rendered using Aspose.Tasks' PresentationFormat with different timescale settings like Days, ThirdOfMonths and Months.

## **Rendering Resource Usage View**
The code snippet in this article reads a source MPP file that has a number of resources assigned to tasks and renders these to an output PDF using the following steps:

1. Create an instance of the Project Reader.
2. Read the source MPP file.
3. Initiate the SaveOptions object with the required timescale settings.
4. Set the presentation format to Resource Sheet.
5. Render the project to PDF output.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Resources-RenderResourceUsageandsheetView-render-task-usage-view.java" >}}

## **Rendering Resource Sheet View**

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Resources-RenderResourceUsageandsheetView-render-resource-sheet-view.java" >}}
