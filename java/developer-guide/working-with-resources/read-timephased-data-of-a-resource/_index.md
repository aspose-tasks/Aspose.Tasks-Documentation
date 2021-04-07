---
title: Read Timephased Data of a Resource
description: "Learn how to read  Microsoft Project (MPP/XML) resource timephased data using Aspose.Tasks for Java."
type: docs
weight: 80
url: /java/read-timephased-data-of-a-resource/
---

Aspose.Tasks for Java supports reading a resource's timephased data from Microsoft Project (MPP) files.

**Reading Timephased Resource Data**
The timephased data is retrieved using the [Resource](https://apireference.aspose.com/tasks/java/com.aspose.tasks/Resource) object's TimeScaleData method. For time-phased data of resource work,

- The TimeScaleData method gets the time-phased data for resource work and takes the project's start and finish dates as input parameters.
- To get the time-phased data for resource cost, the TimeScaleData method takes another input parameter - the time-phased data type as a ResourceCost.

The following piece of code shows to read a resource's time-phased data.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Resources-ReadTimephasedData-reading-time-phases-data.java" >}}
