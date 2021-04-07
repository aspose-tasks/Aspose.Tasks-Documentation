---
title: Writing Metadata to MPP
description: "Learn how to write metadata of tasks, calendars, resources, resource assignments using Aspose.Tasks for C++."
type: docs
weight: 50
url: /cpp/writing-metadata-to-mpp/
---

Aspose.Tasks for C++ API provides a facility for writing metadata to MPP files for calendars, tasks, task links, resources and resource assignments.

## **Writing Metadata to Microsoft Project Files**
The following metadata is used in this example:

- Calendar
  - CalendarName
- Task
  - Contact
  - IsMarked
  - IgnoreWarnings
- TaskLink
  - LagFormat
  - LinkLag
- Resource
  - Type
  - Initials
  - MaxUnits
  - Code
  - Group
  - EmailAddress
  - NTAccount
  - IsGeneric
  - AccrueAt
  - TeamAssignmentPool
  - CostCenter
- ResourceAssignment
  - Uid
  - Work
  - RemainingWork
  - RegularWork
  - Start
  - Finish

Here IsMarked and IgnoreWarnings are newly added fields for a task. Similarly for resources, the TeamAssignmentPool and CostCenter properties are provided.

The following steps are followed in the sample code to demonstrate how to write metadata to MPPs:

1. Open a new, blank MPP file.
2. Add working times on Monday of the project calendar and change the project calendar name.
3. Add three tasks with task links and lags.
4. Add two resources, one budget work and one budget cost resource (four in total).
5. Assign budget resources to the project root task (the project summary task).
6. Assign another two resources to the first and second tasks.
7. Set the project baseline.
8. Add a new task extended attribute.
9. Save changes as an MPP file.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-Miscellaneous-WriteMetadataToMPP-WriteMetadataToMPP.cpp" >}}
