---
title: Aspose.Tasks for .NET 22.3 Release Notes
description: "The page contains the release notes for Aspose.Tasks for .NET 22.3."
type: docs
weight: 98
url: /net/aspose-tasks-for-net-22-3-release-notes/
---

{{% alert color="primary" %}} 

This page contains release notes information for [Aspose.Tasks for .Net 22.3](https://downloads.aspose.com/tasks/net/new-releases/aspose.tasks-for-.net-22.3/).

{{% /alert %}}
## **All Changes**
|**Key**|**Summary**|**Issue Type**|
| :- | :- | :- |
| TASKSNET-10310 | Add cancellation token support for Project loading operation | New Feature |
| TASKSNET-10498 | Add reading/writing of Status date from/to XER file. | Enhancement |
| TASKSNET-10496 | Make WorkingTime immutable | Enhancement |
| TASKSNET-10480 | Add an API to set user-specified callback which allows to substitute absent fonts when a project is rendered to a graphical format | Enhancement |
| TASKSNET-10471 | Remove unnecessary memory allocations when reading Task, Assignment, Resource properties. | Enhancement |
| TASKSNET-2596 | Add support for "Calculation for task and group summary rows" custom field option | Enhancement |
| TASKSNET-10499 | Fix reading\writing of Guids from\to XER file | Bug |
| TASKSNET-10485 | Fix rendering of holidays in Gantt Chart view | Bug |
| TASKSNET-10484 | Fix reading of Finish Milestones from XER format | Bug |
| TASKSNET-10429 | Fix exception when opening MPP file in projects targeting .NET 6.0 in *nix environment | Bug |
| TASKSNET-10483 | Fix parsing of formulas with different separators | Bug |
| TASKSNET-10479 | Fix differences of calculated custom fields between versions | Bug |

## **Public API and Backwards Incompatible Changes**
|**The following public types were added:**|**Description**|
| :- | :- |
| Aspose.Tasks.FontResolveCallbackDelegate | Represents a method callback to handle font resolve event. |
| Aspose.Tasks.FontResolveEventArgs | Provides arguments for the callback that is invoked when font is resolved. |
| Aspose.Tasks.SummaryRowsCalculationType | Specifies the type of a calculation of the custom attribute's value for summary rows. |
| Aspose.Tasks.Visualization.FontDescriptor | Represents font information. |
| Aspose.Tasks.Visualization.FontStyles | Specifies style information applied to text. |

|**The following public methods and properties were added:**|**Description**|
| :- | :- |
| Aspose.Tasks.ExtendedAttributeDefinition.SummaryRowsCalculationType | Gets or sets the type of calculation of the custom attribute's value for summary rows. |
| Aspose.Tasks.FontResolveEventArgs.RequestedFontName | Gets the name of requested font. |
| Aspose.Tasks.FontResolveEventArgs.ResolvedFontName | Gets or sets the name of resolved font. Can be set to control fonts used to render a view. |
| Aspose.Tasks.OleObject.#ctor | Initializes a new instance of the <see cref="T:Aspose.Tasks.OleObject" /> class. |
| Aspose.Tasks.Project.EnumerateAllChildTasks | Recursively enumerates all project's tasks including root task. |
| Aspose.Tasks.Saving.HtmlSaveOptions.FontResolveCallback | Gets or sets a callback which can be used to customize resolved fonts. |
| Aspose.Tasks.Saving.ImageSaveOptions.FontResolveCallback | Gets or sets a callback which can be used to customize resolved fonts. |
| Aspose.Tasks.Saving.PdfSaveOptions.FontResolveCallback | Gets or sets a callback which can be used to customize resolved fonts. |
| Aspose.Tasks.Visualization.FontDescriptor.#ctor(System.String,System.Single) | Initializes a new instance of the <see cref="T:Aspose.Tasks.Visualization.FontDescriptor" /> class with the specified font family and size. |
| Aspose.Tasks.Visualization.FontDescriptor.#ctor(System.String,System.Single,Aspose.Tasks.Visualization.FontStyles) | Initializes a new instance of the <see cref="T:Aspose.Tasks.Visualization.FontDescriptor" /> class with the specified font family, size and style. |
| Aspose.Tasks.Visualization.FontDescriptor.#ctor(Aspose.Tasks.Visualization.FontDescriptor,Aspose.Tasks.Visualization.FontStyles) | Initializes a new instance of the <see cref="T:Aspose.Tasks.Visualization.FontDescriptor" /> class with the specified font and style. |
| Aspose.Tasks.Visualization.FontDescriptor.FontFamily | Gets the name of the font's family. |
| Aspose.Tasks.Visualization.FontDescriptor.Size | Gets size of the font. |
| Aspose.Tasks.Visualization.FontDescriptor.Style | Gets style of the font. |
| Aspose.Tasks.Visualization.TableTextStyle.#ctor(System.Int32,Aspose.Tasks.Visualization.FontDescriptor) | Initializes a new instance of the <see cref="T:Aspose.Tasks.Visualization.TableTextStyle" /> class with the specified font. |
| Aspose.Tasks.Visualization.TableTextStyle.#ctor(System.Int32,System.Single,Aspose.Tasks.Visualization.FontStyles) | Initializes a new instance of the <see cref="T:Aspose.Tasks.Visualization.TableTextStyle" /> class with the specified font size and font style. |
| Aspose.Tasks.Visualization.TableTextStyle.#ctor(System.Int32,Aspose.Tasks.Visualization.FontStyles) | Initializes a new instance of the <see cref="T:Aspose.Tasks.Visualization.TableTextStyle" /> class with the default font settings and the specified font style. |
| Aspose.Tasks.Visualization.TextStyle.#ctor(System.Single,Aspose.Tasks.Visualization.FontStyles) | Initializes a new instance of the <see cref="T:Aspose.Tasks.Visualization.TextStyle" /> class with the default font and specified font size and style. |
| Aspose.Tasks.Visualization.TextStyle.#ctor(Aspose.Tasks.Visualization.FontStyles) | Initializes a new instance of the <see cref="T:Aspose.Tasks.Visualization.TextStyle" /> class with the default font and specified font style. |
| Aspose.Tasks.Visualization.TextStyle.#ctor(Aspose.Tasks.Visualization.FontDescriptor) | Initializes a new instance of the <see cref="T:Aspose.Tasks.Visualization.TextStyle" /> class with the specified font settings. |
| Aspose.Tasks.Visualization.TextStyle.Font | Gets or sets font of the text style. |
| Aspose.Tasks.WorkingTime.#ctor(System.TimeSpan,System.TimeSpan) | Initializes a new instance of the <see cref="T:Aspose.Tasks.WorkingTime" /> class with an interval item with the specified start and finish times. |
| Aspose.Tasks.WorkingTime.#ctor(System.Int32,System.Int32) | Initializes a new instance of the <see cref="T:Aspose.Tasks.WorkingTime" /> class with an interval item with the specified start and finish times. |
| Aspose.Tasks.WorkingTime.From | Gets the beginning of a working time. |
| Aspose.Tasks.WorkingTime.To | Gets the end of a working time. |

|**The following public methods and properties were deleted:**|**Description**|
| :- | :- |
| Aspose.Tasks.WorkWeek.#ctor(Aspose.Tasks.Calendar) |  |

|**The following public enumerations were added:**|**Description**|
| :- | :- |
| Aspose.Tasks.SummaryRowsCalculationType.None | Means the custom attribute's value for summary rows is not calculated. |
| Aspose.Tasks.SummaryRowsCalculationType.Rollup | Means the custom attribute's value for summary rows is calculated using rollup function defined in <see cref="P:Aspose.Tasks.ExtendedAttributeDefinition.RollupType" />. |
| Aspose.Tasks.SummaryRowsCalculationType.UseFormula | Means the custom attribute's value for summary rows is calculated using formula defined in <see cref="P:Aspose.Tasks.ExtendedAttributeDefinition.Formula" />. |
| Aspose.Tasks.Visualization.FontStyles.Regular | Normal text. |
| Aspose.Tasks.Visualization.FontStyles.Bold | Bold text. |
| Aspose.Tasks.Visualization.FontStyles.Italic | Italic text. |
| Aspose.Tasks.Visualization.FontStyles.Underline | Underlined text. |
| Aspose.Tasks.Visualization.FontStyles.Strikeout | Text with a line through the middle. |

## **Examples and additional notes**

**.NET Framework 2.0 deprecation notice**

Starting with ver. 22.9 (September 2022) Aspose.Tasks for .NET will no longer support .NET Framework 2.0.

**Notes on support of .NET 6.0 in \*nix environment**

Related issue: TASKSNET-10429, Fix exception when opening MPP file in projects targeting .NET 6.0 in *nix environment

As a step in adding of support .NET 6.0 in *nix environment we are replacing property TextStyle.FontFamily (Type: System.Drawing.FontFamily) with property TextStyle.Font (Type: Aspose.Tasks.Visualization.FontDescriptor).
The rendering (when project's view is saved to a graphical format) is not supported at the moment because it relies on System.Drawing.Common.
See [Microsoft post|https://docs.microsoft.com/en-us/dotnet/core/compatibility/core-libraries/6.0/system-drawing-common-windows-only] for more details.

**Related issue: TASKSNET-10310 - Add cancellation token support for Project loading operation**

Now CancellationToken can be specified to allow cancellation of long project loading operation (not applicable to versions for .NET Framework 2.0 and 3.5):

{{< highlight csharp >}}

CancellationTokenSource cts = new CancellationTokenSource(); 

var loadOptions = new LoadOptions() { CancellationToken = cts.Token };
Project p = new Project("test.mpp", loadOptions);

{{< /highlight >}}

**Related issue: TASKSNET-10480 - Add an API to set user-specified callback which allows to substitute absent fonts when a project is rendered to a graphical format**

The user can use any font to customize View's text styles using MS Project. When the project is saved, the font information (actually a font name and size) is persisted to MPP file.
Sometimes the resulting MPP file is opened on another environment where the specified font may be missing. To address this issue we introduced FontResolveCallback 
which can be used to intercept font resolving event. The callback is invoked when the project's view is saved to a graphical format and the rendering engine resolves a font to render a text.

{{< highlight csharp >}}
Project project = new Project("Input.mpp");
PdfSaveOptions so = new PdfSaveOptions();
so.PresentationFormat = PresentationFormat.GanttChart;
so.Timescale = Timescale.DefinedInView;
so.FontResolveCallback = delegate(FontResolveEventArgs args)
{
    if (args.RequestedFontName  != args.ResolvedFontName)
    {
        // Looks like the exact font cannot be found and fallback font was resolved.
        // We can override the fallback font.
        args.ResolvedFontName = "Arial";
    }

    // Or simply substitute the specific font:
    if (args.RequestedFontName == "Comic Sans MS")
    {
        args.ResolvedFontName = "Arial";
    }
};

project.Save("Output.pdf", so);
{{< /highlight >}}


**Related issue: TASKSNET-2596 - Add support for "Calculation for task and group summary rows" custom field option**

The API for Extended attributes were improved. The previous ExtendedAttributeDefinition API where ExtendedAttributeDefinition.CalculationType should be one of the following: { None, Lookup, Rollup, Calculation } didn't reflect all the cases such as extended attribute where values for leaf tasks are calculated using formula and values of the summary tasks are calculated using rollup.
ExtendedAttributeDefinition.SummaryRowsCalculationType property (with values None, Rollup, UseFormula) was added to reflect MS Project's model of extended attribute's settings.
ExtendedAttributeDefinition.CalculationType's values are now limited to (None, Lookup, Formula) values.

![Extended attribute settings in MS Project](ExtendedAttributeDefinition.png)


The following example creates an extended attribute which values for leaf tasks are calculated using formula and values for summary tasks are calculated using average rollup:
{{< highlight csharp >}}

var project = new Project("Test.mpp");
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, "Calculated cost");
definition.CalculationType = CalculationType.Formula;
definition.Formula = "[Cost] * 3.14";
definition.SummaryRowsCalculationType = SummaryRowsCalculationType.Rollup;
definition.RollupType = RollupType.Average;

project.ExtendedAttributes.Add(definition);

project.Save("Output.mpp");

{{< /highlight >}}


**Related issue: TASKSNET-10496 - Make WorkingTime immutable**

In order to optimize calendar-related calculations WorkingTime class was made immutable (so properties cannot be modified after object is created).
Also 2 new overloads of constructor of WorkingTime class were added to allow less verbose creation of WorkingTime:

22.2 version:
{{< highlight csharp >}}
WorkingTime wt = new WorkingTime(new DateTime(1, 1, 1, 9, 0, 0), new DateTime(1, 1, 1, 12, 0, 0));
WorkingTime wt2 = new WorkingTime(new DateTime(1, 1, 1, 9, 15, 0), new DateTime(1, 1, 1, 12, 15, 0));
{{< /highlight >}}
22.3+ version:
{{< highlight csharp >}}
WorkingTime wt = new WorkingTime(9, 12);
WorkingTime wt2 = new WorkingTime(new TimeSpan(9, 15, 0), new TimeSpan(12, 15, 0));
{{< /highlight >}}