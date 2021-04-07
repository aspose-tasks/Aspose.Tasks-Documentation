---
title: Reading Resource Timephased Data
description: "Learn how to work with Microsoft Project (MPP/XML) resource timephased data using Aspose.Tasks for C++."
type: docs
weight: 80
url: /cpp/reading-timephased-data/
---

{{% alert color="primary" %}} 

Aspose.Tasks for C++ API supports reading a resource's timephased data from Microsoft Project (MPP) files.

{{% /alert %}}

## **Reading Timephased Resource Data**
The Timephased data is retrieved using the Resource object's TimeScaleData method. For Timephased data of *resource work*, the

- The TimeScaleData method gets the timephased data for resource work and takes the project's start and finish dates as input parameters.
- To get the timephased data for resource cost, the TimeScaleData method takes another input parameter - the timephased data type as a ResourceCost.

The following code example demonstrates reading the Timephased data of a Resource.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithResources-ReadResourceTimephasedData-ReadResourceTimephasedData.cpp" >}}
