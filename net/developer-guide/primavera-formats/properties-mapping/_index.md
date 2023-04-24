---
title: Primavera to Aspose.Tasks for .NET properties mapping
description: "Additional notes on mapping of fields from Primavera P6 formats (XER, P6XML) to Aspose.Tasks for .NET API."
type: docs
weight: 60
url: /net/primavera-formats/properties-mapping
---

Aspose.Tasks API is based on object model of Microsoft Project which differs from model used in Primavera software.
This can lead to confusion, particularly when certain properties share the same name in both models but are calculated differently.
To provide clarity, this article will outline the mapping of Primavera properties to properties of Aspose.Tasks API.

## **Task properties**

Primavera has two distinct entities for tasks: the WBS (Work Breakdown Structure) entity for summary tasks and the Activity 
entity for leaf tasks. However, Aspose.Tasks does not differentiate between these entities and uses the Task entity for mapping in both cases.
Task have PrimaveraPropeties property where values of Primavera-specific properties can be found. The properties are read only and are filled when project is read from Primavera format (XER of P6XML). The values of these properties are not recalculated during lifecycle of the project.
Contrary to this the properties which are mapped to Task's properties are recalculated according to Microsoft Project's logic during lifecycle of the project.


|**Name in Primavera P6**|**Aspose.Tasks for .NET property**|**Name in XER file**|**Name in Primavera XML file**|**Comment**|
| :- | :- | :- | :- |:- |
|Planned Start|Task.Start|target_start_date|PlannedStartDate|The scheduled start date of a task|
|Planned Finish|Task.Finish|target_end_date|PlannedFinishDate|The scheduled finish date of a task|
|Actual Start|Task.ActualStart|act_start_date|ActualStartDate|The date and time when a task actually began|
|Actual Finish|Task.ActualFinish|act_end_date|ActualFinishDate|The date when a task was completed|
|Remaining Early Start|Task.PrimaveraProperties.RemainingEarlyStart|restart_date|RemainingEarlyStartDate|The remaining early start is the same as the early start unless the 'Preserve scheduled early and late dates' option with resource leveling is used.|
|Remaining Early Finish|Task.PrimaveraProperties.RemainingEarlyFinish|reend_date|RemainingEarlyFinishDate|The remaining early finish is the same as the early finish unless the 'Preserve scheduled early and late dates' option with resource leveling is used.|
|Remaining Late Start|Task.PrimaveraProperties.RemainingLateStart|rem_late_start_date|RemainingLateStartDate|The latest date the remaining work for the task should begin without delaying the project finish date.|
|Remaining Late Finish|Task.PrimaveraProperties.RemainingLateFinish|rem_late_end_date|RemainingLateFinishDate|The latest date the remaining work for the task should finish without delaying the project finish date.|
|Original/Planned Duration|Task.Duration|target_drtn_hr_cnt|PlannedDuration|The total working time from the task planned start date to the planned finish date.|
|Actual Duration|-|target_drtn_hr_cnt|ActualDuration|Total working time from the activity actual start date to the actual finish date (for completed tasks) or to the current data date for in-progress tasks.|
|Remaining Duration|Task.RemainingDuration|remain_drtn_hr_cnt|RemainingDuration|The total working time from the task remaining start date to the remaining finish date.|
|At Completion Duration|-|remain_drtn_hr_cnt|AtCompletionDuration|Can be calculated as Task.ActualDuration + Task.RemainingDuration. The total working time from the task's current start date to the current finish date.|
|Actual Labor Units|Task.ActualWork, Task.PrimaveraProperties.ActualLaborUnits|act_work_qty|ActualLaborUnits|The actual units for all labor resources assigned to the task.|
|Remaining Labor Units|Task.RemainingWork|remain_work_qty|RemainingLaborUnits|The remaining units for all labor resources assigned to the task.|
|Planned Labor Units|Task.Work|target_work_qty|PlannedLaborUnits|The planned units for all labor resources assigned to the task.|
|Actual Non Labor Units|Task.PrimaveraProperties.ActualNonLaborUnits|act_equip_qty|ActualNonLaborUnits|The actual units for all nonlabor resources assigned to the task.|
|Remaining Non Labor Units|Task.PrimaveraProperties.RemainingNonLaborUnits|remain_equip_qty|RemainingNonLaborUnits|The remaining units for all nonlabor resources assigned to the task.|
||||||