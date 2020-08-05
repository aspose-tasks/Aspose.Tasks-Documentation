---
title: Public API Changes in Aspose.Tasks 8.8.0
type: docs
weight: 150
url: /java/public-api-changes-in-aspose-tasks-8-8-0/
---

## **Public API and Backwards Incompatible Changes**
**The following public classes were added:**

|**Class name**|**Description**|
| :- | :- |
|com.aspose.tasks.DayLabelDisplay |Specifies how the day label displays. |
|com.aspose.tasks.HourLabelDisplay |Specifies how the hour label displays. |
|com.aspose.tasks.MinuteLabelDisplay |Specifies how the minute label displays. |
|com.aspose.tasks.InvalidPasswordException |Represents the exception type which is thrown when password protected file opening with wrong password. |
|com.aspose.tasks.ProjectDisplayOptions |Represents the display options for a project instance. |
|com.aspose.tasks.TimelineView |Represents a timeline view of a project. |
|com.aspose.tasks.WeekLabelDisplay |Specifies how the week label displays. |
|com.aspose.tasks.YearLabelDisplay |Specifies how the year label displays. |
**The following public fields were added to existing classes:**

|**Field Name**|**Description**|
| :- | :- |
|com.aspose.tasks.DateFormat.Default |Default date format. |
|com.aspose.tasks.Tsk.DISPLAY_ON_TIMELINE |Specifies whether a task should be displayed on a timeline view. |
**The following public methods were added to existing classes:**

|com.aspose.tasks.HeaderFooterInfo.setCenteredText(java.lang.String) |Sets the center aligned text to display in the header or footer. |
| :- | :- |
|com.aspose.tasks.HeaderFooterInfo.setLeftText(java.lang.String) |Sets the left aligned text to display in the header or footer. |
|com.aspose.tasks.HeaderFooterInfo.setRightText(java.lang.String) |Sets the right aligned text to display in the header. |
|com.aspose.tasks.PageInfo.setFooter(com.aspose.tasks.HeaderFooterInfo) |Sets an instance of the HeaderFooterInfo class which represents a footer data. |
|com.aspose.tasks.PageInfo.setHeader(com.aspose.tasks.HeaderFooterInfo) |Sets an instance of the HeaderFooterInfo class which represents a header data. |
|com.aspose.tasks.PageInfo.setLegend(com.aspose.tasks.PageLegend) |Sets an instance of the '@code PageLegend' class which specifies page legend. |
|com.aspose.tasks.PageLegend.setCenteredText(java.lang.String) |Sets the centered text to display in the page legend. |
|com.aspose.tasks.PageLegend.setLeftText(java.lang.String) |Sets the left aligned text to display in the page legend. |
|com.aspose.tasks.PageLegend.setRightText(java.lang.String) |Sets the right aligned text to display in the page legend. |
|com.aspose.tasks.Project.getDisplayOptions |Returns an instance of the ProjectDisplayOptions class. |
|com.aspose.tasks.Table.getAdjustHeaderRowHeight |Returns a flag which determines whether the header row height of the table can be adjusted. |
|com.aspose.tasks.Table.getDateFormat |Gets the date format of the table. |
|com.aspose.tasks.Table.getLockFirstColumn |Returns a flag which determines whether the first column of a table is locked or editable. |
|com.aspose.tasks.Table.getRowHeight |Gets the row height in a table, where the row height is the number of lines of text. |
|com.aspose.tasks.Table.getShowAddNewColumn |Returns a flag which determines whether to show 'Add New Column' interface. |
|com.aspose.tasks.Table.setAdjustHeaderRowHeight(boolean) |Sets a flag which determines whether the header row height of the table can be adjusted. |
|com.aspose.tasks.Table.setDateFormat(int) |Sets the date format of the table. |
|com.aspose.tasks.Table.setLockFirstColumn(boolean) |Sets a flag which determines whether the first column of a table is locked or editable. |
|com.aspose.tasks.Table.setRowHeight(int) |Sets the row height in a table, where the row height is the number of lines of text. |
|com.aspose.tasks.Table.setShowAddNewColumn(boolean) |Sets a flag which determines whether to show 'Add New Column' interface. |
|com.aspose.tasks.TableField.getWrapHeader |Returns a flag which specifies whether the table column heading can wrap to multiple lines, or if it should be truncated when it exceeds the column width. |
|com.aspose.tasks.TableField.getWrapText |Returns a flag which specifies whether the column text can wrap to multiple lines, or if it should be truncated when it exceeds the column width. |
|com.aspose.tasks.TableField.setWrapHeader(boolean) |Sets a flag which specifies whether the table column heading can wrap to multiple lines, or if it should be truncated when it exceeds the column width. |
|com.aspose.tasks.TableField.setWrapText(boolean) |Sets a flag which specifies whether the column text can wrap to multiple lines, or if it should be truncated when it exceeds the column width. |

