---
title: Aspose.Tasks for .NET 9.0.1 Release Notes
type: docs
weight: 90
url: /net/aspose-tasks-for-net-9-0-1-release-notes/
---

## **Major Features**
We have implemented enhancement which allow to read subproject info (inserted project information). New
constructor has been added to Project class to work with Primavera 
Project. Also reading all project UID from Primavera XML has been 
implemented. About six bugs have been fixed. Please see the list of 
changes below.

## **All Changes**
|**Issue Type** |**Key** |**Summary** |
| :- | :- | :- |
|Bug |TASKS-34281 |Exception while adding resource assignment to task with duration ZERO |
|Bug |TASKS-34280 |Calendar exceptions lost when MPP saved and used again |
|Bug |TASKS-34279 |Wrong AssignmentBaselineWork retrieved from Timephased data |
|Bug |TASKS-34275 |Wrong monthly hours extracted while reading Timephased data |
|Bug |TASKS-34274 |Timephased data shown far beyond the project task dates |
|Bug |TASKS-34273 |Wrong timephased data read against holidays |
|Enhancement |TASKS-34258 |Unable to set Task as another SubProject |
|New Feature |TASKS-34271 |Provide constructor for Project(Stream steam,PrimaveraXmlReadingOptions options) |
|New Feature |TASKS-34270 |Read all projects UID from Primavera XML to get list of UID |

