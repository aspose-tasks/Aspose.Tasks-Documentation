---
title: Rendering Task Sheet View
description: "Learn how to render Microsoft Project (MPP/XML) task sheet views using Aspose.Tasks for Java."
type: docs
weight: 260
url: /java/rendering-task-sheet-view/
---

Aspose.Tasks for Java supports rendering project tasks to a variety of formats, such as PDF. Task sheets can be rendered using Aspose.Tasks' PresentationFormat.

**Rendering Task Sheet View**
The code snippet in this article reads a source MPP file that has a number of tasks with assigned resources and renders these to output PDF using the following steps:

1. Create an instance of the Project Reader.
2. Read the source MPP file.
3. Initiate the SaveOptions object with required timescale settings.
4. Set the presentation format to TaskSheet.
5. Render the project to PDF output.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-RenderTaskSheet-render-task-sheet-view.java" >}}
