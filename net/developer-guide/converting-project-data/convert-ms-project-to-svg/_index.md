---
title: Convert MS Project to SVG
type: docs
weight: 40
url: /net/convert-ms-project-to-svg/
---

{{% alert color="primary" %}} 

This article shows how to render project data to SVG format using Aspose.Tasks for .NET.

{{% /alert %}} 


## **Saving a Project as SVG**
The [Project]() class exposes the Save method which is used to save a project in various formats. The Save method allows you to render project data to SVG format using the SaveFileFormat enumeration type.

To save a project to SVG:

1. Load a Microsoft Project file.
1. Save the project to SVG using SaveFileFormat.SVG.
### **Programming Sample**
The following lines of code shows how to achieve this using C#.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-SaveProjectAsSVG-SaveProjectAsSVG.cs" >}}
## **Saving with SvgOptions**
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-UsingSvgOptions-UseSvgOptions.cs" >}}
