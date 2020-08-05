---
title: Aspose.Tasks For Java 9.1.0 Release Notes
type: docs
weight: 10
url: /java/aspose-tasks-for-java-9-1-0-release-notes/
---

## **Major Features**
## **Major Features**
We have implemented Task.DurationText field for mpp writing and 
reading. New constructor has been added to Project class to work with 
Primavera Project. Also reading all project UID from Primavera XML has 
been implemented.About three bugs have been fixed. Please see the list
of changes below. 

We have implemented Task.DurationText field for mpp writing and 
reading. New constructor has been added to Project class to work with 
Primavera Project. Also reading all project UID from Primavera XML has 
been implemented.About three bugs have been fixed. Please see the list
of changes below.
## **All Changes**
All Changes

Issue Type

Key

Summary
# **Public API and Backwards Incompatible Changes**
The following public classes were added:

Class Name

Description

The following public fields were added to existing classes:

Field Name

Description

|**Issue Type** |**Key** |**Summary** |
| :- | :- | :- |
|Task |TASKS-34326 |TASKS-33909 Implement Task.DurationText field writing to mpp 2010/2013 formats |
|Investigation |TASKS-34323 |Read Task.DurationText field from project file |
|New Feature |TASKS-34271 |Provide constructor for Project(Stream steam,PrimaveraXmlReadingOptions options) |
|New Feature |TASKS-34270 |Read all projects UID from Primavera XML to get list of UID |
|Bug |TASKS-34348 |Project reading exception while loading the MPP file |
|Bug |TASKS-34329 |Reading MPP file raises ProjectReadingException |
|Bug |TASKS-34320 |Project reading exception raised while loading the project |

