---
title: Rendering Task Sheet View
type: docs
weight: 260
url: /net/rendering-task-sheet-view/
---

{{% alert color="primary" %}} 

Aspose.Tasks supports rendering project tasks to a variety of formats, such as PDF. Task sheets can be rendered using [PresentationFormat](https://apireference.aspose.com/tasks/net/aspose.tasks.visualization/presentationformat) of Aspose.Tasks API.

{{% /alert %}} 
## **Rendering Task Sheet View**
The code snippet in this article reads a source MPP file that has a number of tasks with assigned resources and renders these to output PDF using the following steps:

1. Create an instance of the [Project](https://apireference.aspose.com/tasks/net/aspose.tasks/project) class.
1. Read the source MPP file.
1. Initiate the [SaveOptions](https://apireference.aspose.com/tasks/net/aspose.tasks.saving/saveoptions) object with required timescale settings.
1. Set the presentation format to TaskSheet.
1. Render the project to PDF output.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-RenderTaskSheetView-RenderTaskSheetView.cs" >}}
