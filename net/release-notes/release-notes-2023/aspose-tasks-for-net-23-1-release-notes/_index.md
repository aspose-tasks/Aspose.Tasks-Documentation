---
title: Aspose.Tasks for .NET 23.1 Release Notes
description: "The page contains the release notes for Aspose.Tasks for .NET 23.1."
type: docs
weight: 100
url: /net/aspose-tasks-for-net-23-1-release-notes/
---

{{% alert color="primary" %}} 

This page contains release notes information for [Aspose.Tasks for .Net 23.1](https://downloads.aspose.com/tasks/net/new-releases/aspose.tasks-for-.net-23.1/).

{{% /alert %}}
## **All Changes**
|**Key**|**Summary**|**Issue Type**|
| :- | :- | :- |
| TASKSNET-10758 | Add an API to access values of Labor Units for projects read from Primavera formats | Enhancement |
| TASKSNET-10756 | Fix reading of task priority column for MPX files where Priority column was saved using enum values. | Enhancement |
| TASKSNET-10755 | Add an API to access fractional number values of Physical Percent Complete and PercentComplete for projects read from Primavera formats. | Enhancement |
| TASKSNET-10759 | Fix calculation of summary task's Duration property for project read from Primavera format: it should correspond to 'Original Duration', not to 'At Completion Duration'. | Bug |
| TASKSNET-10757 | Fix writing of MPX file to fix import errors reported by Microsoft Project 98 when importing MPX file created by Aspose.Tasks. | Bug |
| TASKSNET-10746 | Fix missing constraint dates when saving the specific project | Bug |
| TASKSNET-10745 | Fix IndexOutOfRangeException when saving the specific file to MPX format | Bug |
| TASKSNET-10743 | Fix reading of timephased data from MPP format | Bug |
| TASKSNET-10734 | Fix standard calendar's days are shown as non-working in MS Project when opening a project created without a template | Bug |
| TASKSNET-10740 | Fix reading of Link lag value when reading project from XER file | Bug |

## **Public API and Backwards Incompatible Changes**
|**The following public methods and properties were added:**|**Description**|
| :- | :- |
| Aspose.Tasks.PrimaveraTaskProperties.PhysicalPercentComplete | Gets the value of Physical Percent Complete. |
| Aspose.Tasks.PrimaveraTaskProperties.DurationPercentComplete | Gets the value of duration percent complete. |
| Aspose.Tasks.PrimaveraTaskProperties.UnitsPercentComplete | Gets the value of units percent complete. |
| Aspose.Tasks.PrimaveraTaskProperties.ActualLaborUnits | Gets the value of actual labor units. |
| Aspose.Tasks.PrimaveraTaskProperties.ActualNonLaborUnits | Gets the value of actual non labor units. |
| Aspose.Tasks.PrimaveraTaskProperties.RemainingLaborUnits | Gets the value of remaining labor units. |
| Aspose.Tasks.PrimaveraTaskProperties.RemainingNonLaborUnits | Gets the value of remaining non labor units. |


## **Examples and additional notes**

**Related issue: TASKSNET-10759 - Fix calculation of summary task's Duration property for project read from Primavera format: it should correspond to 'Original Duration', not to 'At Completion Duration'.**

Before 23.1 there were inconsistency with 'Duration' property for tasks read from Primavera P6 XML or XER format.
Duration of non-summary tasks was set to Primavera's 'Original Duration' column, whilst duration of summary tasks was calculated as 'At Completion Duration'.

We fixed the behavior in 23.1 and now 'Duration' for summary and non-summary tasks should correspond to 'Original Duration' column of Primavera P6.
The value of 'At Completion Duration' property can be get as a sum of task.ActualDuration and task.RemainingDuration.