---
title: Render Project to Multipage TIFF
type: docs
weight: 20
url: /java/render-project-to-multipage-tiff/
---

{{% alert color="primary" %}} 

Aspose.Tasks lets you render Gantt chart to multipage TIFFs.

The SaveFileFormat enumeration contains the available output options, including TIFF. The project can be rendered to TIFF with or without compression; supported compression schemes are RLE, CCITT3, CCITT4 and LZW.

{{% /alert %}} 
## **Rendering to Multipage TIFF**
The following code sample:

1. Reads a project file.
1. Sets the output file format.
1. Applies compression and saves an image to disk.
1. Removes compression and saves an image to disk.
### **Code Example**
**Java**

{{< highlight java >}}

 //Source file to be converted to TIFF

String file = "RenderMe.mpp";

Project project = new Project(file);

//Save the project to TIFF

project.save("RenderMe.tif", SaveFileFormat.TIFF);

//Save the project with CCITT4 compression

ImageSaveOptions options = new ImageSaveOptions(SaveFileFormat.TIFF);

options.setTiffCompression(TiffCompression.Ccitt4);

project.save("RenderMe_options.tif", options);

//Remove the compression

options.setTiffCompression(TiffCompression.None);

project.save("RenderMe_comp_none.tif", options);

{{< /highlight >}}
