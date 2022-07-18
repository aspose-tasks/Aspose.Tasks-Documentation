---
title: Rendering Task Sheet View
description: "Learn how to render Microsoft Project (MPP/XML) task sheet views using Aspose.Tasks for .NET."
type: docs
weight: 260
url: /net/rendering-task-sheet-view/
---

Aspose.Tasks for .NET supports rendering project tasks to a variety of formats, such as PDF. Task sheets can be rendered using [PresentationFormat](https://reference.aspose.com/tasks/net/aspose.tasks.visualization/presentationformat) of Aspose.Tasks for .NET API.

## **Rendering Task Sheet View**
The code snippet in this article reads a source MPP file that has a number of tasks with assigned resources and renders these to output PDF using the following steps:

1. Create an instance of the [Project](https://reference.aspose.com/tasks/net/aspose.tasks/project) class.
2. Read the source MPP file.
3. Initiate the [SaveOptions](https://reference.aspose.com/tasks/net/aspose.tasks.saving/saveoptions) object with required timescale settings.
4. Set the presentation format to TaskSheet.
5. Render the project to PDF output.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-RenderTaskSheetView.cs" >}}
