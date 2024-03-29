---
title: Aspose.Tasks for C++ 22.6 Release Notes
description: "The page contains the release notes for Aspose.Tasks for C++ 22.6."
type: docs
weight: 95
url: /cpp/aspose-tasks-for-cpp-22-6-release-notes/
---

{{% alert color="primary" %}} 

This page contains release notes information for [Aspose.Tasks for C++ 22.6](https://downloads.aspose.com/tasks/cpp/new-releases/aspose.tasks-for-c---22.6/).

{{% /alert %}}
## **All Changes**
|**Key**|**Summary**|**Issue Type**|
| :- | :- | :- |
| TASKSNET-10556 | Add IsRoot property to Resource object | Enhancement |
| TASKSNET-10553 | Add properties to access ResourceAssignment's Task and Resource | Enhancement |
| TASKSNET-10469 | Add support of reading of User Defined Types for Primavera P6 XML format | Enhancement |
| TASKSNET-10554 | Fix incorrect calculation of Asn.Finish for assignments with Asn.Units not equal 1 | Bug |
| TASKSNET-10552 | Fix NullReference exception when reading/writing file with absent "TBknAssn.Props" stream | Bug |
| TASKSNET-10569 | Fix resource rate's RateTo property is set incorrectly when reading project from Primavera P6 XML format | Bug |

## **Public API and Backwards Incompatible Changes**
|**The following public methods and properties were added:**|**Description**|
| :- | :- |
| Aspose.Tasks.OutlineCode.#ctor(Aspose.Tasks.OutlineCodeDefinition,Aspose.Tasks.OutlineValue) | Initializes a new instance of the <see cref="T:Aspose.Tasks.OutlineCode" /> class using the specified Outline Code and one of its values. |
| Aspose.Tasks.Resource.IsRoot | Gets the flag indicating whether resource is a root resource. |
| Aspose.Tasks.ResourceAssignment.Task | The task to which a resource is assigned. |
| Aspose.Tasks.ResourceAssignment.Resource | The resource assigned to a task. |


## **Examples and additional notes**

**Related issue: TASKSNET-10553 - Add properties to access ResourceAssignment's Task and Resource**

Task and Resource read-only properties were added for more convenient access to frequently used properties.


{{< highlight cpp >}}
auto project = System::MakeObject<Project>(System::String(u"test.mpp"));
auto assignment = project->get_ResourceAssignments()->GetByUid(1);

// Before: 
auto taskName = assignment->Get(Asn::Task())->Get(Tsk::Name());
// After:
auto taskName = assignment->get_Task()->Get(Tsk::Name());

{{< /highlight >}}