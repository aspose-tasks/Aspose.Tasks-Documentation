---
title: Rendering Resource Sheet View
description: "Learn how to render resource sheet view of Microsoft Project (MPP/XML) files using Aspose.Tasks for .NET."
type: docs
weight: 110
url: /net/rendering-resource-sheet-view/
---

Microsoft Project's Resource Sheet view provides details about all a project's resources. Resource information such as name, type, standard and overtime rates, costs, and calendar can be viewed using this view. Aspose.Tasks for .NET API supports rendering the Resource Sheet to PDF using the PresentationFormat enumerator.

## **Rendering Resource Sheet View**
The code snippet in this article reads a source MPP file that has a number of resources and renders these to output PDF using the following steps:

1. Create an instance of Project Reader.
2. Read the source MPP file.
3. Set the [PresentationFormat](https://reference.aspose.com/tasks/net/aspose.tasks.visualization/presentationformat) to ResourceSheet.
4. Render the project to output PDF.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithResources-RenderResourceSheetView.cs" >}}
