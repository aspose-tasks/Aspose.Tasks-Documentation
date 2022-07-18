---
title: Read Timephased Data of a Resource
description: "Learn how to generate or edit timephased data of Microsoft Project (MPP/XML) resources using Aspose.Tasks for .NET."
type: docs
weight: 80
url: /net/read-timephased-data-of-a-resource/
---

Aspose.Tasks for .NET supports reading a resource's timephased data from Microsoft Project (MPP) files.

## **Reading Timephased Resource Data**
The Timephased data is retrieved using the [Resource](https://reference.aspose.com/tasks/net/aspose.tasks/resource) object's TimeScaleData method. For Timephased data of *resource work*, the

- The TimeScaleData method gets the timephased data for resource work and takes the project's start and finish dates as input parameters.
- To get the timephased data for resource cost, the TimeScaleData method takes another input parameter - the timephased data type as a ResourceCost.

The following piece of code shows reading the Timephased data of a Resource.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithResources-ReadResourceTimephasedData.cs" >}}
