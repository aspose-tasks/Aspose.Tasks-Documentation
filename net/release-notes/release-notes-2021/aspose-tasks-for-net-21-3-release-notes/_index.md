---
title: Aspose.Tasks for .NET 21.3 Release Notes
type: docs
weight: 98
url: /net/aspose-tasks-for-net-21-3-release-notes/
---

{{% alert color="primary" %}} 

This page contains release notes information for [Aspose.Tasks for .Net 21.3](https://downloads.aspose.com/tasks/net/new-releases/-aspose.tasks-for-.net-21.3/).

{{% /alert %}}
## **All Changes**
|**Key**|**Summary**|**Issue Type**|
| :- | :- | :- |
| TASKSNET-4702 | Add a feature to set the document name while printing | New Feature |
| TASKSNET-4705 | Add writing of existing values of enterprise extended attributes | Enhancement |
| TASKSNET-4715 | Fix broken page range printing | Bug |
| TASKSNET-4704 | Fix missing column lines while printing to PDF | Bug |
| TASKSNET-4703 | Fix printing of extra columns lines when printing to PDF | Bug |
| TASKSNET-4700 | Fix wrong Resource Usage when exporting MPP - Microsoft Project 365 | Bug |
| TASKSNET-4699 | Task names disappearing when saving MPP file | Bug |
| TASKSNET-4673 | Fix disappearing of task names after MPP resave | Bug |
| TASKSNET-4721 | Fix incorrect timephased data shown when .MPP file is opened in MS Project | Bug |

## **Public API and Backwards Incompatible Changes**
|**The following public methods and properties were added:**|**Description**|
| :- | :- |
| Aspose.Tasks.Project.Print(System.Drawing.Printing.PrinterSettings,Aspose.Tasks.Saving.PrintOptions,System.String) | Prints project according to the specified printer settings, custom save options and the specified document name using the standard (no User Interface) print controller. |

|**The following public enumerations were added:**|**Description**|
| :- | :- |
| Aspose.Tasks.Field.TaskHyperlinkId | Represents the Hyperlink ID (Task) field. |


## **Examples**

TASKSNET-4702: Add a feature to set the document name while printing:
New overload for Project.Print method was added so that a project can be printed using the specified document name, PrinterSettings and PrintOptions:

{{< highlight csharp >}}
Project project = new Project("test.mpp");
PrintOptions options = new PrintOptions();

PrinterSettings printerSettings = new PrinterSettings
{
            FromPage = 1,
            ToPage = 1,
            PrintRange = PrintRange.SomePages
};

project.Print(printerSettings, options, "Print Document Name");
{{< /highlight >}}