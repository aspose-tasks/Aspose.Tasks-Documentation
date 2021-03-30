---
title: Aspose.Tasks For Java 8.8.0 Release Notes
type: docs
weight: 40
url: /java/aspose-tasks-for-java-8-8-0-release-notes/
---

## **Major Features**
We have significantly improved writing and reading for mpp format. We
have also implemented Task ExtendedAttributes and 
ExtendedAttributeDefinitions reading from MS Project Server. About ten 
bugs have been fixed. Please see the list of changes below. 

We have significantly improved writing and reading for mpp format. We
have also implemented Task ExtendedAttributes and 
ExtendedAttributeDefinitions reading from MS Project Server. About ten 
bugs have been fixed. Please see the list of changes below.
## **All Changes**
All Changes

Issue Type

Key

Summary
# **Public API and Backwards Incompatible Changes**
The following public classes were added:

Class name

Description

The following public fields were added to existing classes:

Field Name

Description

The following public methods were added to existing classes:

|**Issue Type** |**Key** |**Summary** |
| :- | :- | :- |
|Task |TASKS-34220 |Implement reading/writing TableField.WrapText and TableField.WrapHeader fields to mpp format |
|Task |TASKS-34219 |Implement reading/writing Table.LockFirstColumn and Table.AdjustHeaderRowHeight fields to mpp format |
|Task |TASKS-34218 |Implement reading/writing Table.RowHeight and Table.DateFormat fields to mpp format |
|Task |TASKS-34202 |Read Timeline View data from mpp format |
|Task |TASKS-34201 |Read Task.DisplayOnTimeline field |
|Task |TASKS-34180 |Implement Task ExtendedAttributes reading from MS Project DB |
|Task |TASKS-34167 |Implement ExtendedAttributeDefinitions reading from MS Project DB |
|Task |TASKS-34144 |Implement Calendar binary data reading from MSP database |
|Task |TASKS-34116 |Implement Export/Import Project Data as HTML |
|Sub-task |TASKS-34217 |TASKS-33909 Implement reading/writing Table.ShowInMenu field for 2007-2013 mpp formats |
|Sub-task |TASKS-34205 |TASKS-33909 Write Timeline View data to mpp |
|Sub-task |TASKS-34209 |TASKS-33909 Implement Page Setup Header, Footer and Legend text writing to mpp |
|Sub-task |TASKS-34199 |TASKS-33909 Implement Project DisplayOptions reading/writing |
|Enhancement |TASKS-34120 |Date localization while exporting to PDF |
|Bug |TASKS-34225 |StackOverflow exception raised while loading this MPP file |
|Bug |TASKS-34222 |Resaving MPP duplicates hyperlink in Task Notes |
|Bug |TASKS-34221 |Project can not be re-saved and gets stuck in loop |
|Bug |TASKS-34186 |Values set against extended attributes in a task are not visible in MPP while opened in MSP |
|Bug |TASKS-34185 |Extended attribute not maintained in MPP |
|Bug |TASKS-34181 |Dates wrong on link type Finish to Finish with parent task |
|Bug |TASKS-34174 |Wrong remaining work displayed in MSP 2010 using XML saved by Aspose.Tasks |
|Bug |TASKS-34173 |IndexOutOfRangeException occurred during reading from Primavera DB |
|Bug |TASKS-34170 |Wrong Working Days when saving to MPX |
|Bug |TASKS-34149 |Cannot read summary task's data from Primavera DB correctly |

