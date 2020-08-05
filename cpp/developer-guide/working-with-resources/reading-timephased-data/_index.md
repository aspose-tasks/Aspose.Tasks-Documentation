---
title: Reading Timephased Data
type: docs
weight: 80
url: /cpp/reading-timephased-data/
---

{{% alert color="primary" %}} 

Aspose.Tasks API supports reading a resource's timephased data from Microsoft Project (MPP) files.

{{% /alert %}} 
## **Reading Timephased Resource Data**
The Timephased data is retrieved using the Resource object's Timescaledata method. For Timephased data of *resource work*, the

- The Timescaledata method gets the timephased data for resource work and takes the project's start and finish dates as input parameters.
- To get the timphased data for resource cost, the Timesclatedata method takes another input parameter - the timephase data type as a ResourceCost.

The following code example demonstrates reading the Timephased data of a Resource.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithResources-ReadResourceTimephasedData-ReadResourceTimephasedData.cpp" >}}
