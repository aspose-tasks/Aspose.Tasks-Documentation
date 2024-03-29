---
title: Stop or Resume an Assignment
description: "Learn how to stop or resume Microsoft Project (MPP/XML) resource assignments using Aspose.Tasks for .NET."
type: docs
weight: 80
url: /net/stop-or-resume-an-assignment/
---

## **Stop or Resume an Assignment**
The [Asn](https://reference.aspose.com/tasks/net/aspose.tasks/asn) class exposes properties for reading and writing an assignment's stop and resume date:

- Stop reads or writes an assignment's stop date (DateTime).
- Resume reads or writes an assignment's resume date (DateTime).

To see an assignment's stop and resume dates in Microsoft Project:

1. On the Task Usage screen, select **Insert** and then **Column**.
2. Add the desired columns.

### **Getting an Assignment's Stop and Resume Dates using Aspose.Tasks**
If an assignment hasn't been stopped, the stop and resume dates have the value NA. In the evaluation version of Aspose.Tasks, values equal to NA gets the value "1/1/2000". In the licensed version, NA values equal DateTime.MinValue.

In the following example, an assignment's stop and resume dates are displayed in a console window after the code's traversed the assignments in the project.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithResourceAssignments-GetResourceAssignmentStopResumeDates.cs" >}}
