---
title: Aspose.Tasks for .NET - Performance Metrics and Benchmarks
type: docs
weight: 20
url: /net/aspose-tasks-for-net-performance-metrics-and-benchmarks/
---

## **Disclaimer**
{{% alert color="primary" %}} 

This document is provided for information purposes only and the contents hereof are subject to change every quarter of the year. This document is not warranted to be error-free, nor subject to any other warranties or conditions, whether expressed orally or implied in law including implied warranties and conditions of merchantability or fitness for a particular purpose. We specifically disclaim any liability with respect to this document and no contractual obligations are formed either directly or indirectly by this document. This document may not be reproduced or transmitted in any form or by any means, electronic or mechanical, for any purpose.

{{% /alert %}} 
## **Purpose**
Performance is often the first critical factor when choosing a component. This article measures the performance of Aspose.Tasks for .NET. The tests are conducted across the commonly used operating system, hardware components, and configurations.

Performance estimates presented here are intended to help you understand what to expect from Aspose.Tasks for .NET. Naturally, your application performance depends on your data, data access patterns, cache size, other configuration parameters, operating system and hardware etc. The benchmark aims to illustrate how the components perform under minimum hardware conditions, the faster the hardware, the faster the tasks will be processed by the components.
## **Overview**
Benchmarks provide guidelines and help to set basic operational expectations. The topic shows benchmark tests that have been performed against Aspose.Tasks for .NET. The Performance Measures allow even novice users to benchmark the performance of the component they are using. The tests will allow you to objectively benchmark the Aspose.Tasks for .NET using a variety of different speed tests. All the tasks are common and carefully chosen.
## **Testing Methodology**
All the performance tests were conducted on a commonly used hardware and operating system combinations, without customized configuration, tuning or any other performance enhancing techniques. To get accurate readings, we performed all the tasks twice / thrice at a time to better evaluate a component and to get accurate readings.
## **Test Environment**
Windows Vista Home Premium over Intel Core™ 2 Duo 1.83GHz 4 GB of RAM
## **Test Scenarios**
The tests were performed on reading and writing the large project files having a size ranging between 6 – 40 MB. MPP files with 1000 - 8000 records were created using Microsoft Project 2007 and loaded through Aspose.Tasks for .NET 3.6.0. Same files were saved to XML format using Aspose.Tasks for .NET 3.6.0.
## **Results**

|**File Size**|**Number of Records**|**Class/Method Name**|**Scenario Description**|**Time Consumed**|**Comments**|
| :- | :- | :- | :- | :- | :- |
|6 MB|1000|ProjectReader.Read|Test performed on file load|13 Seconds|Pass|
|6 MB|1000|ProjectReader.Write|Test performed on file save|2 Seconds|Pass|
|11 MB|2000|ProjectReader.Read|Test performed on file load|18 Seconds|Pass|
|11 MB|2000|ProjectReader.Write|Test performed on file save|5 Seconds|Pass|
|15 MB|3000|ProjectReader.Read|Test performed on file load|30 Seconds|Pass|
|15 MB|3000|ProjectReader.Write|Test performed on file save|10 Seconds|Pass|
|40 MB|8000|ProjectReader.Read|Test performed on file load|120 Seconds|Pass|
|40 MB|8000|ProjectReader.Write|Test performed on file save|55 Seconds|Pass|

