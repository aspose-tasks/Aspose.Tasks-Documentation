---
title: Read Timephased Data of a Resource
type: docs
weight: 80
url: /net/read-timephased-data-of-a-resource/
---

{{% alert color="primary" %}} 

Aspose.Tasks supports reading a resource's timephased data from Microsoft Project (MPP) files.

{{% /alert %}} 
## **Reading Timephased Resource Data**
The Timephased data is retrieved using the [Resource]() object's Timescaledata method. For Timephased data of *resource work*, the

- The Timescaledata method gets the timephased data for resource work and takes the project's start and finish dates as input parameters.
- To get the timphased data for resource cost, the Timesclatedata method takes another input parameter - the timephase data type as a ResourceCost.

The following piece of code shows reading the Timephased data of a Resource.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithResources-ReadResourceTimephasedData-ReadResourceTimephasedData.cs" >}}
