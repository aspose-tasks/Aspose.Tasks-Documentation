---
title: Rendering Resource Usage View
description: "Learn how to render resource usage view of Microsoft Project (MPP/XML) files using Aspose.Tasks for .NET."
type: docs
weight: 100
url: /net/rendering-resource-usage-view/
---

{{% alert color="primary" %}}

Being able to render individual project views, for example, resource usage against tasks is a common requirement for a developer who works with Microsoft Project (MPP/XML) files. Aspose.Tasks for .NET API supports this requirement and lets you render project resources to various formats e.g. PDF. Resource usage can be rendered using Aspose.Tasks' [PresentationFormat](https://reference.aspose.com/tasks/net/aspose.tasks.visualization/presentationformat) with different timescale settings like Days, ThirdOfMonths and Months.

{{% /alert %}}

## **Rendering Resource Usage View**
The code snippet in this article reads a source MPP file that has a number of resources assigned to tasks and renders these to an output PDF using the following steps:

1. Create an instance of the Project Reader.
2. Read the source MPP file.
3. Initiate the SaveOptions object with the required timescale settings.
4. Set the presentation format to Resource Sheet.
5. Render the project to PDF output.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithResources-RenderResourceUsageView.cs" >}}
