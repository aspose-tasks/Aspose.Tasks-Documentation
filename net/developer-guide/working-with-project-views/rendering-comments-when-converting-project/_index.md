---
title: Rendering Notes When Converting MS Project MPP file
description: "Aspose.Tasks for .NET allows rendering of notes (or comments) while converting MS Project MPP file to PDF or graphical formats."
keywords: "Export project task, resources or assignments with comments, convert mpp project with notes, render notes when exporting mpp project, Aspose.Tasks, C#"
type: docs
weight: 90
url: /net/rendering-comments-when-converting-project/
---

MS Project allows the user to add notes for task, resource or assignment. Notes field contains comment in Rich Text Format:
![Example of task note in MS Project](task_notes_msp.png).

MS Project has "Print notes" setting in view's "Page Setup" dialog. The setting allows the notes to be rendered when project is saved to PDF via "Save As" command.

![Print notes setting in MS Project](print_notes_msp.png)

## **Rendering Task, Resource or Assignment Notes When Converting Project Using Aspose.Tasks for .NET**
Aspose.Tasks for .NET provides [PageViewSettings](https://reference.aspose.com/tasks/net/aspose.tasks.visualization/pageinfo/properties/pageviewsettings).[PrintNotes](https://reference.aspose.com/tasks/net/aspose.tasks.visualization/pageviewsettings/properties/printnotes) flag property to determine whether to print notes under [PageInfo](https://reference.aspose.com/tasks/net/aspose.tasks.visualization/pageinfo).


The following code snippets demonstrates how to enable rendering of task, resource or assignment's comments when saving the project as an image, HTML or PDF file.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-RenderCommentsWhenConverting.cs" >}}

The notes are rendered on last page(-s) of the resulting document.
