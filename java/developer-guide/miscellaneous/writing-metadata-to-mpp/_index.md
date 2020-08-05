---
title: Writing Metadata to MPP
type: docs
weight: 30
url: /java/writing-metadata-to-mpp/
---

{{% alert color="primary" %}} 

Aspose.Tasks provides a facility for writing metadata to MPP files for calendars, tasks, task links, resources and resource assignments.

{{% /alert %}} 
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
  - NtAccount
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

Here IsMarked and IgnoreWarnings are newly added fields for a task. Similarly for resources, the TeamAssignmentPool and CostCenter properties are provided.

The following steps are followed in the sample code to demonstrate how to write metadata to MPPs:

1. Open a new, blank MPP file.
1. Add working times on Monday of the project calendar and change the project calendar name.
1. Add three tasks with task links and lags.
1. Add two resources, one budget work and one budget cost resource (four in total).
1. Assign budget resources to the project root task (the project summary task).
1. Assign another two resources to the first and second tasks.
1. Set the project baseline.
1. Add a new task extended attribute.
1. Save changes as an MPP file.
### **Writing Metadata**
{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Miscellaneous-WriteMetadata-WriteMetadata.java" >}}
