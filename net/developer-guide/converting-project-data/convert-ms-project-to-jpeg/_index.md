---
title: Convert Microsoft Project MPP file to JPEG
description: "Aspose.Tasks for .NET allows converting Microsoft Project (MPP) to JPEG."
keywords: "Export your project to JPEG, MPP to JPG, Convert your MPP to Image, Convert Microsoft Project to JPEG, convert MPP to JPG, save project data to JPEG, Aspose.Tasks, C#"
type: docs
weight: 20
url: /net/convert-ms-project-mpp-to-jpeg/
aliases: 
    - /net/convert-ms-project-to-jpeg/
---

JPEG or JPG is a commonly image format which is using lossy compression. The degree of compression can be adjusted, allowing a selectable trade-off between storage size and image quality. Aspose.Tasks for .NET API lets you save MS Project MPP file to JPEG file format. You can also specify quality of the resulting image(-s).

## **Exporting Project Data to JPEG**

To save a project to JPEG programmatically using Aspose.Tasks for .NET:

1. Load a Microsoft Project MPP file.
2. Optionally make changes to the loaded project.
3. Save the project to JPEG using one of Project.Save method overloads.
Your can pass either SaveFileFormat.JPEG to save project with default settings or pass ImageSaveOptions to customize export options.

The following [article](/tasks/net/common-conversions-options/) describes properties common for all graphical formats.

Also additional options specific to JPEG format can specified. For example, [ImageSaveOptions.JpegQuality](https://reference.aspose.com/tasks/net/aspose.tasks.saving/imagesaveoptions/properties/jpegquality) can be used to set quality of the resulting JPEG file..

Also, the horizontal and vertical resolution in dpi can be controlled using [ImageSaveOptions.HorizontalResolution](https://reference.aspose.com/tasks/net/aspose.tasks.saving/imagesaveoptions/properties/horizontalresolution) and [ImageSaveOptions.VerticalResolution](https://reference.aspose.com/tasks/net/aspose.tasks.saving/imagesaveoptions/properties/verticalresolution).


The code example given below demonstrates how to export your project data to JPEG.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ConvertingProjectData-SaveProjectAsJPEG.cs" >}}
