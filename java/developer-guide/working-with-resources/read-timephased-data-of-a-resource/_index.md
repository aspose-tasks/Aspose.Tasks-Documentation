---
title: Read Timephased Data of a Resource
type: docs
weight: 80
url: /java/read-timephased-data-of-a-resource/
---

{{% alert color="primary" %}} 

Aspose.Tasks supports reading a resource's timephased data from Microsoft Project (MPP) files.

{{% /alert %}} 
## **Reading Timephased Resource Data**
The Timephased data is retrieved using the [Resource](http://www.aspose.com/api/java/tasks/com.aspose.tasks/classes/Resource) object's Timescaledata method. For time-phased data of resource work,

- The Timescaledata method gets the time-phased data for resource work and takes the project's start and finish dates as input parameters.
- To get the time-phased data for resource cost, the Timesclatedata method takes another input parameter - the time-phased data type as a ResourceCost.

**Programming Sample**

The following piece of code shows to read a resource's time-phased data.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Resources-ReadTimephasedData-reading-time-phases-data.java" >}}
