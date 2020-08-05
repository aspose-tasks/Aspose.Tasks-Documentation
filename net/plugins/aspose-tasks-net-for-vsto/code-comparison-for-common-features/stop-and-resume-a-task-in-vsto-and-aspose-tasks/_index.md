---
title: Stop and Resume a Task in VSTO and Aspose.Tasks
type: docs
weight: 90
url: /net/stop-and-resume-a-task-in-vsto-and-aspose-tasks/
---

{{% alert color="primary" %}} 

A tasks's stop date is the date that it should (or did) end. Sometimes, a task has to be stopped temporarily and then resumed later. Microsoft Project can calculate stop dates, or let users enter them manually.

{{% /alert %}} 
## **VSTO**
Below is the code of VSTO Project to Stop and Resume a task:

{{< highlight cs >}}

   string FileName = "MyProject.mpp";

  object missingValue = System.Reflection.Missing.Value;

  Application.FileOpenEx(FileName,

    missingValue, missingValue, missingValue, missingValue,

    missingValue, missingValue, missingValue, missingValue,

    missingValue, missingValue, PjPoolOpen.pjPoolReadOnly,

    missingValue, missingValue, missingValue, missingValue,

    missingValue);

  Project MyProject = Application.ActiveProject;

  Task MyTask = MyProject.Tasks[1];

  // Stop a Task

  dynamic StopedDate = MyTask.Stop;

  // Resume a Task

  dynamic ResumeDate = MyTask.Resume;


{{< /highlight >}}
## **Aspose.Tasks**
The Stop and Resume properties exposed by the [Tsk\](/pages/createpage.action?spaceKey=tasksnet&title=Aspose.Tasks.Tsk+class&linkCreation=true&fromPageId=16288574) class are used to read or write a task's stop and resume date:

- Stop: the date a task stops (DateTime).
- Resume: the data and time a task restarts (DateTime).
#### **Microsoft Project view of Stop and Resume Dates**
To see a task's stop and resume dates:

1. In the Task Entry form, on the **Inset** menu, select **Column**.
1. Add the Stop and Resume columns. 
   **The Stop and Resume columns in Microsoft Project** 
#### **Getting Stop and Resume Dates**
The stop and resume dates are NA, if the task has never stopped. For date values equal to NA, Aspose.Tasks takes the value "1/1/2000" if you're using the evaluation version. When fully licensed, Aspose.Tasks uses DateTime.MinValue for NA values. The following examples displays the stop and resume dates for all the tasks in a project.

{{< highlight cs >}}

   string FileName =  "MyProject.mpp";

  Project MyProject = new Project(FileName);

  Task MyTask = MyProject.RootTask;

  // Stop a Task

  DateTime StoppedDate = MyTask.Stop;

  // Resume a Task

  DateTime ResumeDate = MyTask.Resume;


{{< /highlight >}}
## **Download Running Code**
- [Codeplex](https://asposevsto.codeplex.com/SourceControl/latest#Aspose.Tasks Vs VSTO Project/Stop and Resume a Task/)
- [Github](https://github.com/aspose-tasks/Aspose.Tasks-for-.NET/tree/master/Plugins/Aspose.Tasks%20Vs%20VSTO%20Projects/Code%20Comparison%20of%20Common%20Features/Stop%20and%20Resume%20a%20Task)
- [Code.MSDN](https://code.msdn.microsoft.com/AsposeTasks-Vs-VSTO-v11-168e5b01/view/SourceCode#content)
## **Download Sample Code**
- [Codeplex](https://asposevsto.codeplex.com/releases/view/616887)
- [Github](https://github.com/aspose-tasks/Aspose.Tasks-for-.NET/releases/tag/AsposeTaskNETVsVSTOProjectv1.1)
- [Code.MSDN](https://code.msdn.microsoft.com/AsposeTasks-Vs-VSTO-v11-168e5b01)
